# Week 5 – System Logs and Scheduling

[← Previous Week](week4.md) | [Next Week →](week6.md)

## Overview
Week 5 was centered around monitoring system activity using logs and automating tasks using cron. System logs were inspected to understand service behaviour, and a scheduled task was created to demonstrate job automation.

## Command-Line Evidence

### System Logs
Recent system logs were viewed using journalctl to observe system events and messages.

**Command used:**
`journalctl -n 20`

![Recent logs](images/week5_journalctl_recent.png)

---

### SSH Logs
Logs related to the SSH service were inspected to verify authentication and service activity.

**Command used:**
`journalctl -u ssh`

![SSH logs](images/week5_ssh_logs.png)

---

### Cron Job Status (Initial)
The current user crontab was checked to verify whether scheduled tasks already existed.

**Command used:**
`crontab -l`

![Empty crontab](images/week5_crontab_empty.png)

---

### Cron Job Creation
A scheduled cron job was created to write a test message to a log file every minute.

**Command used:**
`crontab -l`

![Cron job added](images/week5_crontab_added.png)

---

### Cron Job Verification
The output file was checked to confirm that the cron job executed successfully.

**Command used:**
`cat /tmp/week5_cron.log`

![Cron output](images/week5_cron_output.png)

## Review
This week improved understanding of system monitoring and task automation. Inspecting logs using `journalctl` helped interpret system behaviour, while creating a cron job demonstrated how recurring administrative tasks can be automated on a Linux server.
