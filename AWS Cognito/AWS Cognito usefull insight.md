 Don't enable self-registration in your user pool unless you want to open your app to public sign-up. To change this setting, update **Self-service sign-up** in the **Sign-up experience** tab of the user pool console, or update the value of [AllowAdminCreateUserOnly](https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_AdminCreateUserConfigType.html#CognitoUserPools-Type-AdminCreateUserConfigType-AllowAdminCreateUserOnly) in a [CreateUserPool](https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_CreateUserPool.html) or [UpdateUserPool](https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_UpdateUserPool.html) API request.

For information about security features that you can set up in your user pools, see [Using Amazon Cognito user pools security features](https://docs.aws.amazon.com/cognito/latest/developerguide/managing-security.html).

* You can skip public or federated sign-up, and create users based on your own data source and schema
* Run a just-in-time AWS Lambda function that looks up your new user in an existing directory, and populates their user profile from existing data
* add them to groups that Amazon Cognito lists in the access and ID tokens
Note: Amazon Cognito can be a standalone user directory and identity provider (IdP) to your app.

**Your users can sign in with a UI that’s hosted by Amazon Cognito or with your own UI through the Amazon Cognito user pools API**

Import users from a CSV file. Run a just-in-time AWS Lambda function that looks up your new user in an existing directory, and populates their user profile from existing data.

You can add the hosted UI to your existing domain, or use a prefix identifier in an AWS subdomain.

If network traffic to your user pool might be malicious, you can monitor it and take action with AWS WAF web ACLs.

You can upload custom CSS and logos to give the hosted UI a familiar look and feel to your users.


![[Pasted image 20240119112311.png]]
Create a user pool when you want to authenticate and authorize users to your app or API. User pools are a user directory with both self-service and administrator-driven user creation, management, and authentication.
![[Pasted image 20240119112340.png]]
Set up an Amazon Cognito identity pool when you want to authorize authenticated or anonymous users to access your AWS resources.

**An Amazon Cognito user pool and identity pool used together**
