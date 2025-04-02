# 🔎 Wireshark Lab 1: DNS Traffic Analysis

**Date:** April 2025  
**Tool Used:** Wireshark  
**Focus:** Capturing DNS request/response traffic on a live network

---

## 🧪 Objective

Capture real-time DNS traffic and analyze how devices resolve domain names to IP addresses.

---

## 🛠️ Lab Steps

1. Opened Wireshark and selected my Wi-Fi interface  
2. Started a packet capture while browsing common websites  
3. Used the filter `dns` to isolate Domain Name System packets  
4. Identified standard queries and responses between my device and DNS server  
5. Took a screenshot of a DNS packet (see below)

---

## 🔍 What I Captured

- Multiple `Standard query` and `Standard query response` packets  
- Source IP: `192.168.1.170` (my device)  
- Destination IP: `192.168.1.1` (my router/DNS server)  
- Domains queried: Can be decoded from packet bytes (e.g., `www.google.com`, `www.example.com`)  
- Verified DNS runs over UDP and uses port 53

---

## 🖼️ Screenshot

![DNS Packet Screenshot](dns_capture.png)

---

## 💡 What I Learned

- DNS is the first step in almost every web request  
- Tools like Wireshark allow visibility into **how traffic flows** in real time  
- Understanding packet structure helps with threat detection and incident response  
- This is foundational to **network forensics** and **blue team analysis**

---

## 🔜 Next Steps

- Capture HTTP traffic with filter `http`  
- Practice filtering for TCP handshakes and full flows  
- Document a phishing simulation or alert detection scenario
