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

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/9319be66-069e-4170-8aca-5498bc8b12e2"/>
</p>
<p>
Next click the box in the Licensing section and then click th econfirm box. Then click review and create 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/2ae3c544-c562-4247-84f1-878b68045f24"/>
</p>
<p>
Now go to the networking tab and make sure the virtual network, subnet, and the public IP all says (new)
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/40e5830a-4e4a-47ef-873a-d178b6592834"/>
</p>
<p>
Now go to the review and create section 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/d001f26b-93b9-4f36-b146-23d5bcc06528"/>
</p>
<p>
Next let the deployment progess load 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/a4017821-7d27-4ab7-91a6-b04fa467f625"/>
</p>
<p>
Now the process will be complete when there is a green check 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/80d04256-ffcb-4d47-a93a-de6f38304d29"/>
</p>
<p>
Next type virtual machine and you will see DC-1 VM was created
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/04c3a764-33ce-462f-a1f7-6b01300f4a3e"/>
</p>
<p>
Next click create and then go to Azure Virtual Machine 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/69a42173-e8e8-4b79-9fd1-b2fdd064445c"/>
</p>
<p>
Next in the subscriiption section make sure the same subscription that you used for the resource group is selected. Then in Resource Group click AD-Lab then for the name type Cilent-1 and the region click US West US 3
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/7e636d9a-cbdc-4eeb-8e27-99d34d345dce"/>
</p>
<p>
Now for the Image click Windows 10 pro version and the size click Standard E2
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/f8993172-9c42-482e-8a3e-f831c32acf9b"/>
</p>
<p>
Next for the username type labuser and the password the same as DC-1 VM. Then click the Licensing tab then click review and create 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/b5335eee-d6c4-4d58-ae9e-5c4896c93117"/>
</p>
<p>
Now the deployment will be done when a green check appears next to the deployment
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/8cf04195-6679-428e-a77f-06899ae7dc06"/>
</p>
<p>
Next type virtual machines in the search bar 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/f0ed0801-4d05-4531-96e9-054f6d9d1800"/>
</p>
<p>
Next you will see that DC-1 and Cilent-1 was created 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/0f5791a0-296f-40a0-9d8d-4dd40f783b0c"/>
</p>
<p>
Now click DC-1 and click networkng 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/667a5e43-913b-4276-9f10-d2fff584106b"/>
</p>
<p>
Next click on the Network Interface 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/6217f4e0-7135-4bcb-8605-cd54b8b86943"/>
</p>
<p>
Next click on IP Configurations 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/5de5cb97-2158-411d-9b7f-51363d08152b"/>
</p>
<p>
Now click ipconfig1
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/3f192efc-718d-42e4-bdf1-086e76260773"/>
</p>
<p>
We are editing the IP Configurations in the allocation section click Static instead of Dynamic then click save.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/0bc6094c-bb28-41e7-91ee-bdc940843048"/>
</p>
<p>
Now we are going to log into Cilent-1 VM copy the public IP address
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/7cee9a52-24e3-4a47-b743-fda018088b52"/>
</p>
<p>
Next type Remote Desktop Connection and click to open the app
</p>
<br />
