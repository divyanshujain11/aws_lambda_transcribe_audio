# Integrating Amazon Web Services of Amazon transcribe, Amazon S3 bucket, Amazon lambda function

## Step1
Create S3 bucket

S3 bucket : Amazon S3 bucket is an object storage service that allows users to store and retrieve data from anywhere on the web. It provides highly scalable, durable, and secure storage for various types of data, including audio files.

## Step2
Create Lambda function

Lambda function : Amazon Lambda is a serverless compute service that allows users to run code without the need for provisioning or managing servers. It can be used to trigger events and execute code in response to changes in data in Amazon S3 buckets.

## Step3
Connect S3 bucket as a trigger for lambda function.

## Step4
Write a code in lambda function which contact to transcribe service that convert mp3 file to audio file.
![python code](https://github.com/divyanshujain11/aws_lambda_transcribe_audio/blob/fb4269d52db096d325d64d6ad4fbab54e0323381/lambda_function.py)


## Step5
Add IAM roles (Policies) to the Lambda function for connecting these services.
Policies :
   1. Amazon Transcribe.
   2. Amazon S3.
   3. Cloud Watch.

## Step6
Upload mp3 file in S3 bucket.

## Step7
Download Transcribe file in JSON form.

#Video of whole process




https://user-images.githubusercontent.com/77712311/225930373-e50e6d70-3cac-4dec-9fe4-fc43004aaad5.mp4

