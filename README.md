🚀 AWS EC2 & EBS Volume Management
  📌 About the Project
A hands-on AWS project focused on deploying an EC2 instance and managing EBS volumes for persistent storage. This project demonstrates core cloud infrastructure skills including compute provisioning, storage management, and Linux system administration.
   What I Learned
AWS EC2 instance provisioning and configuration
EBS volume creation, attachment, and management
Linux disk formatting and mounting
Persistent storage setup
Snapshot-based backup and recovery
☁️ AWS Services Used
Amazon EC2
Amazon EBS
Security Groups
AWS Console
🛠️ Tech Stack
Linux (Ubuntu / Amazon Linux)
Bash Shell
SSH
AWS CLI (basic)
  Architecture
User → EC2 Instance → EBS Volume → Mounted Storage (/data)
⚙️ Implementation Steps
1. EC2 Setup
Launched an Ubuntu EC2 instance
Configured Security Group for SSH access
2. EBS Volume Creation
Created a gp3 EBS volume
Ensured same Availability Zone as EC2
3. Attach Volume
Attached EBS volume to EC2 instance
4. Connect to Instance
ssh -i key.pem ubuntu@<EC2-PUBLIC-IP>
5. Verify Disk
lsblk
6. Format Disk
sudo mkfs -t ext4 /dev/xvdf
7. Create Mount Point
sudo mkdir /data
8. Mount Volume
sudo mount /dev/xvdf /data
9. Verify Mount
df -h
10. Snapshot Backup
Created EBS snapshot for data backup and recovery.
  Evidence
EC2 instance running
EBS volume attached
Mounted filesystem output
Snapshot created
📈 Outcome
Successfully implemented persistent storage on AWS using EC2 and EBS, along with Linux-based system administration and cloud storage management.
👨‍💻 Author
Tarfi Ansari
Cloud & DevOps Enthusiast
