# Resilient Call DR System

A resilient cloud architecture built for automated toll-free call failover and cross-region disaster recovery...

![AWS](https://img.shields.io/badge/AWS-cloud-orange)
![DR](https://img.shields.io/badge/Disaster--Recovery-Resilient-blue)
![Status](https://img.shields.io/badge/status-active-brightgreen)

## 🧰 Tech Stack
- AWS EC2
- AWS Lambda
- AWS Route 53
- AWS SNS
- Cloudcraft (for architecture design)

## 📈 Use Case
Designed for telecom or enterprise environments requiring seamless call continuity across regions.

## 🚀 Deployment
This system can be deployed using Infrastructure as Code (IaC) with AWS CloudFormation or Terraform (coming soon).

🔄 How It Works
This resilient call DR system functions as follows:

Route 53 Health Checks continuously monitor service endpoints across AWS regions.

If an issue is detected, Route 53 dynamically redirects traffic to a healthy region.

AWS Lambda is triggered to automate configuration updates or notify operations.

SNS (Simple Notification Service) sends alerts to key stakeholders.

Incoming traffic is handled by EC2 instances behind Load Balancers in multiple Availability Zones.

Traffic automatically shifts between US East, EU West, and Asia Pacific regions to ensure minimal disruption.

Security and identity checks are handled at the entry point before routing begins.


## 🧭 Architecture Diagram
The following Cloudcraft diagram illustrates the architecture of the Resilient Call DR System:
![diagram](architecture/cloudcraft-diagram.png)


























