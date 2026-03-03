# Audit and Enforce Least-Privilege IAM Permissions

> **Company:** Amazon | **Difficulty:** Easy

---

#### **Scenario**

A security audit has flagged the IAM user `app-deployer` for having `AdministratorAccess` policy with far more permissions than needed. The user only needs access to:
- **S3**: Read (GetObject) and Add objects (PutObject), list buckets (ListBucket).
- **CloudWatch Logs**: Create log groups (CreateLogGroup), log streams (CreateLogStream), and put log events (PutLogEvents).

#### **Task**

1. Inspect the current policies attached to the `app-deployer` user
2. Remove the overly broad `AdministratorAccess` policy
3. Create a custom managed policy named `AppDeployerPolicy` that grants **only** the required permissions listed above
4. Attach the new policy to the `app-deployer` user

<br>

_Note: You can use either the AWS Management Console or AWS CLI to complete this task._

---
📹 [Video Solution](https://prepare.sh/interview/devops/aws/audit-and-enforce-least-privilege-iam-permissions)