# Module 3 : Assignment 3.6

## Create a serverless node application and deploy to AWS Services (API Gateway, AWS cloudFormation, AWS Lambda and AWS DynamoDB)

### Tools Required and the steps for Serverless Setup
This assignment will be done in a Windows WSL environment.
1. Create a Serverless Account:
    - Sign up at **[Serverless.com](https://www.serverless.com)**.

2. Set Up a GitHub Repository:
    - Create a new GitHub repository.
    - Clone it to your local computer (WSL).

3. Create and Deploy a Serverless App on AWS:
    - Add the **AWS-node-http-api-project** folder to the cloned Git repository.
    - Navigate into the **AWS-node-http-api-project** folder.
    - Open and edit the **serverless.yml** file:
       - Add your organization (**org**) and **app** name at the top.
       - Change the **service** name (include your name in the service name).
       - Comment out the line: **profile: serverless**.
       - Change the **TableName** to include your name.

4. Check and Install Serverless Locally:
    - Verify installation:
      ```
          serverless --version
      ```
    - If not installed, run:
      ```
          npm install serverless -g
      ```
    - Log in to Serverless by running:
      ```
          serverless
      ```
      Choose **"Login/Register"** and follow the link to log in to serverless.com.

5. Install **Plugins** and **Node Packages**:
    - Install the serverless-offline plugin:
      ```
          npm install serverless-offline --save-dev
      ```
    - Initialize a Node package:
      ```
          npm init
      ```
6. Deploy the Serverless App:
    - Deploy the app to AWS with:
      ```
          serverless deploy
      ```
      After deployment, check the endpoint URL and use curl to test the API response.

7. Verify AWS Resources:
    - Check AWS Console for the created resources (API Gateway, Lambda, DynamoDB, CloudFormation).
    - View application metrics on **[Serverless.com](https://www.serverless.com)**.

8. View Serverless CLI Help:
    - For a list of commands, use:
      ```
          serverless --help
      ```
9. Run Locally:
    - To run the Serverless app locally, use:
      ```
          serverless offline
      ```
10. Remove AWS Resources:
    - To remove the serverless setup from AWS, run:
      ```
          serverless remove
      ```
