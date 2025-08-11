# task5-Capture-and-Analyze-Network--Traffic--Using--Wireshark.
# Task 5 – Capture and Analyze Network Traffic Using Wireshark

## 📌 Objective
Capture live network traffic using Wireshark, identify multiple network protocols, and analyze them.

---

## 🛠 Tools Used
- **Wireshark** – Network protocol analyzer
- **Command Prompt** – For generating traffic
- **Web Browser** – For HTTP traffic testing

---

## 📝 Steps Performed
1. Opened **Wireshark** and selected the active network interface (**Wi-Fi**).
2. Started packet capture by clicking the **blue shark fin** icon.
3. Generated traffic:
   - ICMP:  
     ```cmd
     ping google.com
     ```
   - DNS:  
     ```cmd
     nslookup google.com
     ```
   - HTTP:  
     Visited `http://neverssl.com`
4. Allowed capture to run for **about 1 minute**.
5. Stopped capture by clicking the **red square** icon.
6. Applied filters:
   - `icmp`
   - `dns`
   - `http`
7. Saved capture as **`task5_capture.pcap`**.

---

## 📡 Protocols Identified

| Protocol | Description |
|----------|-------------|
| **ICMP** | Used for connectivity tests (`ping`). |
| **DNS**  | Resolves domain names to IP addresses. |
| **HTTP** | Unencrypted web traffic protocol. |

---

## 🔍 Observations
- **ICMP** confirmed network connectivity to `google.com`.
- **DNS** packets resolved `google.com` to its IP address.
- **HTTP** packets from `neverssl.com` showed request/response in plain text.

---

## 📂 File for Submission
- `task5_capture.pcap`
