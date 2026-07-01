# AWS EC2 & EBS Volume Management - Steps

## 1. Launch EC2 Instance
- Created an EC2 instance using Ubuntu (t2.micro)
- Allowed SSH access through security group (port 22)
- Downloaded the key pair for login

---

## 2. Create EBS Volume
- Created a new EBS volume (gp3) from AWS console
- Kept it in the same Availability Zone as EC2 instance

---

## 3. Attach Volume to EC2
- Attached the EBS volume to the running EC2 instance
- Verified the volume is showing as “in-use” in AWS console

---

## 4. Connect to EC2
- Connected to the instance using SSH

ssh -i devops-key.pem ubuntu@65.2.180.45

---

## 5. Check Attached Disk
- Verified the new disk using:

lsblk

---

## 6. Format the Volume
- Formatted the attached EBS volume with ext4 filesystem

sudo mkfs -t ext4 /dev/xvdf

---

## 7. Create Mount Directory
- Created a directory to mount the volume

sudo mkdir /data

---

## 8. Mount the Volume
- Mounted the EBS volume to the directory

sudo mount /dev/xvdf /data

---

## 9. Verify Mount
- Checked if the volume is properly mounted

df -h

---

## 10. Snapshot Backup
- Created a snapshot of the EBS volume from AWS console for backup purposes

---

## Outcome
- Successfully attached and configured EBS volume with EC2
- Learned how persistent storage works in AWS
- Practiced basic Linux disk management and AWS storage concepts
