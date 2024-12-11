# Automatic-Create-Service-Connection

This repository contains the step-by-step guide to automatically create a service connection using Azure Pipelines.

## Documentation Used

1. [Create a service endpoint / Service connection using az DevOps](https://learn.microsoft.com/en-us/rest/api/azure/devops/serviceendpoint/endpoints/create?view=azure-devops-rest-7.1&tabs=HTTP)
2. [Get the project ID](https://learn.microsoft.com/en-us/rest/api/azure/devops/core/projects/list?view=azure-devops-rest-7.1&tabs=HTTP)
3. [Authenticate with Azure DevOps](https://learn.microsoft.com/en-us/azure/devops/cli/azure-devops-cli-in-yaml?view=azure-devops&tabs=bash#authenticate-with-azure-devops)
4. [Create a variable group](https://learn.microsoft.com/en-us/rest/api/azure/devops/distributedtask/variablegroups/add?view=azure-devops-rest-6.0#request-body)

## Steps to Automatically Create a Service Connection Using Azure DevOps Pipelines

1. Go to **Project settings** > **Service Connections** > **Security** and add the **"Project Build Service (Your_Organization)"** as an administrator. If not, you will encounter an issue like the following:
   ![image](https://github.com/user-attachments/assets/c7a616c8-c6d9-4306-8ad7-0222ca89bb83)

2. Use the YAML pipeline attached in the repository as a guide on how to create the pipeline to automatic create a service connection and variable group.
