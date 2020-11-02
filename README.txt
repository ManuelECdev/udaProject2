This project converts the architecture in the file Udacity Project 2.pdf into Cloudformation scripts.

How to deploy the infrastructure:

1. Execute the below command

aws cloudformation create-stack --stack-name network --template-body file://network.yml  --parameters file://networkParameters.json --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM" --region=us-west-2


2. Execute the below command

aws cloudformation create-stack --stack-name server --template-body file://server.yml  --parameters file://serverParameters.json --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM" --region=us-west-2
