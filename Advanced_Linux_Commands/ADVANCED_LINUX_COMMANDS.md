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

### Switching User Accounts

```
su johndoe
```

### Modifying User Accounts

- *Changing User Password*

```
sudo passwd johndoe
```

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

- Create 5 users ("mary", "mohammed", "ravi", "tunji", "sofia") and ensure each user belongs to the devops group

```
sudo adduser mary
```

```
sudo adduser mohammed
```

```
sudo adduser ravi
```

```
sudo adduser tunji
```

```
sudo adduser sofia
```

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

