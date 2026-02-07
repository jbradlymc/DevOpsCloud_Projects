Level 1 — Manual Networking

PROJECT OVERVIEW

This project focuses on fundamental networking concepts by manually building a Local Area Network (LAN), intentionally breaking connectivity, and restoring it through logical troubleshooting.

The goal is to deeply understand how data moves, not to rely on automation or tools that hide the fundamentals.


OBJECTIVES
1. Build a basic LAN using manual IP configuration
2. Understand how IP addressing, subnetting, ARP, and ICMP work together
3. Develop a structured troubleshooting mindset
4. Simulate real-world networking errors and resolve them logically


TOOLS USED
1. Cisco Packet Tracer
2. Windows Command Prompt (CMD)


NETWORK TOPOLOGY
    Devices:
        1. 3 PCs 
        2. Switch (Cisco 2960)
        3. Router (Cisco 1941)

PC1 ─┐
     │
PC2 ─┼── Switch ── Router
     │
PC3 ─┘


IP ADDRESSING PLAN

| Device | IP Address   | Subnet Mask   | Default Gateway |
| ------ | ------------ | ------------- | --------------- |
| Router | 192.168.1.1  | 255.255.255.0 | —               |
| PC1    | 192.168.1.10 | 255.255.255.0 | 192.168.1.1     |
| PC2    | 192.168.1.20 | 255.255.255.0 | 192.168.1.1     |
| PC3    | 192.168.1.30 | 255.255.255.0 | 192.168.1.1     |


STEPS:
1. BUILD: Build the network manually (no DHCP)
2. BREAK: Intentional Failures
    a. Scenario 1 - Wrong IP Address
    b. Scenario 2 - Wrong Subnet Mask
    c. Scenarrio 3 - Wrong Default Gateway Address
3. FIX: Troubleshoot and Fix