# 🟦 Static Website Hosting Using Amazon S3

This project is a simple static website hosted using Amazon S3.  
It includes only two files:

- index.html – Main webpage  
- styles.css – Styling for the page  

This project demonstrates how to deploy a basic static website on Amazon S3 using static website hosting.

---

## 📁 Project Structure

aws-s3-static-website/
│
├── index.html
└── styles.css

---

## 🚀 Features
- Simple HTML + CSS webpage
- Fully hosted on Amazon S3
- Publicly accessible website link
- Beginner-friendly cloud project

---

## ⚙️ How to Deploy on AWS S3

### 1️⃣ Create S3 Bucket
- Go to AWS → S3 → Create bucket  
- Bucket name example: `mayur-static-website`  
- Uncheck “Block all public access”  
- Create bucket

### 2️⃣ Enable Static Website Hosting
- Go to **Properties**
- Scroll to **Static website hosting**
- Enable it
- Index document: `index.html`

### 3️⃣ Upload Your Files
- Upload `index.html`  
- Upload `styles.css`

### 4️⃣ Make Files Public
Select file → Actions → **Make public**

OR use this bucket policy:

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}

### 5️⃣ Get Your Website URL
Go to:
Properties → Static Website Hosting

Example URL:
http://your-bucket-name.s3-website-us-east-1.amazonaws.com

---

## 🧠 What You Learn
- Static hosting using S3  
- Public access & permissions  
- Basic AWS deployment workflow  

---

## 👤 Author
**Mayur Borse**
