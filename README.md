### House_Price_Prediction

### Software And Tools Required

1. [Github Account](https://github.com)
3. [VSCodeIDE](https://code.visualstudio.com)
4. [GitCLI](https://git-scm.com/downloads)

## Create a new Environment 
```
conda create -p myenv python==3.7 -y

```

## Steps for the deployement on AWS using Docker: 

1. Docker build checked
2. GitHub workflow set up
3. Create Iam user in AWS
4. Create a ECR repository (985539791451.dkr.ecr.eu-north-1.amazonaws.com/housepriceprediction)

5. Go to EC2 instance and create a virtual server in cloud and integrate it with the ECR.
-> Select ubuntu-64
6. Connect to EC2 instance

## Docker Setup In EC2 commands to be Executed

#optinal(Setting up the Linux server)

sudo apt-get update -y

sudo apt-get upgrade

#required (Installing all the necessary packages required for docker in the Linux machine)

curl -fsSL https://get.docker.com -o get-docker.sh 

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

## Configure EC2 as self-hosted runner:
Setup github secrets:
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-north-1

AWS_ECR_LOGIN_URI = demo>> 566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = housepriceprediction


