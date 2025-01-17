# Cloud Monitoring and Load Balancing with AWS
## Overview
This project demonstrates how to set up cloud monitoring and load balancing for applications hosted on AWS. It involves launching EC2 instances, configuring an Application Load Balancer (ALB), and setting up CloudWatch alarms to monitor CPU utilization.



## Steps Included

### 1. Launching EC2 Instances
- Created two EC2 instances:
  - One for the `/api` path.
  - One for the `/app` path.
- Configured the instances using Amazon Linux 2 or Ubuntu AMI.
- Set up a security group to allow HTTP traffic (Port 80).

### 2. Setting Up Target Groups
- Configured target groups to manage traffic between instances.
- Ensured both instances were in the same VPC and subnet.

### 3. Configuring CloudWatch Alarms
- Set up an alarm to monitor CPU utilization:
  - Triggered if usage exceeds 80% for 5 consecutive minutes.
- Used an SNS topic to send alerts via email.



## Tools Used
- **AWS EC2**: For launching instances.
- **AWS CloudWatch**: For monitoring metrics and setting alarms.
- **AWS ALB**: For distributing traffic between instances.


## Instructions to Run
1. **Launch EC2 Instances**:
   - Follow the instructions in the `Launch EC2 Instances` section.
2. **Set Up Target Groups**:
   - Ensure both instances are correctly associated with the ALB.
3. **Create CloudWatch Alarm**:
   - Set up the alarm as described to monitor CPU usage.
![image](https://github.com/user-attachments/assets/ea3eb44d-616e-4637-82dc-4429665052f3)
