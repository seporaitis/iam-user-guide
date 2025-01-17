# Actions, Resources, and Condition Keys for AWS IoT Things Graph<a name="list_awsiotthingsgraph"></a>

AWS IoT Things Graph \(service prefix: `iotthingsgraph`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/thingsgraph/latest/ug/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/thingsgraph/latest/APIReference/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/thingsgraph/latest/ug/iot-tg-security.html) permission policies\.

**Topics**
+ [Actions Defined by AWS IoT Things Graph](#awsiotthingsgraph-actions-as-permissions)
+ [Resources Defined by AWS IoT Things Graph](#awsiotthingsgraph-resources-for-iam-policies)
+ [Condition Keys for AWS IoT Things Graph](#awsiotthingsgraph-policy-keys)

## Actions Defined by AWS IoT Things Graph<a name="awsiotthingsgraph-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_awsiotthingsgraph.html)

## Resources Defined by AWS IoT Things Graph<a name="awsiotthingsgraph-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awsiotthingsgraph-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ Workflow ](https://docs.aws.amazon.com/thingsgraph/latest/ug/iot-tg-models-tdm-iot-workflow.html)  |  arn:$\{Partition\}:iotthingsgraph:$\{Region\}:$\{Account\}:Workflow/$\{NamespacePath\}  |  | 
|   [ System ](https://docs.aws.amazon.com/thingsgraph/latest/ug/iot-tg-models-tdm-iot-system.html)  |  arn:$\{Partition\}:iotthingsgraph:$\{Region\}:$\{Account\}:System/$\{NamespacePath\}  |  | 
|   [ SystemInstance ](https://docs.aws.amazon.com/thingsgraph/latest/ug/iot-tg-models-tdm-iot-sdc-deployconfig.html)  |  arn:$\{Partition\}:iotthingsgraph:$\{Region\}:$\{Account\}:Deployment/$\{NamespacePath\}  |   [ aws:ResourceTag/$\{TagKey\} ](#awsiotthingsgraph-aws_ResourceTag___TagKey_)   | 

## Condition Keys for AWS IoT Things Graph<a name="awsiotthingsgraph-policy-keys"></a>

AWS IoT Things Graph defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   [ aws:RequestTag/$\{TagKey\} ](https://docs.aws.amazon.com/thingsgraph/latest/ug//tagging-tg.html/reference_iam-permissions.html#iam-contextkeys)  | Filters access by a key that is present in the request the user makes to the thingsgraph service\. | String | 
|   [ aws:ResourceTag/$\{TagKey\} ](https://docs.aws.amazon.com/thingsgraph/latest/ug//tagging-tg.html/reference_iam-permissions.html#iam-contextkeys)  | Filters access by a tag key and value pair\. | String | 
|   [ aws:TagKeys ](https://docs.aws.amazon.com/thingsgraph/latest/ug//tagging-tg.html/reference_iam-permissions.html#iam-contextkeys)  | Filters access by the list of all the tag key names present in the request the user makes to the thingsgraph service\. | String | 