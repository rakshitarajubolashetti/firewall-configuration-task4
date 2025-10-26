# Task 4 – Firewall Configuration and Testing  

## Objective  
To understand how a firewall works by creating, testing, and deleting a custom rule using Windows Defender Firewall. This helped me learn how firewalls control and protect network traffic.

## Tool Used  
- **System:** Windows 10  
- **Tool:** Windows Defender Firewall with Advanced Security  
- **Command for Testing:**  
  Test-NetConnection -ComputerName 127.0.0.1 -Port 23  

## Steps Performed  
1. Opened the firewall using `wf.msc` and checked existing inbound rules.  
2. Created a new inbound rule to block **TCP Port 23 (Telnet)**.  
3. Tested the rule using PowerShell with the above command. The result showed:  
   WARNING: TCP connect to (127.0.0.1 : 23) failed  
   TcpTestSucceeded : False  
   This confirmed that Port 23 was successfully blocked by the firewall.  
4. Deleted the custom rule after testing to restore default settings.

## What I Learned  
- Firewalls protect systems by filtering inbound and outbound traffic.  
- Blocking insecure ports like Telnet (Port 23) helps improve security.  
- Windows Firewall makes it easy to add, test, and manage security rules.

## Screenshots  
- firewall_dashboard.png – Firewall main screen  
- block_port23.png – Rule created to block Port 23  
- test_block_port23.png – PowerShell test result  

## Conclusion  
This task helped me practically understand how firewall rules work and how they protect a system from unwanted connections. By blocking Telnet (Port 23), I confirmed that Windows Firewall can effectively restrict insecure or unnecessary network traffic.

**Name:** Rakshita B  
**Internship:** Elevate Labs – Cyber Security Internship  

**Submitted by:** Rakshita B  
**Cybersecurity Intern – Elevate Labs**
