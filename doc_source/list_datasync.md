# Actions, Resources, and Condition Keys for DataSync<a name="list_datasync"></a>

DataSync \(service prefix: `datasync`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/datasync/latest/userguide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/datasync/latest/userguide/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/datasync/latest/userguide/iam.html) permission policies\.

**Topics**
+ [Actions Defined by DataSync](#datasync-actions-as-permissions)
+ [Resources Defined by DataSync](#datasync-resources-for-iam-policies)
+ [Condition Keys for DataSync](#datasync-policy-keys)

## Actions Defined by DataSync<a name="datasync-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_datasync.html)

## Resources Defined by DataSync<a name="datasync-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#datasync-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ agent ](https://docs.aws.amazon.com/datasync/latest/userguide/agent.html)  |  arn:$\{Partition\}:datasync:$\{Region\}:$\{AccountId\}:agent/$\{AgentId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#datasync-aws_ResourceTag___TagKey_)   | 
|   [ location ](https://docs.aws.amazon.com/datasync/latest/userguide/location.html)  |  arn:$\{Partition\}:datasync:$\{Region\}:$\{AccountId\}:location/$\{LocationId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#datasync-aws_ResourceTag___TagKey_)   | 
|   [ task ](https://docs.aws.amazon.com/datasync/latest/userguide/task.html)  |  arn:$\{Partition\}:datasync:$\{Region\}:$\{AccountId\}:task/$\{TaskId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#datasync-aws_ResourceTag___TagKey_)   | 
|   [ taskexecution ](https://docs.aws.amazon.com/datasync/latest/userguide/taskexecution.html)  |  arn:$\{Partition\}:datasync:$\{Region\}:$\{AccountId\}:task/$\{TaskId\}/execution/$\{ExecutionId\}  |  | 

## Condition Keys for DataSync<a name="datasync-policy-keys"></a>

DataSync defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   aws:RequestTag/$\{TagKey\}  | Filters create requests based on the allowed set of values for each of the tags\. | String | 
|   aws:ResourceTag/$\{TagKey\}  | Filters actions based on tag\-value associated with the resource\. | String | 
|   aws:TagKeys  | Filters create requests based on the presence of mandatory tags in the request\. | String | 