# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
Author : MYVIZHI S
Reg no : 212224040209
Date :17.03.2026

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

Describe step-by-step how you performed this experiment in your own words.
## Workflow (Student Explanation)

1. First, I reviewed the **existing EC2 architecture** created in the previous experiment.
2. Then, I created a **Launch Template** by specifying the AMI, instance type, security group, and user data.
3. After that, I created an **Auto Scaling Group** using the launch template and set the minimum, maximum, and desired number of instances.
4. Next, I created an **Application Load Balancer** and configured a **target group** to route traffic to the EC2 instances.
5. I attached the **Auto Scaling Group to the target group** so that the load balancer could distribute traffic to the instances.
6. Then, I configured **scaling policies** based on CPU utilization using **Amazon CloudWatch alarms**.
7. Finally, I tested the setup by generating traffic and observed **load balancing and automatic scaling of instances**.


---

## Output Screenshots 
OUTPUT1:

<img width="1919" height="1138" alt="Screenshot 2026-03-15 142642" src="https://github.com/user-attachments/assets/ae238651-7ebd-48b0-a7d9-a899b4aab3d2" />

OUTPUT 2:
<img width="1919" height="1132" alt="Screenshot 2026-03-15 142925" src="https://github.com/user-attachments/assets/0fe069e9-a36c-442d-a773-ddc09283b243" />

OUTPUT 3:

<img width="1919" height="1128" alt="Screenshot 2026-03-15 151413" src="https://github.com/user-attachments/assets/1390f79e-9a14-467c-949a-86c102077300" />


---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
