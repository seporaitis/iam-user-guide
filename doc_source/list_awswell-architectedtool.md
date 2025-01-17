# Actions, Resources, and Condition Keys for AWS Well\-Architected Tool<a name="list_awswell-architectedtool"></a>

AWS Well\-Architected Tool \(service prefix: `wellarchitected`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/wellarchitected/latest/userguide/)\.
+ View a [list of the API operations available for this service](https://docs.aws.amazon.com/wellarchitected/latest/userguide/)\.
+ Learn how to protect this service and its resources by [using IAM](https://docs.aws.amazon.com/wellarchitected/latest/userguide/iam-auth-access.html) permission policies\.

**Topics**
+ [Actions Defined by AWS Well\-Architected Tool](#awswell-architectedtool-actions-as-permissions)
+ [Resources Defined by AWS Well\-Architected Tool](#awswell-architectedtool-resources-for-iam-policies)
+ [Condition Keys for AWS Well\-Architected Tool](#awswell-architectedtool-policy-keys)

## Actions Defined by AWS Well\-Architected Tool<a name="awswell-architectedtool-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. By using policies, you define the permissions for anyone performing an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\. For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ CreateWorkload ](https://docs.aws.amazon.com/wellarchitected/latest/userguide/define-workload.html)  | Creates a new workload\. | Write |  |  |  | 
|   [ DeleteWorkload ](https://docs.aws.amazon.com/wellarchitected/latest/userguide/workloads-delete.html)  | Deletes an existing workload\. | Write |   [ workload\* ](#awswell-architectedtool-workload)   |  |  | 
|   [ GetWorkload ](https://docs.aws.amazon.com/wellarchitected/latest/userguide/workload-details.html)  | Retrieves the specified workload\. | Read |   [ workload\* ](#awswell-architectedtool-workload)   |  |  | 
|   [ ListWorkloads ](https://docs.aws.amazon.com/wellarchitected/latest/userguide/workloads-page.html)  | Lists the workloads in this account\. | List |  |  |  | 

## Resources Defined by AWS Well\-Architected Tool<a name="awswell-architectedtool-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awswell-architectedtool-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ workload ](https://docs.aws.amazon.com/wellarchitected/latest/userguide/iam-auth-access.html)  |  arn:$\{Partition\}:wellarchitected:$\{Region\}:$\{Account\}:workload/$\{ResourceId\}  |  | 

## Condition Keys for AWS Well\-Architected Tool<a name="awswell-architectedtool-policy-keys"></a>

Well\-Architected Tool has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.