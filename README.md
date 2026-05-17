# Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines

<p align="center">
  <img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1 align="center">Azure Network Traffic Analysis Lab (NSGs + Wireshark)</h1>

<p>
This project demonstrates how to inspect and analyze network traffic between Azure Virtual Machines using Wireshark, while also exploring how Network Security Groups (NSGs) control inbound and outbound traffic. The lab focuses on common protocols such as ICMP, SSH, DNS, and HTTP/S.
</p>

---

<h2>Project Summary</h2>

<p>
This tutorial demonstrates how network traffic flows between virtual machines in Microsoft Azure and how Network Security Groups (NSGs) can be used to control that traffic. The project also includes using Wireshark to capture and analyze packets, helping visualize real-time communication between systems.
</p>

<h3>Languages / Tools Used</h3>

- PowerShell
- Command-Line Tools (Command Prompt / Bash)

<h3>Environments Used</h3>

- Microsoft Azure (Virtual Machines)
- Windows 10 (21H2)
- Ubuntu Server 20.04

<h3>Technologies / Protocols Used</h3>

- Wireshark (Packet Analyzer)
- Network Security Groups (NSGs)
- SSH (Secure Shell)
- RDP (Remote Desktop Protocol)
- DNS (Domain Name System)
- HTTP / HTTPS
- ICMP (Internet Control Message Protocol)

---

<h2>High-Level Steps</h2>

- Deploy Virtual Machines in Azure
- Capture Network Traffic Using Wireshark
- Modify Network Security Group Rules
- Analyze Allowed vs Blocked Traffic

---

<h2>Actions and Observations</h2>

<h3>Step 1: Capture Network Traffic</h3>

<p align="center">
  <img width="1252" height="522" alt="image" src="https://github.com/user-attachments/assets/a7d75729-4e42-4157-87e3-ca52ec307ca9" />
</p>

<p>
Wireshark is installed and used to capture live network traffic between virtual machines. Filters are applied to observe specific protocols such as ICMP, DNS, and SSH to understand how data moves across the network.
</p>

<br />

<h3>Step 2: Test Connectivity Between Virtual Machines</h3>

<p align="center">
  <img width="1470" height="957" alt="image" src="https://github.com/user-attachments/assets/20b61023-00d4-4907-a341-bfa014bf8a55" />
</p>

<p>
Connectivity is tested between Azure virtual machines using ICMP (ping). The captured packets in Wireshark show request and reply traffic, confirming successful communication between devices on the same virtual network.
</p>

<br />

<h3>Step 3: Modify Network Security Group Rules</h3>

<p align="center">
  <img width="1427" height="465" alt="image" src="https://github.com/user-attachments/assets/61498c15-fc81-4c3e-b103-74c26a66a18b" />
</p>

<p>
Network Security Group (NSG) rules are modified to either allow or block specific types of traffic. Changes are immediately reflected in network behavior, demonstrating how NSGs enforce security policies at the network level.
</p>

<br />

<h3>Step 4: Observe Blocked vs Allowed Traffic</h3>

<p align="center">
  <img width="1295" height="132" alt="image" src="https://github.com/user-attachments/assets/fe9c7851-e186-48cf-bb4b-51552f05f766" />
</p>

<p>
After modifying NSG rules, Wireshark is used again to observe differences in traffic flow. Blocked traffic no longer appears, while allowed protocols continue to communicate normally, showing how NSGs control network access.
</p>

<br />

---

<h2>Conclusion</h2>

<p>
This project successfully demonstrated how to monitor and analyze network traffic between Azure virtual machines using Wireshark while applying Network Security Groups to control access. The lab provides practical experience in network security, packet analysis, and cloud infrastructure management.
</p>
