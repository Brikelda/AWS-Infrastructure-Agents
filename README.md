# AWS-Infrastructure-Agents
AWS Cloud Infrastructure integrating Java Agents
This was a Lab Report for the Network Programming and Distributed Systems Course. The Project Overview is as follows:
Simulating an agents’ attack (using Java) towards a TCP Server on AWS with initial aim to overload it 
and then extending the cloud architecture to efficiently and effectively control the load. The Java agents and TCP Server 
were implemented into separate EC2 Instances, which were integrated with CloudWatch. The architecture was later 
extended by adding a Network Load Balancer and Auto Scaling.
Key Insights:
• A large number of agents that open TCP Sockets with specific ticker interval were created in an EC2 instance and 
attack a TCP Server in another EC2 instance, overloading it.
• The CPU Utilization from CloudWatch increases, so the server cannot do the defined tasks.
• To solve this, a Network Load Balancer and Auto Scaling were integrated in the system.
• With Auto Scaling, a new EC2 instance (TCP Server) is added as the CPU Utilization exceeds the threshold.
• The Load Balancer distributes the load of agents evenly to the EC2 instances.
• This improved the performance and cost-efficiency
