# Serverless Image Processing with AWS Lambda and S3

This project demonstrates a fully serverless architecture on AWS for image processing tasks such as resizing and watermarking. Users can upload images via an API or directly to an S3 bucket, which triggers a Lambda function to process and store the result.

---

## Tech Stack

- AWS S3 – Stores original and processed images.
- AWS Lambda – Processes images (e.g., resizing, watermarking).
- Amazon API Gateway (optional) – Allows image uploads through an HTTP endpoint.
- AWS DynamoDB (optional) – Stores metadata (filename, timestamp, status).
- IAM Roles & Policies – Secures access between services.

---

## Architecture Overview

User (upload)  
↓  
API Gateway (optional)  
↓  
S3 Bucket - Original Images  
↓ Trigger (Event)  
AWS Lambda Function  
├──→ S3 Bucket - Processed Images  
└──→ DynamoDB Table (optional)

---

## Features

- Event-driven with S3 triggers  
- Serverless and cost-efficient (pay-as-you-go)  
- Auto-scalable and maintenance-free  
- Secured using IAM and S3 bucket policies  
- Optional support for API uploads and image metadata tracking

---

## Security Considerations

- Lambda uses a least-privilege IAM role to access only necessary resources.  
- S3 buckets are protected with bucket policies and optionally private access.  
- All communication is secured via HTTPS when using API Gateway.

---

## Deployment (Optional)

You can deploy this stack using AWS Console, CloudFormation, or Terraform.

---

## Learning Outcomes

- Understand how to build event-driven serverless applications.  
- Learn how to use AWS Lambda + S3 triggers.  
- Implement secure and scalable cloud-native architectures.

---

## Author

Mona Shabka  
mona.shabka@yahoo.com
https://www.linkedin.com/in/mona-shabka-a8058573
Project under Manara Tech Academy

---

## License

This project is for educational purposes.

