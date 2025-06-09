#  IP Addressing (IPv4 Basics)

Every device on a network needs an **IP address** to communicate. It's like your device's identity .

---

## What is an IP Address?

- IP = Internet Protocol
- Unique address for each device in a network
- **IPv4** = 32-bit address
- Written as 4 numbers (called octets), separated by dots

Example:
**192.168.0.1**
-----------------------------------------------------------------------------------------------------

##  Binary View:

Each octet is 8 bits → total 32 bits
So: `11000000.10101000.00000000.00000001`

-----------------------------------------------------------------------------------------------------

##  Classes of IPv4 Addresses:

| Class | Range           | Used For          |
|-------|------------------|-------------------|
| A     | 1.0.0.0 – 126.255.255.255 | Large networks |
| B     | 128.0.0.0 – 191.255.255.255 | Medium networks |
| C     | 192.0.0.0 – 223.255.255.255 | Small networks |
| D     | 224.0.0.0 – 239.255.255.255 | Multicast |
| E     | 240.0.0.0 – 255.255.255.255 | Reserved |

---

## 🏡 Private IP Ranges:

Used inside homes, schools, offices (can’t be accessed from internet directly)

| Class | Private IP Range |
|-------|------------------|
| A     | 10.0.0.0 – 10.255.255.255 |
| B     | 172.16.0.0 – 172.31.255.255 |
| C     | 192.168.0.0 – 192.168.255.255 |

Example: `192.168.1.1` (router)

---

##  simple Terms:

- **Public IP**: Seen on internet, unique globally
- **Private IP**: Used inside LANs, reused across networks
- **Static IP**: Fixed address, doesn’t change
- **Dynamic IP**: Given by DHCP server, can change

---

>  “IP address is your identity in the digital world.”
