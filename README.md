# ☁️ Cloud Resume Challenge

This is my take on the [Cloud Resume Challenge](https://site.pingtoroot.com/), a project designed to showcase cloud skills by building and deploying a personal resume website using AWS services and modern DevOps practices.

## 🧠 What I Learned

This project helped me gain hands-on experience with:

- Core AWS services (S3, CloudFront, Route 53, Lambda, DynamoDB, IAM)
- Backend development using Python and the `boto3` library
- CI/CD automation with GitHub Actions
- Infrastructure as Code concepts
- API creation with AWS Lambda + API Gateway
- Secure data flow between front-end, backend, and database
- DNS and SSL/TLS management via ACM and Route 53


## 📦 Tech Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (Lambda), API Gateway
- **Database**: DynamoDB (on-demand)
- **CI/CD**: GitHub Actions
- **Hosting**: AWS S3 + CloudFront
- **Domain & SSL**: Route 53 + ACM

## 🔄 CI/CD Workflow

The CI/CD pipeline is triggered on pushes to the `main` branch. It performs the following:

- Syncs the frontend code to S3
- Invalidates the CloudFront cache
- Ensures the latest version is served instantly

## 🔢 Visitor Counter

A live visitor counter is integrated into the site. It works as follows:

1. Frontend JS calls the deployed API.
2. The API Gateway triggers a Lambda function.
3. The Lambda function reads/writes to DynamoDB to update the count.
4. Response is returned and rendered on the webpage.



