<h1>Active Directory Home Lab</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
In this home lab we're going to walk through how to create an Active Directory home lab Environment using Oracle Virtual Box. Configuring and running this lab will definitely help show how active directory and windows networking works.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Oracle VirtualBox</b> 
- <b>Windows 10</b>
- <b>Windows Server 2022</b>
- <b>Windows Powershell ISE</b>


<h2>Program walk-through:</h2>

<p align="center">
Network Diagram: <br/>
<img src="https://i.imgur.com/aNSGu02.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install server (Domain Controller) on Oracle Virtual Box: <br/>
<img src="https://i.imgur.com/99045xS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set up IP Addressing:
(a.)	Rename NICs for ease of identification: <br/>
<img src="https://i.imgur.com/dr2SdSq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
(b.)	Then give addressing to the internal only while the INTERNET gets an IP address from the home router: <br/>
<img src="https://i.imgur.com/1TGgqgZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a domain (by installing Active Directory Domain Services) then create dedicated domain admin account:  <br/>
<img src="https://i.imgur.com/XOwsmUj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create an organizational unit for the admin account:  <br/>
<img src="https://i.imgur.com/p8SRaJ5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create RAS/NAT. This is what will allow our client to be able to allow Client be on a VPN but still be able to access the internet through the domain controller (DC) :  <br/>
<img src="https://i.imgur.com/rZmdtAS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setup the DHCP server on the DC. This help client gets an IP address that will let them get on the internet even though they are on a private internal network:  <br/>
<img src="https://i.imgur.com/CbIu7nO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Use PowerShell scripting to create new users on the domain server:  <br/>
<img src="https://i.imgur.com/UTbuyWy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm if the new user group was created:  <br/>
<img src="https://i.imgur.com/n52iRTX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create a windows 10 virtual machine (Client 1):  <br/>
<img src="https://i.imgur.com/jaoaKxK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
(b.) Confirming that the IP Addressing works:  <br/>
<img src="https://i.imgur.com/Xlg8pby.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Attempt pinging the internet to confirm the DNS server works:  <br/>
<img src="https://i.imgur.com/EKXv6eK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 Create RAS/NAT. This is what will allow our client to be able to allow Client be on a VPN but still be able to access the internet through the domain controller (DC) :  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


Oluwatobi Omotayo <omotayotobi2020@gmail.com>
23:14 (0 minutes ago)
to me
Summary:
Building this Active Directory home lab provided hands-on experience in deploying and managing enterprise identity infrastructure. I learned how to install and configure Active Directory Domain Services (AD DS), create and organize domain users and administrative accounts, configure DHCP for automated IP assignment, and implement NAT/RAS to enable secure internal network access with external internet connectivity. Additionally, I gained practical experience using PowerShell scripting to automate user provisioning and managing client systems within a domain environment. These steps reinforced core concepts such as DNS resolution, domain authentication, network segmentation, and centralized access control.  
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
Autofill

;
