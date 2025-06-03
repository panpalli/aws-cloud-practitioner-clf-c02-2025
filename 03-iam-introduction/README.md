# 🔐 03 - IAM (Identity and Access Management) - Introduction

This module introduces AWS IAM – a global service used to manage users, groups, permissions, and policies across your AWS environment.

---

## ✅ What is IAM?

- **IAM** = Identity and Access Management
- It is a **global AWS service**
- Used to control **who can access what** in your AWS account

---

## 👤 IAM Users and 👥 Groups

- **User** = Represents a person or an application
- **Group** = Collection of users with similar permissions
- Groups **cannot contain other groups**
- A user can belong to **multiple groups** or none

### Example:
| Name     | Role       | Group             |
|----------|------------|-------------------|
| Alice    | Developer  | Developers        |
| Bob      | Developer  | Developers        |
| Charles  | Developer  | Developers, Audit |
| David    | Operations | Operations, Audit |
| Edward   | Operations | Operations        |
| Fred     | QA         | (none)            |

---

## 🧾 IAM Policies

- JSON documents that **define permissions**
- Can be attached to **users or groups**
- Example actions: Allow access to EC2, ELB, and CloudWatch

```json
{
  "Effect": "Allow",
  "Action": ["ec2:*", "elasticloadbalancing:*", "cloudwatch:*"],
  "Resource": "*"
}
