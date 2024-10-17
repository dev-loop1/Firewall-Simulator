# Firewall-Simulator
# The following code is only for Ubuntu.

### Features
1) Block IP addresses
2) Block access to certain ports 
3) Block specifed prefixes of IP address (to block networks)
4) Block too many requests made by the same IP in a short period of time (user can specify threshold and time)

### Steps to Run
1) Type the following terminal command: 
   sudo iptables -I INPUT -d 192.168.0.0/24 -j NFQUEUE --queue-num 1
2) Install the requirements netfilterqueue and scapy using pip 
3) Execute firewall.py using python3
### run it with sudo as -- sudo python3 /home/user/downloads/firewall-simulator/firewall.py

### Requirements
1) netfilterqueue
2) scapy
