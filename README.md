AWS EC2 & EBS Volume Management
About the Project
A hands-on AWS project focused on deploying an EC2 instance and managing EBS volumes for persistent storage. The project demonstrates cloud infrastructure fundamentals including compute provisioning, storage management, and Linux system administration.
Key Learnings
AWS EC2 instance provisioning and configuration
EBS volume creation, attachment, and management
Linux disk formatting and mounting
Persistent storage implementation
Snapshot-based backup and recovery
AWS Services Used
Amazon EC2
Amazon EBS
Security Groups
Tech Stack
Linux (Ubuntu / Amazon Linux)
Bash Shell
SSH
AWS CLI (basic)
Architecture
User → EC2 Instance → EBS Volume → Mounted Storage (/data)
Implementation Steps
Launched an Ubuntu EC2 instance and configured Security Groups for SSH access
Created a gp3 EBS volume in the same Availability Zone as EC2
Attached the EBS volume to the running EC2 instance
Connected to the instance using SSH
Verified disk using lsblk
Formatted the EBS volume using ext4 filesystem
Created mount point /data
Mounted the volume to the EC2 instance
Verified persistent storage using df -h
Created an EBS snapshot for backup and recovery
Outcome
Successfully implemented persistent storage on AWS using EC2 and EBS, along with Linux system administration and cloud storage management.
Author
Tarfi Ansari
Cloud & DevOps Enthusiast
