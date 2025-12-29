# How-to-deploy-t-pot
Hi guys, I made a step by step tutorial on how to deploy your first honeypot using T-pot and amazon AWS webservices virtual machine, please read the tutorial.md file for more information

WARNING: If you configure firewall rules or make a misconfiguration you are at risk of exposing your home network so make sure you do everything carefully. if you dont have acces to aws you can use many alternatives.

## STEP 1: Make a AWS account.
<img width="1367" height="714" alt="image" src="https://github.com/user-attachments/assets/04c1be1b-9f82-4b1e-ad90-4bc06f3dcb60" />


first go to https://aws.amazon.com/ec2/?trk=b4354db4-537b-404e-b4df-824e23486182&sc_channel=ps&trk=b4354db4-537b-404e-b4df-824e23486182&sc_channel=ps&ef_id=Cj0KCQiA6sjKBhCSARIsAJvYcpMJe7hDCKj-5SrYJluujarlEN3UYyUhHIlnYOy5jHfEp_tjh34ZHXcaAgA-EALw_wcB:G:s&s_kwcid=AL!4422!3!638364387973!e!!g!!amazon%20ec2&gad_campaignid=19090032168
You will need to pay 1 euro but it will be returned to you after 2-3 business days.

## STEP 2: Create a virtual machine/instance.

Go into your EC2 dashboard once you made your account

<img width="1016" height="578" alt="image" src="https://github.com/user-attachments/assets/a6eef10b-6456-4515-b075-fbc66eed2932" />

Then on the dashboard on the left click on instances

<img width="1317" height="378" alt="image" src="https://github.com/user-attachments/assets/e654f74f-8c4e-4869-8643-3ef56eea47d8" />

Launch the instance

<img width="1369" height="96" alt="image" src="https://github.com/user-attachments/assets/103533f6-8067-4bb6-8dd0-a6253a1b101f" />

## STEP 3: Configure VM settings

Name the vm anything you want , for the os image search debian 11 and then go into the aws marketplace and select the one shown in the picture below:

<img width="1453" height="605" alt="image" src="https://github.com/user-attachments/assets/a5ee15fc-d5a8-4755-b901-11bb330adfb6" />

For the instance type select t3.large

<img width="1073" height="179" alt="image" src="https://github.com/user-attachments/assets/ba814f8a-7abb-48e6-9351-f40b85a65ff1" />

KEY PAIR IMPORTANT!: Please give any name you want and download it into a safe place and dont lose it

SECURITY GROUPS!: Select create a security group option if already not selected and make sure only the "allow ssh trafic from" box is selected and the option "my ip" is also selected

Make sure the storage configuration is the same as the image below
<img width="1067" height="161" alt="image" src="https://github.com/user-attachments/assets/78c8c141-bd4a-4bf9-886b-d60db290f4c5" />

And finally launch the instance!

## STEP 4: Create firewall rules

Go back to The instances tab, then find your instance and click on the instance id. When your in, in the side bar find security groups
<img width="195" height="676" alt="image" src="https://github.com/user-attachments/assets/dc2b8deb-3d72-434c-b775-8018da49e6b2" />

Make sure you fidn the correct security group corresponding to your instance id, go to inbound rules , in the top left you should see edit inbound rules, click on it and add the rules in the image below.


Add these inbound rules:
<img width="1479" height="445" alt="image" src="https://github.com/user-attachments/assets/04f8b9bb-3516-4e3d-9a0e-12acd4bd2864" />

## STEP 5: EStablish SSH connection

In the rules we should SSH into the vm through port 6425 rather then the common ssh port 22.
You can either do this with the command  ''' ssh -i /(location e.g home/(your username on your device e.g admin)/(location of key e.g Downloads)/(keyname.pem) -l admin -p 64295 (your instance ip) '''
(REMOVE BRACKETS)

or with termius

simply get termius by downloading it from your web browser or if you are on linux search up how to install it via terminal

either way you should have successfully sshd into the vm terminal if you followed all previous steps correctly.

Now that you are in 









