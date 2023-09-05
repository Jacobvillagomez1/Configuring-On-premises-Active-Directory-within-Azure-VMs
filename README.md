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

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/8fb28bb8-9e13-4115-8900-2cf8a338ca3b"/>
</p>
<p>
Next paste the IP of Cilent-1 in the computer section 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/56423833-9ca1-4e30-bdde-24c5508c152d"/>
</p>
<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/714f1e25-9e0b-431f-8d73-1da1908ee50e"/>
</p>
<p>
Now tpye for the username type labuser and the password type the password you made for the VM, then click ok
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/06d7c39a-e864-4cfe-9905-a7121d9d2457"/>
</p>
<p>
Next click yes to open the VM
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/9f693248-c914-46ab-aa8e-80bed6da0a67"/>
</p>
<p>
Now you should see the VM loading under the name labuser 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/c70b82b7-4382-47ae-ae0e-d782e8dc8a31"/>
</p>
<p>
Next click no to the following image above 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/b085de07-1e8f-45ff-b7d6-88412bb08c5d"/>
</p>
<p>
Once networks load click yes 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/8b6d5ae6-5c7d-44e4-a20c-05647d3a9a85"/>
</p>
<p>
Now open up command prompt 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/2b4973a6-77b0-4bae-9a9b-d1f225fe96d4"/>
</p>
<p>
Next go back to Azure and copy the Private IP of DC-1
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/32f7e581-f58d-4483-8743-b067b24a708f"/>
</p>
<p>
Go back to Cilent-1 VM and type ping -t the the private IP of DC-1. We are doing a endless ping to see the traffic 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/55e8a294-7e44-44ad-9824-1a41a465ea68"/>
</p>
<p>
Then go to Azure and grab the Public IP of DC-1 VM then load Remote Desktop Connection and open the app  
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/4583ff7e-e4c9-4eb5-88be-fc3c4c4f9995"/>
</p>
<p>
Paste the IP of DC-1 in the computer section then click connect 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/dc52a45a-6782-4d7b-8180-214ce6158c52"/>
</p>
<p>
Next type the username labuser and the password you made for DC-1 VM then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/1b17a0c4-24af-4d5a-b4e8-15c9408a123f"/>
</p>
<p>
Next click yes to log into the VM
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/36f616fd-8423-4235-a9e2-da570f213cf3"/>
</p>
<p>
Once the VM loads let Server Manager load as well. Next once networks load click yes 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/a23e9065-4bde-41be-976a-a044e726775d"/>
</p>
<p>
Next type wf.msc in the search bar of DC-1 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/32520177-a2ef-4f9e-8d4d-9c193d8e8baa"/>
</p>
<p>
Next click on Inbound Rules 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/b27bb6cc-7d6a-493b-8079-b38d1ee2f302"/>
</p>
<p>
Next click the protocol, then look for ICMPv4 protcol
</p>
<br />


<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/6d53aec3-cff6-4b4d-9363-b9040e8577bb"/>
</p>
<p>
Next right click then enable rule for the following in the image above 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/660351d4-7b2b-472e-b355-12f21025cc9e"/>
</p>
<p>
Go back to Cilent-1 VM and you wil see the constant pinging click Ctrl + C then go back to the directory
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/a885a1a1-7ae2-4eac-bb37-66ee8bb7a36b"/>
</p>
<p>
Next go to DC-1 and click add roles and features 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/099486a7-ce1f-4732-b82b-add2bf2fcdb4"/>
</p>
<p>
Click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/75a51ee8-5dd7-4805-8f84-42a1d0191e06"/>
</p>
<p>
Click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/b88aa771-41fb-4283-af7f-d75a598b6bba"/>
</p>
<p>
Click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/3c5e8364-49fd-4a87-91c2-46563e4efb1e"/>
</p>
<p>
Click the box for Active Directory Domain Services 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/5cfef78a-1dc7-4f99-a8dc-88831af6e9c7"/>
</p>
<p>
Click the add features 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/a904d8e1-623f-4df7-adeb-007268c39667"/>
</p>
<p>
Click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/8dce276a-20ca-4919-a1b7-bad2b1f4e1d2"/>
</p>
<p>
Click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/984ab1ef-fb8b-4c3b-b05c-095b5d3ddcca"/>
</p>
<p>
Click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/2696ccd0-c159-48bd-ba14-077cf9e40b64"/>
</p>
<p>
Click Install 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/108624e0-9e54-476f-9c69-ab78f1ce4ed4"/>
</p>
<p>
Next let the installation process start
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/567aa4b3-d65a-4dac-9151-87c2d9f72e71"/>
</p>
<p>
Once the process finishes click close 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/fcf1593b-917c-4d7b-9f44-381e937562e6"/>
</p>
<p>
Next click the caution symbol near manage on the top right 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/067a661f-29a8-471c-a362-82202bb2f9f0"/>
</p>
<p>
Next click Promote this server to a domain controller 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/c709abb1-f85a-46d6-8552-bdb246034825"/>
</p>
<p>
Click add a new forest then type mydomain.com then click next. {NOTE} you can type anything you want just have a .com at the end of it please copy it down to your notepad to not forget 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/f4d0e028-a2fa-442d-8316-ee45eaf005b6"/>
</p>
<p>
Next type the password in for this my password will be Password1 then click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/ed56b7fe-3dd9-4a4a-80d0-3732919bff90"/>
</p>
<p>
Next click next
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/16fed491-7bf9-45b0-984c-97b5e5f769c8"/>
</p>
<p>
Next click next
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/0789fc2f-61fd-458f-b1ab-0c4aad4da4b1"/>
</p>
<p>
Next click next
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/b69dff26-9ddd-4e9d-8aa3-bebb91b9dce0"/>
</p>
<p>
Next click next
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/2dff13dc-20a0-4c9b-97f8-a96fe1b753a1"/>
</p>
<p>
Next click install to finish creating the domain controller 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/851bac16-2857-49a4-97f2-718b3a4470ed"/>
</p>
<p>
Then let the installation process finish 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/88a0dbde-5c1c-48f9-8cbe-5fe5ff4a1cb9"/>
</p>
<p>
You might see the image above for Reconnecting dont click cancel let the VM bandwidth connect back only if it doesnt kick you out properly then click cancel 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/9018461c-8592-46d2-ab77-a721142545c3"/>
</p>
<p>
Go back to Azure and click DC-1 copy the public IP 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/ef0abb63-54b6-420a-97bb-4fed450a9871"/>
</p>
<p>
Next type Remote Desktop Conenction and open the app 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/922279f1-9ef3-47ad-a3f8-3d85294b2e80"/>
</p>
<p>
Now since we made DC-1 under another name click more choices then click use a different account 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/a03503ad-020a-4d26-ad3e-df3ff017c439"/>
</p>
<p>
Next tpye in mydomain.com\labuser for the username and the password is Password1 then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/cbbfdea3-7b3a-4483-925d-c33f49d4c9ce"/>
</p>
<p>
Next click yes to log into the VM {NOTE} if it doesnt work the first time try again to log in. If it still doesn't let you then close Remote Desktop Connection and do the process again 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/d8131e1f-b25f-4d04-b65b-3a53905c75fb"/>
</p>
<p>
Now once you are in the DC-1 VM let Server Manager load on the screen 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/bf8ab7eb-20cd-4f00-9b75-d8a30c299d4f"/>
</p>
<p>
Next click Tools on the top right then go to Active Directory Users and Computers 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/9e37bf8b-9612-411c-b3e4-bce96821898e"/>
</p>
<p>
Next click on mydomain.com folder on the left side 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/aa9f7abb-1250-475c-aa8b-0df5dde626af"/>
</p>
<p>
Next right click anywhere and go to new then to organizational unit 
</p>
<br />


<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/2da9a029-87ec-4608-a92a-275ac7cc3cd5"/>
</p>
<p>
Next type _EMPLOYEES then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/7563f4fb-a7c8-4bd4-9f52-0d527c214e4a"/>
</p>
<p>
Now go back to mydomain.com and right click anywhere again, go to new then to organizational unit 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/1d9d210a-741a-440d-a029-7af26c750663"/>
</p>
<p>
Next type ADMINS then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/43d15d55-415b-4fee-b2ad-36282f6704bc"/>
</p>
<p>
In ADMINS right click then go to new then to user
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/5ecc8a96-b727-41fa-a0bf-0c41169302d4"/>
</p>
<p>
For the first name type jane and the intials can be doe or the last name can be doe. For the user logon name type jane_admin then click next 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/74600f4d-1c15-438b-8364-b4d81b28df2d"/>
</p>
<p>
Next for the password type Password1 then uncheck user must change password at next login  
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/406d7077-f41f-4503-8e0f-5ecf613a367e"/>
</p>
<p>
Next check the box for Password never expires then click next
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/9e6cc56e-cebc-4e35-a847-f869bae00e60"/>
</p>
<p>
Then finish to create the user 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/49a3edab-3467-48d3-857f-f62363bb08ef"/>
</p>
<p>
Now you should see jane doe account in the ADMINS folder if not right click then go to refresh 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/d1fda67c-04db-4a7d-a961-56175140c792"/>
</p>
<p>
Next right click the account and go to properties 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/91b3bde9-8ee8-4d35-b5fa-190dc8850201"/>
</p>
<p>
Next the member of tab then click add 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/43587478-a918-4390-9c7a-a41ad4a8c0b6"/>
</p>
<p>
Next in the enter section type domain then click check names 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/9db1856c-35a1-4321-b1e5-f3ab287927e1"/>
</p>
<p>
Next double click on Domain Admins then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/b0b4fa87-f1a4-4199-938d-cf7359b4e7eb"/>
</p>
<p>
Then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/08e5dea4-a552-4c81-aa08-bfc48793c0cd"/>
</p>
<p>
Then click apply to finish 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/6fa7ba5c-4236-4e03-9f61-7619eb62df9e"/>
</p>
<p>
Next open command prompt then type whoami you will see we are still under labuser and not jane doe next type logoff 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/702a31f2-03ee-4e18-9701-8981a64ba60c"/>
</p>
<p>
Go back to Azure and click DC-1 and copy the Public IP
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/e8e29ad0-2aa7-4b18-8f2a-a582e23980f6"/>
</p>
<p>
Next type Remote Desktop Connection and open the app
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/7d700907-3cc5-431b-98f0-a37d65e1b3ec"/>
</p>
<p>
Next paste DC-1 VM public IP then click connect 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/5f10add9-bf30-4aa7-81ab-d83b1000d0b2"/>
</p>
<p>
Next click more choices then click use a different account
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/9c0046b0-84ef-47c0-a14f-1337cac6fdeb"/>
</p>
<p>
Next type mydomain.com\jane_admin in the username then the password is still Passsword1 then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/08c70bdd-4da0-414e-be79-d51b57e51b9e"/>
</p>
<p>
Next click yes to log into DC-1 VM
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/2b3e72ea-0ceb-453a-8012-d66c78df24c8"/>
</p>
<p>
DC-1 VM should load and you will see the name jane doe.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/e1872b43-6a00-4378-895a-ef730ced9b33"/>
</p>
<p>
Open command line then type whoami and you will see you are logged in as jane_admin 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/991eb684-0118-4420-b7d8-46c8c5b62477"/>
</p>
<p>
Next right click the windows icon on the bottom left then click the system file 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/ca7edc7e-f5a5-4e71-9271-95a201e7bde7"/>
</p>
<p>
Now click Rename this PC (advanced)
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/167d7c20-efb0-4122-b11b-9e0537d4b2b7"/>
</p>
<p>
Next click change 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/09893ccd-1680-437c-87e2-ddcfe9aa58d4"/>
</p>
<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/b149e245-84ee-4bf8-8a37-c8b48eefa62e"/>
</p>
<p>
Next click member of and click the domain circle, then type domain.com then click ok 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/fcdd96ce-0d3b-4e59-919b-9c0fa77da602"/>
</p>
<p>
Now you will see an error displyed on the screen click ok this is because we have to change the NIC in azure for Cilent-1
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/1dc42180-09dc-4ea2-a91e-ee0533ec444a"/>
</p>
<p>
Now go to the Azure portal and go to Virtual Machine then click DC-1, copy the NIC Private IP
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/c56d3f3c-21ea-4519-bbd1-54138e525937"/>
</p>
<p>
Next click Cilent-1 and go to Network Interface and click on cilent 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/d441f8cb-4e31-46e1-b26f-73320b72ed2b"/>
</p>
<p>
Next click DNS servers then click custom 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/940c1feb-2931-4d21-9a39-313d1dd21af7"/>
</p>
<p>
Now paste the NIC Private IP of DC-1 then click save 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/320e0df8-7201-47b9-8416-e845374097ac"/>
</p>
<p>
Next let the process change the NIC
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/cb2f13af-e7ea-4643-8356-9e5ebd18eeb3"/>
</p>
<p>
Once its done you will see a green check you can click the bell icon to see the prcess load 
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs/assets/143027686/48480f92-8917-4975-9a22-81918bac31cb"/>
</p>
<p>
Next go back to Virtual Machine adn click restart then click yes to restart Cilent-1 VM
</p>
<br />
