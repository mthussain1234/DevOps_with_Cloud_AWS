# Launch

1. Launch instance as done before, and assign a name, then we explore the AMI and go through the catalogue, we selected **ubuntu 20.04**.


![download (1)](https://user-images.githubusercontent.com/129314018/232080098-aad120bb-1dd1-4b4a-abd3-ace9236bb81d.png)

2. After sorting out our AMIs, we change our security group, you can use a new one, but we decide to use an existing one as seen below.


![download](https://user-images.githubusercontent.com/129314018/232080162-ae80fa5b-2a4a-44e2-ab4e-318ca0b7f3f2.png)

3. Under the advanced tab, we go under user data and enter our scripting commands as seen below. 

```
#!/bin/bash 
sudo apt update -y 
sudo apt upgrade -y 
sudo apt install nginx -y 
sudo systemctl restart nginx 
sudo systemctl enable nginx
```

![download](https://user-images.githubusercontent.com/129314018/232080187-6a725125-3265-40ce-82b7-8023de7a2fe5.png)

4. We then navigate to our instance details and find our **public ip address**, which we will then paste into our browser to see if nginx has in fact been installed.

We can see the IP matches.

![image](https://user-images.githubusercontent.com/129314018/232084554-c201a1d4-e3a2-4ae0-9378-c5aa1028fa01.png)


# Make an environment

`printenv`: Prints all environment variables.
`env`: Displays all current environment variables and their values.
`printenv variable_name`: Prints the value of the specified environment variable.
`echo $"variable_name`: Prints the value of the specified environment variable.
`export LAST_NAME=hussain`: Creates a new environment variable called LAST_NAME with a value of hussain.
`ls -a`: Lists all files in the current directory, including hidden files.
`sudo nano .bashrc`: Opens the .bashrc file for editing with elevated privileges using the nano editor.
`source .bashrc`: refreshes the .bashrc file, which applies any changes made to it.




