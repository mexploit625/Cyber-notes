 #  NAT & Port Forwarding

##  What is NAT (Network Address Translation)?
- NAT is used to translate private (local) IP addresses to a public IP address before packets are sent to the internet.
- It helps preserve IPv4 addresses and adds a layer of security by hiding internal IPs.

###  Types of NAT:
- **Static NAT** – One-to-one mapping between a private and public IP.
- **Dynamic NAT** – Maps private IPs to any available public IP from a pool.
- **PAT (Port Address Translation)** – Many-to-one. Multiple private IPs share one public IP using different port numbers. Also known as **NAT Overload**.



---

##  What is Port Forwarding?
- A way to allow external devices to access services on a private network through specific ports.
- Commonly used for gaming servers, SSH, web hosting, etc.

###  How It Works:
A router receives a request on a public IP + port and forwards it to a specific private IP + port.

**Example:**  
`203.0.113.5:8080` → forwards to → `192.168.0.10:80`

---

##  why is it matter?
- NAT helps secure internal networks by masking internal IPs.
- Port forwarding is necessary when services need to be reachable from outside — but must be done carefully to avoid vulnerabilities.

---

##  Quick Summary
| Term             | Purpose                               |
|------------------|---------------------------------------|
| NAT              | Translates private ↔ public IPs       |
| Static NAT       | One-to-one mapping                    |
| Dynamic NAT      | One-to-many (from a public IP pool)   |
| PAT              | Many-to-one using port numbers        |
| Port Forwarding  | Routes traffic to devices behind NAT  |
