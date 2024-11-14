# Azure CI/CD Project with GitHub Actions

This project demonstrates a beginner-level CI/CD pipeline using **GitHub Actions** to deploy a web application to **Azure App Service**. The pipeline automates the deployment process, enabling continuous integration and continuous delivery (CI/CD) every time there’s a new commit to the `main` branch.

## Project Overview

### Objectives
- Set up a CI/CD pipeline to automatically deploy code changes to Azure App Service.
- Securely authenticate GitHub Actions with Azure using a Service Principal.
- Document each step with screenshots and descriptions for clarity.

---

## Steps and Screenshots

### 1. Configure Azure App Service
This screenshot shows the Azure App Service configuration for the CI/CD project, set with Node.js 20 LTS, Linux OS, and region selection.

![App Service Configuration](https://github.com/user-attachments/assets/7f7edfe9-db38-4558-a0c6-56e9fbfd7e42)

---

### 2. Generate Service Principal for Authentication
This screenshot shows the Service Principal credentials generated for GitHub Actions deployment. These credentials enable secure authentication with Azure, allowing automated deployments.

![GitHub Secret Creation](https://github.com/user-attachments/assets/0daa647b-fe1e-484e-842c-206c4e5400ec)

---

### 3. Add Service Principal to GitHub Secrets
This screenshot shows the Service Principal JSON added as a GitHub secret named `AZURE_CREDENTIALS`. This secret is used by GitHub Actions to authenticate with Azure securely.

![Service Principal Creation](https://github.com/user-attachments/assets/914502dc-04f3-4f77-ba5c-b91ddd01e2d1)
---

### 4. GitHub Actions Workflow Configuration
This screenshot shows the GitHub Actions workflow setup. The workflow is triggered on every push to the `main` branch, logging into Azure and deploying the latest code to Azure App Service.

![image](https://github.com/user-attachments/assets/5f86332b-23b4-4f46-a05a-eb9ed7599f31)

---

### 5. GitHub Actions Workflow Execution
This screenshot displays the successful execution of the GitHub Actions workflow. The pipeline checks out the code, authenticates with Azure, and deploys the application to Azure App Service, completing the CI/CD process.

![Workflow Execution](https://github.com/user-attachments/assets/bb1fcbad-bac6-417c-9b44-50f98d2dd115)

---

## Key Takeaways

1. **Automated Deployment**: GitHub Actions enables continuous delivery by automatically deploying changes to Azure App Service with each push to the `main` branch.
2. **Secure Authentication**: The use of a Service Principal ensures secure, role-based access to Azure resources from GitHub.
3. **Documentation and Monitoring**: Screenshots and workflow status logs provide visibility into each stage of the CI/CD pipeline, useful for troubleshooting and auditing.

---

This project demonstrates how to automate and streamline deployments to Azure using GitHub Actions, making it an excellent foundation for beginner-level CI/CD projects.
