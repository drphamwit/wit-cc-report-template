# Mythical Mysfits

https://www.mythicalmysfits.com/

## Introduction

Mythical Mysfits is a (fictional) pet adoption non-profit dedicated to helping abandoned, and often misunderstood, mythical creatures find a new forever family! Mythical Mysfits believes that all creatures deserve a second chance, even if they spent their first chance hiding under bridges and unapologetically robbing helpless travelers.

## Features
1. Registration
2. Login/Logout
3. View mysfits 
4. Filter mysfits
5. Adopt mysfits
6. Like mysfits

## System Architecture
![image info](https://d1.awsstatic.com/Getting%20Started/build-modern-app-fargate-lambda-dynamodb-python/architecture-diagram-AWS-Developer-Center_mythical-mysfits-application-architecture-1%401.5x.22db78a48a57bd00cce92f44146e96d3312ab1e3.png)

## Deployment
1. Sign In to the AWS Console
To begin, sign in to the [AWS Console](https://console.aws.amazon.com) for the AWS account you will be using.
2. Creating your Mythical Mysifts IDE
3. Cloning the Mythical Mysfits Workshop Repository

In the bottom panel of your new Cloud9 IDE, you will see a terminal command line terminal open and ready to use. If you close it or need a new one, use the *Window* > *New Terminal* menu.
4. Creating a Static Website in Amazon S3

Choose a name for your bucket and create it using the [```aws s3 mb```](https://docs.aws.amazon.com/cli/latest/reference/s3/mb.html) command, replacing where indicated:

```
aws s3 mb s3://REPLACE_ME_BUCKET_NAME
```
5. Copy the initial page of the Mystical Misfits website (index.html) to your S3 bucket using the [aws s3 cp] command:

```
aws s3 cp ~/environment/aws-modern-application-workshop/module-1/web/index.html s3://REPLACE_ME_BUCKET_NAME/index.html
```

6. Update the S3 Bucket Policy

To serve as a public website, we can create an S3 [Bucket Policy](https://docs.aws.amazon.com/AmazonS3/latest/dev/example-bucket-policies.html) that indicates objects stored within this new bucket are publicly accessible. S3 Bucket Policies are represented as JSON documents that authorizes or denies the invocation of S3 *Actions* (S3 API calls) to *Principals* (in our public example case, anyone). 

The JSON document for the necessary bucket policy is located at: `~/environment/aws-modern-application-workshop/module-1/aws-cli/website-bucket-policy.json`.  This file contains a string that needs to be replaced with the bucket name you've chosen (indicated with `REPLACE_ME_BUCKET_NAME`).

## Demo video (30 pts)

https://www.youtube.com/watch?v=abc

## References (5 pts)

https://github.com/aws-samples/aws-modern-application-workshop

## Team members (5 pts)

* John Doe (doej@wit.edu), Team Lead, Frontend dev
* Alan Smith (smitha@wit.edu), Backend dev, DB

