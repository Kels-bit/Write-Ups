----------------
## Overview
The goal of this lab is to setup a basic Active Directory (AD) domain.

Steps: 
1. Install Windows Server in a Virtual Machine.
2. Promote the server to a Domain Controller (DC).
3. Create an AD domain (e.g., homelab.local).
4. Create organizational units (OUs) for different departments.
5. Create user accounts and groups within these OUs.

____________________
## Steps

### Step 1: Installing Windows Server in a Virtual Machine.
I will be creating a virtual machine running Windows Server 2022 using  VMware Workstation Pro. 

Downloads:  
[VMware Workstation Pro](https://knowledge.broadcom.com/external/article?articleNumber=368667)
[Windows Server 2022](https://www.microsoft.com/en-us/evalcenter/download-windows-server-2022)

Windows Server 2022 installed and running using VMware.

![image1][Capture1]

_________
### Step 2: Promote Sever to a Domain Controller.
Install Active Directory on the server using Server Manager. Once complete promote to a Domain Controller.

Press the Manage tab (upper right) > Add Roles and Features to add Active Directory.

![image2][Capture2]

Once in the Add  Roles and Features Wizard hit next until you reach the Server Roles tab, then click Active Directory Domain Services Role to add to server.

![image3][Capture3]

Keep all default and continue clicking next until Confirmation Tab and click install.

![image4][Capture4]

After a successful installation click promote this server to a domain controller.

![image5][Capture5]

___________
### Step 3:  Create an AD domain (e.g., homelab.local).
Create a AD domain name homelab.local.

![image6][Capture6]

Continue with the Wizard until ready for install. After install, system will restart.

![image7][Capture7]

_________
### Step 4:  Create organizational units (OUs) for different departments.

Navigate to Active Directory Users and Computers.

![image8][Capture8]

Create new OUs within homelab.local domain. (USA, Europe, Asia)
Right click domain New > Organizational Unit

![image9][Capture9]

Create more OUs for practice and for better organization.

![image10][Capture10]

------------
### Step 5: Create user accounts and groups within these OUs.

Create new groups (HR Department, IT, Sales)
_Right click domain > New > Group_

![image11][Capture11]


Create Users, (Bugs Bunny, Daffy Duck, Elmer Fudd, Tweety Bird)
_Right click > New > User_

![image12][Capture12]

[Capture1]: https://github.com/user-attachments/assets/5b47f4b6-b3ec-4a3c-ad1d-4a559e7004e3
[Capture2]: https://github.com/user-attachments/assets/94ac4718-88f5-4eb9-8b03-5c9bb3258c32
[Capture3]: https://github.com/user-attachments/assets/2a642fe0-c64a-4dba-8d12-c8133d88aa21
[Capture4]: https://github.com/user-attachments/assets/54a2bc11-34f4-48e7-8a34-88df8afbf3ea
[Capture5]: https://github.com/user-attachments/assets/9a5115ca-dc15-4f5c-b2a5-06c80fbcb3b2
[Capture6]: https://github.com/user-attachments/assets/1adb8bc1-80c6-42ec-b4bc-5fc104893966
[Capture7]: https://github.com/user-attachments/assets/a5a515e4-d05a-4426-aede-3a3df6486e39
[Capture8]: https://github.com/user-attachments/assets/bbedb625-97ae-45ce-af10-1825f0d88df8
[Capture9]: https://github.com/user-attachments/assets/82fe98f8-1a22-4fcc-ac29-35e23be11c4d
[Capture10]: https://github.com/user-attachments/assets/5e0f2c7e-2b4f-4866-b554-96dbcb7eb1f2
[Capture11]: https://github.com/user-attachments/assets/ae263e55-71f5-41f8-89a8-bd62b7740c02
[Capture12]: https://github.com/user-attachments/assets/6d989784-a41f-44b5-a35d-8bc8a09ea92e

