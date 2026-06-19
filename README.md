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
![Part1](part1-workflow-diagrams/part1-workflow-diagram1.png)

- Upload website files to the S3 Bucket:
![Part2](part1-workflow-diagrams/part1-workflow-diagram2.png)

- Setting up CloudFront Distribution to host website:
![Part3](part1-workflow-diagrams/part1-workflow-diagram3.png)

- Verifying Cloud Distribution is working:
![Part4](part1-workflow-diagrams/part1-workflow-diagram4.png)

- Updating CloudFront Settings for permission access:
![Part5](part1-workflow-diagrams/part1-workflow-diagram5.png)

- Updating S3 Bucket permission settings:
![Part6](part1-workflow-diagrams/part1-workflow-diagram6.png)

- Final Overview of Presentation Tier:
![Part7](part1-workflow-diagrams/part1-workflow-diagram7.png)

- Presentation Tier Completed:
![Part8](part1-workflow-diagrams/part1-workflow-diagram8.png)




