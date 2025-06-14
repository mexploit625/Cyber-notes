# 📡 Common Protocols

These are the core protocols that power the internet — each one handles a specific kind of communication. Understanding them means understanding how data moves, where the weak spots are, and how attackers might sneak in.

---

## HTTP (HyperText Transfer Protocol)

Used for loading websites — basic web browsing.

- Port: 80  
- Not encrypted (data goes in plain text)

---

## HTTPS (HTTP Secure)

Same as HTTP, but encrypted using SSL/TLS.

- Port: 443  
- Keeps login info, personal data, etc. safe

---

## FTP (File Transfer Protocol)

Transfers files between systems.

- Ports: 20 (data), 21 (control)  
- No encryption — insecure by today’s standards

---

## SFTP (SSH File Transfer Protocol)

Secure file transfer over SSH.

- Port: 22  
- Encrypted and safe — preferred over FTP

---

## SSH (Secure Shell)

Remote terminal access, mostly used for servers.

- Port: 22  
- Fully encrypted — very common in Linux environments

---

## Telnet

Also used for remote access — but totally insecure.

- Port: 23  
- Everything is plain text  
- Rarely used now, except for legacy/testing

---

## SMTP (Simple Mail Transfer Protocol)

Used to send emails.

- Port: 25 (or 587 for secure sending)

---

## IMAP (Internet Message Access Protocol)

Reads email while keeping it on the server — good for multi-device use.

- Port: 143 (or 993 for secure)

---

## POP3 (Post Office Protocol v3)

Downloads and removes email from the server.

- Port: 110 (or 995 for secure)  
- Not really used much now

---

## My thoughts 

The more I learn these, the more I see how the internet is just a bunch of systems talking in different languages — each one with its own tone, rules, and vulnerabilities. You mess with the wrong port or leave something open, and that’s all an attacker needs.
