# AWS S3 Static Website Hosting

This project demonstrates hosting a static HTML website on Amazon S3 and deploying it using GitHub Actions.

## Technologies Used

- AWS S3
- GitHub Actions
- GitHub
- HTML

## S3 Bucket Policy

The following bucket policy allows public read access to objects in the S3 bucket:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::app1-payments-prod2-example1.com/*"
    }
  ]
}
