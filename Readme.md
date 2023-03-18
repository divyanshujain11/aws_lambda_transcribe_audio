# Integrating Amazon Web Services of Amazon transcribe, Amazon S3 bucket, Amazon lambda function

## Step1
Create S3 bucket
![s3](https://user-images.githubusercontent.com/77712311/226109244-75e559cc-93ef-4dfe-9a8a-9b948499c393.jpg)
S3 bucket : Amazon S3 bucket is an object storage service that allows users to store and retrieve data from anywhere on the web. It provides highly scalable, durable, and secure storage for various types of data, including audio files.

## Step2
Create Lambda function

Lambda function : Amazon Lambda is a serverless compute service that allows users to run code without the need for provisioning or managing servers. It can be used to trigger events and execute code in response to changes in data in Amazon S3 buckets.
![lambda](https://user-images.githubusercontent.com/77712311/226109253-86063e00-989c-45d3-8d71-2d95c7c08e93.jpg)

## Step3
Connect S3 bucket as a trigger for lambda function.


## Step4
Write a code in lambda function which contact to transcribe service that convert mp3 file to audio file.
![python code](https://github.com/divyanshujain11/aws_lambda_transcribe_audio/blob/fb4269d52db096d325d64d6ad4fbab54e0323381/lambda_function.py)

![code](https://user-images.githubusercontent.com/77712311/226109261-451ea4fd-2fc2-40bd-bc0e-2ed5d5ede389.jpg)


## Step5
Add IAM roles (Policies) to the Lambda function for connecting these services.
Policies :
   1. Amazon Transcribe.
   2. Amazon S3.
   3. Cloud Watch.
![IAM](https://user-images.githubusercontent.com/77712311/226109273-3286a251-3ea2-4925-9e17-d1a353195b68.jpg)

## Step6
Upload mp3 file in S3 bucket.
![upload](https://user-images.githubusercontent.com/77712311/226109364-517d21a7-92b2-47cd-acef-b50724ff7202.jpg)

## Step7
Download Transcribe file in JSON form.
![Successful](https://user-images.githubusercontent.com/77712311/226109288-24b5639c-28bb-4bc5-b9ee-b0873761a8ef.jpg)


# Video of whole process

https://user-images.githubusercontent.com/77712311/225930373-e50e6d70-3cac-4dec-9fe4-fc43004aaad5.mp4

