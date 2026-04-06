# 🛠 Troubleshooting

## ❌ Issue 1: SSM Not Connecting
Error:
SSM Agent unable to acquire credentials

### Cause
No IAM role attached to EC2

### Solution
Attach role with AmazonSSMManagedInstanceCore policy

---

## ❌ Issue 2: Still Not Working After Role
### Cause
Subnet not associated with route table

### Solution
Associate subnet with correct route table

---

##  Issue 3: No Internet Connectivity
### Cause
Missing route:
0.0.0.0/0 → Internet Gateway

### Solution
Add route to enable outbound access

![image](https://github.com/user-attachments/assets/5c7fcaf6-4dc9-4c65-9f08-33b6208c44ef)

![image](https://github.com/user-attachments/assets/300915f9-f39e-4287-bd6a-083363c04570)



##  Key Lesson
Cloud issues are often a combination of:
- IAM misconfiguration
- Networking misconfiguration


