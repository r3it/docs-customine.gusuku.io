---
title: Set AWS Access Key
date: 2018-01-22T16:07:50+09:00
weight: 1340
---
## Summary

Configure access keys to access AWS.

When you use [Run AWS Lambda functions](../aws_lambda), the Authentication is performed with the access key you set here.

## How to use

In advance, create an IAM user, etc., and create access keys in the AWS Management Console.

Then set the necessary access rights. For example, if this credential contains [Run AWS Lambda functions](../aws_lambda), you have to give permission to the IAM user that you created, such as permission to execute the desired Lambda function.

* From a security standpoint, we recommend that you do not give more authority than is necessary.

### Parameters to set

Set the Access Key ID and Secret Access Key.

#### Access Key ID

Specify the Access Key ID.

#### Secret Access Key

Specify the secret access key.

This information is stored encrypted.

## Security Notes

We recommend that you set IAM for the access keys that you want to configure with only the minimum permissions necessary.

The secret access key is encrypted, but when performing an action such as “Executing an AWS Lambda function”, it is decrypted in the browser. It's hard to read as much as possible, but it's not 100% safe.

In the future, we are also considering an improvement to keep secret access keys on the server and not to see any secret access keys from the browser.
