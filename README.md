
# Completed Jav CI project - Jenkins, Nexus, SonarQube, Slack

## Overview
...
### Prerequisites
- JDK 1.8 or later
- Maven 3 or later
- Jenkins, Nexus, SonarQube, Slack

### Completed project status
### Jenkins Status
![preview img](/resultphotos/jenkins.png)

### Jenkins Status
![preview img](/resultphotos/nexus.png)

### Jenkins Status
![preview img](/resultphotos/sonarqube.png)

### Jenkins Status
![preview img](/resultphotos/slack.png)


## Installation and Setup

- To setup Jenkins Server, Nexus and SonarQube servers, Run the scripts in userdata
- To run the pipeline, change the necessary informations in settings.xml,Jenkinsfile and pom.xml

## Workflow:
1. Code Push to GitHub: Pushing code changes to the GitHub repository triggers a webhook notification sent to Jenkins.
2. Jenkins Job Execution: The configured Jenkins job initiates, fetching the latest code from GitHub.
3. Build and Unit Tests: Maven commands are executed within the job to build the Java application and run unit tests.
4. Artifact Upload to Nexus: Upon successful build and tests, the generated JAR file is uploaded to the Nexus repository.
5. Code Quality Analysis: SonarQube scanner analyzes the code, providing metrics and reports on areas like coverage, complexity, potential bugs, and security vulnerabilities.
6. Notifications and Reports: Alert pipeline status to slack

## Contact
chitsanko2522@gmail.com