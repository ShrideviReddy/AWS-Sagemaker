# AWS Sagemaker and Scitkit-learn
This repository contains code for linear regression using scikit-learn in AWS Sagemaker. 
<p align="center">
  <img width="400" height="200" src="images/sagemakerlogo.PNG">
</p>
Amazon SageMaker is a cloud machine-learning platform that was launched in November 2017. SageMaker enables developers to create, train, and deploy machine-learning models in the cloud. SageMaker also enables developers to deploy ML models on embedded systems and edge-devices.
There are different ways to build and train model in AWS Sagemaker.Following are ways which you can use to build and train model:
- Built-in model
- Using framework supported by AWS sagemkaer. E.g. Tensorflow, Pytorch, Scikit-learn, etc.
- Using Docker images for framework not supported by AWS sagemkaer.


In this repository , I am using scikit-learn to predict insurance cost. You can use scikit learn using estimator in AWS sagemaker. 
You can find data [here](https://www.kaggle.com/mirichoi0218/insurance).

For sake of simplicity , I have already done pre-processing and stored train and test data on AWS S3. 

## To get started:
To create Notebook instance in AWS Sagemaker, follow steps given below:
- Open the SageMaker console
- Choose Notebook instances, then choose Create notebook instance.
- On the Create notebook instance page, provide the following information:
    - Notebook instance name : name for your instance
    - Notebook instance type: choose according to your need
    - Elastic Inference: choose if you want inference from notebook or else select none
    - (Optional) Additional configuration lets advanced users create a shell script that can run when you create or start the instance. This script, called a lifecycle       configuration script, can be used to set the environment for the notebook or to perform other functions
    - (Optional) Additional configuration also lets you specify the size, in GB, of the ML storage volume that is attached to the notebook instance.
    - For IAM role, choose either an existing IAM role in your account that has the necessary permissions to access SageMaker resources or choose Create a new role. 
    - For Root access, to enable root access for all notebook instance users, choose Enable.
    - (Optional) Encryption key lets you encrypt data on the ML storage volume attached to the notebook instance using an AWS Key Management Service (AWS KMS) key. If you plan to store sensitive information on the ML storage volume, consider encrypting the information.
    - (Optional) To associate Git repositories with the notebook instance, choose a default repository and up to three additional repositories. 
    - Choose Create notebook instance.
When status is In-service , select Open JupyterLab or Open Jupyter. 
After creating Notebook instance you proceed with your experiment. 
    
