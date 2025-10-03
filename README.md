Firewall Task – Kali Linux (UFW)

Objective

The goal of this task was to configure and test a basic firewall on Linux (Kali) using UFW. I practiced adding, removing, and verifying rules for different ports.

Steps Performed

1)Installed and enabled UFW

sudo apt update
sudo apt install ufw -y
sudo ufw enable


2)Checked current firewall rules

sudo ufw status verbose


3)Added a rule to block inbound traffic on port 23 (Telnet)

sudo ufw deny 23


4)Tested the rule by trying Telnet connection (failed as expected)

telnet localhost 23


5)Allowed SSH on port 22

sudo ufw allow 22


6)Removed the test rule (unblocked port 23)

sudo ufw delete deny 23

Screenshots

All screenshots of each step are available in the /screenshots/ folder.
