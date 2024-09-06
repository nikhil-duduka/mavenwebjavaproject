Maven Java Web Project - Jenkins CI/CD Pipelines
Overview
This project demonstrates a Maven-based Java web application integrated with Jenkins for Continuous Integration (CI) and Continuous Deployment (CD). The project is structured into three distinct Jenkins pipelines that automate the build, test, and deployment stages, ensuring a streamlined and efficient software development lifecycle.

Pipeline Structure
Build Pipeline:

Purpose: Automates the compilation and packaging of the Java web application.
Steps:
Jenkins triggers the pipeline upon code commit.
Maven is used to clean, compile, and package the application into a deployable artifact (e.g., WAR or JAR file).
The build artifact is archived for further stages.
Test Pipeline:

Purpose: Ensures code quality and functionality through automated testing.
Steps:
Executes unit tests using JUnit and integration tests as part of the Maven test phase.
Generates test reports, which are automatically published and made accessible in Jenkins.
Fails the pipeline if any test fails, preventing the deployment of faulty code.
Deploy Pipeline:

Purpose: Automates the deployment of the built artifact to a staging or production environment.
Steps:
Deploys the artifact to a web server (e.g., Apache Tomcat) or a cloud-based environment.
Notifies stakeholders upon successful deployment.
Optionally, includes steps for post-deployment smoke tests to verify that the application is running correctly.
