# AWS IAM Hands-on Practice

## Objective
To implement and validate AWS Identity and Access Management (IAM) by creating users, groups, and policies while following the principle of least privilege.

## AWS Service Used
- AWS Identity and Access Management (IAM)

## Tasks Performed
1. Accessed IAM dashboard and reviewed security recommendations.
2. Created an IAM group named `WebAdmins`.
3. Attached `AmazonEC2ReadOnlyAccess` policy to the group.
4. Created an IAM user `web-user` and added it to the group.
5. Tested IAM user login using the IAM sign-in URL.
6. Verified allowed access to EC2 services.
7. Verified denied access to Amazon S3 when attempting to create a bucket.

## Access Validation
- EC2 access: Allowed (Read-only)
- S3 access:  Access denied (CreateBucket action)

## IAM Concepts Covered
- IAM Users
- IAM Groups
- AWS Managed Policies
- Least Privilege Principle
- Access Validation

## Screenshots
All screenshots related to the above tasks are available in the `screenshots` folder.

## Key Learnings
- Permissions should be assigned using groups instead of directly to users.
- IAM permissions are evaluated at the API action level.
- Least privilege improves overall AWS account security.

## Future Improvements
- Create custom IAM policies
- Enable MFA for IAM users
- Implement IAM roles for EC2 access
