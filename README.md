# ☁️ Cloud Resume Challenge
🚀 **Live Demo:** [site.pingtoroot.com](https://site.pingtoroot.com)

This repository contains my implementation of the [Cloud Resume Challenge](https://cloudresumechallenge.dev/), a hands-on project designed to demonstrate proficiency with core cloud services, DevOps practices, and modern web development.

> **Goal**: Build and deploy a cloud-based resume website using AWS, serverless components, CI/CD, and more.

---

## 🧠 Key Concepts Covered

- Static website hosting on AWS  
- Domain and SSL via Route 53 + ACM  
- Serverless backend using Lambda Function URL and DynamoDB  
- Visitor counter with frontend-backend integration  
- CI/CD automation using GitHub Actions  
- Infrastructure as Code (optional stretch)

---

## 📁 Project Structure

```text
.
├── Main/                     # Frontend code (HTML, CSS, JS)
├── .github/workflows/       # GitHub Actions for CI/CD
├── backend/                 # Lambda function (Python) and test files
├── infrastructure/          # IaC templates (Terraform or CloudFormation)
└── README.md                # This documentation file
```
## 🚀 Architecture Overview
```text
[ Client (Browser) ]
        |
        v
[ CloudFront CDN ]
        |
        v
[ S3 Static Website ] <---> [ Lambda Function URL ] --> [ DynamoDB ]
```
- CloudFront: Caches and serves the website globally.
- S3: Hosts the static resume site.
- Route 53 + ACM: Custom domain and SSL certificate.
- Lambda Function URL (Python): Handles requests directly from the frontend.
- DynamoDB: Stores the count of website visitors.
- GitHub Actions: Automates deployment on code changes.

## 🔧 Tools & Technologies

**AWS Services**: S3, CloudFront, Route 53, ACM, Lambda (Function URL), DynamoDB  
**Languages**: HTML, CSS, JavaScript, Python (boto3)  
**CI/CD**: GitHub Actions  
**Optional**: Terraform / CloudFormation for Infrastructure as Code

---

## ✅ Completed Milestones

- Resume site designed with HTML/CSS  
- Hosted on S3 with public access  
- Secured with HTTPS via ACM + Route 53  
- Deployed through CloudFront  
- Visitor counter with JavaScript  
- Backend using Lambda Function URL (Python) 
- Visitor data stored in DynamoDB  
- CI/CD pipeline with GitHub Actions  
- *(Optional)* IaC with Terraform or CloudFormation  
- *(Optional)* Unit tests for Lambda function

---

## 📚 Resources Used

- [Cloud Resume Challenge Site](https://cloudresumechallenge.dev/)  
- [Jake Jarvis’s S3 Sync GitHub Action](https://github.com/jakejarvis/s3-sync-action)  
- [AWS Documentation](https://docs.aws.amazon.com/)  
- [DynamoDB Python Guide (boto3)](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/dynamodb.html)

---
## 🎥 Video Walkthrough (Spanish)

I've documented this project in a video series on YouTube (in Spanish), where I guide viewers step-by-step through each part of the Cloud Resume Challenge:

- 🔗 [Parte 1 – S3, CloudFront, Route 53](https://www.youtube.com/watch?v=6_SI_eva7CU)
- 🔗 [Parte 2 – Contador de visitas, API, DynamoDB](https://www.youtube.com/watch?v=Rml7gEw4Vx0)
- ⏳ [Parte 3 –  CI/CD con GitHub Actions + Secrets](https://www.youtube.com/watch?v=XQnPbMgv7Fc) 

---
## 🧑‍💻 Author

**Humberto Rodríguez**  
Cloud & Cybersecurity Enthusiast  
[LinkedIn](https://www.linkedin.com/in/humbertoruan/) | [YouTube](https://www.youtube.com/@pingtoroot) 

---

## 📝 License

This project is licensed under the **MIT License** — feel free to fork, reuse, or reference it for your own Cloud Resume Challenge.


 
