# Week 3 – Package Management and Software Installation

[← Previous Week](week2.md) | [Next Week →](week4.md)

## Overview
Week 3 focused on managing software packages on the Linux server. This included updating the system, upgrading installed packages, installing new software, and verifying that services and applications run correctly.

## System Updates
The package list was updated to ensure the system was aware of the latest available software versions.

**Command used:**  
`sudo apt update`

![APT update](images/week3_apt_update.png)

---

## System Upgrade
Installed packages were upgraded to their latest versions to improve security and stability.

**Command used:**   
`apt list --upgradble`

![APT upgrade](images/week3_apt_upgrade.png)

---

## Software Installation
The htop package was installed to provide an interactive process monitoring tool.

**Command used:**  
`sudo apt install htop`

![Install htop](images/week3_install_htop.png)

---

## Software Verification
The installed software was executed to confirm successful installation.

**Command used:**  
`htop`

![htop running](images/week3_htop_running.png)

---

## Review
Week 3 developed practical skills in Linux package management using the APT package manager. Updating and upgrading the system reinforced good maintenance practices, while installing and verifying new software demonstrated effective software management within a Linux server.
