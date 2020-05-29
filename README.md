# AWS_ServerlessWebApp
A serverless web app using AWS Lambda, API Gateway, S3, DynamoDB &amp; Cognito

Phase A - Create the S3 bucket, load content
Step 1: Host a static website (configure S3 to host static website resources; later, JavaScript will come into play to call remote RESTful APIs using AWS Lambda & API Gateway
Step 2: Upload the content
Step 3: Add a bucket policy to allow for public reads 
Step 4: Enable website hosting 
Step 5: Validate the implementation (visit the URL for the S3 bucket)

Phase B - Create user pool, authentication
Step 1: Create user pool with AWS Cognito
Step 2: Add an application to said user pool
Step 3: Update the config.js file in the website S3 bucket
Step 4: Test (visit the website, complete form) 

Phase C - Build serverless backend
Step 1: Create table with DynamoDB 
Step 2: Create IAM role for Lambda function (double check correct policies are in place) 
Step 3: Create Lambda function for request handling 
Step 4: Test the request 

Phase D - Deploy RESTful API 
Step 1: Create a new RESTful API 
Step 2: Create a cognito user pool authorizer 
Step 3: Create a new resource & method 
Step 4: Deploy the API 
Step 5: Update the website's configuration
Step 6: Vaidate implementation 

Phase E - Clean up 
Step 1: Delete S3 bucket or the stack in CloudFormation
Step 2: Delete Cognito user pool 
Step 3: Delete serverless backend (Lamdba, IAM, DynamoDB table) 
Step 4: Delete RESTful API 
Step 5: Delete CloudWatch Log 
