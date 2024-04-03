# Advanced Linux Commands

**Chmod Command**

- Let's create a file

```
touch script.sh
```

- Let's check the permission of the file

```
ls -latr script.sh
```

### Updating file permissions

```
chmod +x script.sh
```

- lets check the permission of the file

```
ls -latr script.sh
```

- We can modify using the numbers

```
chmod 755 script.sh
```

```
chmod 777 script.sh
```

```
ls -latr script.sh
```

- Now lets look at the chown command

- Format for the chown command

```
chown [option] owner:[group] file(s)
```

- Example

```
chown john:developer filename.txt
```

### Superuser Priviledges

- Changing to root user

```
sudo -i
```

- Exit root user

### Creating a user

```
sudo adduser johndoe
```

![1_JohnDoe](/Advanced_Linux_Commands/Images/1_JohnDoe.png)

- Greanting Administrative Priviledges

```
sudo usermod -aG sudo johndoe
```

![2_JohnDoe_AdminPriviledges](/Advanced_Linux_Commands/Images/2_JohnDoe_AdminPriviledges.png)

### Switching User Accounts

```
su johndoe
```

![3_Switching_User_Accounts](/Advanced_Linux_Commands/Images/3_Switching_User_Accounts.png)

### Modifying User Accounts

- *Changing User Password*

```
sudo passwd johndoe
```

![4_Changing_User_Passwds](/Advanced_Linux_Commands/Images/4_Changing_User_Passwds.png)

- Test Login with new user

```

```

![5_Test_Login_New_User](/Advanced_Linux_Commands/Images/5_Test_Login_New_User.png)

### Creating a Group

- To create a group run the following command:

```
sudo groupadd developers
```

### Adding Users to the Group

```
sudo usermod -aG developers johndoe
```

### Verifying Group Memberships

```
id johndoe
```

### Deleting a User

```sudo userdel username
```

### Ensuring Proper Group Permissions

```
sudo chown :developers /path/to/directory
```

### Granting read and write permissions to the group:

```
sudo chmod g+rw /path/to/directory
```

## Side Hustle Task 3

- Create a group on the server and name it 'devops'

```
sudo groupadd devops
```

![6_Creating_Group_devops](/Advanced_Linux_Commands/Images/6_Creating_Group_devops.png)

![7_devops_group](/Advanced_Linux_Commands/Images/7_devops_group.png)

- Create 5 users ("mary", "mohammed", "ravi", "tunji", "sofia") and ensure each user belongs to the devops group

```
sudo adduser mary
```

![8_Mary](/Advanced_Linux_Commands/Images/8_Mary.png)

```
sudo adduser mohammed
```

![9_Mohammed](/Advanced_Linux_Commands/Images/9_Mohammed.png)

```
sudo adduser ravi
```

![10_Ravi](/Advanced_Linux_Commands/Images/10_Ravi.png)

```
sudo adduser tunji
```

![11_Tunji](/Advanced_Linux_Commands/11_Tunji.png)

```
sudo adduser sofia
```

![12_Sofia](/Advanced_Linux_Commands/12_Sofia.png)

-Create 'home' foler for each user

![13_Home_folders_Users](/Advanced_Linux_Commands/13_Home_folders_Users.png)

- Ensure that each user belongs to the devops group

```
sudo usermod -aG devops mary
```

```
sudo usermod -aG devops mohammed
```

```
sudo usermod -aG devops ravi
```

```
sudo usermod -aG devops tunji
```

```
sudo usermod -aG devops sofia
```

![14_Adding_Users_to_devops](/Advanced_Linux_Commands/14_Adding_Users_to_devops.png)

![15_Users_Added_to_devops](/Advanced_Linux_Commands/15_Users_Added_to_devops.png)

- Ensure that the group ownership of each created folder belongs to "devops"

```
sudo usermod :devops /home/mary
```

```
sudo usermod :devops /home/mohammed
```

```
sudo usermod :devops /home/ravi
```

```
sudo usermod :devops /home/tunji
```

```
sudo usermod :devops /home/sofia
```

![16_Group_Ownerhisp_HomeFolders](/Advanced_Linux_Commands/16_Group_Ownerhisp_HomeFolders.png)

![17_Result_Group_Ownerhisp_HomeFolders](/Advanced_Linux_Commands/17_Result_Group_Ownerhisp_HomeFolders.png)
