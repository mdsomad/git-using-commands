# AWS Linux & And Ubuntu UseFull Commands

## 👇 AWS Linux & And Ubuntu local machine from file transfer server machine (ssh) Command

```sh
sudo scp -r -i ssh -i "instance_Key_namme" folder_name ubuntu@ec2-43-205-182-153.ap-south-1.compute.amazonaws.com:local_machine_folder_path_enter

# 👇 Example command
# sudo scp -r -i ssh -i "instanceKey.pem" my-server ubuntu@ec2-43-205-182-153.ap-south-1.compute.amazonaws.com:/home/ubuntu/server

```

## 👇 Yah Hai Sarvar ka PORT Change karne ka command

```sh
export PORT=3000
```

## 👇 Ubuntu Install nginx Commands

```sh
# 👇 yah command se check kar sakte hain nginx install hai kya Nahin

sudo nginx -t
```

```sh
apt-get update
```

```sh
sudo apt install nginx
```

```sh
# 👇 yah command sa nginx ka service & Running check kar sakte hain

service nginx status
```

```sh
# 👇 yah command se nginx ka start kar sakte hain

service nginx start
```

```sh
curl localhost
```

```sh
echo "this is $(hostname)" > /var/www/html/index.html
```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## 👇 Volume Attach & Mount

### Commands Started

- 👇 Volumes & Disk List Show

```sh
lsblk
```

- 👇 Login

```sh
sudo su
```

- 👇 EBS Volume ext4 Format command

```sh
mkfs.ext4 /dev/xvdb
```

- 👇 Create Folder 📁

```sh
mkdir /test
```

- 👇 Volume mount command

```sh
mount /dev/xvdb /test
```

- 👇 Check Mount Volume

```sh
mountpoint /test
```

- 👇 Go Test Folder 📁

```sh
cd /test/
```

- 👇 Testing Create 📄files

```sh
touch 12345678945544

echo "welcome Testing File">demo_for_somadfile.txt
```

- 👇 Show All 📄file & 🗂️ directory

```sh
ls
```

- 👇 Read 📄file

```sh
cat demo_for_somadfile.txt
```

- 👇 Back Folder

```sh
cd ..
```

- 👇 Volume umount command

```sh
umount /test/
```

### Commands End

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## 👇 Old EC2 Instances Detach EBS Volume Then New EC2 Instances Attach Volume Attach & Mount

### Detach an EBS volume from one EC2 Instance and Attach it Another One

### Commands Started

- 👇 Volumes & Disk List Show

```sh
lsblk
```

- 👇 Yah command se check kar sakte hain volume Mein data hai kya Nahin Agar result data Aaya to volume Mein data Nahin Hai Aur Agar result ext4 filesystem Aaya to volume Mein data Hai

```sh
file -s /dev/xvdb
```

- 👇 Create Folder 📁

```sh
mkdir /datat
```

- 👇 Volume mount command

```sh
mount /dev/xvdb /data
```

- 👇 Check Mount Volume

```sh
mountpoint /data
```

- 👇 Go Test Folder 📁

```sh
cd /data/
```

- 👇 Old Instances data New Instances Show data & exist

```sh
ls
```

- 👇 Read 📄file

```sh
cat demo_for_somadfile.txt
```

### Commands End

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## 👇 Resize EBS Volume and Resize the File System

### Commands Start

- 👇 Volumes & Disk List Show

```sh
lsblk
```

- 👇 Check File System

```sh
df -h
```

- 👇 Resize File System

```sh
resize2fs /dev/xvdf
```

### Commands End

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## 👇 Resize ROOT EBS Volume

### Commands Start

- 👇 Volumes & Disk List Show

```sh
lsblk
```

- 👇 Check File System

```sh
df -h
```

- 👇 yah command se file system ko check kar sakte hain

```sh
sudo file -s /dev/xvda1
```

- 👇 login root user

```sh
sudo -i
```

```sh
growpart /dev/xvda 1
```

```sh
lsblk
```

```sh
df -h
```

- 👇 Resize File System

```sh
resize2fs /dev/xvda1
```

- 👇 Check File System

```sh
df -h
```

### Commands End

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## Create First Snapshot - EBS Backup

```sh
lsblk
```

```sh
# 👇 Yah command se check kar sakte hain volume Mein data hai kya Nahin Agar result data Aaya to volume Mein data Nahin Hai Aur Agar result ext4 filesystem Aaya to volume Mein data Hai
file -s /dev/xvdb
```

```sh
sudo
```

```sh
# Login
sudo -i
```

```sh
# Format EBS volume
mkfs.ext4 /dev/xvdb
```

```sh
# 👇 Yah command se check kar sakte hain volume Mein data hai kya Nahin Agar result data Aaya to volume Mein data Nahin Hai Aur Agar result ext4 filesystem Aaya to volume Mein data Hai
file -s /dev/xvdb
```

```sh
mkdir /data
```

```sh
mount /dev/xvdb /data
```

```sh
mountpoint /data
```

```sh
ls
```

```sh
claer
```

```sh
# Sample File Craeated
yes "somad">> abc.txt
```

```sh
Ctrl C
```

```sh
# Check File Size
ls -lh
```

```sh
# Check volume use Size
df -h
```

```sh
# Create test file
echo "this is now file in ebs volume"> /data xyz.txt
```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## Backup Snapshot Restore

### Commands Started

```sh
lsblk
```

```sh
# 👇 Yah command se check kar sakte hain volume Mein data hai kya Nahin Agar result data Aaya to volume Mein data Nahin Hai Aur Agar result ext4 filesystem Aaya to volume Mein data Hai
file -s /dev/xvdf
```

```sh
cd ..
```

```sh
# Craete Folder
mkdir /dataone
```

```sh
mount /dev/xvdf /dataone/
```

```sh
# Check mountpoint
mountpoint /dataone
```

```sh
cd /dataone
```

```sh
ls
```

### Commands End

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## Shell Script

### User Data

```sh
#!/bin/bash

apt-get update
apt-get intall nginx -y
service ngnix start
echo "this is $(hostname)" > /var/www/html/index.html







#!/bin/bash
apt-get update
apt-get install nginx -y
service nginx start
echo "this is $(hostname)" > /var/www/html/index.html






#!/bin/bash

apt-get update
apt-get install nginx -y

echo "this is $(hostname)" > /var/www/html/index.html

service nginx start

```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

```sh
sudo apt-get update
sudo apt-get install stress

# 👇 cpu check
top
#👇 Yah Command se CPU ka load Badha sakte hain
stress -c 5






name first-asg

```
