<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Preparing AD Infrastructure in Azure</h1>
This project outlines the installation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [Project Walkthrough](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create Resource Group
- Create a Virtual Network
- Create a Domain Controller with the Windows Server 2022 Datacenter OS named `dc-1`
    - Username: adminuser
    - Password: AdminSecurePassword123!!!
- Create a CLient VM with the Windows 10 Pro OS name `client-1`
    - Username: labuser
    - Password: SecurePassword123!!!
- Assign `client-1` DNS settings to match the private IP address from `dc-1`

<h2>Deployment and Configuration Steps</h2>

## Create Virtual Network
### Within Azure create a virtual network, this vn with allow the Virtual Machiness to communicate within the same network
<p>
<img src="https://github.com/user-attachments/assets/ad2197a9-c243-4080-a395-6775cce5ad10" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/091eb8ec-bd16-460a-810e-02ed50089eec" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/b54cf44c-1ffb-4e54-9c7c-d7905435191e" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/2ef952ef-9b55-4f0c-8b25-7223e54312f1" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/ee40c40e-a48f-4f5e-8925-6492477fc548" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />


## Creating the Virtual Machines
### Create the Domain Controller VM
<p>
<img src="https://github.com/user-attachments/assets/03fe46f0-14cd-4409-8521-ff6f95d09b46" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/984a29d1-5a11-437d-aa9a-4477b5f5e269" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/6600e096-fe7d-4892-94bf-aeb886e6152a" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/17b0f803-57b2-41b9-8d77-0e029fb00d7c" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/5dcb7277-92dc-4ddd-9bb6-fc58871020b7" width="550" alt="Disk Sanitization Steps"/>
</p>
<br />

### Be sure to check the Licensing to aviod any errors
<p>
<img src="https://github.com/user-attachments/assets/bef855ee-cdf5-42d8-89b3-c9d63783953f" width="550" alt="Disk Sanitization Steps" />
</p>
<br />


### Click on the Network section and assign the `windows-vnet` to the VM
<p>
<img src="https://github.com/user-attachments/assets/46cbaada-41c5-4b4a-8ff2-56c7c03cd2a0" width="550" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/aa0a4ed0-dc9d-42c9-9f5d-668c4d5a1d6b" width="550" alt="Disk Sanitization Steps"/>
</p>

<br />
