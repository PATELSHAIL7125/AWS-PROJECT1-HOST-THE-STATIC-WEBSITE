📁 AWS S3 – Static Website Hosting

This project demonstrates how to deploy a static website on Amazon S3 using AWS services.
It includes setting up a public S3 bucket, enabling static hosting, and deploying HTML/CSS/JS files.

🚀 Live Demo

🔗 Website URL: http://nextwork-website-project-my-first-bucket.s3-website-us-west-2.amazonaws.com/

📸 Screenshots

<img width="1916" height="1088" alt="image" src="https://github.com/user-attachments/assets/3c69b811-ca56-45aa-9578-7f73dedc3692" />
<img width="1919" height="1092" alt="image" src="https://github.com/user-attachments/assets/4179b72f-6cb7-4f5d-85f1-dbd5891d70b8" />
<img width="1918" height="1147" alt="image" src="https://github.com/user-attachments/assets/53f209f2-ed07-478d-9e76-c9a03d6566a3" />


📝 Project Overview

This project showcases:

Hosting a static website on Amazon S3

Configuring public access and bucket policy

Enabling Static Website Hosting

Uploading and serving HTML, CSS, JS files

Understanding AWS deployment basics

This helps demonstrate hands-on experience with cloud hosting and AWS services.

🛠️ Technologies Used

| Component       | Description                       |
| --------------- | --------------------------------- |
| **AWS S3**      | Static website hosting, storage   |
| **HTML/CSS/JS** | Website frontend                  |
| **AWS IAM**     | User permissions for S3           |
| **AWS Console** | Deployment & bucket configuration |


🧪 Steps to Deploy (Quick Guide)

1. Create S3 Bucket

Go to AWS S3 → Create Bucket

Disable "Block Public Access"

Name your bucket (must be globally unique)

2. Upload Website Files

Upload all your HTML, CSS, JS, and assets.

3. Enable Static Website Hosting

Go to Properties → Static Website Hosting

Choose: “Use this bucket to host a website”

Add:

index document: index.html

(optional) Error document: error.html

4. Add Bucket Policy

Paste your policy (replace with your bucket name):

{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-bucket-name/*"
    }
  ]
}

5. Open the Website URL

Copy the Static Website Endpoint and test it.

📘 Learnings

By completing this project, I learned:

How S3 stores and serves static assets

How bucket policies & public access work

How AWS handles static website hosting

Basics of cloud deployment workflows
