This code contains terraform scripts, to create an iam role, an iam policy, spin up a new ec2 instance and attach it to that instance. Security group will be attache to ec2-instance. Terraform also will apply Auto Scaling group for zero downtime.  

Terraform contains an User data script that will install and start httpd server that says "Hello World from Terraform". 

How to use this code:

1. Clone this repo
2. USE IAM ROLE with permissions to avoid "access and secret key"
3. Run terraform init
4. Run terraform plan
5. Run terraform apply
6. Wait approximately 10 min for the terraform script to create your resources
7. From web browser check your IP or DNS to see the output from user data
