# Resizing the root volume of ec2

## Steps
```bash
lsblk #list the blocks
sudo apt install cloud-guest-utils
sudo growpart /dev/xvda1 #grow partition to fullest avaialable volume
lsblk # check the blocks
df -h #check the disk size
sudo resize2fs /dev/xvda1 #resize disk
df -h #check the disk size 
```



