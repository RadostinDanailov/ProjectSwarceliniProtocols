# 🌐 Static Website Deployment on AWS  
# S3 + CloudFront + Terraform + GitHub Actions

This project hosts a static website on **Amazon S3**, delivered globally through **CloudFront**, with fully automated deployments using **GitHub Actions**.  
All infrastructure is provisioned and managed using **Terraform**, ensuring a reproducible, version‑controlled setup.

---

## 🚀 Features

- Static website hosting on Amazon S3  
- Global CDN distribution via CloudFront  
- Automatic HTTPS (CloudFront-managed certificate)  
- Infrastructure as Code using Terraform  
- CI/CD pipeline triggered on every push to `main`  
- Automatic CloudFront cache invalidation  
- Zero‑downtime deployments  

---

## 🏗️ Architecture Overview :


- GitHub Actions deploys the site to S3  
- CloudFront distributes content globally  
- Terraform provisions all AWS resources  

---

## 📁 Project Structure


- GitHub Actions deploys the site to S3  
- CloudFront distributes content globally  
- Terraform provisions all AWS resources  

---

## ⚙️ CI/CD Pipeline (GitHub Actions)

The workflow automatically:

1. Checks out the repository  
2. Configures AWS credentials  
3. Syncs all files to the S3 bucket  
4. Invalidates CloudFront cache  
5. Makes the new version instantly available worldwide  

---


Terraform provisions:

- S3 bucket  
- CloudFront distribution  
- IAM roles/policies (if included)  

---

## 🔐 Required GitHub Secrets

Your GitHub Actions workflow requires these secrets:

| Secret Name | Description |
|-------------|-------------|
| `AWS_ACCESS_KEY_ID` | IAM user access key |
| `AWS_SECRET_ACCESS_KEY` | IAM user secret |
| `AWS_REGION` | AWS region (e.g., eu-west-2) |
| `S3_BUCKET` | Name of the S3 bucket |
| `CLOUDFRONT_DISTRIBUTION_ID` | CloudFront distribution ID |

---

## 🌍 Live URL

Add your CloudFront domain here:

https://d274qj79mowjvv.cloudfront.net/ProjectSwarceliniProtocols.html


## 🧪 Future Improvements

- Add custom domain + Route53 + ACM certificate  
- Add build step (React, Astro, Hugo, etc.)  
- Add preview deployments for feature branches  
- Add CloudWatch monitoring  
- Add WAF for security hardening  








