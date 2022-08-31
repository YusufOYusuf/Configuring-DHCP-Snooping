<h1>Configuring DHCP Snooping</h1>


<h2>Description</h2>
In this lab, I learned to configure DHCP snooping. The DHCP (Dynamic Host Configuration Protocol) snooping feature is used to block unauthorized DHCP servers from distributing IP addresses to DHCP clients.
<br />



<h2>Environments Used </h2>

- <b>Ubuntu 20.04.2 LTS</b> 
- <b>PuTTY SSH Client</b>

<h2>Program walk-through:</h2>

<p align="center">
From the left sidebar click PuTTY SSH Client and proceed to put in the IP address, port number, click Telnet and then click open: <br/>
<img src="https://i.postimg.cc/CxTBKt9H/Screen-Shot-2022-08-30-at-7-33-06-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
In the IOU1 terminal type in command "en" to enter into enable mode <br/>
<img src="https://i.postimg.cc/3w6WPcjv/Screen-Shot-2022-08-30-at-7-34-28-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
<br />
In the IOU1 terminal type command "conf t" to enter into "configuraton mode"  <br/>
<img src="https://i.postimg.cc/Hkrgfs66/Screen-Shot-2022-08-30-at-7-35-54-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the IOU1 terminal window execute the following commands  <br/>
1. ip dhcp snooping <br/>
2. ip dhcp snooping vlan 10 <br/>
3. interface e1/0 <br/>
4. ip dhcp snooping trust <br/>
5. ip dhcp snooping limit rate 25 <br/>
6. end <br/>
<img src="https://i.postimg.cc/3xXYYJM7/Screen-Shot-2022-08-30-at-7-40-28-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the IOU1 terminal type command "show ip dhcp snooping".  <br/>
<img src="https://i.postimg.cc/wB5r17Fx/Screen-Shot-2022-08-30-at-7-42-15-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />








  
  
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
