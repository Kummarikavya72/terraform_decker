# terraform_decker
task 3 Terraform project to provision Docker container

This project demonstrates how to use **Terraform** to provision a local Docker container (Nginx) using Infrastructure as Code (IaC)on an EC2 Amazon Linux instance
Provision a Docker container using Terraform on an EC2 instance.

Tools Used
- Terraform
- Docker
- Amazon EC2
-  Steps Performed
EC2 Instance Setup

  installed:
  - Docker
  - Terraform (manually due to repo issues)
  - Git
![image](https://github.com/user-attachments/assets/8c1ccc65-7437-4931-9f9e-afea8ff8a90c)
 Docker Setup

 Terraform Installation (Manually)
Downloaded and installed 
wget https://releases.hashicorp.com/terraform/1.5.7/terraform_1.5.7_linux_amd64.zip
Created Terraform Config (main.tf)
Terraform Commands Used

terraform init :-Initialize the working directory
![image](https://github.com/user-attachments/assets/2bb96191-3a08-42a6-bb15-8f71d0e751eb)

terraform plan  View the execution plan
terraform apply  Apply changes (provision container)
terraform destroy Destroy the created infrastructure
![image](https://github.com/user-attachments/assets/50105d67-c94d-47f1-b00c-68fe7cd03449)

terraform state list # Check current state resources Logs (Zipped)
Includes:
![image](https://github.com/user-attachments/assets/03b01f95-2fd0-45e9-b5df-a9339ba41138)
init-log.txt
plan-log.txt
apply-log.txt
destroy-log.txt
Output
After terraform apply, access NGINX at:

http://<your-ec2-public-ip>:8080
![image](https://github.com/user-attachments/assets/b2407498-ff97-40ba-bcc4-21bbb213c6cf)
