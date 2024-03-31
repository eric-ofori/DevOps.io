# Creating and launching an Ubuntu Amazon EC2 instance

### Step 1: Sign into your AWS account

- Sign in to your created AWS account

### Step 2: Create the EC2 instance (Ubuntu Server)

- On the top left of your console, select services and search for Elastic Compute Cloud (EC2)

![EC2 DASHBOARD](/Create_EC2_Instance/Images/EC2_DASHBOARD.png)

- From the menu on the left side, select instances.

- Select launch instance on the top right side

![LAUNCH_INSTANCE](/Create_EC2_Instance/Images/LAUNCH_INSTANCE.png)

- Fill the required portions indicating the linux distribution you want to use (in our case Ubuntu 20.04), memory size, the instance name, Security group and key-pair (**do not forget to download and store this is a safe place**).

![EC2_DETAILS](/Create_EC2_Instance/Images/EC2_DETAILS.png)

- Review your chosen options for the instance and finish by launching the instance.

![EC2_SUCCESS](/Create_EC2_Instance/Images/EC2_SUCCESS.png)

### Connecting to your launched EC2 instance (Ubuntu server)##

**There are a number of ways to connect to your server but we are going to use the SSH (Secure Shell) Method.**

- Open up the terminal (in this case we are using Git)

![GIT](/Create_EC2_Instance/Images/GIT.png)

- Navigate to the directory in which the key-pair you created was stored

![KEY_PAIR](/Create_EC2_Instance/Images/KEY_PAIR.png)

- Run `chmod 400 "key-pair"` in your terminal

![CHMOD](/Create_EC2_Instance/Images/CHMOD.png)

- Go to your launched instance and click it to open so you can see its summary.

![INSTANCE_SUMMARY](/Create_EC2_Instance/Images/INSTANCE_SUMMARY.png)

- Select Connect and select client tab.

![SSH_CLIENT](/Create_EC2_Instance/Images/SSH_CLIENT.png)

- Copy the ssh command given under the example and paste in your terminal and press enter
```
ssh -i "key-pair" ubuntu@instance_id
```

![SSH_COMMAND](/Create_EC2_Instance/Images/SSH_COMMAND.png)

- You should be prompted to give a Yes/No response. Type in Yes and you should be inside your Linux server.

![INSTANCE_LOGIN](/Create_EC2_Instance/Images/INSTANCE_LOGIN.png)

# Installing, Updating and Removing Software

### Updating Package Lists

- Update Package lists by running the following command:

```
sudo apt update
```

![UPDATE_PCK_LIST](/Create_EC2_Instance/Images/UPDATE_PCK_LIST.png)

### Installing software packages

- Let us try and install a command called 'tree'

- We will do so by running the following command:

```
sudo apt install tree
```

![TREE](/Create_EC2_Instance/Images/TREE.png)

- Verify the 'tree' installation by runnning the following command (ensure that the DevOps directory is already created with file(s) created inside):
```
tree DevOps/
```

![TREE_VERIFY](/Create_EC2_Instance/Images/TREE_VERIFY.png)

### Updating Installed Packages

- Update installed packages by running the following command:

```
sudo apt upgrade
```

![UPGRADE](/Create_EC2_Instance/Images/UPGRADE.png)

### Removing software packages

- To remove the 'tree' package install earlier, run this command:

```
sudo apt remove tree
```

![REMOVE](/Create_EC2_Instance/Images/REMOVE.png)
