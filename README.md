# Networking Cheatsheet

## Network Devices

| Device | Description |
|--------|-------------|
| **Client** | End-user device requesting network services |
| **Network Interface Card (NIC)** | Hardware component enabling network connectivity (wired/wireless) |
| **Switch** | Forwards data packets between devices on the same network (Layer 2) |
| **Access Point (AP)** | Enables wireless clients to connect to the wired network |
| **Router** | Connects different networks together and routes traffic between them (Layer 3) |
| **Firewall** | Security device that monitors and filters network traffic |
| **Server** | Computer that provides services/resources to clients |

## Network Topology

**Standard Enterprise Network Flow:**
```
Wireless Client → Access Point → Switch → Router → Firewall → Internet
```

**Physical Components:**
- **RJ45**: Standard connector for Ethernet cables
- **Unshielded Twisted Pair (UTP)**: Common copper cabling for networks
- **Fiber Optic**: High-speed cable for long distances or between floors
- **Wiring Closet**: Centralized location for network hardware
- **PoE (Power over Ethernet)**: Powers devices through Ethernet cable

## Network Protocols & Layers

### OSI Model
"Please Do Not Throw Sausage Pizzas Away"

| Layer | Name | Function |
|-------|------|----------|
| 7 | Application | End-user services (HTTP, FTP, SMTP) |
| 6 | Presentation | Data translation, encryption |
| 5 | Session | Maintains connections and sessions |
| 4 | Transport | End-to-end connections (TCP/UDP) |
| 3 | Network | Routing and logical addressing (IP) |
| 2 | Data Link | Physical addressing (MAC) |
| 1 | Physical | Raw bit transmission |

### Key Transport Protocols

- **TCP (Transmission Control Protocol)**: Connection-oriented, reliable
  - Establishes connection before sending data
  - Confirms delivery of packets
  - Used for: Web browsing, email, file transfers

- **UDP (User Datagram Protocol)**: Connectionless, faster
  - Sends data without connection setup
  - No delivery confirmation
  - Used for: Streaming, gaming, DNS lookups

## Network Utility Tools

| Tool | Purpose | Basic Usage |
|------|---------|-------------|
| **nc (netcat)** | Test TCP/UDP connections | `nc -v host port` |
| **curl** | Transfer data with URLs | `curl http://example.com` |
| **tcpdump** | Command-line packet analyzer | `tcpdump -i eth0 port 80` |
| **tshark** | Terminal version of Wireshark | `tshark -i eth0 -f "port 80"` |
| **wireshark** | GUI packet analyzer | Launch and select interface |

## Common Network Configurations

**Home vs. Enterprise:**
- **Home Networks**: Often use all-in-one devices combining router, switch, firewall, AP
- **Enterprise Networks**: Use separate, purpose-built devices for each function

**Vendor-Specific Notes:**
- **Palo Alto Networks**: Enterprise-grade security appliances and firewalls# networking-lab
A hands-on collection of notes, tools, and experiments from my study of computer networking.
