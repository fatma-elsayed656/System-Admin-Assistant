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
 
 ![root privilege](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/e42920b2-5fb3-40a9-85dc-d51c9a67fd8a)

### Main Menu 
**Main Menu** displays options available to System Admin

 ![main menu](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/c293ed72-fc6d-4862-b472-1acfab7ad677)


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

 ![list users](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/d865db67-aa1c-43bb-90ee-852570259809)


 ### List Groups
 **List Groups** option will list all groups in the system from `/etc/group`file (GID ,groupname and users in the group)

![list groups](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/da3119fe-14ef-420c-be96-a433cb7ae1a8)


### Add User
**Add User** Option will ask system admin for new username and check if it exists ,then add the username using `useradd` command

![add user](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/42dcf0f4-f571-4905-bcc7-4cd7fdda27d0)


### Add Group
**Add Group** Option will ask system admin for new group name and check if it exists ,then add the group name using `groupadd` command

![add group](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/2b4ff855-b6bf-4960-aa90-b90cc6e288a2)

### Modify User
**Modify User** Option will display menu contain options to modify existing user using  `usermod`

![modify user](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/d51e3300-1b36-4a3c-b98c-1d1e92914498)


### Modify Group
**Modify Group** Option will display menu contain options to modify existing group using  `groupmod`

![modify group](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/4cd7473e-5292-48ca-bd4e-cc6f12d955de)


### Delete User
**Delete User** Option will ask system admin for username check if exists , then ask the admin to choose delete user with Home Directory or not using `userdel`

![delete user](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/b252be04-d241-48b9-b4dc-698d64525863)


### Delete Group
**Delete Group** Option will ask system admin for group name check if exists , then ask the admin to confirm deletion using `groupdel`

![delete group](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/703cccc0-1e8c-4acf-9d4c-1f329b19e94e)


### Change Password
**Change Password** option will ask system admin to change password for existing user using `passwd`

![change password](https://github.com/fatma-elsayed656/System-Admin-Assistant/assets/135543396/5100048f-1066-4278-b38c-e21a29e29296)

