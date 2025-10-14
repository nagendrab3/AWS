**IAM Users**

An IAM user can interact with AWS through the Management Console, AWS
CLI, or SDKs, based on the permissions you attach.

By default, a newly created IAM user has no permissions. You must attach
policies to grant access.

Methods to Attach IAM Policies

IAM Users: Directly attach policies to the user.

**Access the IAM Console**

**Create IAM User**

1.  Sign in to the (https://aws.amazon.com/console/)
   <img width="732" height="331" alt="image" src="https://github.com/user-attachments/assets/ffb1ea71-357d-4db8-b650-1609dc04384b" />


2.  In the search bar, type IAM and select Identity and Access
    Management.
<img width="701" height="299" alt="image" src="https://github.com/user-attachments/assets/25045d9d-5190-4502-833d-ae4145bded7b" />



3.  On the IAM dashboard, review any security recommendations (e.g.,
    enabling MFA).

<img width="703" height="341" alt="image" src="https://github.com/user-attachments/assets/7e3dbc7b-ccfb-4899-8541-459b6de7e70c" />


4.  In the left navigation pane, click Users to view existing IAM users.
<img width="699" height="317" alt="image" src="https://github.com/user-attachments/assets/70aa4704-e39d-4ee8-b32a-a0e28a6afc6c" />


**Create a New IAM User**

1.  Click **Create users**.

<img width="660" height="291" alt="image" src="https://github.com/user-attachments/assets/a3ca39b5-1a4d-4e4d-9d55-f800cdc8452f" />


2.  Enter **NagendrabA** as the **User name**.

<img width="732" height="274" alt="image" src="https://github.com/user-attachments/assets/1cca851f-92ec-4f61-9af1-7cc6dfea4413" />


3.  Under **Select AWS access type**, choose one or both of the
    following:

-   Access Type Description AWS Management Console access Enables web console sign-in.

-   Programmatic access Generates access keys for CLI/SDK interaction.
<img width="795" height="207" alt="image" src="https://github.com/user-attachments/assets/59048022-2ebc-48db-b546-7946bc2c36e3" />


4.  For Console password, select Custom password and enter your desired
    password.

<img width="706" height="285" alt="image" src="https://github.com/user-attachments/assets/3b00c1fa-eac0-4adb-a2ae-d7aa2411906d" />


5.  Enable Require password reset to force john to set a new password at
    first sign-in.
<img width="631" height="273" alt="image" src="https://github.com/user-attachments/assets/d0e974b1-22ef-4e87-ac68-18429469909d" />



6.  On the Set permissions page, assign policies or skip this step to
    configure permissions later.
<img width="654" height="239" alt="image" src="https://github.com/user-attachments/assets/b6ce8ec8-bc03-4e54-976c-e60e862b8f7a" />


7.  Click Next until you reach the Review page, verify all settings,
    then click Create user.

<img width="655" height="260" alt="image" src="https://github.com/user-attachments/assets/5d24a43c-d668-494e-8180-b2875347723f" />


8.  Choose **Return to users**.

<img width="728" height="88" alt="image" src="https://github.com/user-attachments/assets/92385ae2-c045-4765-9d27-0d0f007bc328" />


**Test the Console Sign-In**

1.  Open a private/incognito browser window.

2.  Navigate to https://aws.amazon.com and click Sign In.

3.  Select IAM user, enter your AWS account ID, then click Next.

4.  Provide Username: NagendrabA and the initial password you set.

5.  You'll be prompted to change the password

6.  Enter the old password, choose a new one, and confirm.

7.  After confirmation, you will be signed in as **NagendrabA**.
