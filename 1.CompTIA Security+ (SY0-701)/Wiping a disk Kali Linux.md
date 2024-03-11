 1. Start and login to your Kali Linux virtual machine as user kali with a password of kali. 
 2. Open a terminal window. 
 3. Type `sudo fdisk -l`. You will be prompted to enter the password for kali. Enter kali and press ENTER. 
 4. Notice the device listing for /dev/sdb. The OS is running from /dev/sda; sda has multiple partitions listed such as sda1, sda2 and so on. 
 5. Create and format a disk partition on /dev/sdb with the following commands:   
    1. `sudo fdisk /dev/sdb `
    2. Type `n` for new partition 
    3. Type `p` for primary 
    4. Press ENTER to accept the rest of the defaults until you return to the Command (m for help): prompt. 
    5. Press `w` to write the changes to disk. 
 6. Format the new partition by typing `sudo mkfs -t ext4 /dev/sdb1`. 
 7. Create a mount point directory for the newly created disk partition by typing `sudo mkdir /datavol`. 
 8. Mount the disk partition in the newly created folder by typing `sudo mount /dev/sdb1 /datavol`. 
 9. Create some sample text files by typing `sudo touch /datavol/file{1,2,3}.txt`. 
 10. View the files by typing `sudo ls /datavol`. 
 11. Now wipe the new disk partition by filling it with random data. Type `sudo dd if=/dev/urandom of=/dev/sdb1`. This will take a few minutes to complete. 
 12. Type `sudo ls /datavol`; this time the sample text files are not listed; the partition has been wiped. 
 13. Type `sudo umount /dev/sdb1` to unmount the wiped disk partition.