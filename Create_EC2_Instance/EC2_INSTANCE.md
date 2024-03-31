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

- Review your chosen options for the instance and finish by launching the instance.

### Connecting to your launched EC2 instance (Ubuntu server)##

**There are a number of ways to connect to your server but we are going to use the SSH (Secure Shell) Method.**

- Open up the terminal (in this case we are using Git)

- Navigate to the directory in which the key-pair you created was stored

- Run `chmod 400 "key-pair"` in your terminal

- Go to your launched instance and click it to open so you can see its summary.

- Select Connect and select client tab.

- Copy the ssh command given under the example and paste in your terminal and press enter

- You should be prompted to give a Yes/No response. Type in Yes and you should be inside your Linux server.

## Installing, Updating and Removing Software

### Updating Package Lists

- Update Package lists by running the following command:

```
sudo apt update
```

### Installing software packages

- Let us try and install a command called 'tree'

- We will do so by running the following command:

```
sudo apt install tree
```

### Updating Installed Packages

- Update installed packaged by running the following command:

```
sudo apt upgrade
```

### Removing software packages

- To remove the 'tree' package install earlier, run this command:

```
sudo apt remove tree
```

