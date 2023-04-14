# How to launch an Instance

![Screenshot_1](https://user-images.githubusercontent.com/129314018/231811265-a7a0d2b8-1867-4ae8-87b6-09727dfe7cce.jpg)

* On AWS dashboard, click search and search "EC2"

![Screenshot_2](https://user-images.githubusercontent.com/129314018/231811274-d60ac50e-6dc4-432f-ab21-f782550d8612.jpg)

* Once on EC2 dashboard, click on launch instance as shown and click launch instance from the drop down.

![image](https://user-images.githubusercontent.com/129314018/231811419-6b4d7144-9b3a-429e-aac6-bd92d9e401f9.png)

* On Name, type your chosen name of the instance. Once down click on browse more AMIs to where we will scroll to find our Ubuntu VM.

![image](https://user-images.githubusercontent.com/129314018/231811598-6aa99fa0-5f8b-49ba-9da3-4b9889eb2bd2.png)

* Once finished scrolling down, click on Ubuntu Server 20.04 as shown above, and keep everything on default and press **Select**

![image](https://user-images.githubusercontent.com/129314018/231811830-9365c3e8-bbfa-42be-8ff0-7bfefdde3342.png)

* On the Key Pair Login, search on Key pair name and in our case we typed **tech221** which gave us our RSA key

![image](https://user-images.githubusercontent.com/129314018/231828793-417f9319-f387-4be5-8703-308c8bc3f930.png)

* Scrolling down to the security group, change the security group name if needed, make sure allow SSH traffic is from **MY IP** so others apart from the owner cannot access it. 
* Also check allow HTTP traffic from the internet

![image](https://user-images.githubusercontent.com/129314018/231814271-86fa9ac5-2ca8-4058-b4bb-435964f33390.png)

* After launching your instance, click on the hyperlinked **Instance ID**, then you will be sent to the page above, check the instance then click connect as marked with the red boxes.

![image](https://user-images.githubusercontent.com/129314018/231814448-e8bafd93-22bf-4e8e-8835-8f63246044fe.png)

* We will be greeted by this screen above, copy and store these command lines.

![image](https://user-images.githubusercontent.com/129314018/231815076-161c9994-b7c9-4bee-840e-a4763909f6da.png)

* After opening GitBash, navigate to your `.ssh` using `cd .ssh`. After that we use our stored commands from the previous step, `chmod 400 tech221.pem` is inputted and entered, then you input the `ssh -i ...` command.

* Then you are prompted if you want to continue, we type `yes`.

![image](https://user-images.githubusercontent.com/129314018/231815244-2c255a50-f611-4f75-9031-39eb4f556bdb.png)


* From this we can see we are now connected to our Ubuntu VM.

# Install Nginx

![image](https://user-images.githubusercontent.com/129314018/231816432-d4c7e2c7-b439-4c32-8f3c-1556c82e9acf.png)


* To install Nginx, we carry on from the previous step, and we use `sudo apt install nginx` to install nginx. We see the outcome in the above picture. We are then prompted if we want to continue, we press `Y`.

![image](https://user-images.githubusercontent.com/129314018/231816774-fa463227-5da3-46d2-8c09-650686367d25.png)

* To check if our nginx has installed properly we use `sudo systemctl status nginx` this will show if the service, being nginx, is in fact running. We can see confirmation of this in the screenshot above.

![image](https://user-images.githubusercontent.com/129314018/231818172-74f4af87-02fc-414f-8d4d-35f7ea3b7bc8.png)

* We go back to our instance details on AWS, and after copying the Public `IPv4 address`, we will paste this into our search bar.

![image](https://user-images.githubusercontent.com/129314018/231818823-0c0c5217-5ac3-46d2-9205-692d8734630c.png)

* After pasting it into our search bar, we can see it Welcomes us to Nginx, signifying that it is in fact installed properly
