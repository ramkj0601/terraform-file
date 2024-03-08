terraform to create a ec2 instance using aws
Create a file filename.tf
#inside a file
  need to provide a provider
     provider "aws" {
     region = "provide the region name"
     }
  need to provide the resource
     resource "aws_instance" "any name" {
     ami = "ami code of amazone linux or any OS"
    instance type ="required type"
    tags = {
    "Name" = "Name of an instance to be created"
   }
 }
Save a file using a command
esc :wq!
# To initiate a terraform use 
command :- terraform init

# To keep in the correct formate of the code return
command :- terraform fmt

# To validate the file
command :- terraform validate

# To preview the changes 
command:- terraform plan

# To execute the changes
command:- terraform apply
  

  
  
