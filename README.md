# Telnet vs SSH Wireshark Lab

## Overview
In this lab, I analyzed the security differences between Telnet and SSH by capturing and inspecting network traffic using Wireshark. The objective was to demonstrate how Telnet transmits data in plaintext, while SSH encrypts all communication to protect sensitive information.

This project highlights a critical cybersecurity concept: insecure protocols like Telnet can expose credentials, while secure protocols like SSH prevent interception through encryption.

---

## Objectives
- Capture Telnet traffic using Wireshark
- Identify plaintext data within Telnet sessions
- Capture SSH traffic using Wireshark
- Analyze encrypted SSH communication
- Compare security differences between Telnet and SSH

---

## Tools Used
- Wireshark
- PuTTY
- Telnet
- SSH (SSHv2)
- Windows Environment

---

## Lab Methodology

### Telnet Traffic Analysis
I initiated a Telnet session while capturing traffic in Wireshark.

Filter used:
```text
tcp.port == 23# Telnet-vs-SSH-Wireshark-Lab
Hands-on Wireshark lab demonstrating plaintext credential exposure in Telnet vs encrypted SSH traffic through packet capture and TCP stream analysis.
## Screenshots

### Telnet Packet Capture
![Telnet Packet Capture](screenshots/telnet-packet-capture.png)

### Telnet TCP Stream (Plaintext Exposure)
![Telnet TCP Stream](screenshots/telnet-tcp-stream.png)

### SSH Packet Capture
![SSH Packet Capture](screenshots/ssh-packet-capture.png)

### SSH TCP Stream (Encrypted Data)
![SSH TCP Stream](screenshots/ssh-tcp-stream.png)
