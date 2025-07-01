# AWS VPC Peering – EC2 Communication Across VPCs

This project demonstrates the setup of **VPC-to-VPC peering** using the AWS Management Console to enable **private communication** between EC2 instances in two different VPCs.

## 🧱 Architecture

![Architecture](architecture.png)

- **Test VPC (10.0.0.0/16)** – Includes public & private subnets
- **Prod VPC (192.168.0.0/16)** – Public subnet with EC2 instance
- **VPC Peering** established between both VPCs
- **Route Tables** updated for bidirectional communication
- **Security Groups** configured for ICMP and SSH traffic

## 🚀 Steps Followed

1. Created 2 VPCs with distinct CIDRs
2. Launched EC2 instances in public subnets
3. Set up a VPC Peering connection and accepted it
4. Updated route tables to allow inter-VPC traffic
5. Modified security groups to allow ICMP (ping) and SSH
6. Verified connectivity using private IPs between EC2s

## 📸 Screenshots (Optional)
- Route tables
- Peering connection
- Security groups
- Ping or SSH success

## 💡 Learnings
- How to configure secure VPC networking
- Route propagation and static routing in AWS
- Importance of CIDR planning and SG rules

## 🔧 Future Improvements
- Automate with Terraform
- Add monitoring/logging with CloudWatch
