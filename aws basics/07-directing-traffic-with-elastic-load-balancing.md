# Directing Traffic with Elastic Load Balancing

1. # Elastic Load Balancing

    Elastic Load Balancing (ELB) automatically distributes incoming application traffic across multiple resources, such as EC2 instances, to optimize performance and reliability. A load balancer serves as the single point of contact for all incoming web traffic to an Auto Scaling group. As the number of EC2 instances fluctuates in response to traffic demands, incoming requests are first directed to the load balancer. From there, the traffic is distributed evenly across the available instances.

    Although ELB and Amazon EC2 Auto Scaling are distinct services, they work in tandem to enhance application performance and ensure high availability. Together, they enable applications running on Amazon EC2 to scale effectively while maintaining consistent performance.

2. # ELB benefits

    1. `Efficent Traffic distribution` 

        ELB evenly distributes traffic across EC2 instances, preventing overload on any single instance and optimizing resource utilization.

    2. `Automatic Scaling`

        ELB scales with traffic and automatically adjusts to changes in demand for a seamless operation as backend instances are added or removed.

    3. `Simplified Management`

        ELB decouples front-end and backend tiers and reduces manual synchronization. It also handles maintenance, updates, and failover to ease operational overhead.

3. # Routing methods

    To optimize traffic distribution, ELB uses several routing methods: Round Robin, Least Connections, IP Hash, and Least Response Time. These routing strategies work together for efficient traffic management and optimal application performance.

    1. `Round Robin`

        Distributes traffic evenly across all available servers in a cyclic manner.

    2. `Least Connections`

        Routes traffic to the server with the fewest active connections, maintaining a balanced load.

    3. `IP Hash`

        Uses the client’s IP address to consistently route traffic to the same server.
    
    4. `Least Response Time`

        Directs traffic to the server with the fastest response time, minimizing latency.

    
