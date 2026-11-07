# Scaling Amazon EC2

1. # Scalability
   
   Scalability refers to the ability of a system to handle an increased load by adding resources. You can scale up by adding more power to existing machines, or you can scale out by adding more machines. Scalability focuses on long-term capacity planning to make sure that the system can grow and accommodate more users or workloads as needed.

2. # Elasticity

   Elasticity is the ability to automatically scale resources up or down in response to real-time demand. A system can then rapidly adjust its resources, scaling out during periods of high demand and scaling in when the demand decreases. Elasticity provides cost efficiency and optimal resource usage at any given moment.

3. # Amazon EC2 Auto Scaling
   
   Amazon EC2 Auto Scaling automatically adjusts the number of EC2 instances based on changes in application demand, providing better availability. It offers two approaches. Dynamic scaling adjusts in real time to fluctuations in demand. Predictive scaling preemptively schedules the right number of instances based on anticipated demand.

            - ex :
            With EC2 Auto Scaling, you maintain the desired amount of compute capacity for your application by dynamically adjusting the number of EC2 instances based on demand. You can create Auto Scaling groups, which are collections of EC2 instances that can scale in or out to meet your application’s needs.


    1. `Minimum Capacity`

        The minimum capacity defines the least number of EC2 instances required to keep the application running. This makes sure that the system never scales below this threshold. It's the number of EC2 instances that launch immediately after you have created the Auto Scaling group. 

    2. `Desired Capacity`

        The desired capacity is the ideal number of instances needed to handle the current workload, which Auto Scaling aims to maintain. If you do not specify the desired number of EC2 instances in an Auto Scaling group, the desired capacity defaults to your minimum capacity.

    3. `Maximum Capacity`

        The maximum capacity sets an upper limit on the number of instances that can be launched, preventing over-scaling and controlling costs. For example, you might configure the Auto Scaling group to scale out in response to increased demand.

        In this example, a maximum of 12 EC2 instances can be launched. Amazon EC2 Auto Scaling will scale between the minimum and maximum number of instances.

    


