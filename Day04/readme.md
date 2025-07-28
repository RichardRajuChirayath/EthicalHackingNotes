# DAY-04 — Networking Concepts

---

## 🖧 **Network**

A **network** is a group of interconnected computers and devices that communicate with each other to share resources and information.

- **Example:** 🖥️ The computers in your school lab connected to the same printer are part of a network.
- **Types:**  
  - 🏠 **LAN** (Local Area Network)  
  - 🌍 **WAN** (Wide Area Network)  
  - 🏙️ **MAN** (Metropolitan Area Network)

---

## 🪢 **Subnet**

A **subnet** (subnetwork) is a smaller, logical division of a larger network, created to organize and improve network performance and security.

- **Purpose:** Helps manage traffic and enhance security within a network.
- **Example:** 🏢 Dividing an office network into subnets for different departments.

---

## 🏷️ **MAC Address**

A **MAC (Media Access Control) address** is a unique identifier assigned to a network interface card (NIC) for communication on the physical network segment.

- **Format:** `00:1A:2B:3C:4D:5E` (six pairs of hexadecimal digits)
- **Use:** Used for communication within the same **local network**.

---

## 🌐 **IP Address (Static and Dynamic) — IPv4 and IPv6**

An **IP (Internet Protocol) address** is a numerical label assigned to each device on a network.

- 🔒 **Static IP Address:** Remains constant and does not change (e.g., servers).
- 🔄 **Dynamic IP Address:** Assigned by a DHCP server and can change over time (e.g., most home devices).
- **IPv4:** `192.168.1.1` (32-bit, four numbers separated by dots)
- **IPv6:** `2001:0db8:85a3:0000:0000:8a2e:0370:7334` (128-bit, eight groups of hexadecimal)
- **Why IPv6?**  
  IPv4 addresses are running out!  
  IPv6 provides a much larger address pool. 🚀

---

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

---

## 📢 **Broadcast**

**Broadcast** refers to sending data from one device to **all** devices on a network segment simultaneously.

- **Example:**  
  🔎 ARP requests are broadcast to find the MAC address of devices on the local network.
- **Limitation:**  
  🚦 Can cause congestion if overused.

---

## 🔄 **NAT (Network Address Translation)**

**NAT** translates private (local) IP addresses to a public IP address before packets are sent to another network, such as the Internet.

- **Purpose:**  
  💡 Conserves public IP addresses  
  🛡️ Improves security by hiding internal addresses
- **Example:**  
  🏠 Multiple devices in a home use one public IP to access the internet.

---

## 🚪 **Port Forwarding**

**Port forwarding** allows external devices to access services on a private network by mapping an external port to an internal IP and port.

- **Use Case:**  
  🎮 Hosting a game server or 🌍 website on your computer so others can connect via the internet.

---
