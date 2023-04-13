# Security Groups


![image](https://user-images.githubusercontent.com/129314018/231758026-a2ecdc27-c44a-48e3-9b0d-e07b79e92f7b.png)

From the Dashboard, click instances to access your instance.

![image](https://user-images.githubusercontent.com/129314018/231758382-413836cc-8eea-4f83-988e-62d58309633b.png)

Using Key terms or any other method, find your instance and click on the instance id which is **hyperlinked**

![image](https://user-images.githubusercontent.com/129314018/231758482-c6599940-1068-4f3b-9e73-ccb4b04e07b3.png)

After clicking on the instance id, you are on the next page, scroll down and click the **security** tab next to details

![image](https://user-images.githubusercontent.com/129314018/231758647-827495b5-e92b-40ff-94ef-0045ecbb1aa3.png)

Looking at the picture above, on security groups click the `sg-.....` hyperlink.

![image](https://user-images.githubusercontent.com/129314018/231762274-1fbb7ca3-0011-4db8-8770-40b75042178f.png)

Scroll down and click edit inbound rules to change the rules.

![image](https://user-images.githubusercontent.com/129314018/231758812-ca866a17-964b-4621-8cc7-8e748405cb61.png)

On this page, scroll down until you see the **Add Rule** button, once clicking a new inbound rule will show, change type to `ssh` and source type to `My Ip` then click save rules.

![image](https://user-images.githubusercontent.com/129314018/231759237-d249692c-f6f2-4dec-855f-15952e72e493.png)

After saving the rules, go back to your instance and click connect as seen above.

![image](https://user-images.githubusercontent.com/129314018/231759336-f51734bc-f855-4282-ae06-8575d5abb387.png)

Once clicking connect it will take you to a new page to connect to the instance. Keep a hold of the 2 commands boxed in red as shown above.

![image](https://user-images.githubusercontent.com/129314018/231759808-89e8bc20-4994-452c-9027-10d1800c374b.png)

When in Git Bash (making sure you run as administrator), run the first command `chmod 400 tech221.pem`. Then copy and paste the example command which is `ssh -i "tech221.pem" ubuntu@ec2-34-243-238-173.eu-west-1.compute.amazonaws.com`.

![image](https://user-images.githubusercontent.com/129314018/231763568-aef7f4cf-601f-4b66-8b80-10f20de0432a.png)

Once clicking `Enter` on the last command, you should be left connected to the Ubuntu System.

