<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com/watch?v=54TKBqKCEFc)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Deployment
- Step 2: Configuration
- Step 3: Post-Deployment

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h3><strong>Deployment Steps</strong></h3>
<ol><li><p><strong>Prepare Azure Environment</strong>:</p><ul><li>Ensure you have an active Azure subscription.</li><li>Set up a Virtual Network (VNet) with appropriate subnets.</li></ul></li><li><p><strong>Create a Windows Server VM</strong>:</p><ul><li>Deploy a VM using a Windows Server image (e.g., 2019/2022).</li><li>Attach the VM to the VNet.</li><li>Configure necessary ports (e.g., RDP, AD DS).</li></ul></li><li><p><strong>Connect to the VM</strong>:</p><ul><li>Use Remote Desktop Protocol (RDP) to log into the VM.</li></ul></li></ol>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h3><strong>Configuration Steps</strong></h3>
<ol start="4"><li><p><strong>Install AD DS Role</strong>:</p><ul><li>Open <strong>Server Manager</strong> and add the <strong>Active Directory Domain Services</strong> role.</li></ul></li><li><p><strong>Promote the Server to a Domain Controller</strong>:</p><ul><li>Configure a new domain (e.g., <code>example.com</code>).</li><li>Set functional levels and install the DNS server role.</li></ul></li><li><p><strong>Configure DNS</strong>:</p><ul><li>Point the VNet’s DNS to the private IP of the VM.</li></ul></li><li><p><strong>Join Additional VMs to the Domain</strong>:</p><ul><li>Deploy additional VMs in the VNet.</li><li>Configure DNS and join them to the domain.</li></ul></li></ol>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
