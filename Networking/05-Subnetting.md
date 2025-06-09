#  Subnetting & CIDR (Simplified)

---

## What is Subnetting?

Subnetting = Splitting a big network into smaller networks (called subnets)

Helps to:
- Organize IPs
- Improve security
- Reduce network traffic
- Save IPs

---

## ♻️ IP Addresses Recap:

- IPv4 = 32-bit
- Written as: `192.168.1.1`

It has 2 parts:
1. **Network** part
2. **Host** part

Example:
**192.168.1.1/24**

Here `/24` means --> First 24 bits = network part  
Remaining 8 bits = host part

---

##  What is CIDR?

CIDR = Classless Inter-Domain Routing  
It's a way to **write subnet masks** in a short form.

###  CIDR Notation:
Instead of writing:
**Subnet mask: 255.255.255.0**
We write:
**/24   ← means 24 bits for network**
---

##  Common CIDR and Subnet Mask Table:

| CIDR | Subnet Mask         | Hosts |
|------|---------------------|-------|
| /8   | 255.0.0.0           | 16 million+ |
| /16  | 255.255.0.0         | 65,534 |
| /24  | 255.255.255.0       | 254   |
| /25  | 255.255.255.128     | 126   |
| /26  | 255.255.255.192     | 62    |
| /27  | 255.255.255.224     | 30    |
| /30  | 255.255.255.252     | 2     |

Hosts = Devices you can connect (minus network & broadcast)

---

##  Example:

You have a network: `192.168.1.0/24`  
You want 2 subnets with ~120 devices each.

Split it into two: `192.168.1.0/25` and `192.168.1.128/25`

That gives:
- 126 hosts in each subnet
- Less traffic
- Better control

---
##  Why Subnet??

- Real-world networks are huge
- You don’t want 1000 devices talking in one network
- Helps isolate traffic & increase speed

---

>  “Subnetting makes a big network feel small and smart.”

