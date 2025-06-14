## NAT & Port Forwarding

Alright, so today I went through NAT and Port Forwarding — two things that kinda sit between your local network and the internet. Here's how I understood it:

---

## 📌 What is NAT?

NAT stands for **Network Address Translation**. Basically, it lets your local/private IP addresses talk to the internet using one public IP.

Think about it like this:  
You're in a house (your private network), and the router is the front door. NAT lets everyone inside that house send stuff out to the world using one shared face — your public IP.

### Types of NAT I came across:

- **Static NAT** → One private IP maps to one public IP. Rarely used unless you're running some specific services.  
- **Dynamic NAT** → Private IPs get mapped to a public IP from a pool. Temporary.  
- **PAT (Port Address Translation)** → This is the one we use most. Multiple devices share one public IP, but each gets a different port. Also called **NAT Overload**.

📌 So if two people in the same network hit the same website, NAT keeps track of who asked for what using ports.

---

## 🚪 What is Port Forwarding?

Now this one’s important if you ever want someone **outside** your network to reach a device **inside** your network.

Let’s say you’re running a game server or an SSH session at home — normally, nobody can reach it from the outside because of NAT. Port Forwarding is like telling the router:  
> “Hey, if anyone knocks on this port, send them to this exact device.”

Example:  
Public IP: `203.0.113.10:8080`  
Port Forwarding sends it to: `192.168.1.5:80`

So yeah, it punches a hole through NAT to let specific traffic in. Powerful but risky if misused.

---

## 🔒 Why does this matter?

- NAT keeps our internal IPs hidden and adds a layer of protection.  
- Port Forwarding is great for remote access or hosting stuff, **but** it's also how a lot of attacks get in if you're careless.

---

## 🧠 TL;DR

| Term             | What it does                            |
|------------------|------------------------------------------|
| NAT              | Hides internal IPs behind a public one   |
| Static NAT       | One-to-one mapping                      |
| Dynamic NAT      | Maps from a pool of public IPs          |
| PAT              | Many devices share one public IP (via ports) |
| Port Forwarding  | Lets outsiders reach devices inside your LAN |

---

That’s it for this one. Makes sense now why routers are a big deal in security. They’re the gatekeepers.
