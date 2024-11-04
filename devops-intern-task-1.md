### Objective:
Create a FastAPI application that provisions EC2 instances using the AWS SDK (Boto3).

### Task Overview:
Develop a RESTful API using FastAPI that allows users to provision and manage Amazon EC2 instances. The application should include endpoints for creating, listing, starting, stopping, and terminating EC2 instances.

> Note: You have the option to implement just two primary APIs: one for creating EC2 instances and another for terminating them.

### Requirements:
#### 1. Environment Setup
- Set up a Python environment with FastAPI and Boto3.
- Ensure the application can run locally and is ready for deployment on an AWS EC2 instance.

#### 2. API Endpoints
Implement the following endpoints:
- POST /instances: Create a new EC2 instance.
    - Input: Instance type, AMI ID, key pair name, security group.
    - Output: Instance ID and status.
- GET /instances: List all EC2 instances.
    - Output: Instance IDs, types, states, and public IPs.
- POST /instances/{instance_id}/start: Start an existing EC2 instance.
    - Output: Confirmation message with the instance status.
- POST /instances/{instance_id}/stop: Stop an existing EC2 instance.
    - Output: Confirmation message with the instance status.
- DELETE /instances/{instance_id}: Terminate an existing EC2 instance.
    - Output: Confirmation message with the instance status.

#### 3. AWS SDK Integration
- Use Boto3 to interact with the AWS EC2 service.
- Ensure proper error handling for AWS API calls (e.g., handling exceptions for insufficient permissions or invalid parameters).

#### 4. Documentation
- Provide clear documentation on how to set up and run the application.
- Include examples of API requests and responses using tools like Postman or curl.

#### 5. Security Considerations
- Implement basic security measures such as input validation and error handling to prevent common vulnerabilities.

#### 6. Deployment (Optional)
- If time permits, deploy the FastAPI application on an EC2 instance or use AWS Lambda for a serverless approach.

### Deliverables:
- Source code hosted in a GitHub repository.
- A README file with setup instructions and API documentation.
- A short video demonstration of the application in action (optional).
