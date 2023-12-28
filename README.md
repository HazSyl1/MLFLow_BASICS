# MLFLow_BASICS

## DagsHub:

MLFLOW_TRACKING_URI=https://dagshub.com/HazSyl1/MLFLow_BASICS.mlflow \
MLFLOW_TRACKING_USERNAME=HazSyl1 \
MLFLOW_TRACKING_PASSWORD=a7a47b400fa96a13114cdb46a08acb04513b3b29 \
python script.py

```bash

export MLFLOW_TRACKING_URI=https://dagshub.com/HazSyl1/MLFLow_BASICS.mlflow

export MLFLOW_TRACKING_USERNAME=HazSyl1

export MLFLOW_TRACKING_PASSWORD=a7a47b400fa96a13114cdb46a08acb04513b3b29
```

# AWS

1.Login 
2.Create IAM user with AdmiinistratorAccess
3.Export the credetials in your AWS CLI by running "aws configure"
4.Create a s3 bucket
5.Create EC2 machine (Ubuntu) & add Security froups 5000 port

## Run the follpwing coman on EC2 machine 
```bash
sudo apt update
sudo apt install python3-pip
sudo pip3 install virtualenv
mkfir mlflow
cd mlflow
pipenv install mlflow
pipenv install awscli
pipenv install boto3
pipenv shell


## aws credentials
aws configure 

mlflow server -h 0.0.0.0 --default-artifact-root s3://mlflow-buc23

export MLFLO_TRACKING_URI=http://ec2-54-227-102-144.compute-1.amazonaws.com:5000/

```