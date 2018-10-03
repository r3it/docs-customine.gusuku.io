---
title: Invoke AWS Lambda Function
date: 2018-01-22T16:07:50+09:00
weight: 1400
---
## Summary

Execute an AWS Lambda function.

## How to use

[Configure AWS Access Keys](../aws_set_access_key) to configure the authentication settings to run Lambda.

### Parameters to set

Set Authentication Region, Lambda Function Name Parameters to pass to Lambda.

#### Authentication

Specifies the authentication method.

[Configure AWS Access Keys](../aws_set_access_key) or [Get Authentication with AWS Cognito](../aws_cognito), which specifies one of the following actions:

#### Region

Specifies the AWS region where the Lambda function you want to execute resides.

Please specify a region name like “ap-northeast-1” instead of “Tokyo”.

#### Lambda Function Name

Specifies the Lambda function name.

#### Parameters to Pass to Lambda

Type the parameters that you want to pass to Lambda.

```
='{"date": "' & date_1 & '"}'
```

It is also possible to write expressions above:
