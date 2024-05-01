# Simple Cloud-Based Online Music Subscription Application

## Overview
The online music subscription application provides users with access to a vast library of music tracks. Users can register, log in, and search for music based on title, artist, or year. The application is fully hosted on AWS, utilizing services such as EC2, S3, API Gateway, Lambda, and DynamoDB.

This project, completed individually within a month from March to April 2024 as part of the Cloud Computing course, earned a distinguished **High Distinction** mark.

## Architecture
- **AWS EC2**: Hosts the web server environment (Apache2) where the HTML website is deployed. Users can access the application by entering the root Public IPv4 DNS of the EC2 instance in their web browser or by running it locally.
- **AWS S3**: Functions as a repository for storing images of artists referenced in the application, facilitating efficient retrieval and management of media content.
- **AWS API Gateway**: Provides RESTful APIs for communication between the client-side application and backend services.
- **AWS Lambda (Python)**: Executes Python-based backend logic to handle various tasks, including user authentication, registration, music search queries, and management of user's music subscriptions. Lambda functions provide scalable and cost-effective computing resources, ensuring optimal performance.
- **AWS DynamoDB**: Serves as the database solution for storing user login credentials and music metadata. It comprises three distinct tables: one for user login information, one for music details, and one for managing subscription information. DynamoDB's flexible and scalable architecture enables efficient data storage and retrieval, supporting the dynamic requirements of the application.
