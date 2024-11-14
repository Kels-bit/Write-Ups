-----------------------------------------
## Overview
This goal of this lab is to setup a basic Active Directory (AD) domain.
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

![[Active Directory Running (step 1).png]]

_________
### Step 2: Promote Sever to a Domain Controller.
Install Active Directory on the server using Server Manager. Once complete promote to a Domain Controller.

Press the Manage tab (upper right) > Add Roles and Features to add Active Directory.

![[Add AD (Step 2).png]]

Once in the Add  Roles and Features Wizard hit next until you reach the Server Roles tab, then click Active Directory Domain Services Role to add to server.

![[Check AD (Step 2).png]]

Keep all default and continue clicking next until Confirmation Tab and click install.

![[Install AD (Step 2).png]]

After a successful installation click promote this server to a domain controller.

![[Promte AD (Step 2).png]]

___________
### Step 3:  Create an AD domain (e.g., homelab.local).
Create a AD domain name homelab.local.

![[Domain AD (step 3).png]]

Continue with the Wizard until ready for install. After install, system will restart.

![[Domain install AD (step 3).png]]

_________
### Step 4:  Create organizational units (OUs) for different departments.

Navigate to Active Directory Users and Computers.

![[Create OUs (Step 4).png]]

Create new OUs within homelab.local domain. (USA, Europe, Asia)
Right click domain New > Organizational Unit

![[New OUs (Step 4).png]]

Create more OUs for practice and for better organization.

![[More OUs (Step 4).png]]

------------
### Step 5: Create user accounts and groups within these OUs.

Create new groups (HR Department, IT, Sales)
_Right click domain > New > Group_

![[Create Groups (Step 5).png]]


Create Users, (Bugs Bunny, Daffy Duck, Elmer Fudd, Tweety Bird)
_Right click > New > User_

![[Create Users (Step 5).png]]