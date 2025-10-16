**IAM policies and permissions**

IAM policies and permissions control who can perform which actions on which resources. 
Applying the Principle of Least Privilege granting only the access needed to perform a task—helps secure your environment.

**Principle of Least Privilege**

Grant users and roles only the permissions they require. In this example, Nagendra creates three groups:

Admins (Devi and Akhila): full management rights across AWS services.

Developers: access limited to a specific Sales folder.

Test (Manoj and saleem): no access to the Sales folder


Applying least privilege minimizes the blast radius if credentials are compromised.

**Defining Permissions**

A permission is a fine-grained control that authorizes an action on an AWS resource.

**Common permission examples:**

ec2:StartInstances – start an EC2 instance

s3:GetObject – download an object from an S3 bucket

sqs:CreateQueue – create a new SQS queue

sns:DeleteTopic – delete an SNS topic

 **Policy**

A policy is a collection of one or more permissions.

What Is an IAM Policy?

An IAM policy is a JSON document that defines:

Who (user, group, role) can perform

What actions on

Which resources


**IAM Policies Defined**

IAM policies manage access and permissions in AWS

A policy defines the permisiions and actions for an identity or resource.

Rukes that define what resources an entity can access and what operations they can perform.

IAM policies provide fine-grained access control for resources and services.

==> Policy Types

IAM policies fall into two primary categories:

1. Identity-based policy:

Users, groups, roles

Grant permissions to IAM identities

2. Resource-based policy

AWS resources (e.g., S3, Lambda)

Attach policies directly to resources themselves.


You can attach an identity-based policy to a group of developers or assign a role to an EC2 instance so your applications inherit those permissions.

==> Identity-based Policy Example

Below is a sample JSON identity policy with two statements:

{
  "Version": "20XX-10-16",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": [
        "s3:*"
      ],
      "Resource": [
        "arn:aws:s3:::<bucket-name>"
      ]
    },
    {
      "Effect": "Allow",
      "Action": [
        "ec2:StartInstances"
      ],
      "Resource": [
        "arn:aws:ec2:<region>:<account-id>:instance/<instance-id>"
      ]
    }
  ]
}


==> The first statement allows all S3 actions on a specific bucket.

==> The second statement allows starting a particular EC2 instance.

==> Example: Creating an Identity Policy

Follow these steps in the AWS Management Console to create and attach an identity-based policy to a group:

Sign in to the IAM console.

Navigate to Policies > Create policy.

Use the JSON editor to paste your policy document.

Review and Create policy.

Attach the new policy to your IAM group.

