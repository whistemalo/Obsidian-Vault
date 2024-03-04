what is a user pool?

This topic describes six common scenarios for using Amazon Cognito.

The two main components of Amazon Cognito are user pools and identity pools. User pools are user directories that provide sign-up and sign-in options for your web and mobile app users. Identity pools provide AWS credentials to grant your users access to other AWS services.

A user pool is a user directory in Amazon Cognito. Your app users can sign in either directly through a user pool, or federate through a third-party identity provider (IdP). The user pool manages the overhead of handling the tokens that are returned from social sign-in through Facebook, Google, Amazon, and Apple, and from OpenID Connect (OIDC) and SAML IdPs. Whether your users sign in directly or through a third party, all members of the user pool have a directory profile that you can access through an SDK.

With an identity pool, your users can obtain temporary AWS credentials to access AWS services, such as Amazon S3 and DynamoDB. Identity pools support anonymous guest users, as well as federation through third-party IdPs.

You have access to the following features when you authenticate local users:

* Implement your own web front-end that calls the Amazon Cognito user pools API to authenticate, authorize, and manage your users.

* Set up multi-factor authentication (MFA) for your users. Amazon Cognito supports time-based one-time password (TOTP) and SMS message MFA.
* Secure against access from user accounts that are under malicious control. 
* Create your own custom multi-step authentication flows. 
* Look up users in another directory and migrate them to Amazon Cognito.




1. Go to the [Amazon Cognito console](https://console.aws.amazon.com/cognito/home). If prompted, enter your AWS credentials.
    
2. Choose **User Pools**.
    
3. In the top-right corner of the page, choose **Create a user pool** to start the user pool creation wizard.
    
4. In **Configure sign-in experience**, choose the federated providers that you want to use with this user pool. For more information, see [Adding User Pool Sign-in Through a Third Party](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-identity-federation.html).
5. In **Configure security requirements**, choose your password policy, multi-factor authentication (MFA) requirements, and user account recovery options. For more information, see [Security in Amazon Cognito](https://docs.aws.amazon.com/cognito/latest/developerguide/security.html).
    
6. In **Configure sign-up experience**, determine how new users will verify their identities when signing up, and which attributes should be required or optional during the user sign-up flow. For more information, see [Managing users in user pools](https://docs.aws.amazon.com/cognito/latest/developerguide/managing-users.html).
7.  In **Configure message delivery**, configure integration with Amazon Simple Email Service (Amazon SES) and Amazon Simple Notification Service (Amazon SNS) to send email and SMS messages to your users for sign-up, account confirmation, MFA, and account recovery. For more information, see [Email Settings for Amazon Cognito User Pools](https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-email.html) and [SMS message settings for Amazon Cognito user pools](https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-sms-settings.html).
    
8. In **Integrate your app**, name your user pool, configure the hosted UI, and create an app client. For more information, see [Add an App to Enable the Hosted Web UI](https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-configuring-app-integration.html)
    
9. Review your choices in the **Review and create** screen and modify any selections you wish to. When you are satisfied with your user pool configuration, select **Create user pool** to proceed.

