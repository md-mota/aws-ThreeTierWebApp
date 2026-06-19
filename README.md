# AWS Three‑Tier Web Application

A fully serverless, scalable, and globally distributed three‑tier web application built using Amazon S3, CloudFront, API Gateway, Lambda, and DynamoDB. This project demonstrates how modern cloud applications are architected using AWS native services.

---

## Project Overview

This project implements a complete **three‑tier architecture**:

- **Presentation Tier** – Static website hosted on S3 and delivered globally via CloudFront  
- **Logic Tier** – Serverless backend using AWS Lambda + API Gateway  
- **Data Tier** – NoSQL database using DynamoDB  

The goal of this project is to design, deploy, and connect all three layers into a functional cloud application that retrieves user data through a serverless API and displays it through a globally distributed front end.

---

## Architecture Overview and Workflow Diagrams

### Part 1: Presentation Tier

- Creating the S3 Bucket:  
<img src="part1-workflow-diagrams/part1-workflow-diagram1.png" width="700">

- Upload website files to the S3 Bucket:  
<img src="part1-workflow-diagrams/part1-workflow-diagram2.png" width="700">

- Setting up CloudFront Distribution to host website:  
<img src="part1-workflow-diagrams/part1-workflow-diagram3.png" width="700">

- Verifying Cloud Distribution is working:  
<img src="part1-workflow-diagrams/part1-workflow-diagram4.png" width="700">

- Updating CloudFront Settings for permission access:  
<img src="part1-workflow-diagrams/part1-workflow-diagram5.png" width="700">

- Updating S3 Bucket permission settings:  
<img src="part1-workflow-diagrams/part1-workflow-diagram6.png" width="700">

- Final Overview of Presentation Tier:  
<img src="part1-workflow-diagrams/part1-workflow-diagram7.png" width="700">

- Presentation Tier Completed:  
<img src="part1-workflow-diagrams/part1-workflow-diagram8.png" width="500">

---

### Part 2: Logic Tier

- Creating the Lambda Function that will fetch data from the Database:  
<img src="part2-workflow-diagrams/part2-workflow-diagram1.png" width="600">

- Create a new API in API Gateway to carry requests to the Lambda Function:  
<img src="part2-workflow-diagrams/part2-workflow-diagram2.png" width="600">

- Create API resource that will handle the API requests:  
<img src="part2-workflow-diagrams/part2-workflow-diagram3.png" width="600">

- Create the API method that allows things to be done with the resource:  
<img src="part2-workflow-diagrams/part2-workflow-diagram4.png" width="600">

- Deploy API and make accessible through a public endpoint:  
<img src="part2-workflow-diagrams/part2-workflow-diagram5.png" width="600">

- Logic Tier Completed:  
<img src="part2-workflow-diagrams/part2-workflow-diagram6.png" width="500">

---

### Part 3: Data Tier

- Create DynamoDB table to store user data:  
<img src="part3-workflow-diagrams/part3-workflow-diagram1.png" width="700">

- Adding sample data to the DynamoDB table:  
<img src="part3-workflow-diagrams/part3-workflow-diagram2.png" width="700">

- Lambda function created like in Logic Tier:  
<img src="part3-workflow-diagrams/part3-workflow-diagram3.png" width="700">

- Implementing Lambda Function Code like in Logic Tier:  
<img src="part3-workflow-diagrams/part3-workflow-diagram4.png" width="700">

- Testing the Lambda Function with Lambda Function Test:  
<img src="part3-workflow-diagrams/part3-workflow-diagram5.png" width="700">

- Grant DynamoDB access to Lambda:  
<img src="part3-workflow-diagrams/part3-workflow-diagram6.png" width="700">

- Testing Lambda Function again after DB access:  
<img src="part3-workflow-diagrams/part3-workflow-diagram7.png" width="700">

- Final Workflow of Data Tier:  
<img src="part3-workflow-diagrams/part3-workflow-diagram8.png" width="700">

- Data Tier Completed:  
<img src="part3-workflow-diagrams/part3-workflow-diagram9.png" width="500">

---