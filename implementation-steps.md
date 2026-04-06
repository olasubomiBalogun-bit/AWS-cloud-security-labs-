# ⚙️ Implementation Steps

## Step 1: Create IAM Role
- Service: EC2
- Policy attached: AmazonSSMManagedInstanceCore

## Step 2: Attach Role to EC2
- Navigate to EC2 instance
- Actions → Security → Modify IAM Role
- Attach created role

## Step 3: Configure Networking
- Verified route table has:
  0.0.0.0/0 → Internet Gateway
- Associated subnet with route table

## Step 4: Connect via Session Manager
- EC2 → Connect → Session Manager
- Established connection successfully

## Step 5: Remove SSH Access
- Deleted inbound rule for port 22

## ✅ Result
Secure access achieved without exposing the instance to the internet.
