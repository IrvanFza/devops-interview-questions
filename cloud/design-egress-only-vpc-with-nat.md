# Design Egress Only VPC with NAT

> **Company:** Twitch | **Difficulty:** Medium

---

#### **Scenario**

We need to prepare infrastructure for `ECS` tasks and `EC2` instances. It has to span across at least two Availability Zones. These workloads require **outbound internet access** to download updates and call external APIs. However, inbound access is **not allowed**. Additionally application should send data to `S3` in **cost effective** way and so we have to deploy necessary infrastructure for that traffic too.

***Note:** You are required to design the VPC networking architecture only. Creation of ECS clusters, services, or EC2 instances is not part of this task.*

#### **Task**

Design and implement a VPC network architecture `10.0.0.0/16` that meets the following requirements:

1. **Network Isolation:** Workloads must reside in subnets across two Availability Zones with no public IP addresses and must not be directly reachable from the internet.
2. **Egress Control:** Workloads must be able to initiate outbound connections to the public internet over HTTP and HTTPS. The internet must not be able to initiate connections to them.
***Note:** You should create and configure a new non-default security group.*
3.  **Egress Restrictions:** Outbound traffic from workloads should be limited to only the required protocols and destinations.
4. **Cost Awareness:** The architecture should account for cost-efficient routing when accessing AWS-managed services, minimizing unnecessary NAT Gateway usage.

<br>

_Note: You can use either the AWS Management Console or AWS CLI to complete this task._

---
📹 [Video Solution](https://prepare.sh/interview/devops/aws/design-egress-only-vpc-with-nat)