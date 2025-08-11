# Task 5 – Capture and Analyze Network Traffic Using Wireshark

## Objective
To capture live network traffic, identify multiple network protocols, and analyze them using Wireshark.

---

## Tools Used
- **Wireshark** (GUI-based network protocol analyzer)
- **Command Prompt** (to generate traffic using `ping` and `nslookup`)
- **Web Browser** (to generate HTTP traffic)

---

## Steps Performed

1. **Opened Wireshark** and selected the active network interface (**Wi-Fi**).
2. **Started the packet capture** by clicking the **blue shark fin** icon.
3. Generated different types of traffic:
   - **ICMP traffic** by running:
     ```cmd
     ping google.com
     ```
   - **DNS traffic** by running:
     ```cmd
     nslookup google.com
     ```
   - **HTTP traffic** by visiting:
     ```
     http://neverssl.com
     ```
4. Let the capture run for about **1 minute**.
5. **Stopped the capture** by clicking the **red square** icon.
6. Applied filters in Wireshark to view specific protocols:
   - `icmp`
   - `dns`
   - `http`
7. Saved the capture as `task5_capture.pcap` for submission.

---

## Protocols Identified

| Protocol | Description |
|----------|-------------|
| **ICMP** | Internet Control Message Protocol – used for connectivity tests (`ping`). |
| **DNS**  | Domain Name System – resolves domain names to IP addresses. |
| **HTTP** | Hypertext Transfer Protocol – used for unencrypted web traffic. |

---

## Observations
- ICMP packets confirm network connectivity to `google.com`.
- DNS packets show the request and response for resolving `google.com` to its IP address.
- HTTP packets captured from visiting `neverssl.com` show the full request/response in plain text.

---

## File for Submission
- **Capture File:** `task5_capture.pcap`
