# AWS-serverless-microservice-powertuning
A serverless backend powered by AWS Lambda, API Gateway, and DynamoDB — scalable and low-maintenance. This project also measures the performance and cost trade-offs of different memory configurations, validates real traffic behavior, and applies the optimal configuration. 

# Architecture
<img width="2813" height="1210" alt="Architecture-diagram" src="https://github.com/user-attachments/assets/55b35c7d-77f5-4f7d-b5d6-a54a6087e6a0" />



# AWS Components 

1 - Create custom IAM policy and role - To enable access to DynamoDB and Cloudwatch.

2 - Lambda - Create the function CRUD logic resides here.

3 - APIG - Create a REST API - POST method (due to payload to enter items or list DDB items).

4 - DynamoDB - Create table.

5 - POSTMAN - to test API calls and Load testing simulation.
