---
title: Run JavaScript
date: 2018-01-22T16:07:50+09:00
weight: 2000
---
## Summary

Runs any JavaScript.

## How to use

### Parameters to set

Set JavaScript.

#### JavaScript

Directly write JavaScript to be executed.

You can use the kintone object as you would any regular kintone customization.

##### **How do I return a value and refer to it from other actions?**

The return result from this JavaScript can be referenced by other actions in an expression such as $1. Return can also return Promise.

```
return "Hello, World!";
```

##### **How do I reference the results of other actions?**

If you want to see the results of other actions from this JavaScript, you can reference them via the customine object. For example, the result of action 1 is customine[1] can be retrieved.

```
alert("The result of action 1 is [" + customine[1] + "]！");
```

However, the result of an action must be completed before the action can be taken correctly.
