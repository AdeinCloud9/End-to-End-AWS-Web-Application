# End-to-End-AWS-Web-Application

## Objective

This project is a simple web application built from scratch using various AWS services. The application performs basic math calculations and stores the results in a DynamoDB table.


### Skills Learned

- AWS Amplify: Deploying and hosting web applications using AWS Amplify.
- HTML and JavaScript: Creating and scripting interactive web pages.
- AWS Lambda: Writing and deploying serverless functions using Python.
- API Gateway: Creating and managing REST APIs to integrate with backend services.
- DynamoDB: Designing and interacting with NoSQL databases in AWS.
- IAM (Identity and Access Management): Managing roles and policies for secure access control.
- Serverless Architecture: Building applications with a serverless approach for scalability and efficiency.
- AWS CLI: Using the AWS Command Line Interface for managing AWS services.

## Services Used
- AWS Amplify for hosting the web application
- AWS Lambda for executing backend logic
- AWS IAM for managing permissions
- Amazon API Gateway for creating a REST API
- Amazon DynamoDB for database storage


## Steps

*Ref 1: Web Application Architecture*
![diagram-export-5-28-2024-7_51_47-PM](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/0ab24d92-cebc-4e3f-a6b0-c65240ea6aed)


### 1. Web Page Creation
*Ref 2: Created an index.html file* 
![Screenshot 2024-05-28 202410](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/0fc1d4d3-d366-4129-beed-02ab2a522fc0)


### 2. Deploying with AWS Amplify
*Ref 3: Initialize Amplify Project*
![Screenshot 2024-05-28 202706](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/0fd0b1a2-d55e-45c6-a1cf-86c95407336f)

*Ref 4: Deployed the Web Page*
![Screenshot 2024-05-28 203240](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/5161ac88-383a-4e27-b1e0-e93830d9ea36)

### 3. Lambda Function for Math Calculations
*Ref 5: Created lambda function*
![Screenshot 2024-05-28 205714](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/6f94f30a-27dc-4dd8-bbd8-9f0821a24c8e)


### 4. Created REST API with API Gateway
*Ref 6: Created a new REST API*
Setup Resource and Method
Added a POST method to the resource.
In the method settings, I set the integration type to Lambda Function.
Selected the PowerOfMathFunction, Lambda function I created.
![Screenshot 2024-05-28 204540](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/0c0ac4e4-7b2b-4aa0-bfbd-4d8920252eda)


### 5. Persisting Data with DynamoDB
*Ref 7: Added DynamoDB Permissions to Lambda and Updated the Lambda function to write the result to DynamoDB*

![Screenshot 2024-05-28 204907](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/f9c431fa-2249-48df-85ba-e36ab963f96b)

![Screenshot 2024-05-28 205942](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/0de7eadc-9ba9-4088-ae42-d3b659c5ac6d)

![image](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/66d28122-09c0-4850-bba8-1f6127d8b689)


![Screenshot 2024-05-28 210152](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/060a921e-2d67-42c3-895e-6403442766be)

*Ref 8: Attached the AmazonDynamoDBFullAccess policy to the role used by my Lambda function in the IAM service of the AWS console*

![Screenshot 2024-05-28 210855](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/f8679bd3-80f4-41d2-9f9f-6a30f9e1bebf)


### 6. Invok API from Web Page
Updated index.html with the API Gateway endpoint URL. 

### 7. Re-deployed the updated index.html using Amplify
*Ref 9: Updated index.html*
![Screenshot 2024-05-28 211833](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/bfddc2fa-5efc-4017-82d8-dc20a7154ab8)
![Screenshot 2024-05-28 212018](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/561dffea-26b3-4432-83a6-2cadbf4312d2)

### 8. MathMinds Test
![Screenshot 2024-05-28 212126](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/eb969440-f7b2-411a-870a-9341630a14ee)
![Screenshot 2024-05-28 212147](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/6153f80f-575d-4cf1-83ca-f2b7bfa8573d)
![Screenshot 2024-05-28 212206](https://github.com/AdeinCloud9/End-to-End-AWS-Web-Application/assets/170884766/2e555490-8a2e-4081-acf4-70ba652f058c)
