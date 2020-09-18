# Network

---

## ToC

- [Network](#network)
  - [ToC](#toc)
  - [Network: MISC](#network-misc)
  - [Xaas](#xaas)
  - [XaaS Comparison](#xaas-comparison)
  - [Latency vs Bandwidth](#latency-vs-bandwidth)
- [IP Addresses](#ip-addresses)
  - [DNS](#dns)
  - [IPv4](#ipv4)
  - [IP Addressing: Classful vs Classless](#ip-addressing-classful-vs-classless)
  - [IPv4: Reserved IP Addresses](#ipv4-reserved-ip-addresses)
  - [IPv6:](#ipv6)
  - [TCP / IP Model](#tcp--ip-model)
  - [OSI Model](#osi-model)
  - [Tools](#tools)
  - [Network Devices](#network-devices)
  - [LAN Topology](#lan-topology)
  - [LAN Access Control Methods](#lan-access-control-methods)
  - [WLAN](#wlan)
  - [Network Cables](#network-cables)
  - [TCP / IP](#tcp--ip)
  - [Cache](#cache)
- [VPN](#vpn)
  - [What's VPN?](#whats-vpn)
    - [Types](#types)
  - [VPN vs Leased Line](#vpn-vs-leased-line)
  - [Internet VPN technologies](#internet-vpn-technologies)
  - [Protocols](#protocols)


---

## Network: MISC

- NFS: Network File System


>>>

## Xaas

- IaaS: Infrastructure
  - Similar to conventional hosting services, however you can customize hardwares flexibly
- PaaS: Platform
- SaaS: Software
- BaaS / mBaaS: Backend 

>>>

## XaaS Comparison

|                | On-Premises |          IaaS          |                      PaaS                       |                  SaaS                   |
| -------------- | :---------: | :--------------------: | :---------------------------------------------: | :-------------------------------------: |
| Application    |    user     |          user          |                      user                       |                provider                 |
| Data           |    user     |          user          |                      user                       |                provider                 |
| Runtime        |    user     |          user          |                    provider                     |                provider                 |
| Middleware     |    user     |          user          |                    provider                     |                provider                 |
| OS             |    user     |          user          |                    provider                     |                provider                 |
| Virtualization |    user     |        provider        |                    provider                     |                provider                 |
| Servers        |    user     |        provider        |                    provider                     |                provider                 |
| Storage        |    user     |        provider        |                    provider                     |                provider                 |
| Networking     |    user     |        provider        |                    provider                     |                provider                 |
| Examples:      |    user     | EC2, GCE, DigitalOcean | GAE, Beanstalk, Heroku, Azure, RedHat OpenShift | Google Apps, Salesforce, Dropbox, Slack |

## Latency vs Bandwidth

---

# IP Addresses

>>>

## DNS



>>>

## IPv4

- 4 Bytes = 32 Bits

>>>


## IP Addressing: Classful vs Classless

|         |         Network Address          |  Host Address  | First Octet |     Mask      | CIDR  |             Range             |
| :-----: | :------------------------------: | :------------: | :---------: | :-----------: | :---: | :---------------------------: |
| Class A |   1 Byte = "0" + 7 bits( 2^7)    | 3 Bytes (2^24) |  0xxxxxxx   |   255.0.0.0   |  /8   |   0.0.0.0 - 127.255.255.255   |
| Class B | 2 Bytes = "10" + 14 bits (2^14)  | 2 Bytes (2^16) |  10xxxxxx   |  255.255.0.0  |  /16  | 128.0.0.0 to 191.255.255.255  |
| Class C | 3 Bytes = "110" + 21 bits (2^21) |  1 Byte (2^8)  |  110xxxxx   | 255.255.255.0 |  /24  | 192.0.0.0 to 223.255.255.255  |
| Class D |                -                 |       -        |  1110xxxx   |       -       |   -   | 224.0.0.0 to 239.255.255.255  |
| Class E |                -                 |       -        |  1111xxxx   |       -       |   -   | 240.0.0.0 and 255.255.255.255 |

- Note that some special addresses such as `0.0.0.0`, `127.x.x.x` are reserved

>>>

## IPv4: Reserved IP Addresses

- 0.0.0.0/8
  - This network
- 0.0.0.0/32
- 127.0.0.0/8
  - Loop Back
- 169.254.0.0/16
  - Link Local
- 172.16.0.0/12
- 192.168.0.0/16
- 224.0.0.0/4 (224.0.0.0 to 224.0.0.255)
  - Multi Cast
- 240.0.0.0/4
  - Includes `255.255.255.255/32` which shows the all the hosts on the network


>>>


## IPv6:


>>>

## TCP / IP Model

>>>

## OSI Model

>>>

## Tools

- Wireshark
- Firebug (dead?)

>>>

## Network Devices

- DTE: Data Terminal Equipment
- DCE: Data Circuit Terminating Equipment
- Hub
- Repeater
- Bridge
- Router
- Switch

>>>

## LAN Topology

- Bass
- Star
- Ring

>>>

## LAN Access Control Methods

- CSMA/CD
- Token Passing

>>>

## WLAN

- 

>>>

## Network Cables

- 


>>>

## TCP / IP

>>>

## Cache



---

# VPN

>>>

## What's VPN?

- Safe

### Types
- Internet VPN
  - Cheap but not so safe as others
- IP-VPN
  - Closed network for the ISP and its users
  - No need for encryption, however expensive
- Entry VPN
- WAE: Wide Area Ethernet
  - Highly customizable, but expensive and narrow

>>>

## VPN vs Leased Line

- Leased Line (専用線) is physical

>>>

## Internet VPN technologies

- Tunneling
- 

## Protocols

- IPsec-VPN
- L2TP
- PPTP
- SSL-VPN

>>>