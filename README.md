## Spring Boot Application Containerization Using Reusable Workflow with Caching

## springbootapp-aws-devops
Spring Boot microservices application with with devops in AWS


### Problem Statement and Motivation
Yoda Insurance is a leading global insurance provider based in the U.S. The company offers products and services like home insurance, health insurance, car insurance, and life insurance. Currently, the company uses a monolithic application architecture, but it started facing 
difficulties in managing application deployments with the organization's growth.Seeing these challenges, the company decided to transition from its monolithic application architecture to a microservice application architecture. They also planned to implement DevOps CI/CD and other necessary automation. Yoda Insurance has chosen AWS as its primary cloud provider for servers, databases, and application deployments.

### Objectives:
To transition a company’s application architecture from monolithic to microservice, implement DevOps CI/CD, and leverage AWS for efficient application deployments, server management, and database hosting.

### Expected Task(s)

1. Create a code repository in CodeCommit to store microservice source code
2. Commit the Spring Boot microservice source code to the CodeCommit repository
3. Set up a CodePipeline to add a checkout stage that pulls code from the CodeCommit repository
4. Integrate CodeBuild into the CodePipeline as the build stage to execute a Maven build and generate a JAR artifact
5. Add Docker build steps to the CodeBuild project and then publish the Docker image to the Docker registry.
6. Store the deployment YAML file in a GitHub repository with container configurations
7. Store the service YAML file with a Load Balancer type to secure an  external endpoint for the microservice
8. Establish a CodeBuild project for deployment to the EKS Cluster
9. Configure the kubectl command to execute the YAML manifest files on the EKS Cluster
