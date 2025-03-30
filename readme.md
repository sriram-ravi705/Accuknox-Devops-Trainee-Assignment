# Accuknox-Devops-Trainee-Assignment

---

##  Problem Statement 1: 

### Wisecow Application on Kubernetes

This project involves containerizing the Wisecow application and deploying it on a Kubernetes cluster, ensuring secure TLS communication and automating the CI/CD pipeline.

Repository link: [Wisecow Kubernetes Deployment Repository](https://github.com/sriram-ravi705/wisecow-app).

### Key Features:
- **Dockerization:** Created a Dockerfile to build and containerize the Wisecow application.
- **Kubernetes Deployment:** Deployed the application to AWS EKS with Kubernetes.
- **TLS Encryption:** Ensured secure communication using TLS certificates.
- **CI/CD Pipeline:** Automated build and deployment using GitHub Actions.

### Key Components:
1. **Dockerfile:** Builds the container image with dependencies (fortune-mod, cowsay).
2. **Kubernetes Deployment & Service:** Deployed the application and exposed it within the Kubernetes cluster.
3. **Ingress Setup:** Configured NGINX Ingress for routing external traffic to the application.
4. **CI/CD Pipeline:** GitHub Actions automatically build and push Docker images, update Kubernetes deployments, and notify via email.

---

## Problem Statement 2:

### objectives 1: Automated Backup Solution

This script automates periodic backups of a specified directory to an AWS S3 bucket, compresses the directory, and sends an email notification about the backup status.

Repository link: [Automated Backup Solution Repository](http://github.com/sriram-ravi705/Bash-Script/tree/main/Automated%20Backup%20Solution).

### Features:
- **Automatic Backups:** Schedules regular backups using `cron`.
- **Compression:** Uses `zip` to compress the backup directory.
- **Cloud Upload:** Uploads the backup to an AWS S3 bucket.
- **Status Email:** Sends a status report using `curl` to a configured email service (e.g., Mailgun, SendGrid).

### Requirements:
- **AWS CLI:** Configured with the necessary credentials.
- **cron:** For scheduling the backup task.
- **curltab:** For sending email notifications.

---

### objectives 2: Log File Analyzer

This script analyzes Nginx web server logs and generates a detailed report about key metrics, including the top IP addresses, response codes, paths, methods, and user agents.

Repository link: [Log File Analyzer Repository](https://github.com/sriram-ravi705/Bash-Script/tree/main/Log%20File%20Analyzer).

### Features:
- **Log Analysis:** Extracts meaningful insights from Nginx logs.
- **Key Metrics:** Identifies top IPs, response codes, requested paths, methods, and user agents.
- **Report Generation:** Uses `goaccess` for an interactive, detailed log report.
- **Email Report:** Sends the generated report via email using `curl`.
- **Automation:** Scheduled using `cron` for regular log analysis.

### Requirements:
- **Nginx Logs:** Must be accessible in the standard log file location.
- **goaccess:** For generating log reports.
- **curl:** For sending the report via email.
- **crontab:** For automating the log analysis task.

---
