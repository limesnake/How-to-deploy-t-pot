# How-to-deploy-t-pot
Hi guys, I made a step by step tutorial on how to deploy your first honeypot using T-pot and amazon AWS webservices virtual machine, please read the tutorial.md file for more information

WARNING: If you configure firewall rules or make a misconfiguration you are at risk of exposing your home network so make sure you do everything carefully. if you dont have acces to aws you can use many alternatives.

STEP 1: Make a AWS account.
<img width="1367" height="714" alt="image" src="https://github.com/user-attachments/assets/04c1be1b-9f82-4b1e-ad90-4bc06f3dcb60" />


first go to https://aws.amazon.com/ec2/?trk=b4354db4-537b-404e-b4df-824e23486182&sc_channel=ps&trk=b4354db4-537b-404e-b4df-824e23486182&sc_channel=ps&ef_id=Cj0KCQiA6sjKBhCSARIsAJvYcpMJe7hDCKj-5SrYJluujarlEN3UYyUhHIlnYOy5jHfEp_tjh34ZHXcaAgA-EALw_wcB:G:s&s_kwcid=AL!4422!3!638364387973!e!!g!!amazon%20ec2&gad_campaignid=19090032168
You will need to pay 1 euro but it will be returned to you after 2-3 business days.

STEP 2: Create a virtual machine/instance.

Go into your EC2 dashboard once you made your account

<img width="1016" height="578" alt="image" src="https://github.com/user-attachments/assets/a6eef10b-6456-4515-b075-fbc66eed2932" />

Then on the dashboard on the left click on instances

<img width="1317" height="378" alt="image" src="https://github.com/user-attachments/assets/e654f74f-8c4e-4869-8643-3ef56eea47d8" />

Launch the instance

<img width="1369" height="96" alt="image" src="https://github.com/user-attachments/assets/103533f6-8067-4bb6-8dd0-a6253a1b101f" />

STEP 3: Configure VM settings

Name the vm anything you want , for the os image search debian 11 and then go into the aws marketplace and select the one shown in the picture below:

<img width="1453" height="605" alt="image" src="https://github.com/user-attachments/assets/a5ee15fc-d5a8-4755-b901-11bb330adfb6" />






