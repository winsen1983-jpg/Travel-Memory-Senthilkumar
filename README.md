# Travel-Memory-Senthilkumar
Travel Memory-Senthilkumar

Travel Memory Project – Deployment Documentation
Project Overview

This document summarizes the deployment and configuration process for the Travel Memory Project, including infrastructure setup, backend and frontend deployment, load balancer configuration, AMI creation, and reverse proxy implementation.

1. EC2 Instance Creation

Successfully created EC2 instances for the application deployment.

<img width="975" height="70" alt="image" src="https://github.com/user-attachments/assets/50ab9893-ad5f-4ee2-b48b-60f4fecdab7c" />


Insert EC2 Instance Creation Screenshot Here
2. Security Group Configuration

Configured Security Groups with the required inbound and outbound rules to allow application traffic.

<img width="975" height="226" alt="image" src="https://github.com/user-attachments/assets/d8c07716-8ca0-45a9-8aea-cdd6d0aaa6b6" />


Insert Security Group Screenshot Here

3. Backend Working Status

Verified that the backend application is running successfully.

<img width="975" height="427" alt="image" src="https://github.com/user-attachments/assets/9e320c6b-e430-483c-9ffd-6bdc263b4bc7" />


Insert Backend Working Screenshot Here
4. Frontend Working Status

Verified that the frontend application is deployed and accessible.

<img width="975" height="456" alt="image" src="https://github.com/user-attachments/assets/0c7db930-07b8-4339-9021-ce87ef20efc3" />


Insert Frontend Working Screenshot Here

5. Add Experience Page

Successfully tested the Add Experience functionality.

<img width="975" height="485" alt="image" src="https://github.com/user-attachments/assets/a37b3be1-3f2c-4841-9a1f-6fa7e5acdf08" />


Insert Add Experience Page Screenshot Here

6. Backend Configuration

Configured backend services including:

Environment variables
Database connection
API configuration
Required dependencies
<img width="975" height="824" alt="image" src="https://github.com/user-attachments/assets/1f731809-4171-4983-bc4b-662635bd15e8" />


Insert Backend Configuration Screenshot Here

7. Frontend Configuration

Configured frontend application with:

API endpoint configuration
Build process
Environment variables
<img width="949" height="667" alt="image" src="https://github.com/user-attachments/assets/dae09bfe-938f-4460-a9ba-c5f4bce4dbef" />


Insert Frontend Configuration Screenshot Here

8. Backend Deployment

Successfully deployed the backend application on the EC2 instance.

<img width="975" height="464" alt="image" src="https://github.com/user-attachments/assets/a79ce62e-862a-4c9e-ba50-799af7799324" />


Insert Backend Deployment Screenshot Here

9. AMI Creation

Created Amazon Machine Images (AMIs) for both Backend and Frontend servers for future deployments.

Backend AMI

<img width="975" height="204" alt="image" src="https://github.com/user-attachments/assets/1eb2950c-9824-4081-b4c7-43f5fcdd370e" />


Frontend AMI

<img width="975" height="161" alt="image" src="https://github.com/user-attachments/assets/4c128a80-9bbd-4d90-afd8-89720af5f75f" />
e

10. Launching Instances from AMIs

Using the created AMIs, launched new EC2 instances for both:

Backend Server
Frontend Server
<img width="975" height="179" alt="image" src="https://github.com/user-attachments/assets/19de8516-5967-4e8b-8221-74f542e2605e" />


Insert EC2 Instances Created from AMIs Screenshot Here

11. Target Group Creation

Created Target Groups for routing traffic through the Load Balancer.

📷 Screenshot

Insert Target Group Screenshot Here

12. Load Balancer Configuration

Configured Application Load Balancer (ALB) to distribute incoming traffic between application instances.

<img width="975" height="139" alt="image" src="https://github.com/user-attachments/assets/ffd653ed-afeb-47b4-961a-0346ee4056d7" />


Insert Load Balancer Screenshot Here

13. Backend Reverse Proxy Configuration

Configured Reverse Proxy (Nginx) for the backend application.

Configuration Highlights
Installed Nginx
Configured proxy settings
Forwarded requests to backend application
Restarted and verified Nginx service
<img width="975" height="440" alt="image" src="https://github.com/user-attachments/assets/69cf7b1a-e82b-4a37-b73a-8a5e67528cc4" />


Insert Nginx Configuration Screenshot Here

<img width="975" height="254" alt="image" src="https://github.com/user-attachments/assets/2f3218eb-34b9-48e1-aa8f-88cde5dc8b2a" />


Insert Reverse Proxy Working Screenshot Here

14. Final Application Verification

Verified that:

✅ Frontend is accessible
✅ Backend APIs are responding
✅ Load Balancer is routing traffic correctly
✅ Reverse Proxy is functioning
✅ Add Experience feature works successfully
✅ Application is fully operational
📷 Screenshot

Insert Final Working Application Screenshot Here

Project Architecture
                    Users
                      │
                      ▼
          Application Load Balancer
               /                \
              /                  \
      Frontend EC2          Backend EC2
                                   │
                             Reverse Proxy
                                   │
                            Backend Service
                                   │
                               Database
Conclusion

The Travel Memory Project was successfully deployed on AWS by completing the following tasks:

Created EC2 instances
Configured Security Groups
Deployed Backend and Frontend
Configured Backend and Frontend environments
Created AMIs for backup and scaling
Launched new instances from AMIs
Configured Target Groups
Configured Application Load Balancer
Implemented Reverse Proxy using Nginx
Verified end-to-end functionality of the application

This format is suitable for submission as a project report or documentation and can be enhanced by inserting your screenshots under each corresponding section.
