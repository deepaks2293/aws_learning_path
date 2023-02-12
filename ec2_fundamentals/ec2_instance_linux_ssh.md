First, ensure that you have the appropriate permissions to access the EC2 instance via SSH. This can be done by verifying that your security group has an inbound rule allowing SSH access from your IP address.

Locate the public IP address or DNS hostname of the EC2 instance you wish to connect to.

Open a terminal window on your local machine and use the SSH command to connect to the EC2 instance. The syntax for the SSH command is as follows:

ssh -i <path-to-ssh-key> <username>@<public-ip-or-dns-hostname>


    Replace <path-to-ssh-key> with the file path to your SSH private key, <username> with the username for the EC2 instance (e.g. "ubuntu" for Ubuntu-based AMIs), and <public-ip-or-dns-hostname> with the public IP address or DNS hostname of the EC2 instance.

    If this is the first time you are connecting to the instance, you may receive a prompt to add the EC2 instance's public key to your list of known hosts. Type "yes" to continue.

    You should now be connected to the EC2 instance via SSH and can execute commands as needed.

Here is a diagram to help illustrate the process:

   +---------------------------------------+
   |           Local machine               |
   +---------------------------------------+
                    |
                    |
                    |
             +-------------+
             |  Internet   |
             +-------------+
                    |
                    |
                    |
   +---------------------------------------+
   |           EC2 instance                |
   +---------------------------------------+


In summary, to SSH into an EC2 instance using Linux, you need to have the appropriate permissions, know the public IP address or DNS hostname of the instance, use the SSH command with the correct syntax, and accept the public key the first time you connect.


===============================================================================

Permissions 0644 for 'ec2_key_pair.pem' are too open

The error message "Permissions 0644 for 'ec2_key_pair.pem' are too open" typically occurs when the permissions on the private key file used to connect to an EC2 instance via SSH are set to be too permissive.

In order to fix this error, you need to change the permissions on the private key file to be more restrictive. The recommended permission for a private key file is 400, which means that only the owner of the file has read and write permissions, and no other users or groups have any permissions at all.

You can change the permission on the private key file using the following command in the terminal:

chmod 400 /path/to/ec2_key_pair.pem


Make sure to replace "/path/to/ec2_key_pair.pem" with the actual path to your private key file. Once you have changed the permission on the private key file, you should be able to connect to your EC2 instance via SSH without encountering the "Permissions 0644 for 'ec2_key_pair.pem' are too open" error.
