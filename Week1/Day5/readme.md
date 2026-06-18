# Day 5 – TCP/UDP, Ports & Nmap

## Theory
- TCP three-way handshake: SYN → SYN-ACK → ACK.
- Common ports: 21 FTP, 22 SSH, 25 SMTP, 53 DNS, 80 HTTP, 443 HTTPS, 3389 RDP.
- UDP is fast and connectionless, used for streaming, gaming, DNS.
- Nmap scan types: ping sweep (-sn), version detection (-sV), port range (-p), full scan (-p-).

## Lab
- Launched TryHackMe AttackBox.
- Deployed Nmap target (or used scanme.nmap.org).
- Ran ping sweep, default scan, service detection, and full port scan.
- Successfully identified open ports and service versions (e.g., HTTP on 80, SSH on 22).

( Port 80 was filtered/closed on the target; Nmap correctly reported this.)
