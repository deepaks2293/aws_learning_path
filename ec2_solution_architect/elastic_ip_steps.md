    Log in to the AWS Management Console and go to the EC2 dashboard.

    From the EC2 dashboard, select "Elastic IPs" from the sidebar.

    Click on the "Allocate new address" button to allocate a new Elastic IP.

    Once you have allocated an Elastic IP, select it from the list of available addresses and click the "Actions" button.

    From the drop-down menu, select "Associate IP address" and choose the EC2 instance you want to associate with the Elastic IP.

    Click the "Associate" button to complete the process.

Once the Elastic IP is associated with the EC2 instance, you can use it to access your application or service running on the instance using a static IP address that remains the same even if the instance is stopped or started.

It's important to note that AWS charges for unused Elastic IP addresses, so it's a good practice to release any Elastic IPs that are no longer in use to avoid unnecessary charges. You can release an Elastic IP by selecting it from the Elastic IPs list and clicking the "Release addresses" button.
