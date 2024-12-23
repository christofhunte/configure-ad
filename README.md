<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (22H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1
- Step 2
- Step 3
- Step 4

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/Z6rVp93.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First step I did was create a Resource Group in Azure and titled it "Active-Directory-Lab".
</p>
<br />

<p>
<img src="https://i.imgur.com/cRjq0oK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next step I did was create a virtual network and subnet for the virtual machines to run on. I placed the virtual network in the the Resource Group I created.
</p>
<br />

<p>
<img src="https://i.imgur.com/R3cztcO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/7JuFful.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/UtjTLIv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I then created a virtual machine for the domain controller and titled it "dc-1". I set its operating system to Windows Server 2022 with the username "chlabuser". I also set it's size to 2 vcpus with a 16 GiB memory to be certain the server can handle all that I will be doing going forward.
</p>
<br />

<p>
<img src="https://i.imgur.com/0gLg1pf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/EVM8NNu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/zohJrYl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I created another virtul machine for the client titled "client-1". I gave it the same Username and password as "dc-1" for lab purposes. I attached it to the same virtual network and resource group as "dc-1" and used Windows 10 (22H2) for the image.
</p>
<br />

<p>
<img src="https://i.imgur.com/W34r5bK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I set Domain Controller’s NIC Private IP address to be static so that when I set Client-1's DNS settings to DC-1's private IP address, there wouldn't be any change which would cause confusion later navigating client-1's server.
</p>
<br />

<p>
<img src="https://i.imgur.com/W34r5bK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I set Domain Controller’s NIC Private IP address to be static so that when I set Client-1's DNS settings to DC-1's private IP address, there wouldn't be any change which would cause confusion later navigating client-1's server.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
