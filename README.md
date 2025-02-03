# Scalable-Infrastructure-Deployment-Using-AWS-EC2-RDS
Creating a high avaliable Cloud environiment for an Database based application by using EC2 auto-scaling. 

Creating EC2 instances: 
Add MySQL/Aurora along with ssh and HTTP ports.
![image](https://github.com/user-attachments/assets/b92cb403-7aed-4493-914e-f69907139a9b)

Note: Install apache web server in the instance

![image](https://github.com/user-attachments/assets/d926f05a-1418-4b3d-8870-4c8dcfd35a95)


EC2 instance is created.

![image](https://github.com/user-attachments/assets/57a27298-2fa7-4359-9fc3-c18eb1e9483b)


Now connect to EC2 instances “Ubuntu”

![image](https://github.com/user-attachments/assets/14694d82-ca1a-46b8-89c2-23d6b245c3b7)


Installing PHP and MySQL on the instances.

Add the repository into ubuntu instance which enables us to install the required php version.

![image](https://github.com/user-attachments/assets/7df438a4-4885-481c-94cc-0551cfe2221c)

![image](https://github.com/user-attachments/assets/d54bc948-f801-4c33-b96b-1c07ff7ab9f0)

Create RDS (Releation DataBase service) with MYSQL DB engine.

![image](https://github.com/user-attachments/assets/4b5a3c17-8760-4411-b389-6e6376e08f01)


![image](https://github.com/user-attachments/assets/a5a42215-85db-4b3d-9914-c0819b75bafa)

Choose version of the engine and Free tier template is more suitable for the project.

![image](https://github.com/user-attachments/assets/dec2f3d5-a325-4823-8e2a-1ee6c0a2942a)

Give the user name and passwords as mentioned.

![image](https://github.com/user-attachments/assets/d3726c99-8c65-4217-8794-acd727e42fe9)

Update the php code with the RDS endpoint.

![image](https://github.com/user-attachments/assets/ae5a62a4-5752-47c6-83b1-aa67f4ce06b4)

Now login through the MySQL database.
Use an RDS endpoint which will be available under the dashboard of the created RDS instance, username and password of database.

![image](https://github.com/user-attachments/assets/367f702c-66e4-49e2-9445-95bc753d2783)

Verify the database available under the databases, go through database and verify the tables.

![image](https://github.com/user-attachments/assets/4b43bc9e-0e28-41da-a044-c1b09ff27fc6)

We can also add the data directly into MYSQL DataBase.

![image](https://github.com/user-attachments/assets/0c5d841a-0326-4b48-be42-84eecbbc1cf6)

Storing the login details through the webpage in DataBase.

![image](https://github.com/user-attachments/assets/2da0c556-f41d-4ab1-a9d7-6a953ad5902e)


![image](https://github.com/user-attachments/assets/1e6880e5-00c6-40e5-b724-409d1026094b)

Check the entered details through the website in the database.

![image](https://github.com/user-attachments/assets/49c1b896-7644-4f49-ad00-24653dcafa9f)

Creating an image for the instance.

![image](https://github.com/user-attachments/assets/c014246e-9555-4a2c-82a8-5c9f676fb416)

![image](https://github.com/user-attachments/assets/79c07035-50da-4e41-a77c-36fb33d01900)

Once the image is created, Launch the template and the created image

![image](https://github.com/user-attachments/assets/fd5adc96-2e08-4f5e-b26d-af97fba7da2e)

Add the security group and create a template.

![image](https://github.com/user-attachments/assets/8b78b95f-52ee-414c-a7cf-d5c2d2dd601a)

Attach the template to the Auto Scaling group.
Give a name to the auto-scaling group and the template we created.

![image](https://github.com/user-attachments/assets/9b25afae-4274-44ba-b370-5dd7c31404d0)

Select the Availability zones and proceed further.

![image](https://github.com/user-attachments/assets/836d3e7e-1420-494a-baf0-1d992ee474b5)

Add an application Load Balancer

![image](https://github.com/user-attachments/assets/f9fdcca5-a3f2-4552-9de7-6311363de00d)

Set a no.of instance you want to create 

![image](https://github.com/user-attachments/assets/e85f00bf-11cd-43f2-8935-9d48385692db)

 Auto Scaling group is created.

![image](https://github.com/user-attachments/assets/93c6f690-8314-4435-b956-c160ac60b381)




