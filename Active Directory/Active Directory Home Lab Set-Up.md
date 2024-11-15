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
[Capture2]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%202%20(Step%202).png
[Capture3]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%203%20(Step%202).png
[Capture4]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%204%20(Step%202).png
[Capture5]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%205%20(Step%202).png
[Capture6]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%206%20(step%203).png
[Capture7]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%207%20(step%203).png
[Capture8]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%208%20(Step%204).png
[Capture9]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%209%20(Step%204).png
[Capture10]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%2010%20(Step%204).png
[Capture11]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%2011%20%20(Step%205).png
[Capture12]: https://github.com/Kels-bit/Assets/blob/main/AD-Images-Lab-1/Capture%2012%20(Step%205).png
