
==> IAM policies and permissions

IAM policies and permissions control who can perform which actions on which resources. 
Applying the Principle of Least Privilege granting only the access needed to perform a task—helps secure your environment.

==> Principle of Least Privilege

Grant users and roles only the permissions they require. In this example, Nagendra creates three groups:

Admins (Devi and Akhila): full management rights across AWS services.

Developers: access limited to a specific Sales folder.

Test (Manoj and saleem): no access to the Sales folder


Applying least privilege minimizes the blast radius if credentials are compromised.

==> Defining Permissions

A permission is a fine-grained control that authorizes an action on an AWS resource.

==> Common permission examples:

ec2:StartInstances – start an EC2 instance

s3:GetObject – download an object from an S3 bucket

sqs:CreateQueue – create a new SQS queue

sns:DeleteTopic – delete an SNS topic

==> Policy

A policy is a collection of one or more permissions.

==> What Is an IAM Policy?
An IAM policy is a JSON document that defines:

Who (user, group, role) can perform
What actions on
Which resources


