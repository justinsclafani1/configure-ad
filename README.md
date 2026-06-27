<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in Microsoft Azure</h1>

This project demonstrates the deployment and configuration of an on-premises Active Directory environment using Microsoft Azure Virtual Machines.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop
- Active Directory Domain Services

<h2>Operating Systems Used</h2>

- Windows Server 2025
- Windows 11 (25H2)

<h2>Implementation Overview</h2>

1. Azure infrastructure was deployed including a Resource Group, Virtual Network, and virtual machines for the Domain Controller and client system.
2. Active Directory Domain Services was installed and the server was promoted to a domain controller for the domain.
3. Domain configuration was completed, including Organizational Units, administrative accounts, and domain join operations.
4. Additional administration tasks were performed using PowerShell, Group Policy configuration, and authentication log validation.

<h2>Implementation Evidence</h2>

<p>
<img width="959" height="382" alt="Resource Group and Virtual Network" src="https://github.com/user-attachments/assets/b4ed082d-a4c9-48d1-b087-ec4138d5098c" />
</p>
<p>
Azure Resource Group and Virtual Network configured to support the Active Directory environment.
</p>
<br />

<p>
<img width="959" height="295" alt="DC-1 Virtual Machine Creation" src="https://github.com/user-attachments/assets/d26b68f8-1e97-4dae-b25f-5ce959c711e6" />
</p>
<p>
Windows Server 2025 virtual machine (DC-1) deployed as the Active Directory Domain Controller.
</p>
<br />

<p>
<img width="959" height="381" alt="Client-1 and DNS Configuration" src="https://github.com/user-attachments/assets/17406a98-a6cb-429f-957b-d7feb9699294" />
</p>
<p>
Windows 11 client virtual machine deployed with DNS configured to reference the Domain Controller.
</p>
<br />

<p>
<img width="560" height="365" alt="Active Directory Domain Services Install and Domain Promotion" src="https://github.com/user-attachments/assets/badfbab6-52f6-4fef-9f09-9170c0811012" />
</p>
<p>
Active Directory Domain Services installed and DC-1 promoted to domain controller for the mydomain.com domain.
</p>
<br />

<p>
<img width="558" height="361" alt="Organizational Units and Admin User (jane_admin)" src="https://github.com/user-attachments/assets/114a5490-0c71-478f-ba4b-cbefbc4892d9" />
</p>
<p>
Organizational Units and an administrative account were created within Active Directory for domain management.
</p>
<br />

<p>
<img width="556" height="356" alt="Domain Join and CLIENTS Organizational Unit" src="https://github.com/user-attachments/assets/9eba21fe-787c-4498-84a7-6d8a16b8c374" />
</p>
<p>
Client-1 was joined to the domain, and its computer object was placed into a dedicated Organizational Unit.
</p>
<br />

<p>
<img width="819" height="463" alt="Network Verification" src="https://github.com/user-attachments/assets/7dce13d6-a43f-4024-afae-df1ea8d57781" />
</p>
<p>
Network connectivity and DNS resolution between Client-1 and the Domain Controller confirmed.
</p>
<br />

<p>
<img width="758" height="421" alt="Powershell User Creation" src="https://github.com/user-attachments/assets/a4b465af-9801-447c-a928-16d76fe884cb" />
</p>
<p>
Multiple Active Directory user accounts created via PowerShell automation and confirmed within Active Directory Users and Computers.
</p>
<br />

<p>
<img width="686" height="185" alt="User Login Test" src="https://github.com/user-attachments/assets/de33ebf3-cbd6-4f9b-9556-4c8ad9d692da" />
</p>
<p>
Domain user authentication validated through successful login to Client-1.
</p>
<br />

<p>
<img width="581" height="359" alt="Group Policy Lockout Configuration" src="https://github.com/user-attachments/assets/d54b3ba5-c997-4dc6-ba44-688133bf0c8f" />
</p>
<p>
Account lockout policy configured via Group Policy to enforce authentication security controls.
</p>
<br />

<p>
<img width="302" height="395" alt="Account Lockout and Recovery" src="https://github.com/user-attachments/assets/d92de9bd-88e8-4569-bf7a-e3c359273ecc" />
</p>
<p>
Account lockout behavior and recovery process validated within Active Directory.
</p>
<br />

<p>
<img width="932" height="407" alt="Event Viewer Authentication Logs" src="https://github.com/user-attachments/assets/b1d3e8ba-e42b-4b70-8990-b9c6d39d9fb9" />
</p>
<p>
Security event logs analyzed in Event Viewer to validate authentication activity, including successful and failed login attempts.
</p>
<br />
