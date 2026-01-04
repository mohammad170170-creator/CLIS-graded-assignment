# Question 4 – System Monitoring and Disk Usage

## Commands and Explanations

1. System Uptime Verification
Command:
uptime
Explanation: Shows time elapsed since last boot, number of users, and load average.

2. User Process Listing
Command:
ps -u $USER
Explanation: Lists all processes running under current user account.

3. CPU Usage Analysis
Command:
top -b -n 1 | sort -k9 -r | head -n 12
Explanation: Displays the processes consuming the highest CPU.

4. Background Process Execution
Command:
sleep 300 &
jobs
Explanation: Starts a command in background and verifies it is running.

5. Process Priority Management
Command:
ps -o pid,comm,nice -u $USER
renice -n 5 -p <PID>
Explanation: Changes the priority (niceness) of one of your own processes.

6. Memory Usage Monitoring
Command:
free -h
Explanation: Displays memory usage in a human-readable format.

7. Disk Space Inspection
Command:
df -h ~
Explanation: Shows disk space usage for filesystem containing home directory.

8. Shell Identification
Command:
echo $SHELL
Explanation: Displays the shell currently in use.

9. Output Redirection
Command:
uptime >> system_report.txt
free -h >> system_report.txt
df -h >> system_report.txt
Explanation: Redirects output of system commands into a file.

10. Disk Usage Visualization (Optional)
Command:
# ncdu ~  (Not installed, skipped)
Explanation: Interactive disk usage analyzer. Skipped because ncdu is not installed.
