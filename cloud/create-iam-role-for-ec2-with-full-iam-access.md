# Create IAM Role for EC2 with Full IAM Access

> **Company:** Coinbase | **Difficulty:** Easy

---

#### **Scenario**

Your team needs an EC2 instance to manage IAM resources programmatically. To follow AWS security best practices, you should use an IAM role instead of embedding credentials.

#### **Task**

Create an IAM role named `IAMFullAccessEC2` that:
- Allows the EC2 service to assume the role
- Has the `IAMFullAccess` AWS managed policy attached

<br>

_Note: You can use either the AWS Management Console or AWS CLI to complete this task._

---
📹 [Video Solution](https://prepare.sh/interview/devops/aws/create-iam-role-for-ec2-with-full-iam-access)