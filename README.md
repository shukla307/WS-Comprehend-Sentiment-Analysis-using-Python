# AWS-Comprehend-Sentiment-Analysis-using-Python

Sentiment analysis using BOTO3 for Python on Amazon Comprehend

This projects uses BOTO3 package for python.

What is Amazon Comprehend?
It’s a collection of pre-trained Natural Language Processing models and you can use to analyze your text. You can customize some of the models for your particular output types (document classification, entities detection).

AWS API Setup
Steps:

Create an AWS account
Create a user that has appropriate permissions (Comprehend, S3)
Create and download access keys
Use AWS CLI (Command Line Interface) to create environment variabes folder
Install BOTO3 package

AWS Comprehend Cost
** Free AWS Tier: Limit 50K units (5M characters) a month, $1 per 10K units after that.** 1 unit is 100 characters, and every tweet is ~2 units. In a scheduled job I am analyzing 1K tweets at once, so the free tier runs out fast. Be sure to check pricing before you proceed.

Three Ways to Run Sentiment Analysis
The notebook shows these three ways to run the analysis.

One text document at a time. Feed data directly from python, receive results back into python. Real time.
A batch of up to 25 documents. Feed data directly from python, receive results back into python. Real time.
Create an asynchronous Analysis Job. Feed the data from an S3 bucket. The results are saved into an S3 bucket. More powerful, but a lot more involved.

Reference.

Boto3 S3: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html

Boto3 Comprehend: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html
