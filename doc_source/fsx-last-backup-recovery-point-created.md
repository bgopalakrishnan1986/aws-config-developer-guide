# fsx\-last\-backup\-recovery\-point\-created<a name="fsx-last-backup-recovery-point-created"></a>

Checks if a recovery point was created for Amazon FSx File Systems\. The rule is NON\_COMPLIANT if the Amazon FSx File System does not have a corresponding recovery point created within the specified time period\. 

**Identifier:** FSX\_LAST\_BACKUP\_RECOVERY\_POINT\_CREATED

**Trigger type:** Periodic

**AWS Region:** All supported AWS regions except China \(Beijing\), China \(Ningxia\), AWS GovCloud \(US\-East\), AWS GovCloud \(US\-West\), Asia Pacific \(Jakarta\), Asia Pacific \(Osaka\), Europe \(Milan\), Africa \(Cape Town\) Region

**Parameters:**

resourceTags \(Optional\)Type: String  
Tags of Amazon FSx File Systems for the rule to check, in JSON format\.

resourceId \(Optional\)Type: String  
ID of Amazon FSx File System for the rule to check\.

recoveryPointAgeValue \(Optional\)Type: intDefault: 1  
Numerical value for maximum allowed age\. No more than 744 for hours, 31 for days\.

recoveryPointAgeUnit \(Optional\)Type: StringDefault: days  
Unit of time for maximum allowed age\. Accepted values: 'hours', 'days'\.

## AWS CloudFormation template<a name="w79aac11c32c17b7d313c15"></a>

To create AWS Config managed rules with AWS CloudFormation templates, see [Creating AWS Config Managed Rules With AWS CloudFormation Templates](aws-config-managed-rules-cloudformation-templates.md)\.