# Module 3 : Assignment 3.6

## Create a serverless node application and push to AWS API Gateway, AWS cloudFormation, AWS Lambda and AWS DynamoDB

- This assignment working on windows WSL envionment
- Create a account at https://www.serverless.com/
- Create a new github repository and clone it at local computer (WSL)
- Add in the AWS-node-http-api-project folder inside the git repository. 
- Locate into the AWS-node-http-api-project folder
- Open and edit ```serverless.yml```
    - add org and app on top of yml file
    - change the ```service``` name (include your name)
    - comment this line ```profile: serverless```
    - Change the ```TableName``` (include your name)
- check serverless app install locally
    - ```serverless --version```
- If not exist then need to installed
    - ```npm install serverless -g```
- Login to serverless type command below
    - ```serverless```
    - Choose ```Login/Register``` and click on the link to login serverless.com
- Run below command to install plugins
    - ```npm install serverless-offline --save-dev```
- Run below command to install node package
    -```npm init```

- Run below command to start serverless deployment
    -```serverless deploy```
    - Once deploy success, you can see the endpoint url. Click will invoke the api call. use curl <endpoint url> to view the api response.
    - You can access AWS to check entry created on API Gateway, Lambda, DynamoDB, CloudFormation
    - You can access [serverless.com](https://www.serverless.com/) to view the application metrics

- View serverless cli command help 
    - ```serverless --help```

- To run the serverless on local computer
    - ```serverless offline```

- To remove all the serverless setup on AWS services.
    - ```serverless remove``

