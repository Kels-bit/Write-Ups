_____
## __Overview__
The goal of this lab is to create and configure Group Policy Objects (GPO) for the homelab.local domain.
### Activities:
1. Password Policy
2.  Drive Mapping Policy
3.  Desktop Wallpaper Policy  
4.  Control Panel Policy
5.  USB Storage Policy
6.  Account Lockout Policy
_____
## __Activities__

### Check: Make sure Group Policy Management Console (GPMC) is installed on the Windows Server.

Make sure the Group Policy Management feature is installed for the Windows Server.

![GPM check](https://github.com/user-attachments/assets/b11fcdb1-a398-42b9-9d72-0ea305f671cf)

_Right Click your Domain > Choose the Create a GPO in this domain, and link here... option_

![Create GPO](https://github.com/user-attachments/assets/73ad343e-3b0f-4109-a630-33e10e8d146d)

### Activity #1: Create a Password Policy
Set a password policy to enforce strong passwords and enhance security.
- Password Age
- Password length 
- Password Complexity Requirements

![Act 1 Password set up](https://github.com/user-attachments/assets/82b7e7a9-9faa-4496-98e6-a8deb5451273)

_Creating the Password Policy_

![Act 1 Password Policy made](https://github.com/user-attachments/assets/3e24a7c6-237a-4b54-abc0-c8c262fdc112)

_successful creation of new "Password Policy"_

Navigate to Computer Configuration > Policies > Windows Settings > Security Settings > Account Policies > Password Policy to configure the policy.

![Act 1 Password nav -5 ](https://github.com/user-attachments/assets/b01bca0c-5192-467c-94ff-2fa2594fb45c)

Set Password Age setting to 90 days. (Password will expire after 90 days.)

![Act Password Age - 6](https://github.com/user-attachments/assets/5b34f2d3-d65f-4185-a00f-80b5e65708c4)


Set Password Length to 12 characters min.

![Act Password Length - 7](https://github.com/user-attachments/assets/3f2f0161-94e6-4ab4-bea0-bc0a37309c16)

Set Password Complexity. 

![Act Password Complex - 8](https://github.com/user-attachments/assets/0f8c2933-c58b-40d2-98b7-96f6cd054cd1)


Screenshot of all the Policies Configured for the Password Policy that was created.

![Act Password settings - 9](https://github.com/user-attachments/assets/cd6196e7-a8f8-4288-a493-7142f6e70b68)


_____
### Activity #2: Create a Drive Mapping Policy
Maps network drives for users when they log in.

Successful creation of the new Drive Mapping Policy.

![Act 2 Drive map - 11](https://github.com/user-attachments/assets/7c93f11a-9cc2-4677-adf6-5b1d80ce7caa)


Navigate: User Configuration > Preferences > Windows Settings > Drive Maps

![Act 2 Drive map - 12](https://github.com/user-attachments/assets/3ed49f8e-82e6-4d8f-9b34-fa31d0babd9c)


Right Click Drive Maps 

- Name the location \\servername\folder
- Make it consistent buy choosing the same drive letter 

![Act 2 Drive map - 13](https://github.com/user-attachments/assets/b2b3fc16-27fd-4fb7-ba0b-599ffbce17b2)

_____
### Activity #3: Create a Desktop Wallpaper Policy
Sets a default wallpaper for all users.

Successful Creation of the neew Desktop Wallpaper Policy

![Act 3 Desktop Wallpaper Policy - 14](https://github.com/user-attachments/assets/d0c9dd05-2138-47f5-bbc7-0ae618a54bc0)


Right click the policy then navigate to User Configuration > Policies >  Administrative Templates > Desktop > Desktop > Desktop Wallpaper

![Act 3 Desktop Wallpaper Policy - 15](https://github.com/user-attachments/assets/f0562d3a-186f-4e4c-b9e8-8cb436861062)


Click Enable, choose the path, and wallpaper style to configure the policy.
![Act 3 Desktop Wallpaper Policy - 16](https://github.com/user-attachments/assets/c874fa83-e36a-4719-b349-b64e490d85c8)

_____
### Activity #4: Create a Control Panel Policy
Prevents users from accessing the Control Panel.

Successful creation of the new Control Panel Policy.

![Act 4 Control Panel - 17](https://github.com/user-attachments/assets/e3737a95-3dab-4f74-8992-cb495b86c918)


Right click the policy then navigate to User Configuration > Policies > Administrative Templates >  Control Panel > Prohibit access to Control Panel and PC settings.

![Act 4 Control Panel - 18](https://github.com/user-attachments/assets/810cee46-0e58-44a2-8a60-d62aa0c58254)


Click the Enable option and apply to restrict access to the Control Panel.

![Act 4 Control Panel - 19](https://github.com/user-attachments/assets/a1d4fab0-e1b1-451c-ad13-018765944314)

_____
### Activity #5: Create a USB Storage Policy
Prevents users from using USB storage devices.

Successful creation of the new USB Device Policy.

![Act 5 USB Devices - 20](https://github.com/user-attachments/assets/c9161bc0-ba20-48da-844d-db964751f219)

Right click the policy then navigate to Computer Configuration > Policies > Administrative Templates >  Systems > Removable Storage Access > All Removable Storage Classes: Deny all access.

![Act 5 USB Devices - 21](https://github.com/user-attachments/assets/33326647-e91a-4254-82e7-37473e388c71)


Check the enable option and apply.

![Act 5 USB Devices - 22](https://github.com/user-attachments/assets/5038dc82-fd1b-40cc-8675-50cc5c06a72c)


_____
### Activity #6: Create an Account Lockout Policy
Set account lockout settings to prevent brute force attacks.
- Account lockout duration (Until System Admin resets it.).
- Account lockout failed attempts (5).

Successful creation of the new Account Lockout Policy.

![Act 6 Account lockout - 23](https://github.com/user-attachments/assets/4e36bb67-bcfa-41fa-b102-db19acf22709)


Right click the policy then navigate to Computer Configuration > Policies >  Windows Settings > Security Settings > Account Policy > Account Lockout.

![Act 6 Account lockout - 24](https://github.com/user-attachments/assets/6debc725-0528-4f31-ac18-592952894833)

Accounts will stayed lockout until an Admin resets it.

![Act 6 Account lockout - 25](https://github.com/user-attachments/assets/8b493728-1ffb-43f5-9b11-6cdc7258c76d)

Accounts will be locked after 5 failed logon attempts.

![Act 6 Account lockout - 26](https://github.com/user-attachments/assets/19022eb3-b088-4ee4-875b-2da4458fd99a)


