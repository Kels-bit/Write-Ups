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
Check GPM Pic
_Right Click your Domain > Choose the Create a GPO in this domain, and link here... option_
Create GPO pic
### Activity #1: Create a Password Policy
Set a password policy to enforce strong passwords and enhance security.
- Password Age
- Password length 
- Password Complexity Requirements

Act 1 Password set pic
_Creating the Password Policy_
Act 1  Password Policy made pic
_successful creation of new "Password Policy"_
Navigate to Computer Configuration > Policies > Windows Settings > Security Settings > Account Policies > Password Policy to configure the policy.
pic 5
Set Password Age setting to 90 days. (Password will expire after 90 days.)
pic 6

Set Password Length to 12 characters min.
pic 7
Set Password Complexity 
pic 8

Screenshot of all the Policies Configured for the Password Policy  that was created.
pic 9

_____
### Activity #2: Create a Drive Mapping Policy
Maps network drives for users when they log in.

Create Drive Mapping Group Policy
Pic 11

Navigate: User Configuration > Preferences > Windows Settings > Drive Maps
pic 12

Right Click Drive Maps 
Name the location \\servername\folder 
Make it consistent buy choosing the same drive letter 

pic 13
_____
### Activity #3: Create a Desktop Wallpaper Policy
Sets a default wallpaper for all users.
pic 14

Right click the policy then navigate to User Configuration > Policies >  Administrative Templates > Desktop > Desktop > Desktop Wallpaper 
pic 15

Click Enable, choose the path, and wallpaper style to configure the policy.
pic 16
_____
### Activity #4: Create a Control Panel Policy
Prevents users from accessing the Control Panel.

Create a Control Panel Policy.
pic 17

Right click the policy then navigate to User Configuration > Policies > Administrative Templates >  Control Panel > Prohibit access to Control Panel and PC settings.

pic 18

Click the Enable option and apply to restrict access to the Control Panel.

Pic 19
### Activity #5: Create a USB Storage Policy
Prevents users from using USB storage devices.

Create USB Device Policy
Pic 20

Right click the policy then navigate to Computer Configuration > Policies > Administrative Templates >  Systems > Removable Storage Access > All Removable Storage Classes: Deny all access
pic 21

Check the enable options and apply
pic 22

_____
### Activity #6: Create an Account Lockout Policy
Set account lockout settings to prevent brute force attacks.
- Account lockout duration (Until System Admin resets it.).
- Account lockout failed attempts (5).

Create an Account Lockout Policy
pic 23

Right click the policy then navigate to Computer Configuration > Policies >  Windows Settings > Security Settings > Account Policy > Account Lockout 
 pic 24

Accounts will stayed lockout until an Admin resets it.
pic 25

Accounts will be locked after 5 failed logon attempts.
pic 26