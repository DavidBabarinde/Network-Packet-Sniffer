# 🕵️‍♂️ Network Packet Sniffer

A Python-based network sniffer using **Scapy** that captures and logs network packets in real time.

## 🚀 Features
- Captures **live network traffic** on a specified interface.
- Supports **protocol filtering** (ARP, BOOTP, ICMP).
- Logs **source & destination MAC addresses** with timestamps.
- Allows **custom packet count & timeout settings**.
- Runs in **promiscuous mode** to capture all packets on the network.

## ⚙️ Installation
Make sure you have **Python 3** and **Scapy** installed.

### **1️⃣ Clone the repository**
```sh
git clone https://github.com/your-username/network-packet-sniffer.git
cd network-packet-sniffer

## 2️⃣ Install Dependencies
pip install scapy

🎯 Usage
Run the script as root/admin: sudo python3 packet_sniffer.py
You will be prompted to:
	•	Select a network interface (e.g., eth0, wlan0).
	•	Choose the number of packets to capture.
	•	Set a time limit for sniffing.
	•	Apply an optional protocol filter (ARP, BOOTP, ICMP).

##📜 Example Output
* Enter the interface on which to run the sniffer (e.g. 'eth0'): wlan0
* Enter the number of packets to capture (0 is infinity): 10
* Enter the number of seconds to run the capture: 5
* Enter the protocol to filter by (arp|bootp|icmp|0 is all): icmp
* Please give a name to the log file: packets_log.txt

✅ Interface wlan0 set to PROMISC mode.
✅ Capturing ICMP packets for 5 seconds...
✅ Log saved to packets_log.txt
