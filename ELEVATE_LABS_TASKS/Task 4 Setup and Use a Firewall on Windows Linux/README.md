# 🔥 Cyber Security Internship — Task 4  
## Setup and Use a Firewall on Linux (UFW)

### 🎯 Objective
The goal of this task was to configure and test basic firewall rules using **UFW (Uncomplicated Firewall)** in **Kali Linux**, to understand how network traffic is filtered and protected.

### 🧰 Tools Used
- Operating System: Kali Linux  
- Tool: UFW (Uncomplicated Firewall)  
- Environment: Linux Terminal  

### 🧭 Steps I Followed
I began by checking if UFW was installed and active using `sudo ufw status`. If not, I installed it with `sudo apt install ufw -y`. Then, I enabled the firewall with `sudo ufw enable` and viewed the current configuration using `sudo ufw status verbose`, which by default allows outgoing connections and denies incoming ones. Next, I added a rule to block port 23 (used by Telnet, which is insecure) using `sudo ufw deny 23`. To ensure I could still connect via SSH, I allowed port 22 using `sudo ufw allow 22`. I verified all the active rules by running `sudo ufw status numbered`, which displayed the list of allowed and denied ports. To test the rule, I ran `nc -zv localhost 23`, which showed “Connection refused,” confirming the Telnet port was blocked successfully. Once testing was complete, I restored the firewall to its original state by removing the rule with `sudo ufw delete deny 23`. Finally, I temporarily disabled the firewall using `sudo ufw disable`.

### 🧠 What I Learned
Through this task, I learned how to configure and manage a firewall using UFW on Linux. I understood how firewalls filter incoming and outgoing traffic, the importance of blocking unused or insecure ports like Telnet, and how to safely allow trusted connections like SSH. I also learned how UFW simplifies complex firewall configurations into easy-to-use commands.

### ✅ Conclusion
This task helped me gain practical experience in network security and firewall management. It taught me how to protect a system from unauthorized access by controlling network traffic. Using UFW, I could easily block risky ports, verify rules, and maintain a secure system configuration. This enhanced my understanding of how firewalls play a crucial role in securing both personal and enterprise networks.

### 📁 Repository Contains
- Screenshot of UFW rules from terminal  
- This README.md file  
- Terminal command outputs (optional evidence of configuration)

**Completed By:** ELEVEATE LABS Cyber Security Intern  
**Task:** Firewall Configuration using UFW on Kali Linux
