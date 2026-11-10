# Containers and Orchestration on AWS

1. # Containers and VMs

    A container packages your application with everything it needs to run, so it works the same on any computer. This helps to move, update, and manage. Containers are faster and lighter than virtual machines (VMs) because they share the host computer’s operating system. VMs use a hypervisor to run full, separate operating systems, which makes them less resource-efficient and have longer startup times.

2. # Deployment consistency with containers

    When a developer’s environment differs from staging or production, deployments can fail and become difficult to debug. Containers solve this by keeping the application’s environment consistent everywhere, making deployments smoother and assisting troubleshooting.

3. # Scaling containers with orchestration

    As containerized applications scale, managing them becomes more complex. A setup that began with a few containers on a single host can quickly grow into hundreds or thousands of containers across multiple hosts. At that scale, manually handling container lifecycle, monitoring, and general operations becomes unsustainable. This is where orchestration tools come in. They automate deployment, scaling, and management to keep everything running smoothly.4

4. # AWS container services

    AWS has a set of tools for managing containers that fits into three categories: orchestration, registry, and compute.

    1. `Amazon ECS`

        Amazon Elastic Container Service (Amazon ECS) is a scalable container orchestration service for running and managing containers on AWS, like Docker containers. Docker is a software platform for building, testing, and deploying applications quickly.

        1. `Amazon ECS launch types`

            - **Amazon ECS with Amazon EC2** is ideal for small-to-medium businesses that need full control over infrastructure. Suitable for custom applications requiring specific hardware or networking configurations, with the flexibility of Amazon EC2 and the simplicity of Amazon ECS.

            - **Amazon ECS with AWS Fargate** is perfect for startups or small teams building web applications with variable traffic. It's a serverless option—no server management required—so teams can focus on development while Amazon ECS handles scaling and orchestration.

    2. `Amazon EKS`

        Amazon Elastic Kubernetes Service (Amazon EKS) is a fully managed service for running Kubernetes on AWS. It simplifies deploying, managing, and scaling containerized applications using open-source Kubernetes, with ongoing support and updates from the broader community.


        1. `Amazon EKS launch types`


            - **Amazon EKS with Amazon EC2:** This is best for enterprises needing full control over infrastructure. It offers deep customization of EC2 instances alongside Kubernetes scalability—ideal for complex, large-scale workloads.

            - **Amazon EKS with AWS Fargate:** This is great for teams wanting Kubernetes flexibility without managing servers. It combines Kubernetes power with serverless simplicity, helping to scale applications quickly across various use cases.

5. # Amazon ECR

    Amazon Elastic Container Registry (Amazon ECR) is where you can store, manage, and deploy container images. It supports container images that follow the Open Container Initiative (OCI) standards. You can push, pull, and manage images in your Amazon ECR repositories using standard container tooling and command line interfaces (CLIs).


6. # Fargate


    AWS Fargate is a serverless compute engine for containers. It works with both Amazon ECS and Amazon EKS. Fargate is a container hosting platform, unlike Amazon ECS and Amazon EKS, which are both container orchestration services.

    When using Fargate, you do not need to provision or manage servers. Fargate manages your server infrastructure for you. You can focus more on innovating and developing your applications, and you pay only for the resources that are required to run your containers.


7. # When to use what?


    **Amazon ECS** is a scalable service for orchestrating containers on AWS, whereas **Amazon EKS** helps simplify **Kubernetes** deployment. **Amazon ECR** stores and manages OCI-compliant container images, integrating with **Amazon ECS**, **Amazon EKS**, and **Fargate**. **Fargate** is a serverless compute engine for containers, removing the need to manage infrastructure and working with **Amazon ECS** and **Amazon EKS**.


