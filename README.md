AWS High Availability Web Application Project

📌 Project Description

This repository demonstrates a high-availability web application deployment on AWS using core cloud, monitoring, and automation services.

The architecture includes:

* Custom VPC and subnets across multiple Availability Zones
* Two EC2 virtual machines running Nginx with different web pages
* Application Load Balancer distributing traffic between instances
* CloudWatch monitoring, alarms, and dashboard
* SNS email notifications for alerts
* Automated start/stop scheduling using Lambda + EventBridge
* S3 bucket for storing application files

This project shows real-world DevOps concepts such as availability, monitoring, alerting, and cost optimization.

---

🏗️ Architecture Overview

Networking:

* Custom VPC created
* Multiple subnets in different AZs
* Internet connectivity configured

Compute Layer:

* VM-1

  * EC2 instance created
  * Nginx installed
  * Web application deployed

* VM-2

  * EC2 instance created
  * Nginx installed
  * Different web application deployed

Load Balancing:

* Application Load Balancer (ALB)

  * Target group configured
  * Both VMs marked healthy
  * Traffic distributed between instances

Monitoring & Alerts:

* CPU utilization alarms configured
* SNS email notification triggered on alarm
* CloudWatch dashboard created to visualize metrics

Automation:

* Lambda functions created for:

  * Starting instances at 9 AM
  * Stopping instances at 5 PM

* EventBridge schedules trigger Lambda automatically

Storage:

* S3 bucket used to store web application files

---

📷 Screenshots Included in This Repository!!

Infrastructure Creation:

* `VPC-CREATED.png` → VPC creation
* `SUBNETS.png` → Subnets in multiple AZs

EC2 Instances & Web Apps:

* `VM-1-CREATED.png`, `VM-2-CREATED.png` → Instance creation
* `VM-1.png`, `VM-2.png` → Running instances
* `ALB-VM-1.png`, `ALB-VM-2.png` → Web output from both VMs

Load Balancer:

* `TARGET-GROUP.png` → Healthy targets behind ALB

Monitoring:

* `CPU-VM-1.png`, `CPU-VM-2.png` → CPU metrics
* `CPU-LAMBDA.png` → Alarm-triggered automation
* `DASHBOARD-VM'S.png` → CloudWatch dashboard

Notifications:

* `SNS-EMAIL-CPU.png` → Email alert received

Automation Scheduling:

* `START-SCHEDULE.png`, `STOP-SCHEDULE.png` → EventBridge rules
* `9AM-LAMBDA.png`, `5PM-LAMBDA.png` → Lambda execution proof

Storage:

* `S3-BUCKET.png` → Web files stored in S3

---

🚀 Key DevOps Concepts Demonstrated

* High availability using multi-AZ deployment
* Load balancing with Application Load Balancer
* Monitoring and alerting with CloudWatch + SNS
* Infrastructure automation using Lambda & EventBridge
* Cost optimization through scheduled instance shutdown
* Cloud storage integration with S3

---

🧠 Learning Outcome

After completing this project, I gained hands-on experience in:

* Designing production-style AWS architecture
* Implementing monitoring and automated response
* Understanding real DevOps operational workflow
* Managing cloud cost and reliability

---

👨‍💻 Author

Name: Jabaraj V


