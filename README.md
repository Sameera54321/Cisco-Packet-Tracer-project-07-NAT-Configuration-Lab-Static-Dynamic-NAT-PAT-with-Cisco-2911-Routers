# Cisco-Packet-Tracer-project-07-NAT-Configuration-Lab-Static-Dynamic-NAT-PAT-with-Cisco-2911-Routers
I’m excited to share my latest Cisco Packet Tracer project – a NAT (Network Address Translation) configuration lab. The topology includes two Cisco 2911 routers, two 2960 switches, two client PCs, and a server.

![image alt](https://github.com/Sameera54321/-Cisco-Packet-Tracer-project-05-Inter-VLAN-Inter-Subnet-Routing-Lab-Server-PCs-Laptops-Two-Switches/blob/main/14.jpg?raw=true)

## 📌 Summary

## NAT Configuration Lab is a Cisco Packet Tracer simulation that teaches Network Address Translation (NAT) in a small routed environment. The topology consists of:

    2 routers – Router1 (NAT border) and Router2 (simulating external network or ISP)

    2 switches – access layer for end devices

    2 PCs (PC0 on inside network, PC1 on outside network)

    1 server (Server0 on outside network)

### Typical addressing :

| Device | Interface | IP Address | Role |
| :--- | :--- | :--- | :--- |
| PC0 | NIC | 192.168.1.10/24 | Inside host |
| Router1 (G0/0) | Inside | 192.168.1.1/24 | Default gateway for inside |
| Router1 (G0/1) | Outside | 200.1.1.1/24 | Public / external |
| Router2 (G0/0) | External network | 200.1.1.2/24 | Next hop |
| Router2 (G0/1) | Server network | 203.0.113.1/24 | Gateway for server |
| Server0 | NIC | 203.0.113.10/24 | External server |
| PC1 | NIC | 203.0.113.20/24 | External client |

### NAT configurations demonstrated:

    Static NAT – map 192.168.1.10 to a fixed public IP (e.g., 200.1.1.100)

    Dynamic NAT – pool of public IPs (200.1.1.101 – 200.1.1.110)

    PAT (Overload) – share 200.1.1.1 for all inside hosts

The lab includes verification commands, ACLs for NAT, and troubleshooting steps.

## ✨ Features

    ✅ 2 Cisco 2911 routers – full NAT support (static, dynamic, PAT)

    ✅ 2 Cisco 2960 switches – basic access layer

    ✅ Inside & outside network separation

    ✅ PCs and server – test connectivity from private to public

    ✅ NAT translations – viewable with show ip nat translations

    ✅ Full Packet Tracer file (.pkt) – ready to load and configure

    ✅ Documentation – IP plan, NAT commands, verification steps

## 🛠️ Built With

    Cisco Packet Tracer – version 8.x

    CLI – router and switch configuration

## 🤝 Contributing

Contributions are welcome! To extend this lab:

    Fork the repository.

    Add a second inside network (VLANs) with router‑on‑a‑stick.

    Implement NAT64 or IPv6 transition mechanisms.

    Add a firewall (ASA) between routers.

    Include Wireshark captures showing NAT translation in action.

    Open a pull request with a clear description.
