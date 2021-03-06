# Amazon EC2 Block Device Mapping Property<a name="aws-properties-ec2-blockdev-mapping"></a>

The Amazon EC2 block device mapping property is an embedded property of the  resource\. For block device mappings for an Auto Scaling launch configuration, see [AutoScaling Block Device Mapping](aws-properties-as-launchconfig-blockdev-mapping.md)\.

## Syntax<a name="w3ab2c21c14d555b7"></a>

### JSON<a name="aws-properties-properties-ec2-blockdev-mapping-syntax.json"></a>

```
{
   "DeviceName" : String,
   "Ebs" : EC2 EBS Block Device,
   "NoDevice" : Boolean,
   "VirtualName" : String
}
```

### YAML<a name="aws-properties-properties-ec2-blockdev-mapping-syntax.yaml"></a>

```
DeviceName: String
Ebs: EC2 EBS Block Device
NoDevice: Boolean
VirtualName: String
```

## Properties<a name="w3ab2c21c14d555b9"></a>

`DeviceName`  
The name of the device within Amazon EC2\. For more information, see [Device Naming on Linux Instances](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/device_naming.html) in the *Amazon EC2 User Guide for Linux Instances*\.  
*Required: *Yes  
*Type*: String

`Ebs`  
*Required: *Conditional You can specify either `VirtualName` or `Ebs`, but not both\.  
*Type*: \.

`NoDevice`  
This property can be used to unmap a defined device\.  
*Required: *No  
*Type*: Boolean

`VirtualName`  
The name of the virtual device\. The name must be in the form `ephemeralX ` where *X* is a number starting from zero \(0\); for example, `ephemeral0`\.  
*Required: *Conditional You can specify either `VirtualName` or `Ebs`, but not both\.  
*Type*: String

## Examples<a name="w3ab2c21c14d555c11"></a>

### Block Device Mapping with two EBS Volumes<a name="w3ab2c21c14d555c11b2"></a>

This example sets the EBS\-backed root device \(/dev/sda1\) size to 50 GiB, and another EBS\-backed device mapped to /dev/sdm that is 100 GiB in size\.

```
"BlockDeviceMappings" : [
   {
      "DeviceName" : "/dev/sda1",
      "Ebs" : { "VolumeSize" : "50" }
   },
   {
      "DeviceName" : "/dev/sdm",
      "Ebs" : { "VolumeSize" : "100" }
   }
]
```

### Block Device Mapping with an Ephemeral Drive<a name="w3ab2c21c14d555c11b4"></a>

This example maps an ephemeral drive to device /dev/sdc\.

```
"BlockDeviceMappings" : [
   {
      "DeviceName"  : "/dev/sdc",
      "VirtualName" : "ephemeral0"
   }
]
```

### Unmapping an AMI\-defined Device<a name="w3ab2c21c14d555c11b6"></a>

To unmap a device defined in the AMI, set the `NoDevice` property to an empty map, as shown here:

```
{
   "DeviceName":"/dev/sde",
   "NoDevice": {}
}
```

## See Also<a name="w3ab2c21c14d555c13"></a>

+ [Amazon EC2 Instance Store](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html) in the *Amazon Elastic Compute Cloud User Guide*