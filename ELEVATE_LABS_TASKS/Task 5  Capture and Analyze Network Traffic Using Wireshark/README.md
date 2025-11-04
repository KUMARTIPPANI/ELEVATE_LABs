# 🌐 Cyber Security Internship — Task 5  
## Capture and Analyze Network Traffic Using Wireshark  

### 🎯 Objective  
The goal of this task was to use **Wireshark** to capture live network packets and analyze the data to understand how different network protocols work. The objective was to develop practical knowledge of packet capturing, network protocol identification, and traffic analysis.

### 🧰 Tools Used  
- **Tool:** Wireshark (Free and Open Source)  
- **Operating System:** Kali Linux (can also be used on Windows)  
- **File Format:** .pcap (Packet Capture File)  

### 🧭 Steps I Followed  
I started the task by installing Wireshark on my system using the command `sudo apt install wireshark -y` in Kali Linux. After installation, I launched Wireshark from the applications menu. Once the interface opened, I selected my active network interface (eth0/WLAN) to begin capturing live packets. I clicked on the “Start Capturing” button to begin monitoring network traffic in real time. While Wireshark was capturing packets, I performed simple network activities such as browsing a few websites, performing Google searches, and pinging external servers using `ping google.com` in the terminal. These actions generated live traffic across various network protocols. After around one minute, I clicked on the red stop button to stop the capture process. The captured packets appeared in a list showing details such as source and destination IPs, protocols used, packet length, and info.  

Next, I applied filters in Wireshark to analyze specific types of traffic. For example, I used filters like `http`, `dns`, and `tcp` in the top filter bar to isolate packets of those types. This helped me study the flow of data in each protocol individually. In the **HTTP packets**, I could see browser requests and responses between my system and web servers. In the **DNS packets**, I observed the process of domain name resolution where my system queried DNS servers to resolve website names to IP addresses. In the **TCP packets**, I saw the handshake process that establishes communication between devices, including the SYN, SYN-ACK, and ACK packets. I also noted the difference between TCP (reliable and connection-oriented) and UDP (unreliable but faster).  

After identifying these protocols, I went to **File → Export Specified Packets → Save As**, and saved the captured traffic as a `.pcap` file for documentation. This file can be opened anytime later in Wireshark to reanalyze the same traffic data.  

### 📊 Protocols Identified  
- **HTTP (HyperText Transfer Protocol):** Used for web communication between browser and web servers.  
- **DNS (Domain Name System):** Converts domain names into IP addresses for easier access.  
- **TCP (Transmission Control Protocol):** Handles reliable data transmission between systems.  

### 🧠 What I Learned  
This task gave me practical exposure to how data travels over the internet and how protocols work together in the TCP/IP model. I learned how to use Wireshark to capture, filter, and analyze different network packets. I understood how each protocol plays a specific role in communication — from domain resolution (DNS) to establishing reliable connections (TCP) and data exchange (HTTP). I also learned how packet analysis helps in detecting network issues, suspicious traffic, and even security breaches.  

### ✅ Conclusion  
This was one of the most interesting tasks as it provided hands-on experience in **network packet analysis**. Using Wireshark, I observed how devices communicate in real time and gained insights into the structure of packets, protocols involved, and their functions. This task improved my understanding of how network monitoring tools can be used for **security analysis and troubleshooting**. It also highlighted the importance of encrypted traffic (like HTTPS) for privacy, as Wireshark cannot decrypt such packets. Overall, this task enhanced my practical knowledge of **network behavior, data flow, and security monitoring**.

### 📁 Repository Contains  
- Wireshark capture file (.pcap)  
- Screenshots of capture and filtered packets  
- This README.md file  

**Completed By:** ELEVEATE LABS Cyber Security Intern  
**Task:** Capture and Analyze Network Traffic Using Wireshark
