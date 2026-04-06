# 📌 Project Overview

## 🎯 Objective
The goal of this project was to secure remote access to an AWS EC2 instance by eliminating SSH and replacing it with a more secure alternative.

## 🏗 Architecture
- EC2 instance hosted in a public subnet
- IAM role attached to instance
- Route table configured for internet access
- No inbound SSH access

## 🔐 Security Approach
Traditional SSH access exposes servers to the internet. This project replaces it with AWS Systems Manager Session Manager, which:
- Uses IAM authentication
- Does not require open ports
- Provides logging and auditing

## 🚀 Outcome
A secure, scalable, and production-style access method aligned with cloud security best practices.
