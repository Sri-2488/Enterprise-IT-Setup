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
* Created Users, Groups and assigned Users in Groups.

   <img width="374" alt="s1" src="https://github.com/user-attachments/assets/5d852c53-4b11-43af-b578-8d1012dbd53c" /> </br>
   <img width="380" alt="s2" src="https://github.com/user-attachments/assets/328a567c-e654-4894-a163-36f576b54b36" /></br>
   <img width="375" alt="s3" src="https://github.com/user-attachments/assets/d25e4526-8f17-47d5-a091-31a5db24dec6" /> </br>
   <img width="382" alt="s4" src="https://github.com/user-attachments/assets/790a3bd1-dde8-45d9-8134-2ef591babb6e" /> </br>
   <img width="518" alt="s6" src="https://github.com/user-attachments/assets/f8c9ed53-e286-448d-862e-a64b57c4a475" /> </br>
    ![s7](https://github.com/user-attachments/assets/ecd97538-1eca-4b22-a527-2f00a1781909)  </br>
     ![s13](https://github.com/user-attachments/assets/52451660-c33c-4139-b6eb-e1b51f791e6a)   </br>
     ![s12](https://github.com/user-attachments/assets/4328cddc-c29c-48d9-944e-67db00f8900c)           </br>
      ![s14](https://github.com/user-attachments/assets/fc7269e7-0e35-46a4-8ee4-9a9c8834e189)     </br>
       ![s16](https://github.com/user-attachments/assets/f5e6e2da-f118-4743-9446-be7542c879cf)   </br>


**Step-5: Connected the Windows Client Machine to the Domain**
* Setup a Windows 10 virtual machine that functions as a client.
* Established a connection to the domain controller then proceed to join the domain.
* Need to check that the client is listed in the Active Directory management console.

  <img width="392" alt="p45" src="https://github.com/user-attachments/assets/9c86ba18-3d15-412a-9dc2-f2182558db02" /> </br>
  ![s26](https://github.com/user-attachments/assets/14b93711-41b9-49fb-bd53-9aac3e002bb3)             </br>
  ![s27](https://github.com/user-attachments/assets/d7a758fb-229c-4918-9d75-dbef312c0711)               </br>
![s28](https://github.com/user-attachments/assets/ec03ea2a-bcd0-4767-b64a-92ed606ef73f)                 </br>
![s29](https://github.com/user-attachments/assets/1b9a03d6-ca6e-409b-841c-656413d47384)                 </br>
![s30](https://github.com/user-attachments/assets/0115bacd-e282-458a-b0a6-d8931d8b9c58)                 </br>
![s31](https://github.com/user-attachments/assets/9bec7a0d-e4a4-4467-ac4b-77cea8efd19c)                 </br>
![s32](https://github.com/user-attachments/assets/072bd4aa-a0db-4c6e-9919-77c133e03c27)                  </br>
![s34](https://github.com/user-attachments/assets/147d4c79-5034-48b8-a940-5191b6b61a0a)


  

**Step-6: Configured Group Policies**
* Enforced security policies through the use of Group Policy Management.
* Created Organizational Units (OU), created some of the policies in them and assigned users or groups to the policies.
* Applied policies to domain-joined users and machines.

![s17](https://github.com/user-attachments/assets/952b447e-20bb-4c3e-8d36-f32aa67498be)             </br>
![s18](https://github.com/user-attachments/assets/1d532666-b722-46f2-9908-3383a09c63ff)             </br>
![s21](https://github.com/user-attachments/assets/fe57f3de-414b-44be-b7b5-015e05675bb1)             </br>
![s23](https://github.com/user-attachments/assets/da29ebaf-b5d1-4407-a19e-c2bb7d1a0f6d)              </br>
![s24](https://github.com/user-attachments/assets/8f9338a8-c765-43c8-8258-92b2f89be8c8)              </br>
![s25](https://github.com/user-attachments/assets/7f16ceb6-1f29-4a78-a825-6b437647c214)              </br>


**Step-7: Configured File Sharing & Remote Access**
* Established shared folders on Windows Server to permit access across the entire network.
* Tested file access from client machines.
* Ensured Remote Desktop is functional.
![s36](https://github.com/user-attachments/assets/3060cbba-df67-43fd-b9d9-14d57c4325cf) </br>
![s37](https://github.com/user-attachments/assets/e170bbe8-c037-411f-903f-93fb7ff19ae0) </br>
![s38](https://github.com/user-attachments/assets/d5b6e68c-967e-43c1-8d34-9d7593c53df5) </br>

 
**Step-8: Install and Configure a Linux Server**
* Instsalled an Ubuntu Server Virtual Machine and established SSH configuration to enable secure remote connections.
  
<img width="522" alt="p2" src="https://github.com/user-attachments/assets/be425a8d-ca68-44a7-99fc-f230d76c9d09" /> </br>

<img width="491" alt="q3" src="https://github.com/user-attachments/assets/42feb1b2-ce05-4830-ba4c-a116140a9e91" /> </br>

![s39](https://github.com/user-attachments/assets/a47cf99e-a9cb-40ec-ac31-de9bd455930b)    </br>
![s40](https://github.com/user-attachments/assets/97c219de-9472-4363-90f6-85ce676add2f)    </br>

![s41](https://github.com/user-attachments/assets/d768a3c8-47b6-49f1-93aa-1116ae122768)     </br>

**Step-9: Deployment of Cloud Services on AWS**
* Established an AWS account before launching an EC2 instance using Windows or Linux.
* Configured firewall controls to enable SSH and RDP connectivity.
* Remotely connected and configured cloud-based services.
  
<img width="515" alt="r3" src="https://github.com/user-attachments/assets/3021daf5-c77e-4e3d-89a2-9e84b4c2a0d2" /> </br>
<img width="486" alt="s42" src="https://github.com/user-attachments/assets/d52e8e9e-b811-43bf-b976-d768b5ce08b1" /> </br>
<img width="598" alt="s43" src="https://github.com/user-attachments/assets/5a095010-a4ba-46c7-a580-9967626970f7" />  </br>
<img width="650" alt="r8" src="https://github.com/user-attachments/assets/9fe40536-ad9a-4199-8642-0ab9402bbaa0" />  </br>
<img width="487" alt="r10" src="https://github.com/user-attachments/assets/5276de7a-6e58-47ff-b014-3715cf18cd6d" /> </br>
<img width="715" alt="r11" src="https://github.com/user-attachments/assets/e1852912-9638-4cff-9f81-8a46fc2f790e" />  </br>
<img width="680" alt="r12" src="https://github.com/user-attachments/assets/4a259ec1-e3ae-4bab-b714-e33c5a720f6e" /> </br>
<img width="581" alt="r13" src="https://github.com/user-attachments/assets/fdd174ee-9399-408d-a565-885f78748259" />


 





# Project Goals
This project aims to create an extensive Windows Server network environment via VMware Workstation featuring Active Directory Domain Services (AD DS) setup and domain joining for Windows clients. The project extends to setting up an Ubuntu Linux virtual machine for testing purposes while configuring network services and deploying an AWS EC2 instance to replicate cloud-based operations. This project delivers practical experience for users to merge on-premise data centers with cloud platforms while concentrating on remote access methods and security settings.

# Conclusion
The completion of this project involved deploying Windows Server on VMware and both configuring Active Directory along with linking Windows clients to the domain. The AWS EC2 instance was set up to function in a cloud environment while delivering a flexible testing setting. The system configuration enables streamlined management of network services and user policies along with secure remote access which leads to strong integration across infrastructure components.

# Troubleshooting
* During the Windows Server setup on VMware Workstation improper network configuration emerged as a common issue which created connection problems between the virtual machine and other network devices. Proper configuration of the VM’s network adapter to use Bridged or NAT settings solved these connectivity problems.
* The Windows Server required proper DNS settings to communicate with AWS resources since incorrect configurations block this communication leading to verification needs.
* The server’s IP address should be static to prevent domain join failures since dynamic IPs can cause these issues. The configuration of security groups for AWS EC2 instances must allow inbound and outbound traffic on necessary ports such as 3389 for RDP and 22 for SSH.
* Remote access failure occured because of Windows Server or AWS firewall settings which necessitates opening essential ports or editing security group rules.
* When sharing a file, check the permissions under the Security tab in the folder's properties to determine whether access is granted to everyone or restricted to a specific group within the domain.
* AWS EC2 instances experienced slow performance and connection drops when the selected instance type lacks necessary resources which required changing to a suitable instance type to fix these issues.

# Future Improvements
The next phase of development focuses on deployment automation with Terraform, AWS service expansion including S3 and Lambda, and improved security through multi-factor authentication for remote access. Utilizing AWS resource optimization along with instance type experimentation helps to scale infrastructure effectively.

# Author

Srija Chowdary
(All the screenshots above showcase the work I have done.)

# License

MIT License

                                                 
