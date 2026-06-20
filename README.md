# AWS-serverless-microservice-powertuning
A serverless backend powered by AWS Lambda, API Gateway, and DynamoDB — scalable and low-maintenance. This project tunes Lambda memory allocation to strike the right balance between cost optimization and performance efficiency.

# Architecture
<img width="2813" height="1210" alt="Architecture-diagram" src="https://github.com/user-attachments/assets/55b35c7d-77f5-4f7d-b5d6-a54a6087e6a0" />



# AWS Components Setup 

1 - IAM - Create custom IAM policy and role in order to enable access to DynamoDB.

<img width="2519" height="1264" alt="create-policy" src="https://github.com/user-attachments/assets/00c9b7a1-ab52-4252-8fe8-ff27e50d5bdc" />

2 - Lambda - Business logic resides here.

<img width="1801" height="1162" alt="lambda-basic-info" src="https://github.com/user-attachments/assets/38c14b18-a80e-4496-81da-4a2f05048443" />

3 - DynamoDB - NoSQL database for storage.

<img width="2269" height="887" alt="create-dynamo-table" src="https://github.com/user-attachments/assets/0eb7047e-3e70-4117-ba90-ff2937380579" />

4 - APIGateway - Create and deploy a REST API. Integrate with lambda function created earlier.

<img width="2298" height="1018" alt="create-new-api" src="https://github.com/user-attachments/assets/db77794e-3858-4988-b442-90c8774c3442" />

5 - POSTMAN - Execute API we created in previous steps from local machine.

<img width="1273" height="467" alt="Postman " src="https://github.com/user-attachments/assets/c19e5cd3-8862-411a-8ccf-09eeb4c3d1fa" />

# Load Testing
Simulate concurrent requests to validate performance in postman

<img width="1278" height="792" alt="Lambda - Running" src="https://github.com/user-attachments/assets/71f80fe8-17c7-429d-afcc-3b65d2c7c465" />

# Performance Optimization (AWS Lambda Power Tuning)
Run Opensource AWS Lambda Power Tuning tool at 128 MB and 1024 MB.

Results
• 128 MB: Slowest and highest cost
• 1024 MB: Fastest and lowest total cost

<img width="1770" height="811" alt="Lambda Tuning before" src="https://github.com/user-attachments/assets/f74408ab-147b-46f1-aaa3-0a7c45d6c760" />

# Key Takeaways

AWS Lambda allocates vCPU (compute capacity) in proportion to the memory assigned to a function. Increasing memory doesn't just add RAM, it also speeds up execution.
This creates a meaningful tradeoff. While higher memory increases the cost per millisecond, it can reduce total execution duration enough to lower the overall cost, since Lambda bills based on duration, not just memory size. 
In other words, more memory doesn't always mean more cost. Lambda tweaking is how you can get a balance between cost optimization and performance efficiency.





