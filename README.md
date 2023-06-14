# System Admin Assistant Project 👩‍💻

System Admin Assistant V1.0 ,
This program was designed to help system admins with daily tasks.
The program provide the tools admin need in interactive and organized Inreface using `Whiptail`

## Features

This program helps System Admin perform Tasks like :
 - List Users
 - List Groups
 - Add User
 - Add Group
 - Modify User 
    - Modify UID
    - Add Comment
    - Change Login Name
    - Change Primary GID
    - Lock User
    - Unlock User
    - Change Password 
    - Change default Shell
    - Change Home Directory
 - Modify Group
   - Modify GID
   - Append Users
   - Change Group Name
 - Delete User 
 - Delete Group
 - Change Password
 
## Instructions
 :warning:**Warning** : You need to Run the program with root user or user have root privilege using `sudo`
 
 <div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/349559d9-1e5b-4875-8220-bd1ba15ea26b"> </div>

### Main Menu 
**Main Menu** displays options available to System Admin

 <div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/017ea1fe-7acf-467f-9b4f-e240c632e8f3"> </div>

### List Users
**List Users** option will list all users in the system
from `/etc/passwd` file ( UID ,username ,Directory and default Shell).
> :bulb: **Tip** : I used `printf` to display output in table
> ``` bash
># print header
>printf "%0s  %5s  %20s  %25s\n" "UID"  "User Name"  "Home Dir" "Shell"
># print separator
>printf "=%.0s"  $(seq 1 70)
># insert a newline
>printf "\n"
> ```

 <div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/572d7ff8-9b3a-40f2-b068-926416cafb1b"> </div>

 ### List Groups
 **List Groups** option will list all groups in the system from `/etc/group`file (GID ,groupname and users in the group)

<div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/185e5a2e-3fc5-4e60-aa7d-1d4646c21232"> </div>

### Add User
**Add User** Option will ask system admin for new username and check if it exists ,then add the username using `useradd` command

<div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/af44eafc-15bc-42eb-82b1-8a10382ee83d"> </div>

### Add Group
**Add Group** Option will ask system admin for new group name and check if it exists ,then add the group name using `groupadd` command
<div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/0ba89162-a09a-498a-91b0-4670195b2270"> </div>

### Modify User
**Modify User** Option will display menu contain options to modify existing user using  `usermod`

<div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/40c015d6-f505-4376-a57a-41f6a23d498a"> </div>

### Modify Group
**Modify Group** Option will display menu contain options to modify existing group using  `groupmod`

<div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/e23d3f7d-61e3-4827-a5dc-f319f028c900"> </div>

### Delete User
**Delete User** Option will ask system admin for username check if exists , then ask the admin to choose delete user with Home Directory or not using `userdel`

<div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/8b077847-d79e-4d97-b056-c77a2d4cfd2b"> </div>

### Delete Group
**Delete Group** Option will ask system admin for group name check if exists , then ask the admin to confirm deletion using `groupdel`

<div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/83f91ac7-b299-49ed-a1fd-08380e8490e4"> </div>

### Change Password
**Change Password** option will ask system admin to change password for existing user using `passwd`

<div> <img src="https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/17092283-6949-449a-aecd-d72941ed7ab5"> </div>
