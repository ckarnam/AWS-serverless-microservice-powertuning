# AWS-serverless-microservice-powertuning
A serverless backend powered by AWS Lambda, API Gateway, and DynamoDB — scalable and low-maintenance. This project also measures the performance and cost trade-offs of different memory configurations, validates real traffic behavior, and applies the optimal configuration. 

# Architecture
<img width="2813" height="1210" alt="Architecture-diagram" src="https://github.com/user-attachments/assets/55b35c7d-77f5-4f7d-b5d6-a54a6087e6a0" />



# AWS Components 

1 - Create custom IAM policy and role - To enable access to DynamoDB and Cloudwatch.
<img width="2519" height="1264" alt="create-policy" src="https://github.com/user-attachments/assets/00c9b7a1-ab52-4252-8fe8-ff27e50d5bdc" />

2 - Lambda - Business logic resides here. CRUD logic for accessing database
<img width="1801" height="1162" alt="lambda-basic-info" src="https://github.com/user-attachments/assets/38c14b18-a80e-4496-81da-4a2f05048443" />

3 - APIGateway - Create a REST API - POST method.
<img width="2298" height="1018" alt="create-new-api" src="https://github.com/user-attachments/assets/db77794e-3858-4988-b442-90c8774c3442" />


4 - DynamoDB - NoSQL database for storage.
<img width="2269" height="887" alt="create-dynamo-table" src="https://github.com/user-attachments/assets/0eb7047e-3e70-4117-ba90-ff2937380579" />


5 - POSTMAN - To test API calls and Load testing simulation.
