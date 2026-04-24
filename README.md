# 🌐 Wireshark Traffic Analysis Lab

## 🎯 Objective
The purpose of this lab was to capture and analyze live network traffic using Wireshark in order to understand how DNS requests, TCP connections, and web traffic operate at the packet level. This helps build foundational skills for SOC (Security Operations Center) analysis and network threat detection.

---

## 🧰 Tools Used
- Wireshark
- Internet browser (Chrome)
- Active network connection (Wi-Fi)

---

## ⚙️ Lab Setup & Process

1. Installed and launched Wireshark on a local machine.
2. Selected the active network interface (Wi-Fi) and started packet capture.
3. Generated normal web traffic by visiting multiple websites such as:
   - Google
   - YouTube
   - Amazon
4. Captured traffic for approximately 3–5 minutes.
5. Stopped the capture and applied filters to analyze different types of network traffic.

---

## 🔍 Analysis Performed

### 📡 DNS Traffic
- Filter used: `dns`
- Observed multiple DNS queries resolving domain names such as google.com and youtube.com.
- This demonstrated how devices translate domain names into IP addresses before connecting to servers.

### 🔌 TCP Connections
- Filter used: `tcp`
- Identified active TCP sessions between the local machine and external IP addresses.
- Observed continuous packet exchanges supporting web browsing activity.

### 🌐 HTTP/HTTPS Traffic
- Filter used: `http` (when available)
- Reviewed web request and response patterns between client and web servers.

### 📊 Packet-Level Inspection
- Selected individual packets and analyzed protocol layers:
  - Ethernet Layer
  - Internet Protocol (IP)
  - Transmission Control Protocol (TCP)
  - Application Layer Data

---

## 📸 Evidence
Screenshots included in the `/screenshots` directory:
- Active packet capture session
- DNS query results
- TCP connection analysis
- Packet details breakdown
- Filtered traffic views

---

## 🧠 Key Findings
- DNS traffic reveals which domains a system is attempting to reach.
- TCP connections show persistent communication between client and external servers.
- Packet inspection provides insight into how data is structured and transmitted across networks.
- Normal web browsing generates a large amount of background network activity that can be monitored and analyzed in a SOC environment.

---

## 🔐 SOC Relevance
This lab simulates real-world SOC tasks such as:
- Monitoring network traffic for anomalies
- Identifying communication patterns
- Investigating potential malicious or unusual connections
- Understanding baseline “normal” network behavior for comparison

---

## 🚀 Conclusion
This exercise strengthened my understanding of network protocols and packet analysis. It provides foundational experience relevant to SOC operations, incident response, and network security monitoring.
