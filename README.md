
# Deploy Netflix-Clone on EKS Using Devsecops Pipeline

In this DevSecOps project we will deploy Netflix clone Application as a docker container on Kubernetes cluster through a secure CICD pipeline using Jenkins, the popular CICD tool.
Along with Jenkins we are also use many other popular and demanding devops tool like Docker, Sonarqube, Trivy, Prometheus, Grafana and even Argocd and helm for Kubernetes deployment.








## Steps to create this project

To complete the tasks you mentioned, you can follow this step-by-step guide:

1. **Create an EC2 Instance with Larger RAM and Storage:**

   - Log in to the AWS Management Console.
   - Navigate to the EC2 service.
   - Launch a new EC2 instance and select an instance type with the desired RAM and storage.

2. **Clone the Repository:**

   - SSH into your EC2 instance.
   - Use the `git` command to clone your repository.

3. **Install Docker:**

   - Update the package manager: `sudo yum update`
   - Install Docker: `sudo yum install docker`
   - Start the Docker service: `sudo service docker start`

4. **Create an API Key from TMDB Website:**

   - Go to the TMDB website and create an API key.

5. **Run Docker Images with the API Key:**

   - Use the `docker run` command to run your Docker images with the TMDB API key.

6. **Install SonarQube through Docker Images and Run It:**

   - Pull the SonarQube Docker image: `docker pull sonarqube`
   - Run the SonarQube container: `docker run -d -p 9000:9000 sonarqube`

7. **Install Trivy:**

   - Install Trivy for vulnerability scanning. You can find installation instructions on the Trivy GitHub repository.

8. **Install Jenkins:**

   - Install Jenkins using your package manager or by downloading the Jenkins WAR file.
   - Start Jenkins: `java -jar jenkins.war`

9. **Install Packages in Jenkins:**

   - In the Jenkins web interface, go to "Manage Jenkins" > "Manage Plugins" and install the following plugins:
     1. Eclipse Temurin Installer
     2. SonarQube Scanner
     3. NodeJs Plugin
     4. Email Extension Plugin

10. **Configure SonarQube with Jenkins:**

    - In the Jenkins web interface, go to "Manage Jenkins" > "Configure System" and configure your SonarQube server using the credentials.

11. **Check Whether the Build Is OK:**

    - Create a Jenkins job that builds your project and runs SonarQube analysis.

12. **Install Docker Plugins and OWASP Dependency Checking:**

    - In the Jenkins web interface, go to "Manage Jenkins" > "Manage Plugins" and install the following plugins:
      - OWASP Dependency-Check
      - Docker
      - Docker Commons
      - Docker Pipeline
      - Docker API
      - docker-build-step

13. **Configure Docker with Jenkins:**

    - Add Docker Hub or your Docker repository credentials in Jenkins credentials.

14. **Run a Check to Verify No Errors:**

    - Create a Jenkins job that builds and deploys your Dockerized application.

15. **Create Another Server for Monitoring Tools:**

    - Launch a new EC2 instance or another server for monitoring tools.

16. **Install Prometheus:**

    - SSH into the new server.
    - Download and configure Prometheus.
    - Run Prometheus on port 9090.

17. **Install Node Exporter:**

    - Install Node Exporter on the monitoring server to collect system metrics.

18. **Configure Prometheus and Jenkins Plugin:**

    - Configure Prometheus to scrape Node Exporter metrics.
    - Install Jenkins Prometheus plugin.

19. **Install Grafana:**

    - SSH into the monitoring server.
    - Download and configure Grafana.
    - Run Grafana on port 3000.

20. **Add Data Source and Import Dashboard in Grafana:**

    - In the Grafana web interface, add Prometheus as a data source.
    - Import a suitable dashboard for your application.

21. **Implement Notification Services in Jenkins:**

    - Configure email notifications in your Jenkins jobs.
    - You can use the "Email Extension Plugin" for this purpose.

22. **Create an AWS EKS Cluster and Install Argo CD using Helm:**

    - Set up an AWS EKS cluster.
    - Install Argo CD using Helm on the EKS cluster.

Each step involves a set of specific commands and configurations. Make sure to consult the documentation for each tool and service for detailed instructions on setting up and configuring them properly.

## Feedback

If you have any feedback, please reach out to us at sunilkurthakoti06@gmail.com

