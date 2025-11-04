# Phishing Email Analysis — ELEVEATE LABS

This README explains how I analyzed a suspicious phishing-style email on **Kali Linux**, documents the findings from the email headers and HTML content, lists the artifacts I saved, and shows how to upload the work to GitHub.

**Evidence file:** `36339167-8284-484f-a0f4-696d059b3b42.jpg` (screenshot of the email)

---

## What I did (simple steps)
1. Opened the email image in Kali and saved a screenshot as the evidence file.  
2. Viewed the email raw headers (from the original .eml or mail client) to trace delivery path and authentication results.  
3. Inspected the HTML body to check links, images, and hidden tracking pixels.  
4. Noted red flags, listed findings and recommendations, and saved everything in a project folder.

---

## Commands and tools I used
- View network / interface (if needed): `ip a`  
- View or open the saved .eml / text file: `less email.eml` or open with a text editor.  
- Take a window screenshot: `gnome-screenshot -w -f 36339167-8284-484f-a0f4-696d059b3b42.jpg`  
- Move files into project folder: `mkdir -p ~/Phishing_Email_Task && mv 36339167-8284-484f-a0f4-696d059b3b42.jpg ~/Phishing_Email_Task/`  
 
