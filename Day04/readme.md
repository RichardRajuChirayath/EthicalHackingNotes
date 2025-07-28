# DAY-04

---

## Network

A network is a group of interconnected computers and devices that communicate with each other to share resources and information.

- **Example:** The computers in your school lab connected to the same printer are part of a network.
- **Types:** LAN (Local Area Network), WAN (Wide Area Network), MAN (Metropolitan Area Network)

---

## Subnet

A subnet (subnetwork) is a smaller, logical division of a larger network, created to organize and improve network performance and security.

- **Purpose:** Helps manage traffic and enhance security within a network.
- **Example:** Dividing an office network into subnets for different departments.

---

## MAC Address

A MAC (Media Access Control) address is a unique identifier assigned to a network interface card (NIC) for communication on the physical network segment.

- **Format:** Usually displayed as six pairs of hexadecimal digits (e.g., 00:1A:2B:3C:4D:5E)
- **Use:** Used for communication within the same local network.

---

## IP Address (Static and Dynamic) — IPv4 and IPv6

An IP (Internet Protocol) address is a numerical label assigned to each device on a network.

- **Static IP Address:** Remains constant and does not change (e.g., servers).
- **Dynamic IP Address:** Assigned by a DHCP server and can change over time (e.g., most home devices).
- **IPv4:** 32-bit address, written as four numbers separated by dots (e.g., 192.168.1.1).
- **IPv6:** 128-bit address, written as eight groups of hexadecimal numbers (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).
- **Why IPv6?** IPv4 addresses are running out due to the large number of internet devices; IPv6 provides a much larger pool.

---

## TCP/UDP

- **TCP (Transmission Control Protocol):** Connection-oriented protocol. Ensures reliable delivery of data (checks for errors and correct order). Used for web browsing, emails, file transfers.
- **UDP (User Datagram Protocol):** Connectionless protocol. Faster but less reliable (no error checking or ordering). Used for online gaming, video streaming, VoIP.

| Feature      | TCP                     | UDP                    |
|--------------|-------------------------|------------------------|
| Connection   | Connection-oriented     | Connectionless         |
| Reliability  | Reliable (guaranteed)   | Unreliable (best-effort)|
| Speed        | Slower                  | Faster                 |
| Use Cases    | Web, Email, FTP         | Video, Gaming, VoIP    |

---

## Broadcast

Broadcast refers to sending data from one device to all devices on a network segment simultaneously.

- **Example:** ARP (Address Resolution Protocol) requests are sent as broadcasts to find the MAC address of devices on the local network.
- **Limitation:** Can cause congestion if overused.

---

## NAT (Network Address Translation)

NAT translates private (local) IP addresses to a public IP address before packets are sent to another network, such as the Internet.

- **Purpose:** Conserves public IP addresses and improves security by hiding internal addresses.
- **Example:** Multiple devices in a home use one public IP to access the internet.

---

## Port Forwarding

Port forwarding allows external devices to access services on a private network by mapping an external port to an internal IP and port.

- **Use Case:** Hosting a game server or website on your computer so others can connect via the internet.

---

## Practical Exercises

1. **Find your computer's MAC address:**
   - On Windows: `ipconfig /all`
   - On Linux/Mac: `ifconfig` or `ip link`
2. **Check your IP address:**
   - On Windows: `ipconfig`
   - On Linux/Mac: `ifconfig` or `ip addr`
3. **Test connectivity using TCP/UDP:**
   - Use `ping` (ICMP) for basic connectivity (not TCP/UDP, but related).
   - Try sending files using FTP (TCP) and streaming a video (UDP).

---

## Additional Resources

- [Cisco Networking Basics](https://www.cisco.com/c/en/us/solutions/enterprise-networks/what-is-networking.html)
- [IPv6 Explained (Microsoft)](https://learn.microsoft.com/en-us/windows-server/networking/technologies/ipv6/ipv6-overview)
- [TCP vs UDP (Cloudflare)](https://www.cloudflare.com/learning/ddos/glossary/user-datagram-protocol-udp/)

---

## Glossary

- **LAN:** Local Area Network
- **WAN:** Wide Area Network
- **DHCP:** Dynamic Host Configuration Protocol
- **NAT:** Network Address Translation
- **ARP:** Address Resolution Protocol

---

*For any questions or clarifications, refer to your instructor or the above resources!*
