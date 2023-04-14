# AMI

![ami_lifecycle](https://user-images.githubusercontent.com/129314018/232039655-cdb9c9c6-b128-4949-9e9a-07677755d4cf.png)

This diagram is explored through the steps below. In the AWS , instances can be created and launched using pre-configured virtual machine images known as AMIs. It includes the operating system, software programmes, and data, as well as all the other information required to begin an instance.


## Creating AMI from current instance
![Screenshot_3](https://user-images.githubusercontent.com/129314018/232033278-73c8e20a-1b57-4aca-bcea-241e2f5c75ad.jpg)

Navigate to **instances** and after checking your instance, hover over actions, on image and templates, and click **create image**

![Screenshot_4](https://user-images.githubusercontent.com/129314018/232033290-34a09a8e-31f8-4c75-b7e1-7a35d63308f8.jpg)

Change image name and image description as necessary. Then click create image to create it.

![image](https://user-images.githubusercontent.com/129314018/232037816-e10ddb81-8489-4346-b531-7eec0be99397.png)

If and when you need to rollback, you will navigate to the AMI tab.

Once created, check the AMI, and click **Launch from AMI**.

![image](https://user-images.githubusercontent.com/129314018/232035154-5ac3aa56-80c5-49b7-bb1a-6c92384c8eb2.png)

Make a name as necessary for your instance, and due to the AMI, we already have it pre-selected.

![image](https://user-images.githubusercontent.com/129314018/232035204-6892fdc2-af54-4671-ba0c-12e099bfb2d8.png)

Key Pair name - find the key pair name in our case it was **tech221**.

![image](https://user-images.githubusercontent.com/129314018/232035470-f3e33557-372b-4f75-857f-1a430bbd8c82.png)

Navigate back to instances, and the instance we just created we will check it and press connect.

![image](https://user-images.githubusercontent.com/129314018/232035589-9abe641e-9ca7-42f7-901c-bdd977f0508d.png)

Once clicking connect we copy and paste the `chmod ...` command and then we copy and paste the `ssh -i ...` command.

Looking below we also change the `ssh -i...` command by changing the `root` to `ubuntu`.

![Screenshot_6](https://user-images.githubusercontent.com/129314018/232033298-ead39c6f-b45b-4ef4-9d71-d14fc820ead9.jpg)

The reason we change it to `ubuntu`, is if we paste the code as suggested, we get this error message: 

```
Warning: Permanently added 'ec2-52-214-230-151.eu-west-1.compute.amazonaws.com' (ED25519) to the list of known hosts.
Please login as the user "ubuntu" rather than the user "root".
```

It actually prompts us to use `ubuntu`
