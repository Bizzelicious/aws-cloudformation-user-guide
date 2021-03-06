# Amazon Cognito UserPool DeviceConfiguration<a name="aws-properties-cognito-userpool-deviceconfiguration"></a>

`DeviceConfiguration` is a property of the [AWS::Cognito::UserPool](aws-resource-cognito-userpool.md) resource that defines the device configuration of an Amazon Cognito User Pool\.

## Syntax<a name="aws-properties-cognito-userpool-deviceconfiguration-syntax"></a>

### JSON<a name="aws-properties-cognito-userpool-deviceconfiguration-syntax.json"></a>

```
{
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-cognito-userpool-deviceconfiguration-challengerequiredonnewdevice)" : Boolean,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-cognito-userpool-deviceconfiguration-deviceonlyrememberedonuserprompt)" : Boolean
}
```

### YAML<a name="aws-properties-cognito-userpool-deviceconfiguration-syntax.yaml"></a>

```
[[ERROR] BAD/MISSING LINK TEXT](#cfn-cognito-userpool-deviceconfiguration-challengerequiredonnewdevice): Boolean
[[ERROR] BAD/MISSING LINK TEXT](#cfn-cognito-userpool-deviceconfiguration-deviceonlyrememberedonuserprompt): Boolean
```

## Properties<a name="aws-properties-cognito-userpool-deviceconfiguration-properties"></a>

`ChallengeRequiredOnNewDevice`  
Indicates whether a challenge is required on a new device\. Only applicable to a new device\.  
*Type*: Boolean  
*Required: *No

`DeviceOnlyRememberedOnUserPrompt`  
If true, a device is only remembered on user prompt\.  
*Type*: Boolean  
*Required: *No