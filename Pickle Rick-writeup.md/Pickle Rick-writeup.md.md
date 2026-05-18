


**title:**  "[Pickle Rick] - TryHackMe"

**date:**  17-05-2026

**Difficulty:** Easy

**Time to complete:** ~2 Hours

**url:**  https://tryhackme.com/room/picklerick


## ScreenShots:
1. https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/pickle%20rick%20cd%20injection.jpeg

2. https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/pickle%20rick%20f12.jpeg

3. https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/pickle%20rick%20feroxbuster.jpeg

4. https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/pickle%20rick%20nikto.jpeg

5. https://github.com/ahmadqattan2001-art/TryHackMe-writeups/blob/main/screenshots/pickle%20rick%20nmap.jpeg
## Skills gained:

Command injection,  Automated web vulnerability scanner (Nikto).
## Goal

To find hidden strings, by inspecting the site source, and injecting a command in the Command panel for a Reverse Shell.
## Tools Used

- Nmap

- Feroxbuster

- Nikto
- Netcat (rlwrap)

- php reverse monkey

## Attack Chain (Red Team)
1. scanning for open services **(SSH, HTTP)**
2. discovering hidden directories   **(/assests.../robots.txt)**
3. scanning web server for known vulnerabilities, misconfigurations. **(/login.php)**
4. viewing the page source for any commands or mistakenly leaved comments
5. logging in
6. start listener
7. inject the reverse shell command
## Root Cause

leaving hardcoded secrets and easy discoverable directories leaded to  gain access to the Command Panel after successfully logging in to the user page.

 
## Mitigation

Not completely sure but removing any kind of leads to reverse shell connections would mitigate the problem.
