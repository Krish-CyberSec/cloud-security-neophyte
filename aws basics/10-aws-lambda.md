# AWS Lambda

1. # Lambda

    Lambda is a serverless compute service that runs code in response to events without the need to provision or manage servers. It automatically manages the underlying infrastructure, scaling resources based on the volume of requests. You are charged only for the compute time consumed, down to the millisecond. Lambda handles execution, scaling, and resource allocation. You can optimize performance by configuring the appropriate memory size for your function.

2. # How Lambda works

    1. `Upload code to Lambda`


        First, upload the code to Lambda, which uploads as a Lambda function.

    2. `Set code to trigger from an event source`

        Next, configure your code to be triggered by events, like AWS services, mobile apps, or HTTP requests.

    3. `Run code when triggered`

        Your code runs only when an event occurs, like a file upload or user action. Lambda automatically handles all the server management, scaling, and infrastructure. The Lambda runtime executes your function code using the event data passed to it. This way, your code runs reliably, securely, and efficiently—without you managing the servers or environment it runs in.

    4. `Pay only for the compute time used`

        You are charged only for the compute time consumed, down to the millisecond. The price depends on the amount of memory that you allocate to your function.

3. # Lambda use cases

    Lambda is ideal for building responsive, event-driven applications across a wide range of industries. Here are three real-world examples that show how Lambda helps companies scale efficiently, reduce operational overhead, and only pay for what they use.

    