# BMW Airline Ticket Booking Application
### CI/CD Pipeline using Azure DevOps and Microsoft Azure

## 📌 Project Overview

This project demonstrates how I implemented a **multi-stage CI/CD pipeline using Azure DevOps** for my BMW Airline Ticket Booking Application.

I developed the application using Visual Studio and deployed it to Azure App Service through Azure Cloud. The main goal of this project was to automate the build, testing, and deployment workflow using different pipeline stages and separate Web Apps for each environment.

Through this project, I gained practical experience with Azure DevOps, continuous integration, continuous delivery, and application deployment in the cloud.

## 🎯 Project Objectives

- Implement an automated CI/CD pipeline using Azure DevOps.
- Build and manage the application using Visual Studio.
- Organize the deployment process into multiple stages.
- Deploy the application to separate Azure Web Apps for different environments.
- Understand how applications move from development to production.
- Practice cloud deployment and release management using Microsoft Azure.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Microsoft Azure | Cloud platform |
| Azure DevOps | CI/CD pipeline management |
| Azure Pipelines | Build and deployment automation |
| Visual Studio | Application development |
| Azure App Service | Hosting the web application |
| Git | Source code version control |
| YAML / Pipeline Configuration | Multi-stage pipeline definition, if applicable |

## 🔄 CI/CD Pipeline Architecture

I created a multi-stage pipeline in Azure DevOps with the following stages:

### 1. Build Stage
- Retrieves the application source code from the repository.
- Builds the application using the configured build process.
- Prepares the build artifact for subsequent stages.

### 2. Development Stage
- Deploys the application to a dedicated Development Web App in Azure App Service.
- Provides an environment to verify the initial deployment.
- Helps identify issues before promoting the application to later stages.

### 3. Quality Assurance (QA) Stage
- Deploys the application to a separate QA Web App.
- Provides an environment for testing application functionality and deployment readiness.
- Helps verify that the application is ready for production.

### 4. Production Stage
- Deploys the application to a dedicated Production Web App.
- Makes the application available through its production URL.
- Represents the final stage of the deployment pipeline.

## 🏗️ Pipeline Workflow

```text
       Source Code Repository
                 |
                 v
           Build Stage
                 |
                 v
        Development Stage
        (Development Web App)
                 |
                 v
       Quality Assurance Stage
             (QA Web App)
                 |
                 v
         Production Stage
        (Production Web App)
                 |
                 v
        Live Azure Application
```

Each deployment environment uses a different Azure Web App, helping keep development, testing, and production deployments separate.

## ☁️ Azure Resources

The project uses the following Azure resources:

- **Azure DevOps Project:** Manages the repository and pipeline.
- **Azure Pipeline:** Automates the multi-stage workflow.
- **Development Web App:** Hosts the development deployment.
- **QA Web App:** Hosts the quality assurance deployment.
- **Production Web App:** Hosts the production deployment.

The Web Apps are configured as separate deployment targets for their respective stages.

## 🚀 Key Features

- Multi-stage CI/CD pipeline.
- Automated application build process.
- Environment-specific deployments.
- Separate Azure Web Apps for Development, QA, and Production.
- Cloud-based application hosting with Azure App Service.
- Source code and pipeline management through Azure DevOps.
- Practical implementation of a cloud deployment workflow.

## 📚 What I Learned

While implementing this project, I gained hands-on experience with:

- Configuring multi-stage pipelines in Azure DevOps.
- Building and deploying applications using Visual Studio and Azure.
- Deploying web applications to Azure App Service.
- Managing different deployment environments.
- Understanding CI/CD concepts and release workflows.
- Organizing application deployments from development to production.

## 🔧 How the Pipeline Works

1. Commit or push application changes to the configured source repository.
2. Run the Azure DevOps pipeline according to its trigger configuration.
3. Build the application and generate the required deployment artifact.
4. Deploy the application to the Development Web App.
5. Deploy to the QA Web App for quality verification.
6. Deploy to the Production Web App after the required checks or approvals.

*Note: The actual triggers, testing steps, approvals, and stage dependencies depend on the pipeline configuration.*

## 👨‍💻 About This Project

This project is part of my hands-on learning journey in Microsoft Azure and Azure DevOps. It helped me understand how a multi-stage CI/CD pipeline can be used to deploy a web application across different environments.

I built this project to strengthen my practical knowledge of cloud computing, application deployment, and CI/CD automation.

---

**Project:** BMW Airline Ticket Booking Application  
**Cloud Platform:** Microsoft Azure  
**CI/CD Tool:** Azure DevOps  
**Development Environment:** Visual Studio  
**Hosting Service:** Azure App Service
