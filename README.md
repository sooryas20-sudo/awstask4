# AWS Task 4 - EC2 + EBS Volumes + Snapshots

## Task Overview
- Launched Linux and Windows EC2 instances with web servers
- Created 5GB EBS volume and attached to both instances
- Took EBS snapshot and created new volume from snapshot

## Tech Stack
- AWS EC2 (Linux + Windows)
- AWS EBS (Elastic Block Store)

## Steps Performed

### Linux EC2
- AMI: Amazon Linux 2023
- Web server: Nginx (auto-installed via user_data)
- EBS volume mounted at /mydata

### Windows EC2
- AMI: Windows Server 2022
- Web server: IIS (auto-installed via PowerShell user_data)
- EBS volume initialized via Disk Management as E: drive

### EBS Operations
1. Created 5GB gp2 EBS volume
2. Attached to Linux EC2 → formatted → mounted at /mydata
3. Created snapshot of the volume
4. Created new 5GB volume from snapshot
5. Attached snapshot volume to Windows EC2

## Screenshots
See /screenshots folder for all output proofs.
