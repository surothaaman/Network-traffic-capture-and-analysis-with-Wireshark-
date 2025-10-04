# EX 9 : Network-traffic-capture-and-analysis-with-Wireshark
## AIM:
To capture and analyze network traffic using Wireshark in order to observe protocols, packets, and potential anomalies.
## Requirements:
- **Hardware:**
    - Computer with internet access
    - Network adapter (Ethernet/Wi-Fi)
- **Software:**
    - Wireshark (latest stable version)
    - Sample PCAP files (optional for offline analysis)
## Architecture:
```mermaid
flowchart TD
    A[Network Interface Card] --> B[Wireshark Packet Capture Engine]
    B --> C[Packet Decoder & Protocol Analyzer]
    C --> D[Packet Display & Filtering Interface]
    D --> E[Investigator Analyzes Network Data]
    E --> F[Findings: IPs, Ports, Protocols, Anomalies]
```
## DESIGN STEPS:
### Step 1:
Install Wireshark on the system.



### Step 2:
Launch Wireshark and select the network interface (Ethernet/Wi-Fi).

### Step 3:
Start the capture, apply filters (like http, tcp, ip.addr == x.x.x.x) to analyze specific traffic, and stop the capture after observing relevant data.
### Step 4:
**Analyze traffic to identify:**
  - Source & Destination IP addresses
  - Protocols (HTTP, DNS, TCP, UDP, etc.)
  - Suspicious activities (e.g., unusual ports, repeated requests).
## PROGRAM:
Wireshark Packet Capture and Filter Usage
## 1. Open Wireshark and Select a Network Interface
• Launch Wireshark.
• Select an active interface (like Wi-Fi or Ethernet) to start capturing packets.

<img width="1920" height="1080" alt="Screenshot (29)" src="https://github.com/user-attachments/assets/1da86ebd-d2b0-4aba-a97f-3a0d7f080393" />

## 2. Start Capturing Packets
• Click the blue shark fin icon or double-click the interface.
• Wireshark will start capturing all real-time traffic.

<img width="1920" height="1080" alt="Screenshot (30)" src="https://github.com/user-attachments/assets/8809d3f7-e71d-4007-bb50-8d2efb802868" />


## 3. Apply Filters to Focus on Specific Traffic
• Use filters like http, ip.addr == 192.168.1.1, or tcp.port == 80 in the top filter
bar to narrow down results.

<img width="1920" height="1080" alt="Screenshot (31)" src="https://github.com/user-attachments/assets/deb86b6e-a05e-4ac3-8c62-123ba19e5d90" />




## 4. Analyze Packet Details
• Click on a packet to view its detailed breakdown including frame, Ethernet,
IP, TCP/UDP layers, and data payload.



<img width="1920" height="1080" alt="Screenshot (32)" src="https://github.com/user-attachments/assets/40428547-e4f4-4546-a04c-56168305e58d" />



## 5. Export or Save the Capture
• Go to File > Save As to store the capture in .pcap format for future analysis.


<img width="1920" height="1080" alt="Screenshot (33)" src="https://github.com/user-attachments/assets/14c5fe9f-5799-48da-8478-e5d716903803" />





## OUTPUT:
Captured Packets with Protocol Analysis and Detailed Packet Info

## RESULT:
Network traffic was successfully captured and analyzed using Wireshark.
