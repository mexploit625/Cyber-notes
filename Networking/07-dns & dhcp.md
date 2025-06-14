# DHCP & DNS

---

## DHCP (Dynamic Host Configuration Protocol)

DHCP is what lets devices get their IP addresses and network settings **automatically** instead of having to set everything manually.

How it works, step-by-step:  
1. When a device connects to a network, it basically shouts: “Hey, I need an IP address!”  
2. The DHCP server replies with an available IP address plus other info like subnet mask, default gateway, DNS server addresses, and how long the device can keep this IP (called the lease time).  
3. The device accepts the offer, and the server confirms it.  
4. Now the device is ready to communicate on the network.

This makes managing networks way easier, especially when there are tons of devices coming and going.

---

## DNS (Domain Name System)

DNS is like the internet’s phone book. It translates the easy-to-remember website names (like `google.com`) into IP addresses that computers use to find each other.

Here’s a simple overview of the process:  
- You type a website name into your browser.  
- Your device asks a DNS server, “Hey, what’s the IP for this name?”  
- The DNS server responds with the IP address.  
- Your browser then uses this IP to connect to the website.

DNS has multiple layers: root servers, top-level domain (TLD) servers like `.com` or `.net`, and authoritative servers that actually hold the final info.  

One important thing: DNS can be attacked through methods like DNS spoofing, where attackers trick your system into going to fake IP addresses. So securing DNS is important.

---

## Summary

- **DHCP** automatically hands out IP addresses and network info to devices — makes network setup painless.  
- **DNS** translates domain names into IPs so we don’t have to memorize numbers — makes browsing easy.  
- Both work quietly in the background but are absolutely crucial for the internet to function smoothly.
