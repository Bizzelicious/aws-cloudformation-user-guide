# AWS Lambda Function DeadLetterConfig<a name="aws-properties-lambda-function-deadletterconfig"></a>

`DeadLetterConfig` is a property of the [AWS::Lambda::Function](aws-resource-lambda-function.md) resource that specifies a Dead Letter Queue \(DLQ\) that AWS Lambda \(Lambda\) sends events to when it can't process them\. For example, you can send unprocessed events to an Amazon Simple Notification Service \(Amazon SNS\) topic, where you can take further action\.

## Syntax<a name="w3ab2c21c14e1314b5"></a>

### JSON<a name="aws-properties-lambda-function-deadletterconfig-syntax.json"></a>

```
{
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-lambda-function-deadletterconfig-targetarn)" : String
}
```

### YAML<a name="aws-properties-lambda-function-deadletterconfig-syntax.yaml"></a>

```
[[ERROR] BAD/MISSING LINK TEXT](#cfn-lambda-function-deadletterconfig-targetarn): String
```

## Properties<a name="w3ab2c21c14e1314b7"></a>

`TargetArn`  
The Amazon Resource Name \(ARN\) of a resource where Lambda delivers unprocessed events, such as an Amazon SNS topic or Amazon Simple Queue Service \(Amazon SQS\) queue\. For the Lambda function [execution role](http://docs.aws.amazon.com/lambda/latest/dg/with-s3-example-create-iam-role.html), you must explicitly provide the relevant permissions so that access to your DLQ resource is part of the execution role for your Lambda function\.   
*Required: *No  
*Type*: String