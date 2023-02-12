    Go to the AWS Management Console and navigate to the EC2 dashboard.
    Click on the "Security Groups" option in the navigation pane.
    Click on the "Create Security Group" button to create a new security group.
    Give your security group a name and a description.
    Choose the VPC that the security group will be associated with.
    Add inbound and outbound rules to the security group. Inbound rules control the traffic that is allowed to come into the instances associated with the security group, while outbound rules control the traffic that is allowed to leave the instances.
    Review the rules and click on the "Create" button to create the security group.

Once the security group is created, you can associate it with instances in the same VPC. You can do this by selecting the instances, choosing the "Actions" button, and then selecting the "Networking" option. From there, you can add the security group to the instance.

It is important to note that security groups are stateful, meaning that any outbound traffic that is allowed is automatically allowed to come back in. This simplifies the configuration of security groups, as you only need to configure inbound rules. It is also important to follow best practices when configuring security groups to ensure that your instances are properly protected.
