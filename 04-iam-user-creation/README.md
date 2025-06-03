# 👥 04 - IAM User & Group Creation (Hands-on)

In this module, we practiced how to securely manage IAM users, groups, and permissions using the AWS Console.

---

## ✅ Key Takeaways

### 🌍 IAM is a Global Service
- IAM is not tied to a specific AWS region.
- You cannot select a region when using IAM.

---

### 👤 IAM User Creation

- A **root user** is created when the AWS account is set up.
- It is **not recommended** to use the root user for daily operations.
- Instead, create an **admin-level IAM user**.

### Steps Taken:
1. Navigated to IAM console
2. Created a user named `Stephane`
3. Gave user **console access**
4. Set a **custom password** (disabled "require password reset")
5. Created a group named `admins` with the `AdministratorAccess` policy
6. Added the user to the group

---

### 🛡️ Permission Inheritance
- IAM users **inherit permissions from their group**.
- Stephane did **not have a policy attached directly**, but gained `AdministratorAccess` via the group `admins`.

---

### 🏷️ Optional: Tagging Resources
- Tags can include metadata such as:
  - `Department: Engineering`
- Tags help with organisation and billing, but are optional.

---

## 🔐 IAM vs. Root User: Visual Tip

| User Type   | Display in Console         | Usage Recommendation |
|-------------|----------------------------|------------------------|
| Root User   | Top-right shows Account ID only | ❌ Avoid daily use |
| IAM User    | Top-right shows Account ID + Username | ✅ Use for day-to-day |

---

## 🔗 Custom Sign-in URL

- A sign-in alias (e.g., `aws-stephane-v5`) was created
- This makes sign-in easier with a memorable link:  
  `https://aws.amazon.com/console/aws-stephane-v5`

---

## 🧪 Browser Tip

To test IAM and root users **at the same time**:
- Use a normal window for root
- Use a **private/incognito window** for IAM user login

---

## 💬 Reflection

> IAM user and group creation is one of the most essential steps for secure AWS account management. Creating granular permissions and avoiding root usage are best practices every AWS administrator should follow.
