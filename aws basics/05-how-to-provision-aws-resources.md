# How to Provision AWS Resources


1. # Interacting with AWS services

    All interactions with services are powered by APIs. You can access these APIs through three primary methods: the AWS Management Console, the AWS CLI, or the AWS SDK. Let's review these methods.

    1. `AWS Management Console`

        The AWS Management Console is a web interface for managing AWS services, offering quick access to services, search functionality, and simplified workflows. With the mobile app, you monitor resources, view alarms, and check billing, supporting multiple logged-in identities at once.


        **Good for**: Users who prefer a visual, easy-to-use interface for managing and configuring AWS services
    
    2. `AWS CLI`

        With the AWS CLI, you manage multiple AWS services directly from the command line across Windows, macOS, and Linux. You can automate tasks through scripts, such as launching EC2 instances.



        **Good for**: Advanced users and developers who need to automate tasks, script actions, and manage AWS resources efficiently from the command line
    
    3. `AWS SDK`
        
        The AWS SDK simplifies integrating AWS services into your applications by providing APIs for various programming languages. AWS offers documentation and sample code for languages like C++, Java, and .NET to help you get started.

        **Good for**: Developers looking to integrate AWS services into their applications using language-specific APIs


2. # Compute and shared responsibility

    <img width="1200" height="700" alt="image" src="https://github.com/user-attachments/assets/e260d1b5-ac54-4923-b4d4-64184c7d8b16" />


    The AWS Shared Responsibility Model outlines the division of duties between the customer and AWS. AWS handles the security of the cloud (hardware and infrastructure), whereas the customer is responsible for security in the cloud (applications, data, and access control).

    An unmanaged service like Amazon EC2 requires you to perform all of the necessary security configuration and management tasks. When you deploy an EC2 instance, you are responsible for configuring security, managing the guest operating system (OS), applying updates, and setting up firewalls (security groups). You will learn more about managed and unmanaged services later.


