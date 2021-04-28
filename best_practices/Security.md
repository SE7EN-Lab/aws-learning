Tracking activities on AWS
--------------------------
- Enable CloudTrail across all geographic regions and AWS services.
- Turn on CloudTrail log file validation so that any changes made to the log file itself after it has been delivered to the S3 bucket is trackable to ensure log file integrity.
- Turn on multifactor authenthication (MFA) to delete CloudTrail S3 buckets, and encrypt all CloudTrail log files in flight and at rest.

Identity & Access management on AWS
------------------------------------
- When creating IAM policies, ensure that they’re attached to groups or roles rather than individual users
- Provision access to a resource using IAM roles instead of providing an individual set of credentials that could be compromised leading to unauthorized access to the resource.
- Adopt least privilege policy while allowing IAM users access to resources
- Ensure MFA is activated for individual accounts and limit the number of IAM users with admin privileges.
- Practice IAM access key rotation & Strong password policy for all IAM accounts.
- Validate the IAM policy using IAM policy simulator.