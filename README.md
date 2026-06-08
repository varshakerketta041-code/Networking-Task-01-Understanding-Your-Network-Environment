#  Networking Task 01: Understanding Your Network Environment

> **Internship Assignment** | Network Fundamentals | Varsha Kerketta

---

##  Overview

This task covers the fundamentals of understanding a network environment — from identifying system-level network details to explaining core networking concepts and performing connectivity tests.

---

##  Repository Structure

```
Networking_Task_01/
├── README.md
└── Networking_Task_01_Varsha_Kerketta.pdf
```

---

##  Task Breakdown

### Part A — Network Information

Documented the following details from the system using the `hostname` and `ipconfig /all` commands on Windows:

| # | Network Detail | Value |
|---|----------------|-------|
| 1 | Hostname | `DESKTOP-7G5TP3R` |
| 2 | IPv4 Address | `192.168.1.100` |
| 3 | MAC Address | `5C-54-AB-3F-2D-1E` |
| 4 | Default Gateway | `192.168.1.1` |
| 5 | DNS Server | `8.8.8.8` (Google DNS) |

**Commands used:**
```bash
hostname          # Retrieves device name
ipconfig /all     # Retrieves full network configuration
```

---

### Part B — Basic Networking Concepts

Key networking concepts explained:

- **IP Address** — A unique numerical label assigned to each device on a network for identification and communication.
- **MAC Address** — A hardware-level identifier assigned by the manufacturer; fixed to the device unlike an IP address.
- **Default Gateway** — The router (typically `192.168.1.1`) that connects the local network to the internet.
- **DNS (Domain Name System)** — Translates human-readable domain names (e.g., `google.com`) into IP addresses.
- **Public vs Private IP** —
  - *Public IP*: Assigned by the ISP, unique globally, internet-accessible (e.g., `8.8.8.8`)
  - *Private IP*: Assigned by the router, used within local networks, not directly accessible from the internet (e.g., `192.168.1.100`)

---

### Part C — Basic Network Diagram

A simple network diagram illustrating the flow:

```
[ INTERNET ]
     |
[ ISP Network ]
     |
[ Router / Wi-Fi ] — IP: 192.168.1.1
     |
[ Your Device (PC) ] — IP: 192.168.1.100
```

- **Internet** — Global network for websites, emails, and online services.
- **ISP Network** — Bridges your home network to the internet.
- **Router** — Manages local traffic and routes requests to/from the internet.
- **Device** — Sends requests and receives responses via the router.

---

### Part D — Network Connectivity Test

Performed basic connectivity tests using standard networking commands.

**Commands used:**

| Command | Platform | Purpose |
|---------|----------|---------|
| `ipconfig` | Windows | Displays IP, subnet mask, gateway, and adapter info |
| `ip addr` / `ifconfig` | Linux | Same as above for Linux systems |
| `ping google.com` | Both | Tests reachability and measures round-trip latency |
| `tracert` / `traceroute` | Win / Linux | Shows the hop-by-hop path packets take to a destination |

**Key Findings:**
- Google (`google.com`) was successfully reachable via `ping`
-  Multiple hops were observed in `tracert` output — each hop represents a router forwarding the packet one step closer to Google's servers

---

## Tools & Commands Reference

```bash
# Windows
hostname
ipconfig /all
ping google.com
tracert google.com

# Linux
ip addr
ifconfig
ping google.com
traceroute google.com
```

---

## Author

**Varsha Kerketta**  
Internship — Networking Module  
Task 01: Understanding Your Network Environment

---
