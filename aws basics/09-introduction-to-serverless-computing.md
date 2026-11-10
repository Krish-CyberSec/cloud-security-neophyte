# Introduction to Serverless Computing


1. # Unmanaged and managed services

    AWS offers both unmanaged and managed services to suit different levels of control and responsibility. By understanding this model, you will know which tasks AWS manages and which you are responsible for, helping you secure and manage your cloud resources effectively.

    1. `Unmanaged and managed services`

        With unmanaged compute services like Amazon EC2, AWS takes care of the underlying physical infrastructure, but you're responsible for setting up, securing, and maintaining the operating system, network configurations, and applications on your instances. Managed services, on the other hand, reduce the amount of infrastructure you need to manage. While AWS handles much of the operational overhead, you might still need to perform some provisioning or configuration depending on the service.


    2. `Fully-managed services`

        Fully-managed services—like serverless ones—take abstraction even further, eliminating the need to provision or manage any servers at all. The underlying infrastructure is fully managed by AWS, so you can focus entirely on writing and deploying code. Later in this module, you will explore Lambda. Lambda is a serverless compute service where AWS handles the infrastructure, scaling, and availability, while you remain responsible for securing and managing your application code.


  <img width="1200" height="700" alt="image" src="https://github.com/user-attachments/assets/4d199a5b-737f-4052-a066-b1a8607b9c67" />

2. # When to use what?


    With **unmanaged services** like Amazon EC2, you set up and manage everything: the operating system, security updates, and network settings. AWS only takes care of the physical hardware. 

    **Managed services** handle most of the infrastructure for you, but you still need to set up things like deployment options, scaling, and environment settings. 

    With **fully managed services** like AWS Lambda, you don’t manage any servers at all. You upload your code, and AWS takes care of the rest, including infrastructure, scaling, and availability.
