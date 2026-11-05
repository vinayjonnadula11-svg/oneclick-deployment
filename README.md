# Dual Website Deployment using Docker

## Project Overview

This project demonstrates the deployment of two separate web applications using Docker and Nginx.

The first application is a frontend website built using npm, while the second application is a Gradle-based web application packaged as a WAR file.

Both applications are containerized using Docker and served through Nginx, allowing them to run independently and simultaneously.

## Technologies Used

- Git & GitHub
- Jenkins
- npm
- Node.js
- Gradle
- Docker
- Nginx
- Apache Tomcat
- PowerShell

## Project Workflow

```text
                 GitHub Repository
                        |
                      Jenkins
                        |
             +----------+----------+
             |                     |
       Frontend Build         Gradle Build
             |                     |
         npm install          Gradle Build
             |                     |
         npm run build         WAR Package
             |                     |
             +----------+----------+
                        |
                 Docker Images
                        |
             +----------+----------+
             |                     |
       Frontend Container    Gradle Container
             |                     |
           Nginx                 Nginx
             |                     |
             +----------+----------+
                        |
                  Browser Access
```

## Application Deployment

| Application | Build Tool | Deployment |
|---|---|---|
| Frontend Website | npm | Docker + Nginx |
| Gradle Website | Gradle | Docker + Nginx |

Both applications run in separate Docker containers.

## Project File Structure

```text
oneclick-deployment/
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   ├── script.js
│   ├── package.json
│   ├── package-lock.json
│   ├── build.js
│   ├── Dockerfile
│   ├── Dockerfile.gradle
│   ├── Jenkinsfile
│   ├── nginx/
│   └── build/
│       └── libs/
│           └── gradle-tomcat-app.war
│
└── README.md
```

> Note: This is a sample structure. Update it to match the actual files and folders in your GitHub repository.

## Website Screenshots

### Frontend Website — npm + Nginx

Add your frontend website screenshot here.

![Frontend Website Screenshot](images/frontend-website.png)

### Gradle Website — Gradle + Nginx

Add your Gradle website screenshot here.

![Gradle Website Screenshot](images/gradle-website.png)

## Project Objectives

- Deploy multiple websites using Docker containers.
- Build frontend applications using npm.
- Package web applications using Gradle.
- Serve web applications using Nginx.
- Understand Docker image creation and container management.
- Run multiple applications independently on a single machine.
- Understand the CI/CD workflow using Jenkins and GitHub.

## Key Learnings

- Docker image creation and container deployment.
- Multi-application container management.
- npm-based frontend build process.
- Gradle-based application packaging.
- Nginx configuration and web server deployment.
- GitHub repository management.
- Understanding CI/CD pipeline concepts.

## Conclusion

This project provides practical experience in deploying multiple web applications using Docker and Nginx. It demonstrates how frontend and Gradle-based applications can be built, containerized, and deployed independently while following a structured DevOps workflow.
