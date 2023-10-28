
# Deploy Netflix-Clone on EKS Using Devsecops Pipeline

In this DevSecOps project we will deploy Netflix clone Application as a docker container on Kubernetes cluster through a secure CICD pipeline using Jenkins, the popular CICD tool.
Along with Jenkins we are also use many other popular and demanding devops tool like Docker, Sonarqube, Trivy, Prometheus, Grafana and even Argocd and helm for Kubernetes deployment.

# steps to create this project

1. **Create EC2 Instance:** Provision an AWS EC2 instance with increased RAM and storage for your application.

2. **Clone Repository:** Copy your project code from a version control repository to your EC2 instance.

3. **Install Docker:** Set up the Docker containerization platform on the EC2 instance.

4. **Obtain TMDB API Key:** Acquire an API key from The Movie Database (TMDB) for accessing movie-related data.

5. **Run Docker Images:** Deploy Docker containers with your application using the TMDB API key.

6. **Install SonarQube:** Set up SonarQube for code quality analysis using a Docker image.

7. **Install Trivy:** Install Trivy, a vulnerability scanner for containers and images.

8. **Install Jenkins:** Install the Jenkins automation server on your EC2 instance.

9. **Jenkins Plugins:** Add essential Jenkins plugins (Eclipse Temurin Installer, SonarQube Scanner, NodeJs Plugin, Email Extension) for your project.

10. **Configure SonarQube:** Integrate SonarQube with Jenkins by configuring credentials and analysis.

11. **Build Verification:** Verify the success of your project builds using Jenkins.

12. **Docker Plugins & OWASP:** Install Jenkins plugins for Docker and OWASP Dependency-Check to enhance security and automation.

13. **Docker Configuration:** Configure Docker integration in Jenkins, including credentials.

14. **Monitoring Server:** Set up a new server for monitoring tools.

15. **Install Prometheus:** Install the Prometheus monitoring system on the monitoring server.

16. **Install Node Exporter:** Install Node Exporter to collect system metrics on your EC2 instance.

17. **Prometheus Configuration:** Configure Prometheus to collect and store metrics from your services.

18. **Install Grafana:** Install Grafana for creating dashboards and visualizing metrics.

19. **Grafana Setup:** Configure Grafana, including setting up data sources and importing dashboards.

20. **Jenkins Notifications:** Implement notification services in Jenkins for build status alerts.

21. **AWS EKS Cluster & Argo CD:** Create an Amazon EKS cluster and Install Argo CD on the EKS cluster.

Use Helm to install Node Exporter on your EKS cluster nodes.

22. **Kubernetes Monitoring:** Configure Jenkins for Kubernetes and monitor it through Grafana.



# Project Details With Screenshots

**Creating an EC2 Instances** 
   
![Screenshot (183)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/cb458c69-bf46-4358-8fd2-fcb4d4195aae)

**Building the jobs in Jenkins**

![Screenshot (184)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/7df8aa5c-e76b-4aa5-8a28-256cec040407)

**Inspecting the Code quality in Sonarqube**

![Screenshot (185)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/7dde825d-daff-46e8-b49e-c9ef5397fcb4)

**pushing an Docker image to the Docker Hub**

![Screenshot (186)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/d060615c-5c15-494a-a723-382f9832578d)

**collecting the Metrics through node exporter**

![Screenshot (198)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/ea32f406-adf3-49bc-9b9c-287b39b1229c)

**Collecting and Storing metrics in prometheus**

![Screenshot (187)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/94b71bec-34dc-414e-ba7b-e9a6eab421fe)

**Monitoring metrics of different tools in Grafana**

![Screenshot (188)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/1d1c66c7-477b-4a88-96f0-d4a380faf921)

**creating an Eks Cluster for Deployment**

![Screenshot (189)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/5a7bdd23-f83c-45d0-9b07-3e72460325c2)


![Screenshot (190)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/a1713930-277c-47e3-82f5-d3218847d966)

**security groups ports to be allowed**

![Screenshot (194)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/a6a4ea47-52db-4a74-8bbd-c15b36a7172b)


![Screenshot (195)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/00987e78-799a-4402-a1d9-e3ae0c1f1703)


**NETFLIX-CLONE has been deployed**

![Screenshot (191)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/5927e4cc-cbe1-424b-a823-2fb5043440c0)


![Screenshot (193)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/f29b58d1-a26d-4f0b-a326-38ec3e89a92b)


![Screenshot (192)](https://github.com/sunilkurthakoti/DevSecOps-Project/assets/131526336/0996d283-a664-4310-9f05-12b566ec35d3)

## Feedback

If you have any feedback, please reach out to us at sunilkurthakoti06@gmail.com

