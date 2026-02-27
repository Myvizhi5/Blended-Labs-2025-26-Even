# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: MYVIZHI S
* **Register Number**: 212224040209_____________________
* **Date of Submission**: 27.02.2026__________________

---

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)

---

## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

---

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

---

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

---

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

---

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

---

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.

---

### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1. ---First, I created a VPC in Amazon Web Services. I gave it a CIDR block of 10.0.0.0/16. This
VPC acts as my private network where all my resources will be created.
Next, I created a public subnet inside the VPC with CIDR 10.0.1.0/24. I enabled auto-assign
public IP so that any instance launched in this subnet will automatically get a public IP
address.
2--After that, I created an Internet Gateway and attached it to my VPC. This allows my VPC to
communicate with the internet.
Then, I created a route table and added a default route (0.0.0.0/0) pointing to the Internet
Gateway. I associated this route table with my public subnet. This step ensures that traffic
from my subnet can reach the internet.
3--Next, I created a security group which acts as a virtual firewall. I allowed inbound traffic for
SSH on port 22 and HTTP on port 80.
4--After completing the network setup, I launched an EC2 instance using Amazon Linux 2 AMI
with instance type t2.micro. I selected my VPC, public subnet, created security group, and
key pair.
5--Finally, I connected to the EC2 instance using SSH and installed the Apache web server. I
started the service and created a simple HTML page. Then I copied the public IP address of
the instance and opened it in a web browser. The webpage was displayed successfully.


---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created
<img width="1912" height="1012" alt="Screenshot 2026-02-27 101200" src="https://github.com/user-attachments/assets/c7e1ed5c-2c12-4bd4-9f04-71e70264b93b" />


---

### Screenshot 2: EBS Volume Attached to EC2

<img width="1919" height="1005" alt="Screenshot 2026-02-27 102340" src="https://github.com/user-attachments/assets/4470de31-da40-4ffb-93d7-936c25c26f30" />


---

### Screenshot 3: Mounted Volume with Data

<img width="1600" height="552" alt="image" src="https://github.com/user-attachments/assets/581190cd-fad2-41c2-84cb-46b976684943" />


---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
