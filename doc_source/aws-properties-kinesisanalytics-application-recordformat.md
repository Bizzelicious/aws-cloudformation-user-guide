# Amazon Kinesis Data Analytics Application RecordFormat<a name="aws-properties-kinesisanalytics-application-recordformat"></a>

The `RecordFormat` property type describes the record format and relevant mapping information that should be applied to schematize the records on the stream\. 

 `RecordFormat` is a property of the [AWS::KinesisAnalytics::Application](aws-resource-kinesisanalytics-application.md) property type\. 

## Syntax<a name="aws-properties-kinesisanalytics-application-recordformat-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-kinesisanalytics-application-recordformat-syntax.json"></a>

```
{
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-kinesisanalytics-application-recordformat-mappingparameters)" : MappingParameters,
  "[[ERROR] BAD/MISSING LINK TEXT](#cfn-kinesisanalytics-application-recordformat-recordformattype)" : String
}
```

### YAML<a name="aws-properties-kinesisanalytics-application-recordformat-syntax.yaml"></a>

```
  [[ERROR] BAD/MISSING LINK TEXT](#cfn-kinesisanalytics-application-recordformat-mappingparameters): 
    MappingParameters
  [[ERROR] BAD/MISSING LINK TEXT](#cfn-kinesisanalytics-application-recordformat-recordformattype): String
```

## Properties<a name="aws-properties-kinesisanalytics-application-recordformat-properties"></a>

`MappingParameters`  
When configuring application input at the time of creating or updating an application, provides additional mapping information specific to the record format \(such as JSON, CSV, or record fields delimited by some delimiter\) on the streaming source\.   
 *Required*: No  
 *Type*: [Kinesis Data Analytics Application MappingParameters](aws-properties-kinesisanalytics-application-mappingparameters.md)  
 *Update requires*: No interruption 

`RecordFormatType`  
The type of record format \(e\.g `CSV` or `JSON`\.\)  
 *Required*: Yes  
 *Type*: String  
 *Update requires*: No interruption 