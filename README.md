<h1>Active Directory Home Lab</h1>

<!-- ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo) 

--!>

<h2>Description</h2>
In this project, I built a basic Windows networking environment lab with an active directory, DHCP and other networking services using a virtual box and a PowerShell script that automated the creation of 1000 users on the private network. A Domain controller was installed on the virtual machine using the server 2019 ISO and configured by giving it two network adaptors one for the internal network and the other for the internet, I installed the active directory where my domain (practicelab.com) was created and configured with NAT and Routing so that clients on the private network can reach the internet through the Domain Controller, and then the DHCP, which will automatically assign an IP to the windows 10 client.
I have provided relevant screenshots that capture the steps I took in this project.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 


<h2>Environments Used </h2>

- <b>Windows 10 IS0 </b> (21H2)
<br />
- <b>Oracle Virtual Box</b> (21H2)
<br />
- <b>Server 2019 IS0</b> (21H2)






<h2>Program walk-through:</h2>

<p align="center">
The Diagram schema of what we want to do: <br/>
<img src="https://i.imgur.com/ZcZHACo.png" height="80%" width="80%" alt="Schema Diagram"/>
<br />


<br />
The Virtual Box and Domain Comptroller installed (Server 2019 ISO):  <br/>
<img src="https://i.imgur.com/bX82w1m.png" height="80%" width="80%" alt="Domain comptroller installation Step"/>
<br />


<br />
Setting up IP for our internal network:  <br/>
<img src="https://i.imgur.com/daTLkFX.png" height="80%" width="80%" alt="Dsetting up internal IP"/>
<br />


<br />
Installing Active Directory in the Domain Comptroller: <br/>
<img src="https://i.imgur.com/VOzXEaD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<br />
Configuring Active Directory:  <br/>
<img src="https://i.imgur.com/uk1NBOJ.png" height="80%" width="80%" alt="server configuration"/>
<br />


<br />
Creating Organisational Units (practiselab.com):  <br/>
<img src="https://i.imgur.com/8Iy1ogE.png" height="80%" width="80%" alt="organisational configuration"/>
<br />


<br />
Configuring DHCP:  <br/>
<img src="https://i.imgur.com/lMIaZgP.png" height="80%" width="80%" alt="server configuration"/>
<br />

<br />
Creating over 1000 users:  <br/>
<img src="https://i.imgur.com/Eym5xBM.png" height="80%" width="80%" alt="server configuration"/>
<br />


<br />
1000 users created in Active Directory:  <br/>
<img src="https://i.imgur.com/0y7Yv15.png" height="80%" width="80%" alt="server configuration"/>
<br />



<br />
Windows 10 client installed and configured properly, note that the gateway IP is same IP with the DHCP Server, so to access the internet this client has to go throught the Domain Comproller where we have the DHCP server :  <br/>
<img src="https://i.imgur.com/hkKLAq1.png" height="80%" width="80%" alt="Clients connects to internet via DHCP"/>
<br />


<br />
Domain Controller (practicelab.com) works fine and responds as seen below:  <br/>
<img src="https://i.imgur.com/LXNKq8o.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />


<br />
Windows 10 Client also connects and responds to the internet:  <br/>
<img src="https://i.imgur.com/W5RrsUX.png" height="80%" width="80%" alt="Active Directory Steps"/>
<br />



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
