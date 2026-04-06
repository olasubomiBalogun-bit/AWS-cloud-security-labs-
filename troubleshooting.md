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




##  Key Lesson
Cloud issues are often a combination of:
- IAM misconfiguration
- Networking misconfiguration


