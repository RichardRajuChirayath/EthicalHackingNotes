# DAY-04 — Networking Concepts

## 🖧 **Network**
A **network** is a group of interconnected computers and devices that communicate with each other to share resources and information.
- **Example:** 🖥️ The computers in your school lab connected to the same printer are part of a network.
- **Types:**  
  - 🏠 **LAN** (Local Area Network)  
  - 🌍 **WAN** (Wide Area Network)  
  - 🏙️ **MAN** (Metropolitan Area Network)

## 🪢 **Subnet**
A **subnet** (subnetwork) is a smaller, logical division of a larger network, created to organize and improve network performance and security.
- **Purpose:** Helps manage traffic and enhance security within a network.
- **Example:** 🏢 Dividing an office network into subnets for different departments.

## 🏷️ **MAC Address**

A MAC address is a unique code given to every device’s network card, like a digital name tag. It helps devices recognize each other within the same local network (like Wi-Fi at home). It looks something like 00:1A:2B:3C:4D:5E and is usually permanent. Unlike IP addresses, MAC addresses don’t change and work at a lower level of communication. You can find yours using ipconfig /all (Windows) or ifconfig (Linux/Mac).
- **Format:** `00:1A:2B:3C:4D:5E` (six pairs of hexadecimal digits)
- **Use:** Used for communication within the same **local network**.

## 🌐 **IP Address (Static and Dynamic) — IPv4 and IPv6**
An **IP (Internet Protocol) address** is a numerical label assigned to each device on a network.
- 🔒 **Static IP Address:** Remains constant and does not change (e.g., servers).
- 🔄 **Dynamic IP Address:** Assigned by a DHCP server and can change over time (e.g., most home devices).
- **IPv4:** `192.168.1.1` (32-bit, four numbers separated by dots)
- **IPv6:** `2001:0db8:85a3:0000:0000:8a2e:0370:7334` (128-bit, eight groups of hexadecimal)
- **Why IPv6?**  
  IPv4 addresses are running out!  
  IPv6 provides a much larger address pool. 🚀


## 📦 **TCP/UDP**
- **TCP (Transmission Control Protocol):**  
  - ☑️ Connection-oriented  
  - Ensures reliable delivery (checks for errors and order)  
  - Used for: 🌐 Web Browsing, ✉️ Email, 📁 File Transfers
- **UDP (User Datagram Protocol):**  
  - 🚫 Connectionless  
  - Faster but less reliable (no error checking/order)  
  - Used for: 🎮 Online Gaming, 📺 Video Streaming, 📞 VoIP

| Feature      | 🛡️ TCP                      | ⚡ UDP                   |
|--------------|-----------------------------|-------------------------|
| Connection   | Connection-oriented         | Connectionless          |
| Reliability  | Reliable (guaranteed)       | Unreliable (best-effort)|
| Speed        | Slower                      | Faster                  |
| Use Cases    | Web, Email, FTP             | Video, Gaming, VoIP     |

## 📢 **Broadcast**
**Broadcast** refers to sending data from one device to **all** devices on a network segment simultaneously.
- **Example:**  
  🔎 ARP requests are broadcast to find the MAC address of devices on the local network.
- **Limitation:**  
  🚦 Can cause congestion if overused.

## 🔄 **NAT (Network Address Translation)**
**NAT** translates private (local) IP addresses to a public IP address before packets are sent to another network, such as the Internet.
- **Purpose:**  
  💡 Conserves public IP addresses  
  🛡️ Improves security by hiding internal addresses
- **Example:**  
  🏠 Multiple devices in a home use one public IP to access the internet.

  <!DOCTYPE html>
<html>
<head>
</head>
<body>

  <h1>Nmap Command </h1>

 
  <pre>sudo nmap -Pn -A -sV -O -p 1-1000 -sS -vv --script default -oN scan_output.txt 192.168.1.1</pre>

  <h2>Explaination of Flags</h2>
  <table border="1">
    <tr>
      <th>Flag</th>
      <th>Meaning</th>
    </tr>
    <tr><td>-Pn</td><td>Skip host discovery (treat all hosts as online)</td></tr>
    <tr><td>-A</td><td>Aggressive scan (OS detection, version detection, script scan, traceroute)</td></tr>
    <tr><td>-sV</td><td>Detect service versions</td></tr>
    <tr><td>-O</td><td>Enable OS detection</td></tr>
    <tr><td>-p 1-1000</td><td>Scan ports 1 through 1000</td></tr>
    <tr><td>-sS</td><td>SYN scan (stealthy, requires root)</td></tr>
    <tr><td>-vv</td><td>Very verbose output</td></tr>
    <tr><td>--script default</td><td>Run default Nmap scripts</td></tr>
    <tr><td>-oN scan_output.txt</td><td>Save output in normal format to file</td></tr>
    <tr><td>192.168.1.1</td><td>Target IP or domain</td></tr>
  </table>

  

</body>
</html>


## 🚪 **Port Forwarding**
**Port forwarding** allows external devices to access services on a private network by mapping an external port to an internal IP and port.
- **Use Case:**  
  🎮 Hosting a game server or 🌍 website on your computer so others can connect via the internet.
