# Configuring-On-premises-Active-Directory-within-Azure-VMs
<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1
- Step 2
- Step 3
- Step 4

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/2ab35262-3971-4727-a542-e245a44edd3b"/>
</p>
<p>
First go to Microsoft Azure and type Resource Group 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/bbaa41e2-d3fb-4479-a90c-f4462759f6ea"/>
</p>
<p>
Next click create to create the Resource Group
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/7d172964-31b9-4803-a324-ad768c70c8c5"/>
</p>
<p>
Now for the name type AD-LAb and the region under US West US 3 then go to the review and create tab 
</p>
<br />


<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/20b91653-279e-4a5d-9731-4ed229abd1ce"/>
</p>
<p>
Next the validation pass through 
</p>
<br />


<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/423985b6-0399-48c6-b659-14f64e9f8c89"/>
</p>
<p>
Now once the process is done you will see the Resource Group was created 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/ad25a52e-2b2c-444d-b1e9-5be18b516090"/>
</p>
<p>
Type Virtual Machine in the search bar 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/cfa8962d-0b01-4711-b314-dbd18edc04d5"/>
</p>
<p>
Next click Azure Virtual Machine to create the VM
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/21a7d91a-4c51-46cd-9361-784fea32dc2c"/>
</p>
<p>
Now for the resource group click AD-LAb, and the virtual machine name type DC-1. The region put under US West US 3 and the image under Windows Server
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/3bb65ff1-041d-4d79-8484-bf9405119a99"/>
</p>
<p>
Next the size needs to be under Standard E2 and teh username under labuser and the password under your own unique password. Remember to open a notepad and type all your info out so you dont lose it.
</p>
<br />
