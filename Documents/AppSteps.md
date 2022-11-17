# App proccess Steps

## 1) Database
testing the database connection at aws RDS
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/TestDataBase1.png)

----

## 2) Host front End on s3 Bucket
After S3 Bucket creation and setting the Static website Enabled
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/staticHostingS3.png)

----

## 3) deploy Back End on ElasticBeanstalk
### Adding Environment variables to the ElasticBeanstalk after creation
Include all the needed variables to connect DB
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/elasticBeanConfigs.png)

### Checking the ElasticBeanstalk health after adding all variables
checking the EB health after adding the Environemts to connect DB
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/elasticBeanEnv.png)


###  BackEnd Runtime
URL of the BackEnd server on GET REQUEST (http://udagram-api-dev.eba-hrbq3mf4.us-east-1.elasticbeanstalk.com/)
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/ElasticBeanGET.png)

## 4) Connect FrontEnd With BackEnd
Connecting to the S3 website after connecting API with FrontEnd and DB
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/FrontEndWebPage.png)

## 6) Create the Github Repo
Add all files into repo after build and commit it to github 
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/GitHubRepo.png)

## 7) Connect to CircleCi
###  CircleCi Environment list
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/CircleCi_EnvVariables.png)

###  CircleCi Build
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/circleCi_Build.png)

###  CircleCi Deploy
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/deploySuccess.png)

### Last CircleCi Status
![img](https://github.com/KarimAyman97/Udagram-Deployment/blob/main/Images/buildHoldDeploy.png)
