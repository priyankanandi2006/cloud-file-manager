# Cloud File Manager using AWS EC2 & S3

## Project Topic
Cloud File Manager - Upload and Download files using AWS EC2 and S3.

## Architecture
User (Laptop) -> EC2 Instance (t3.micro, Amazon Linux) -> S3 Bucket
![Architecture Diagram](architecture-diagram.jpeg)

Architecture Diagram created using draw.io / diagrams.net
Flowchart created using Lucidchart / draw.io

## How it Works
1. Create EC2 Instance
2. Create S3 Bucket
3. Create file in EC2: echo "Hello Cloud" > test.txt
4. Upload EC2 to S3: aws s3 cp test.txt s3://priyanka-cloud-file-manager-2026/test.txt
5. Download S3 to EC2: aws s3 cp s3://priyanka-cloud-file-manager-2026/test.txt downloaded.txt
6. Verify: cat downloaded.txt
7. Stop EC2 Instance

## Tools Used
- AWS EC2, AWS S3, AWS CLI
- GitHub
- draw.io for Architecture, Lucidchart for Flowchart

## Result
Upload and Download both successful.
