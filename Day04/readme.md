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

---

## Broadcast

Broadcast refers to sending data from one device to all devices on a network segment simultaneously.

- **Example:** ARP (Address Resolution Protocol) requests are sent as broadcasts to find the MAC address of devices on the local network.
- **Limitation:** Can cause congestion if overused.

---

## NAT (Network Address Translation)

NAT is a process where a network device (usually a router) modifies the source or destination IP address of packets to allow multiple devices to share a single public IP address.

- **Benefit:** Conserves public IP addresses and adds a layer of security.
- **Example:** Your home router uses NAT to let all your devices access the internet with one public IP.

---

## Port Forwarding

Port forwarding is a technique used to redirect network traffic from one address and port number to another.

- **Purpose:** Allows external devices to access services on a private network, such as a web server or gaming server.
- **Example:** Setting up port forwarding on your router so you can access your home security camera from anywhere.

---
