
**Title:**  "[Anthem] - TryHackMe"

**Date:**  14-12-2025

**Difficulty:** Easy

**Time to complete:** ~2 hours

**Url:**  https://tryhackme.com/room/anthem

## categories:

- Nmap scan

- Gobuster

- rdesktop

## ScreenShots:
1-https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/anthem%20nmap.jpg

2-https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/anthem%20gobuster.jpg

3-https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/anthem%20robots.txt.jpg

4.https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/anthem%20backup%20file.jpg

## Skills gained:
- using nmap to scan open ports and exploit them
- finding hidden directories by using gobuster
- rdesktop --> a vritual machine for windows in kali linux 
  
## Goal

to exploit windows machine 
## Tools Used

- Nmap

- Gobuster

- rdesktop


## Attack Chain 
- nmap -->ip-target .... gobuster for the hidden directories .... 
- rdesktop -->virtual windows machine ....
-  social engineering --> noted the full names of the authors .. tried their names as an username and password in the windows virtaul machine
- reaching to the hidding files through control panel .... then changing the security settings of the hidden file "backup"  for safely access, which includes the password of the adminstrator.
## Root Cause
1-  Website exposed employee full names publicly
2-No multi-factor authentication
3-No encryption on sensitive configuration files

## Mitigation

1-Enforce strong password policy.
2-Remove sensitive backup files from user-accessible directories
