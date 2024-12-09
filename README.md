# AWS_Terraform_Project

🌟 My First DevOps Project: Terraform on AWS 🚀
Welcome to my Terraform project! This repository showcases how I deployed a scalable and secure infrastructure on AWS using Infrastructure as Code (IaC) principles.

🗺️ Project Overview
This project demonstrates the deployment of a high-availability web application setup using Terraform. Here's what it includes:

Custom VPC: A virtual private cloud with public subnets in different availability zones.
Secure Networking: Configured Internet Gateway, Route Tables, and a Security Group for safe and efficient communication.
Web Servers: Two EC2 instances running web applications with automated configuration.
Load Balancing: An Application Load Balancer (ALB) for seamless traffic distribution.
Scalable Storage: An S3 bucket for potential data storage needs.
⚙️ Architecture
Here’s a high-level breakdown of the infrastructure:

1️⃣ VPC

CIDR Block: Defined using variables.
Two public subnets for high availability.
2️⃣ Internet Access

Internet Gateway for outbound access.
Route Table with a default route pointing to the gateway.
3️⃣ Security

Security Group allowing HTTP (80) and SSH (22) traffic.
4️⃣ Compute Instances

Two EC2 instances in separate subnets.
User-data scripts automate application setup.
5️⃣ Load Balancer

Application Load Balancer to distribute traffic evenly.
Health checks ensure reliability.
6️⃣ Outputs

ALB DNS name for direct access to the deployed application.

🛠️ Getting Started
Follow these steps to replicate or experiment with this project:

### Prerequisites
- Terraform installed on your system.
- AWS account with proper IAM permissions.
- Basic knowledge of Terraform and AWS.

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>

2.Initialise the Terraform and Apply the config!

📂 File Structure
  main.tf: Core infrastructure definition.
  provider.tf: AWS provider configuration.
  terraform.tfstate: Tracks the state of the deployed resources.
  userdata.sh & userdata1.sh: Scripts for configuring the web servers.

🌐 Output
After deployment, Terraform will provide the DNS of the Application Load Balancer, which you can use to access the web application.

🎯 Key Learnings
  Implementing a scalable cloud infrastructure using Terraform.
  Configuring AWS resources for high availability and fault tolerance.
  Automating web server deployment with user data scripts.
  Integrating an ALB to manage traffic efficiently.
  
🤝 Contributions and Feedback
If you have suggestions, feedback, or ideas to improve this project, feel free to open an issue or submit a pull request. Let’s collaborate!

🚀 Future Enhancements
  Add auto-scaling for EC2 instances.
  Implement monitoring and alerting using CloudWatch.
  Integrate a CI/CD pipeline for seamless updates.
  
📢 Let’s Connect!
If you found this project interesting or have any questions, let’s connect on LinkedIn or GitHub.

