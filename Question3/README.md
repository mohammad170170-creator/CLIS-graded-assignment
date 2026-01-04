## Commands and Explanations

1. **File Creation**
Command:
echo "This is sample data for link testing" > sample_data.txt
# Question 3 – File Management, Links, and Disk Usage

## Objective
The objective of this question is to understand Linux file creation, hard and symbolic links, inode numbers, file metadata, and disk usage commands.

## Commands and Explanations

1. File Creation
Command:
echo "This is sample data for link testing" > sample_data.txt
Explanation: Creates a file with sample text.

2. Hard Link Creation
Command:
ln sample_data.txt sample_hard.txt
Explanation: Creates a hard link. Shares the same inode as the original file.

3. Symbolic Link Creation
Command:
ln -s sample_data.txt sample_soft.txt
Explanation: Creates a symbolic link. Has a different inode and points to original file.

4. Inode Verification
Command:
ls -i sample_data.txt sample_hard.txt sample_soft.txt
Explanation: Shows inode numbers. Hard link shares inode, symbolic link does not.

5. File Metadata
Command:
stat sample_data.txt
Explanation: Displays permissions, size, ownership, timestamps.

6. Disk Usage
Command:
du -sh ~
Explanation: Shows total disk usage of home directory in human-readable format.

7. File Size Overview
Command:
ls -lh ~
Explanation: Shows size of all files in human-readable format.

8. Link Deletion Test
Command:
rm sample_soft.txt
ls sample_data.txt
Explanation: Deletes symbolic link without affecting original file.

9. du command demonstration
Command:
du -sh ~
du -h --max-depth=1 ~
Explanation: Shows disk usage of folders with different depth options.

10. df command demonstration
Command:
df -h
df -Th
Explanation: Shows disk space usage of filesystems.
Explanation: This command creates a file named sample_data.txt in my home directory and adds sample text to it.
# Question 3 – File Management, Links, and Disk Usage

## Objective
The objective of this question is to understand Linux file creation, hard and symbolic links, inode numbers, file metadata, and disk usage commands.
