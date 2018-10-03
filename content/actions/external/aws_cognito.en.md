---
title: Get Credentials Using AWS Cognito
date: 2018-01-22T16:07:50+09:00
weight: 1360
---
## Summary

Get your credentials using AWS Cognito.

## How to use

In advance, create your Cognito identity pool in the AWS Management Console.

Enable "Access for Unauthenticated Identities" for the identity pool you just created, and set the required permissions in Unauthenticated Roles.

* From a security standpoint, we recommend that you do not give more authority than is necessary.

### Parameters to set

Set RegionIdentity Pool Identity.

#### Region

Specifies the region in which the identity pool is located.

#### Identity Pool ID

Specifies the ID of the identity pool.

## Limitations

It does not support getting authenticated roles by Cognito authenticated users.

## Security Notes

We recommend that you set IAM for the access keys that you want to configure with only the minimum permissions necessary.

Privileges assigned to “Unauthenticated Roles” are effectively “Published Features/Anyone Can Use”.
