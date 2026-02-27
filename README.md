🚀 CI/CD Docker Pipeline with AWS Notifications & Monitoring
📌 Project Overview

This project demonstrates an end-to-end DevOps workflow that automatically builds and deploys a Dockerized application using GitHub Actions, sends real-time deployment notifications via AWS Lambda (SMS), and provides system monitoring using Prometheus and Grafana.

It showcases core cloud engineering skills including CI/CD automation, containerization, serverless integration, and observability.

🌐 Live Demo

👉 Deployed Application:
https://69a1f79bc5f3037eb1b5c513--profound-meringue-98e53d.netlify.app/

You can visit this link to view the running application deployed through the CI/CD workflow.

🧰 Technologies Used

GitHub Actions — CI/CD pipeline automation

Docker — Containerization

Docker Hub — Image registry

AWS API Gateway — HTTP endpoint

AWS Lambda — Serverless compute

Amazon SNS — SMS notifications

Prometheus — Metrics collection

Grafana — Visualization dashboards

🏗️ System Architecture


<img width="1536" height="1024" alt="ChatGPT Image Feb 27, 2026, 11_59_52 PM" src="https://github.com/user-attachments/assets/7e9850b8-05c4-4e72-b5af-125623eebc41" />



Services created via Docker Compose:

🧩 App Container — Static HTML website

📊 Prometheus — Scrapes metrics

📈 Grafana — Displays dashboards

Access locally:

App → http://localhost:8080

Prometheus → http://localhost:9090

Grafana → http://localhost:3000

⚙️ CI/CD Pipeline Architecture
🔹 Automated Deployment Flow
GitHub Push (main branch)
        │
        ▼
GitHub Actions Pipeline
        │
        ├── Checkout repository
        ├── Docker build
        ├── Push image to Docker Hub
        │
        ▼
Deployment Notification
(API Gateway → Lambda → SNS → SMS)
☁️ AWS Serverless Notification Architecture
GitHub Actions
      │
      ▼
API Gateway (HTTP Endpoint)
      │
      ▼
AWS Lambda Function
      │
      ▼
Amazon SNS
      │
      ▼
SMS Notification to User

This ensures real-time alerts after each deployment.

🧪 How the Pipeline Works

Code is pushed to the main branch

GitHub Actions workflow triggers automatically

Docker image is built from the repository

Image is pushed to Docker Hub

Monitoring stack is deployed

AWS Lambda is invoked via API Gateway

SMS notification is sent via SNS

📊 Monitoring Setup

<img width="758" height="350" alt="Screenshot 2026-02-28 000358" src="https://github.com/user-attachments/assets/d576e6d7-6fd3-47c4-9429-9c969f064c96" />


🔔 Features

✔ Automated CI/CD pipeline
✔ Containerized application
✔ Serverless deployment notifications
✔ Real-time SMS alerts
✔ Monitoring with Prometheus & Grafana
✔ Production-style architecture

🎯 Use Cases

DevOps pipeline demonstrations

Cloud engineering portfolio project

Monitoring & observability learning

Serverless integration example

📚 Future Enhancements

Deploy to AWS EC2/ECS

Add alerting rules in Grafana

Monitor container resource usage

Integrate email/Slack notifications

Use AWS ECR instead of Docker Hub

👨‍💻 Author

Waleed Ahmed
BCA Student | Aspiring Cloud & DevOps Engineer

⭐ Key Learning Outcomes

This project demonstrates:

CI/CD automation

Docker workflows

Serverless architecture

Cloud monitoring fundamentals

Real-world DevOps practices

💡 Built as part of hands-on cloud engineering practice.
