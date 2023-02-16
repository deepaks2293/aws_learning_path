An Elastic IP (EIP) is a static, public IPv4 address that you can allocate to your AWS account. Unlike the dynamic public IP address that is assigned to an EC2 instance by default, EIPs can be easily reassigned between instances and are not released until you explicitly release them.

EIPs are commonly used in scenarios where you need a persistent IP address for your application, such as when you're running a web server or a database server. By using an EIP, you can avoid having to update DNS records every time you stop and start your instance or replace it with a new one.

To allocate an EIP, you first need to go to the EC2 dashboard in the AWS Management Console and select "Elastic IPs" from the sidebar. From there, you can click the "Allocate new address" button to get a new EIP. Once you have an EIP, you can associate it with an EC2 instance by selecting the instance and clicking the "Associate IP address" button.

One important thing to keep in mind is that AWS charges for EIPs that are not associated with a running instance. Therefore, you should release any EIPs that you're not currently using to avoid unnecessary charges.

In summary, Elastic IP is a useful feature in AWS that provides a static public IP address that can be easily reassigned between instances, making it a convenient solution for scenarios where a persistent IP address is needed.
