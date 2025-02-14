# Enterprise-IT-Setup
The project focuses on setting up and deploying an IT infrastructure through VMware Workstation and Windows Server while implementing Active Directory Domain Services (AD DS) and Ubuntu Server together with AWS cloud services. This project establishes virtual machines for Windows and Linux systems and integrates the setup with AWS cloud services.

# Technologies Used
* **VMware Workstation**-  Virtualization platform
* **Windows Server 2022** – Core infrastructure server
* **Active Directory Domain Services (AD DS)** – User and resource management
* **Windows 10/11 Client Machine** – Domain-joined workstation
* **Ubuntu Server** – Linux-based server integration
* **AWS EC2 Instance** – Cloud service deployment

# Setup and Deployment
**Step1: Set Up VMware Workstation & Create Virtual Machines**
* Installed VMware Workstation on the host machine.
* Established virtual machines for Windows Server and Windows Client with an Ubuntu Server machine.
  <img width="364" alt="1" src="https://github.com/user-attachments/assets/fff2cc68-5433-42b3-9ae8-50cc0aebeb80" />
  
**Step-2: Installed Windows Server on the VM**
* Loaded Windows Server ISO and complete installation.
* Configured Computer Name, static IP and administrative credentials.

**Step-3: Configured Windows Server & Enable Remote Desktop**
* Given the server a new name then configure network settings.
* Turn on Remote Desktop Protocol (RDP) for accessing machines remotely.
  <img width="493" alt="p6" src="https://github.com/user-attachments/assets/b8902602-c587-4ab4-8822-9a5bec569124" />

**Step-4: Set up AD DS by installing the role through Server Manager and promoting the server to a domain controller.** 
* Installed AD DS role via Server Manager.
* Elevated the server to function as a domain controller and initialize a new domain.
* Confirmed Active Directory Domain Services (AD DS) configuration through Active Directory Users and Computers.
  
  <img width="404" alt="p13" src="https://github.com/user-attachments/assets/9a477089-6f46-4506-bbcb-b56699be353e" />
  <img width="400" alt="p25" src="https://github.com/user-attachments/assets/6b84aedd-abf5-487a-bde6-d6475d5bcf53" />
  <img width="500" alt="p21" src="https://github.com/user-attachments/assets/ff033ee4-1b08-4ef1-a2c0-b70244941f95" />

**Step-5: Connected the Windows Client Machine to the Domain**
* Setup a Windows 10 virtual machine that functions as a client.
* Established a connection to the domain controller then proceed to join the domain.
* Need to check that the client is listed in the Active Directory management console.
  
  <img width="501" alt="p51" src="https://github.com/user-attachments/assets/f2ac809a-589c-4a9a-a8b1-1c3fc6d51dfe" />

**Step-6: Configured Group Policies**
* Enforced security policies through the use of Group Policy Management.
* Applied policies to domain-joined users and machines.
  
  <img width="410" alt="p33" src="https://github.com/user-attachments/assets/ac8d7f37-cf28-49df-8b2b-51a3b31ea988" />

**Step-7: Configured File Sharing & Remote Access**
* Established shared folders on Windows Server to permit access across the entire network.
* Tested file access from client machines.
* Ensured Remote Desktop is functional.
  
  <img width="500" alt="p64" src="https://github.com/user-attachments/assets/4adc84c0-d691-454b-a422-fe7fcdc5cc16" /> 

  <img width="509" alt="p66" src="https://github.com/user-attachments/assets/95267543-4ced-4824-adfb-f9fb74f2de89" />

**Step-8: Install and Configure a Linux Server**
* Instsalled an Ubuntu Server Virtual Machine and established SSH configuration to enable secure remote connections.
  
<img width="522" alt="p2" src="https://github.com/user-attachments/assets/be425a8d-ca68-44a7-99fc-f230d76c9d09" />

<img width="491" alt="q3" src="https://github.com/user-attachments/assets/42feb1b2-ce05-4830-ba4c-a116140a9e91" />

<img width="503" alt="q6" src="https://github.com/user-attachments/assets/e77ed3c9-f81b-430b-9709-4233a9176dbe" />

**Step-9: Deployment of Cloud Services on AWS**
* Established an AWS account before launching an EC2 instance using Windows or Linux.
* Configured firewall controls to enable SSH and RDP connectivity.
* Remotely connected and configured cloud-based services.
  
<img width="515" alt="r3" src="https://github.com/user-attachments/assets/3021daf5-c77e-4e3d-89a2-9e84b4c2a0d2" />

<img width="515" alt="r5" src="https://github.com/user-attachments/assets/3670ec3f-079e-4adb-a493-648070949a24" />

<img width="478" alt="r6" src="https://github.com/user-attachments/assets/386beb20-8fc2-41b6-a0b8-79f693a1a2e6" />

# Project Goals
* 



                                                 
