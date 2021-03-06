# AWS CodeDeploy DeploymentGroup Deployment Revision<a name="aws-properties-codedeploy-deploymentgroup-deployment-revision"></a>

`Revision` is a property of the [AWS::CodeDeploy::DeploymentGroup](aws-resource-codedeploy-deploymentgroup.md) property that defines the location of the AWS CodeDeploy application revision to deploy\.

## Syntax<a name="w3ab2c21c14d337b5"></a>

### JSON<a name="aws-properties-codedeploy-deploymentgroup-deployment-revision-syntax.json"></a>

```
{
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-properties-codedeploy-deploymentgroup-deployment-revision-githublocation)" : GitHubLocation,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-properties-codedeploy-deploymentgroup-deployment-revision-revisiontype)" : String,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-properties-codedeploy-deploymentgroup-deployment-revision-s3location)" : S3Location
}
```

### YAML<a name="aws-properties-codedeploy-deploymentgroup-deployment-revision-syntax.yaml"></a>

```
[[ERROR] BAD/MISSING LINK TEXT](#cfn-properties-codedeploy-deploymentgroup-deployment-revision-githublocation):
  GitHubLocation
[[ERROR] BAD/MISSING LINK TEXT](#cfn-properties-codedeploy-deploymentgroup-deployment-revision-revisiontype): String
[[ERROR] BAD/MISSING LINK TEXT](#cfn-properties-codedeploy-deploymentgroup-deployment-revision-s3location):
  S3Location
```

## Properties<a name="w3ab2c21c14d337b7"></a>

`GitHubLocation`  
If your application revision is stored in GitHub, information about the location where it is stored\.  
*Required: *No  
*Type*: [AWS CodeDeploy DeploymentGroup Deployment Revision GitHubLocation](aws-properties-codedeploy-deploymentgroup-deployment-revision-githublocation.md)

`RevisionType`  
The application revision's location, such as in an S3 bucket or GitHub repository\. For valid values, see [RevisionLocation](http://docs.aws.amazon.com/codedeploy/latest/APIReference/API_RevisionLocation.html) in the *AWS CodeDeploy API Reference*\.  
*Required: *No  
*Type*: String

`S3Location`  
If the application revision is stored in an S3 bucket, information about the location\.  
*Required: *No  
*Type*: [AWS CodeDeploy DeploymentGroup Deployment Revision S3Location](aws-properties-codedeploy-deploymentgroup-deployment-revision-s3location.md)