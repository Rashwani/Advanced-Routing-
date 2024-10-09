
# Advanced Request Routing and Load Balancing with AWS

This project showcases how to build a robust architecture that handles **Advanced Request Routing** and **Load Balancing** using **Amazon EC2** and **Application Load Balancer (ALB)**. The solution ensures efficient traffic management, high availability, and fault tolerance by dynamically routing requests based on predefined rules.

## Project Overview

In this project, I set up advanced request routing and load balancing using **Application Load Balancer (ALB)** with **Amazon EC2** instances to manage and distribute incoming traffic. This architecture ensures optimized request distribution and high availability by routing traffic based on path, host headers, and more.

This project was developed as part of the **Digital Cloud Training** bootcamp, where I learned how to implement advanced routing policies and load balancing strategies on AWS.

### Key Features
- **Application Load Balancer (ALB)**: Used for routing traffic to different target groups based on request conditions such as path or host header.
- **Path-Based Routing**: Configured ALB rules to route traffic to different EC2 instances based on URL paths.
- **Host-Based Routing**: Set up routing rules that direct traffic based on host headers.
- **Health Checks**: Configured ALB to continuously check the health of EC2 instances to ensure traffic is only routed to healthy targets.
- **Highly Available EC2 Instances**: Deployed EC2 instances across multiple Availability Zones for fault tolerance and high availability.

## Architecture

The solution includes:
1. **Application Load Balancer (ALB)**: Distributes incoming traffic based on advanced routing rules (e.g., path-based or host-based routing).
2. **Amazon EC2 Instances**: Hosts the application in different target groups, ensuring fault tolerance and availability.
3. **ALB Health Checks**: Continuously monitors EC2 instances to ensure traffic is routed only to healthy instances.
4. **Auto Scaling**: Automatically adjusts the number of EC2 instances based on traffic demand, ensuring scalability.

![Architecture Diagram]

## AWS Services Used
- **Application Load Balancer (ALB)**: For advanced request routing and load balancing.
- **Amazon EC2**: Provides compute capacity to host the application.
- **Amazon CloudWatch**: Monitors performance metrics and triggers scaling events.
- **Amazon Route 53**: Configured to route traffic to the ALB with advanced routing policies.
- **AWS Auto Scaling**: Dynamically adjusts the number of EC2 instances based on traffic patterns.

## How to Deploy
1. Clone the repository to your local environment.
2. Deploy EC2 instances across multiple Availability Zones using the provided CloudFormation template.
3. Configure **Application Load Balancer (ALB)** with advanced routing rules for path-based and host-based routing.
4. Set up health checks in ALB to monitor the health of EC2 instances and route traffic accordingly.
5. Test request routing by accessing different paths and hosts and observing the load balancing behavior.

## Lessons Learned
- **Advanced Routing with ALB**: Leveraging ALB for path-based and host-based routing simplifies traffic management for complex applications.
- **Health Checks**: ALB health checks ensure that traffic is only routed to healthy instances, enhancing fault tolerance.
- **Auto Scaling**: Scaling EC2 instances automatically in response to traffic ensures high availability during peak times without manual intervention.

## Next Steps
- Integrate **AWS Lambda** to handle serverless request processing alongside EC2 instances.
- Implement **AWS WAF** for added security and protection against web attacks.
- Explore further routing options like geolocation-based routing for global applications.

## Acknowledgments

This project was completed as part of the **Digital Cloud Training** bootcamp. 

## Conclusion

This project demonstrates how to build a highly available, scalable, and fault-tolerant architecture using **Amazon EC2** and **Application Load Balancer (ALB)**. With advanced request routing and automatic scaling, the solution is equipped to handle complex traffic management for modern applications.

![Screenshot 2024-04-12 183322](https://github.com/user-attachments/assets/9cfea3d4-8007-44da-855b-42812d0eab46)
