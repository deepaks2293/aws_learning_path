EC2 instance roles are a way to grant an AWS EC2 instance permissions to access other AWS resources, without requiring the use of access keys. Instance roles are associated with an IAM role, which specifies the permissions that are granted to the instance. EC2 instances can assume the role associated with their instance profile and access AWS services and resources that the role has permissions to access. This simplifies the process of granting permissions to instances and enhances security by reducing the need to embed credentials within an instance.


STEPS:

    Create an IAM role in the IAM console and define the necessary permissions for the resources you want to access.
    Launch an EC2 instance and specify the IAM role to be used by the instance.
    Connect to the instance and verify that it has the correct permissions to access the resources.

Here are more detailed steps for each of these:

    Create an IAM role:
        Open the IAM console and click "Roles" in the left navigation pane.
        Click "Create role" and select "EC2" as the AWS service that will use the role.
        Choose the permissions policy/policies that you want to assign to the role. You can use an existing policy or create a custom policy.
        Give the role a name and create it.
    Assign the IAM role to an EC2 instance:
        Launch an EC2 instance as you normally would.
        In the "Configure Instance Details" section, expand the "Advanced Details" tab and select the IAM role you just created in the "IAM role" dropdown list.
        Complete the remaining steps to launch the instance.
    Verify that the instance has the correct permissions:
        Connect to the instance using SSH or RDP.
        Run commands to access the resources that you have granted permissions to the IAM role, such as AWS CLI commands or SDK calls.
        If the commands complete successfully, the instance has the correct permissions. If they fail, check the IAM role and the permissions assigned to it.



