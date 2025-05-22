# 🛡️ AWS IAM Role-Based Access Control Simulation

## 📉 Project Summary
This project simulates a real-world implementation of **Role-Based Access Control (RBAC)** in AWS using **Identity and Access Management (IAM)**. It demonstrates how to create and manage IAM users, groups, and custom policies. It also includes permission testing to verify policy behavior.

---

## 🔺 Objectives
- Create custom IAM policies for specific job functions.
- Organize users into groups and manage permissions through group policies.
- Attach permission boundaries where needed.
- Log in as users to test and validate permissions.
- Showcase group policy inheritance and management efficiency.

---

## 🔧 Tools & Services Used
- AWS IAM Console
- IAM Policy JSON Editor
- AWS Management Console (for testing)

---

## 🔮 Key Roles Simulated
- **Developer** (`developer01`)
- **Analyst** (`analyst01`)
- **Junior Developer** (`juniorDev`)
- **Admin** (`adminUser`)

---

## 💪 Actions Performed
### 1. **Created Custom Policies**
Example:
```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Action": ["ec2:DescribeInstances", "s3:ListBucket"],
      "Resource": "*"
    }
  ]
}
```

### 2. **Created Groups and Attached Policies**
- Developers Group → Developer Policy
- Admins Group → Full Access Policy
- Analysts Group → Read-only access

### 3. **Created IAM Users and Assigned Groups**
- Users were added to groups based on job functions.

### 4. **Permission Boundary Testing**
- Explored attaching permission boundaries to control max permissions (optional).

### 5. **User Access Testing**
- Logged in as different users.
- Tried actions like:
  - Launch EC2
  - List S3 Buckets
  - Access IAM console
- Verified access based on permissions.

---

## 🔐 Key Concepts Practiced
- Least Privilege Principle
- Group vs. User Policy Attachment
- Permission Boundaries
- Access Inheritance

---

## 📷 Screenshots (Suggestions)
- IAM Dashboard
- Custom Policy Editor
- User Group Membership
- Access Denied / Access Allowed Test Cases

---

## ✅ Project Outcome
- Successfully created and tested a scalable, secure IAM structure.
- Demonstrated policy behavior via real-world login simulations.
- Validated best practices in AWS identity management.

---

## 🚀 What to Improve Next
- Implement MFA across all users.
- Integrate with AWS CloudTrail to log IAM activity.
- Automate with Terraform or AWS CLI.
- Add role-switching and advanced trust relationships.

---

## 📊 Related Topics
- AWS Security Best Practices
- Zero Trust Model
- Identity Federation

---

## 🎓 Credits
Project built and tested by **Ekeoma Miracle** as part of IAM training and access control simulation.

Feel free to fork, test, and extend this IAM setup!
