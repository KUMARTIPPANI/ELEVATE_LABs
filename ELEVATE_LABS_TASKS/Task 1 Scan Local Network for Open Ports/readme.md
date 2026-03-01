This repo is for Task 1 of the Elevate Labs Cyber Security Internship: Scanning my local network for open ports using Nmap.

I started by downloading and installing Nmap from their official site. Then, I checked my local IP range—it was something like 192.168.1.0/24 using the ipconfig command.

Next, I ran a TCP SYN scan with: nmap -sS 192.168.1.0/24. It found a few devices with open ports, like port 80 on one IP for HTTP, and port 22 on another for SSH.

I jotted down the IPs and ports, researched what services they might be running (e.g., web servers or remote access), and thought about risks like hackers exploiting them if not secured.

I didn't save the full results file, but I have screenshots of the commands and outputs. Optionally, I used Wireshark to sniff the packets during the scan, which was cool to see the SYN packets flying around.

From this, I learned basics of network recon and why open ports can be risky. For security, I'd recommend firewalls to block unnecessary ports and keeping software updated.
GitHub steps I followed:
1. Created a new repo named ELEVATE_LABs-INTERNSHIP-Task1.
2. Cloned it locally with git clone.
3. Added this README, screenshots, and any text files.
4. Committed with git commit -m "Task 1 done".

5. Pushed with git push.
