  Cyber Security Internship Task 4 — Firewall Configuration

🧩 Objective
Configure and test basic firewall rules on Windows or Linux to understand how firewalls manage and filter network traffic.  
By completing this task, you’ll gain hands-on experience with inbound/outbound rules and traffic filtering.



🧱 What is a Firewall?
A firewall is a network security tool that monitors and controls incoming and outgoing traffic based on predefined rules.  
It acts as a barrier between a trusted internal network and untrusted external networks like the Internet.



⚙️ Task Steps (Windows Version)

 🪟 1. Open Windows Defender Firewall
- Press `Windows + R` → type `wf.msc` → hit Enter.  
- This opens Windows Defender Firewall with Advanced Security.



 🧾 2. View Existing Rules
- Click Inbound Rules and Outbound Rules in the left pane.  
- Observe which apps or ports are already allowed or blocked.  
    "Take a screenshot for documentation."



 3. Block Port 23 (Telnet)
1. Click Inbound Rules → New Rule  
2. Select Port → TCP → enter `23` → Next  
3. Choose Block the connection → Next  
4. Apply to Domain, Private, and Public → Next  
5. Name it: `Block Telnet Port 23` → Finish

 "Take a screenshot of the rule created."



  4. Test the Rule
Open Command Prompt and run:
```bash
telnet localhost 23
