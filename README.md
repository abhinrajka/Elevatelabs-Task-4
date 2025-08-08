# Linux Firewall Lab using UFW

## 📌 Objective
Configure and test basic firewall rules on Kali Linux using **UFW (Uncomplicated Firewall)** to control inbound and outbound traffic.

## 🛠 Tools Used
- **Operating System:** Kali Linux  
- **Firewall Tool:** UFW (Uncomplicated Firewall)  

---

## 🔹 Steps Performed

### 1️⃣ Enable UFW
```bash
sudo apt install ufw -y
sudo ufw enable
sudo ufw status verbose

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
Expected Result: Connection should fail.

5️⃣ Allow SSH on Port 22
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
UFW is a simple yet powerful firewall management tool for Linux.

In this lab, we:

Enabled UFW and checked its status.

Listed existing firewall rules.

Blocked Telnet access on port 23 and confirmed the block.

Allowed SSH traffic on port 22.

Removed the Telnet block to restore the default state.

Outcome:
Successfully learned and demonstrated basic firewall management techniques on Linux using UFW.

📂 Repository Contents
README.md – Documentation with steps and screenshots.

Screenshots – Images demonstrating each step.

Task4_Firewall_Report.pdf – Full PDF report of the lab.
