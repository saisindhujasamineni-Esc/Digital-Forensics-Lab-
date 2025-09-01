# Experiment -3 : Capturing and Analyzing Network Traffic using Wireshark

## 🎯 Aim
To capture live network traffic and analyze packets using **Wireshark**, helping understand communication patterns, detect issues, or identify suspicious activities.

---

## 📖 Description
Wireshark is a free and open-source packet analyzer. It allows you to **see what’s happening on your network in real time**.  
With Wireshark, you can capture data packets as they travel across a network, view their details, and analyze protocols like HTTP, TCP, UDP, DNS, and more.  

It is widely used by network administrators, cybersecurity professionals, and forensic investigators to troubleshoot problems and investigate security incidents.

---

## 🛠️ Tools Required
- **Wireshark** (download from [https://www.wireshark.org](https://www.wireshark.org))  
- A computer with network access (Windows/Linux/macOS)  
- Administrator/root privileges (needed to capture packets)  

---

## 📝 Procedure
**Install and Launch Wireshark**  
   - Download and install Wireshark.  
   - Run it with administrator/root privileges to capture live traffic.  

**Select a Network Interface**  
   - On startup, Wireshark shows a list of available network interfaces (e.g., Wi-Fi, Ethernet).  
   - Select the one you want to monitor (e.g., `Wi-Fi` if you’re on wireless).  

**Start Capturing Traffic**  
   - Click the **blue shark fin icon** (Start Capturing).  
   - Wireshark begins recording live traffic and displays packets in real time.  

**Apply Filters for Clarity**  
   - Use the filter bar to focus on specific traffic. Examples:  
     - `http` → Show only HTTP traffic  
     - `ip.addr == 192.168.1.1` → Show traffic involving a specific IP  
     - `tcp.port == 80` → Show traffic on port 80  

**Analyze Packets**  
   - Click on a packet to view its details in three sections:  
     - **Packet List Pane** (top): Summary of all packets  
     - **Packet Details Pane** (middle): Protocol breakdown (Ethernet, IP, TCP/UDP, etc.)  
     - **Packet Bytes Pane** (bottom): Raw data in hex/ASCII  

**Follow a Stream**  
   - Right-click on a TCP/HTTP packet → **Follow → TCP Stream**.  
   - This shows the full conversation between client and server in plain text (useful for analyzing requests/responses).  

**Stop and Save the Capture**  
   - Click the **red square icon** (Stop Capturing).  
   - Save the capture as a `.pcapng` file for later analysis or reporting.  

**Look for Suspicious/Important Data**  
   - Check for unusual IPs, large data transfers, or repeated failed connections.  
   - Export findings into reports if required.  

---

## Result
By following this process, you can **capture live network traffic and analyze it with Wireshark**.  
This helps in learning how networks work, solving connectivity issues, and identifying potential security threats in digital forensics and cybersecurity investigations.
