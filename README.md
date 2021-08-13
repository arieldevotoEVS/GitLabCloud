# GitLabCloud
Deployment of Cloudformation code that builds the whole environment for GitLab

## Steps to deploy the cloudformation script to AWS
1. Download AWS CLI
2. Create a new profile under ~/.aws/config and ~/.aws/credentials and give access details to connect to AWS
3. Make sure you have the name of the KeyPair that needs to be used to create the instance. this appears in the script as:
```KeyName: arieldevoto```
4. execute ``` aws cloudformation create-stack --stack-name gitlab --template-body file://stack.yaml``. this will create all resources within the script
``
