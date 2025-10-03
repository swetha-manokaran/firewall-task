Firewall Task – Kali Linux (UFW)
🔹 Objective

The goal of this task was to configure and test a basic firewall on Linux (Kali) using UFW. I practiced adding, removing, and verifying rules for different ports.

🔹 Steps Performed

Installed and enabled UFW

sudo apt update
sudo apt install ufw -y
sudo ufw enable


Checked current firewall rules

sudo ufw status verbose


Added a rule to block inbound traffic on port 23 (Telnet)

sudo ufw deny 23


Tested the rule by trying Telnet connection (failed as expected)

telnet localhost 23


Allowed SSH on port 22

sudo ufw allow 22


Removed the test rule (unblocked port 23)

sudo ufw delete deny 23

🔹 Screenshots

All screenshots of each step are available in the /screenshots/ folder.
