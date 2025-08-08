🔥 Task 4 – Setup and Use a Firewall on Linux (UFW)




🎯 Objective
Configure and test basic firewall rules to control network traffic using UFW (Uncomplicated Firewall) on Kali Linux.

🛠 Tools Used
UFW – User-friendly firewall management tool for Linux

Kali Linux – Security-focused Linux distribution

🚀 Steps Performed
1️⃣ Enable UFW
bash
Copy
Edit
sudo apt install ufw -y
sudo ufw enable
sudo ufw status verbose
✅ Verified UFW status.

2️⃣ List Current Rules
bash
Copy
Edit
sudo ufw status numbered
3️⃣ Block Inbound Traffic on Port 23 (Telnet)
bash
Copy
Edit
sudo ufw deny 23/tcp
sudo ufw status numbered
4️⃣ Test the Rule
bash
Copy
Edit
telnet localhost 23
❌ Connection attempt failed, confirming the block.

5️⃣ Allow SSH (Port 22)
bash
Copy
Edit
sudo ufw allow 22/tcp
sudo ufw status numbered
6️⃣ Remove the Telnet Block Rule
bash
Copy
Edit
sudo ufw delete <rule_number>
sudo ufw status numbered
📄 Summary
In this task, the following was accomplished:

Enabled UFW and checked its status

Listed current firewall rules

Added a rule to block Telnet (port 23)

Tested the rule to ensure traffic was blocked

Allowed SSH (port 22) access

Removed the Telnet block to restore the original state

📂 Report
📎 Click here to view the full PDF report with screenshots

📌 Author
Abhinraj
💼 Cybersecurity Enthusiast | SOC Analyst | Penetration Tester
