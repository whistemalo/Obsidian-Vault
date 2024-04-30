
So I want to implement or create a pipeline of data that will collect all relevant info from the materials that the institution buy on every days activities and track them down to where does that products ends.

First I need to star by doing some research of how should I tackle down this task, not long ago a created a database where I feed all of the data transformed and cleaned from that database I build a bunch of power Bi Dashboards with some basics KPI;s buy that wasn't enough  as a institution we need to process and analyze all of the incoming data to generate accurate  forecasting of the materials that are being consumed by the project technicians  on the field.

There are 2 main databases, one of the is from the old system is a sql server 2016 with about 4 thousand tables with no descriptions, compose keys, string primary keys and every bad practice that you can imagine... on the other hand there is a pgsql database that serves the new system that is being develop with newer technologies using c# and react js for the frontend.

About how I'm going to tackle this problem I was thinking that I need to start by defining the tools that I'll be using.

The root of the problem starts with the "Request of necessity or requisition request" therefore I was thinking about a unified request table  taking data from both databases... but then I start remembering that the last time I build a database for that purpose I ended up using Laravel framework just for migrations... This time I want to explore new alternatives looking for tools that best suite this specific task that can do migrations, rollback and maybe seeding...

At the end I choose flyway  as  my main tool to manage all migrations and version my database schemas, it seems a bit old and it works with java  I found tools like phinx  that is based on PHP and its like laravel migrations but it doesn't seems to be that popular or have  and active community for that I desisted on using it, futher more I choose flyway because it manage migrations with pure sql giving me the absolute control of the database that im creating
