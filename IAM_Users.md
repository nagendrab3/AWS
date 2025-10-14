**IAM Users**

An IAM user can interact with AWS through the Management Console, AWS
CLI, or SDKs, based on the permissions you attach.

By default, a newly created IAM user has no permissions. You must attach
policies to grant access.

Methods to Attach IAM Policies

IAM Users: Directly attach policies to the user.

**Access the IAM Console**

**Create IAM User**

1.  Sign in to the [**AWS Management
   

2.  In the search bar, type IAM and select Identity and Access
    Management.



3.  On the IAM dashboard, review any security recommendations (e.g.,
    enabling MFA).



4.  In the left navigation pane, click Users to view existing IAM users.


**Create a New IAM User**

1.  Click **Create users**.



2.  Enter **NagendrabA** as the **User name**.



3.  Under **Select AWS access type**, choose one or both of the
    following:

-   Access Type Description AWS Management Console access Enables web
    > console sign-in.

-   Programmatic access Generates access keys for CLI/SDK interaction.


4.  For Console password, select Custom password and enter your desired
    password.



5.  Enable Require password reset to force john to set a new password at
    first sign-in.



6.  On the Set permissions page, assign policies or skip this step to
    configure permissions later.


7.  Click Next until you reach the Review page, verify all settings,
    then click Create user.



8.  Choose **Return to users**.



**Test the Console Sign-In**

1.  Open a private/incognito browser window.

2.  Navigate to https://aws.amazon.com and click Sign In.

3.  Select IAM user, enter your AWS account ID, then click Next.

4.  Provide Username: NagendrabA and the initial password you set.

5.  You'll be prompted to change the password

6.  Enter the old password, choose a new one, and confirm.

7.  After confirmation, you will be signed in as **NagendrabA**.
