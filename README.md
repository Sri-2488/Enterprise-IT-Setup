# Enterprise-IT-Setup
The project focuses on setting up and deploying an IT infrastructure through VMware Workstation and Windows Server while implementing Active Directory Domain Services (AD DS) and Ubuntu Server together with AWS cloud services. This project establishes virtual machines for Windows and Linux systems and integrates the setup with AWS cloud services.

# Technologies Used
* **VMware Workstation**-  Virtualization platform
* **Windows Server 2022** – Core infrastructure server
* **Active Directory Domain Services (AD DS)** – User and resource management
* **Windows 10 Client Machine** – Domain-joined workstation
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

   <img width="374" alt="s1" src="https://github.com/user-attachments/assets/5d852c53-4b11-43af-b578-8d1012dbd53c" /> </br>
   <img width="380" alt="s2" src="https://github.com/user-attachments/assets/328a567c-e654-4894-a163-36f576b54b36" /></br>
   <img width="375" alt="s3" src="https://github.com/user-attachments/assets/d25e4526-8f17-47d5-a091-31a5db24dec6" /> </br>
   <img width="382" alt="s4" src="https://github.com/user-attachments/assets/790a3bd1-dde8-45d9-8134-2ef591babb6e" /> </br>
   <img width="518" alt="s6" src="https://github.com/user-attachments/assets/f8c9ed53-e286-448d-862e-a64b57c4a475" /> </br>
  ![s7](https://github.com/user-attachments/assets/920362d6-4f22-44fb-8623-d28b83e35349)                                  </br>
 ![s13](https://github.com/user-attachments/assets/9f813242-1862-4577-af33-d31a6ff2c72b)                                </br>
  ![s12](https://github.com/user-attachments/assets/f7fb115e-5fb3-4996-8166-99c9ca05d8ca)                              </br>
 
![s14](https://github.com/user-attachments/assets/6e294462-2a6d-46bb-a4d2-5a9f18b08c81)                                             </br>
 ![s16](https://github.com/user-attachments/assets/be3fb6f4-a570-4371-9f3c-bd377114a7db)                                       </br>


**Step-5: Connected the Windows Client Machine to the Domain**
* Setup a Windows 10 virtual machine that functions as a client.
* Established a connection to the domain controller then proceed to join the domain.
* Need to check that the client is listed in the Active Directory management console.

  <img width="239" alt="p29" src="https://github.com/user-attachments/assets/7f63a396-f00a-4684-a369-3c470c80e4b2" /> </br>

  <img width="392" alt="p45" src="https://github.com/user-attachments/assets/9c86ba18-3d15-412a-9dc2-f2182558db02" /> </br>

  <img width="221" alt="p46" src="https://github.com/user-attachments/assets/89f4cf63-8df4-4067-a0b9-944ec2988b06" /> </br>

  <img width="304" alt="p48" src="https://github.com/user-attachments/assets/2f9c7d95-6303-4152-8004-922f8533ecdb" /> </br>

  
  <img width="501" alt="p51" src="https://github.com/user-attachments/assets/f2ac809a-589c-4a9a-a8b1-1c3fc6d51dfe" />

**Step-6: Configured Group Policies**
* Enforced security policies through the use of Group Policy Management.
* Applied policies to domain-joined users and machines.

  <img width="455" alt="p36" src="https://github.com/user-attachments/assets/1d5cff6e-3a55-4afc-95a3-45f5d6a0a002" /> </br>

  <img width="503" alt="p40" src="https://github.com/user-attachments/assets/c54db154-2077-4d7f-a4bb-d20800151660" /> </br>

  <img width="491" alt="p39" src="https://github.com/user-attachments/assets/71480a23-1808-401f-83c0-252ba2bb82d1" /> </br>

  <img width="410" alt="p33" src="https://github.com/user-attachments/assets/ac8d7f37-cf28-49df-8b2b-51a3b31ea988" />

**Step-7: Configured File Sharing & Remote Access**
* Established shared folders on Windows Server to permit access across the entire network.
* Tested file access from client machines.
* Ensured Remote Desktop is functional.

  <figure>
  <img width="500" alt="p64" src="https://github.com/user-attachments/assets/4adc84c0-d691-454b-a422-fe7fcdc5cc16" /> 
  <figcaption> Windows Server</figcaption>

    <img width="503" alt="p50" src="https://github.com/user-attachments/assets/9acfd50f-8487-48ee-bf6a-e1462e2df892" />

  <img width="509" alt="p66" src="https://github.com/user-attachments/assets/95267543-4ced-4824-adfb-f9fb74f2de89" />
    <figcaption> Windows 10 Client Machine <figcaption> 
   </figure>
**Step-8: Install and Configure a Linux Server**
* Instsalled an Ubuntu Server Virtual Machine and established SSH configuration to enable secure remote connections.
  
<img width="522" alt="p2" src="https://github.com/user-attachments/assets/be425a8d-ca68-44a7-99fc-f230d76c9d09" /> </br>

<img width="491" alt="q3" src="https://github.com/user-attachments/assets/42feb1b2-ce05-4830-ba4c-a116140a9e91" /> </br>

<img width="503" alt="q6" src="https://github.com/user-attachments/assets/e77ed3c9-f81b-430b-9709-4233a9176dbe" />

**Step-9: Deployment of Cloud Services on AWS**
* Established an AWS account before launching an EC2 instance using Windows or Linux.
* Configured firewall controls to enable SSH and RDP connectivity.
* Remotely connected and configured cloud-based services.
  
<img width="515" alt="r3" src="https://github.com/user-attachments/assets/3021daf5-c77e-4e3d-89a2-9e84b4c2a0d2" /> </br>

<img width="515" alt="r5" src="https://github.com/user-attachments/assets/3670ec3f-079e-4adb-a493-648070949a24" /> </br>

<img width="478" alt="r6" src="https://github.com/user-attachments/assets/386beb20-8fc2-41b6-a0b8-79f693a1a2e6" />

# Project Goals
This project aims to create an extensive Windows Server network environment via VMware Workstation featuring Active Directory Domain Services (AD DS) setup and domain joining for Windows clients. The project extends to setting up an Ubuntu Linux virtual machine for testing purposes while configuring network services and deploying an AWS EC2 instance to replicate cloud-based operations. This project delivers practical experience for users to merge on-premise data centers with cloud platforms while concentrating on remote access methods and security settings.

# Conclusion
The completion of this project involved deploying Windows Server on VMware and both configuring Active Directory along with linking Windows clients to the domain. The AWS EC2 instance was set up to function in a cloud environment while delivering a flexible testing setting. The system configuration enables streamlined management of network services and user policies along with secure remote access which leads to strong integration across infrastructure components.

# Troubleshooting
* During the Windows Server setup on VMware Workstation improper network configuration emerged as a common issue which created connection problems between the virtual machine and other network devices. Proper configuration of the VM’s network adapter to use Bridged or NAT settings solved these connectivity problems.
* The Windows Server required proper DNS settings to communicate with AWS resources since incorrect configurations block this communication leading to verification needs.
* The server’s IP address should be static to prevent domain join failures since dynamic IPs can cause these issues. The configuration of security groups for AWS EC2 instances must allow inbound and outbound traffic on necessary ports such as 3389 for RDP and 22 for SSH.
* Remote access failure occured because of Windows Server or AWS firewall settings which necessitates opening essential ports or editing security group rules.
* AWS EC2 instances experienced slow performance and connection drops when the selected instance type lacks necessary resources which required changing to a suitable instance type to fix these issues.

# Future Improvements
The next phase of development focuses on deployment automation with Terraform, AWS service expansion including S3 and Lambda, and improved security through multi-factor authentication for remote access. Utilizing AWS resource optimization along with instance type experimentation helps to scale infrastructure effectively.

# Author

Srija Chowdary

# License

MIT License

                                                 
