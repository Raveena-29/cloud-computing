
# AWS PRACTICALS

# AWS PRACTICALS

## 1. Launch Your First Amazon EC2 Instance

**Objective:** Deploy a virtual machine on AWS using Amazon EC2.

**Steps:** 

a) Launch an EC2 instance from the AWS Management Console.  
b) Use a pre-configured AMI (e.g., Amazon Linux 2).  
c) Configure security groups to allow SSH access.  
d) Connect to the instance using SSH.

**1. go to EC2 -> Launch Instance**

<img width="1470" height="807" alt="image" src="https://github.com/user-attachments/assets/8a302564-98c6-4579-bc60-27901987ec81" />
<img width="1470" height="795" alt="image" src="https://github.com/user-attachments/assets/6b2ddf6f-5005-49e5-8081-e36184986c44" />
<img width="1470" height="798" alt="image" src="https://github.com/user-attachments/assets/86340658-549d-483d-8117-ebfe3dc9a307" />

**2. EC2 instance is successfully created. -> Click on Connect**

<img width="1470" height="799" alt="image" src="https://github.com/user-attachments/assets/6d38413d-f8e9-46f4-bf89-871a48d59fbe" />
<img width="1470" height="796" alt="image" src="https://github.com/user-attachments/assets/0d14c7a6-6e75-4864-b6b9-a489e3227e91" />
<img width="1470" height="797" alt="image" src="https://github.com/user-attachments/assets/cd0354a8-62b9-4c6e-8777-2c3f718d93f5" />
<img width="1470" height="794" alt="image" src="https://github.com/user-attachments/assets/f09853c8-6051-45ab-8400-f5c14dcba37d" />


## 2. Set Up a VPC

**Objective:** Build and configure a Virtual Private Cloud (VPC).

**Steps:**

a) Create a custom VPC with both a public and a private subnet.  
b) Launch one EC2 instance in the public subnet and another in the private subnet.  
c) Set up an Internet Gateway to enable internet access for the public subnet.  
d) Configure a NAT Gateway to allow instances in the private subnet to access the internet.

**1. Go to Dashboard -> VPC -> Create VPC**

<img width="1470" height="802" alt="image" src="https://github.com/user-attachments/assets/757f0e8e-66e1-4546-9fb3-cef166a91e84" />
<img width="1470" height="791" alt="image" src="https://github.com/user-attachments/assets/ae7a73c2-dd56-4655-8070-5468983a2a6f" />
<img width="1470" height="790" alt="image" src="https://github.com/user-attachments/assets/89648593-9b87-406a-a9dd-1288fa3bf8dc" />
<img width="1464" height="772" alt="image" src="https://github.com/user-attachments/assets/af184a6a-31be-433f-81f4-413975f4e8a1" />

**Create two subnets: public and private**

<img width="1470" height="796" alt="image" src="https://github.com/user-attachments/assets/b33c3306-b917-4bcd-9e1f-d7f7b41dcd58" />
<img width="1470" height="800" alt="image" src="https://github.com/user-attachments/assets/3d98f3cd-3ce7-4436-a2c4-262faebde535" />
<img width="1470" height="794" alt="image" src="https://github.com/user-attachments/assets/06d9a5c3-9a41-44ff-8f86-ae9761546eac" />

**Create a Internet Gateway And attach it to VPC**

<img width="1470" height="800" alt="image" src="https://github.com/user-attachments/assets/f43ba972-d54d-4df6-86b9-11ba7766c870" />
<img width="1470" height="803" alt="image" src="https://github.com/user-attachments/assets/652c2ce5-16ad-4a31-9885-1cc578a2b795" />
<img width="1470" height="800" alt="image" src="https://github.com/user-attachments/assets/ddbd556c-9b03-4666-8541-e12f42f71198" />

**Configure Route Table: Create Route table -> Click on Edit routes -> Destination: anywhere and target will be the internet gateway that we just created -> Go to the subnet associations -> Edit the explicit subnet associations -> Select the public subnet and save it**

<img width="1470" height="799" alt="image" src="https://github.com/user-attachments/assets/25ac6cd3-d43a-46a5-9613-acf0b7918e1a" />
<img width="1470" height="803" alt="image" src="https://github.com/user-attachments/assets/2ead7c4d-f04b-4315-93cd-816ef0c71614" />
<img width="1470" height="800" alt="image" src="https://github.com/user-attachments/assets/ac0ce9fd-b880-47a9-93da-f94115654d2a" />
<img width="1470" height="801" alt="image" src="https://github.com/user-attachments/assets/7b5a6fdb-8693-4cc8-a9a5-e41492feb1a0" />
<img width="1470" height="803" alt="image" src="https://github.com/user-attachments/assets/75ff3fc0-096c-40df-ac57-8952de2f987a" />
<img width="1470" height="784" alt="image" src="https://github.com/user-attachments/assets/9f5d9db5-8773-4d9c-b741-d0d2252fcd6e" />

**Now go to EC2 -> launch instance and create a public-instance: In network settings set: VPC-> yourVPC, subnet-> public subnet, auto assign IP address -> enable**  
<img width="1469" height="802" alt="image" src="https://github.com/user-attachments/assets/8d133f92-7cbb-4bfb-8180-ca038782a814" />
<img width="1465" height="784" alt="image" src="https://github.com/user-attachments/assets/8068e356-ff8f-487c-bd9d-137a780090af" />
<img width="1470" height="789" alt="image" src="https://github.com/user-attachments/assets/72e9b806-ba40-4c01-8e1f-c3743607a6f1" />

**Similarly Create a private instance: In network settings set: VPC-> yourVPC, subnet-> private subnet**  
<img width="1470" height="800" alt="image" src="https://github.com/user-attachments/assets/546a0d67-0a15-4cae-83c0-a185ed6ac10f" />
<img width="1470" height="789" alt="image" src="https://github.com/user-attachments/assets/a54e49db-f178-4290-8ef7-8c3f3c3fb3d9" />
<img width="1465" height="790" alt="image" src="https://github.com/user-attachments/assets/28fdc807-6585-4855-835b-7d28ced4cdc6" />
<img width="1470" height="798" alt="image" src="https://github.com/user-attachments/assets/886367cf-387e-4c62-877d-aa73f2e269d5" />

**Now connect both instances: Private will fail but Public runs successfully**
<img width="1470" height="795" alt="image" src="https://github.com/user-attachments/assets/d883ce97-d211-412f-9dc9-5b8a116a2fa8" />
<img width="1470" height="797" alt="image" src="https://github.com/user-attachments/assets/ad36abe9-0f36-45d3-9484-709290025322" />
<img width="1470" height="796" alt="image" src="https://github.com/user-attachments/assets/1f22d527-517f-4625-a334-0efeca0f1694" />
<img width="1470" height="808" alt="image" src="https://github.com/user-attachments/assets/94257554-886a-4f1f-8fb1-a0b5613d3bf2" />

## 3. Configure Auto Scaling and Load Balancing  
**Objective: Set up an auto-scaling group and load balancer.**  

**Steps:**  
a) Create an Auto Scaling Group and define a launch template.  
b) Configure scaling policies (e.g., scale up when CPU utilization exceeds 70%).  
c) Deploy an Application Load Balancer (ALB) to distribute traffic.  
d) Test auto-scaling by simulating high traffic.  

**EC2 -> Create Launch template**
<img width="1470" height="808" alt="image" src="https://github.com/user-attachments/assets/db1c7a1e-9afe-4528-99c7-57efc26b4a8b" />
<img width="1470" height="805" alt="image" src="https://github.com/user-attachments/assets/7a9aad91-a59e-4099-82ae-8618db161254" />
<img width="1467" height="801" alt="image" src="https://github.com/user-attachments/assets/808eadce-5e34-41f5-89fa-529955baa7c1" />
<img width="1470" height="803" alt="image" src="https://github.com/user-attachments/assets/ff62d283-76a2-4dfe-ad73-6e1766105402" />
<img width="1470" height="804" alt="image" src="https://github.com/user-attachments/assets/fbfdfc8e-b7ea-42ff-9504-59e204df45e5" />

**Create a public subnet 2 and attach it to the public route table**
<img width="1470" height="800" alt="image" src="https://github.com/user-attachments/assets/909a271d-c45d-4a3f-b139-7c0402fafc16" />

<img width="1470" height="799" alt="image" src="https://github.com/user-attachments/assets/3aabeae9-818a-4d33-a9ec-bedc31a68861" />


**Create an Auto scaling group**

<img width="1470" height="794" alt="image" src="https://github.com/user-attachments/assets/80cfa46e-3319-45ba-90cc-b7d8863b5bb6" />
<img width="1470" height="796" alt="image" src="https://github.com/user-attachments/assets/60b8bda9-9d53-42da-85c9-b9c513b94773" />

<img width="1470" height="801" alt="image" src="https://github.com/user-attachments/assets/0b997255-56af-420f-830a-24398f8f78dd" />

<img width="1470" height="788" alt="image" src="https://github.com/user-attachments/assets/4f4ad827-ed78-452a-8709-3930e9a9b2af" />

<img width="1470" height="792" alt="image" src="https://github.com/user-attachments/assets/62aa0932-c7a9-4e08-ae67-e9ee223dd43b" />

<img width="1470" height="779" alt="image" src="https://github.com/user-attachments/assets/a1bbb0c3-86b6-48dd-89e6-c80b1ec558e5" />

<img width="1470" height="795" alt="image" src="https://github.com/user-attachments/assets/40dc672e-229d-4ea7-9154-906722198cdc" />

<img width="1470" height="808" alt="image" src="https://github.com/user-attachments/assets/c92a952d-979c-4afd-8ae4-dd4d6587d588" />


<img width="1470" height="799" alt="image" src="https://github.com/user-attachments/assets/34471f40-fd6f-45ab-94db-576886fa55a7" />

**Now go to load balancer and copy the DNS and browser it in a browser**

<img width="1470" height="791" alt="image" src="https://github.com/user-attachments/assets/6874b31b-6553-45d9-b036-640cbc56ce85" />

## 4. Deploying a Static Website on the Cloud  
**Objective: Host a static website using cloud storage services.**  

**Steps:**  
a) Deploy a static website using any of the following:  
- AWS S3
- Azure Blob Storage
- GCP Cloud Storage  
b) Configure permissions and enable public access.


<img width="1470" height="808" alt="image" src="https://github.com/user-attachments/assets/f29078a6-6fa0-4baa-885f-619056534b72" />


<img width="1470" height="808" alt="image" src="https://github.com/user-attachments/assets/7e2016b7-2636-4932-a0c9-57de782d026e" />

<img width="1470" height="800" alt="image" src="https://github.com/user-attachments/assets/e0e6ada8-f9ab-4535-891a-bbe133c6f282" />

Uploading files

<img width="1470" height="801" alt="image" src="https://github.com/user-attachments/assets/f1871453-7ed2-4f19-93b5-25f708b58bd3" />

<img width="1470" height="805" alt="image" src="https://github.com/user-attachments/assets/832b5176-0af0-4019-9b01-c63ec9513633" />


<img width="1470" height="794" alt="image" src="https://github.com/user-attachments/assets/0ba78e30-a68e-449c-b44a-d8810e19b61f" />

**Then go to permissions -> static website hosting**

<img width="1470" height="797" alt="image" src="https://github.com/user-attachments/assets/1dd11023-5660-4d51-afd0-d62fc56b0064" />


<img width="1470" height="882" alt="image" src="https://github.com/user-attachments/assets/f7a346ed-16b7-4838-a24d-9e7c15e350ff" />


## Monitor Resources Using AWS CloudWatch  
**Objective: Use CloudWatch to monitor AWS resources.**  
**Steps:**  
a) Set up CloudWatch metrics for an EC2 instance (e.g., CPU utilization).  
b) Create a CloudWatch Alarm to send notifications when a threshold is exceeded.  
c) Configure an SNS topic for email notifications.  
d) Test the setup by simulating high CPU usage.  

**Create a EC2**

<img width="1470" height="787" alt="image" src="https://github.com/user-attachments/assets/9dda35c6-401c-4b0f-b8cc-fec444a74f9b" />

**Go to Cloudwatch -> metrices -> EC2**

<img width="1470" height="802" alt="image" src="https://github.com/user-attachments/assets/caf3492b-ee82-4e13-a791-8044dadbecbc" />

<img width="1470" height="789" alt="image" src="https://github.com/user-attachments/assets/2dab6b81-cc8c-4c7d-be27-8bfe068d9bff" />


<img width="1470" height="797" alt="image" src="https://github.com/user-attachments/assets/84214e67-fc6d-49a0-91dd-2eb463fc659f" />

<img width="1470" height="799" alt="image" src="https://github.com/user-attachments/assets/90d59b9a-3d7c-4891-9554-1908e7b6ddfd" />

<img width="1470" height="802" alt="image" src="https://github.com/user-attachments/assets/00be5e48-9032-4ff7-8669-73d3f567cf75" />

<img width="1470" height="810" alt="image" src="https://github.com/user-attachments/assets/75b1d3c2-c286-4b82-b611-e1b04685a7ec" />

<img width="1470" height="793" alt="image" src="https://github.com/user-attachments/assets/08d635bc-3c8a-43d0-9b20-f354b9b6ede3" />

<img width="1470" height="805" alt="image" src="https://github.com/user-attachments/assets/cfd239e7-05b8-4b8a-957a-3899a9534335" />

<img width="1470" height="803" alt="image" src="https://github.com/user-attachments/assets/f6af604b-3a4f-44e8-88a9-d4b128171ac9" />

<img width="1470" height="816" alt="image" src="https://github.com/user-attachments/assets/fde6ed4c-1dc4-48d0-a450-22fdb906a153" />

<img width="1470" height="807" alt="image" src="https://github.com/user-attachments/assets/adf4d18b-5990-48b5-9275-d9d2948319d4" />


<img width="1470" height="800" alt="image" src="https://github.com/user-attachments/assets/e5ed9ce5-fdc6-48e7-889a-06423d877e16" />

<img width="1470" height="807" alt="image" src="https://github.com/user-attachments/assets/70faa0d0-3d1b-4d8c-b9bb-f0eecd4e517f" />

















