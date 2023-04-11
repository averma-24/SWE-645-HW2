Group Project Members:
1) Name : Simran Bayas G-Number-G01351582 Email-sbayas@gmu.edu
2) Name : Abhishek Verma GNumber-G01358661 Email-averma24@gmu.edu
Contributions :
Simran Bayas (G01351582) and Abhishek Verma (G01358661) collaborated collectively to complete HW2. Our joint effort and teamwork resulted in the successful completion of the project.
The ReadMe file consists of the overview of HW-2, please refer to the SWE645-HW2-Installation&SetupInstructions provided in the zip file submission for detailed instructions to replicate the steps if needed.
Project Submission Zip File Folder Structure:
The HW2-SWE645-GroupProject contains the following: 1) Project Codebase -
1. DockerFile
2. Jenkinsfile
3. studentSurveyForm.war 4. main folder
1. studentSurveyForm folder 2. webapp folder
1. index.html
2. studentFormStyle.css 3. META-INF folder
4. WEB-INF folder
2) Video Recording Folder 3) YAML Files
1. k8.yaml
2. student-survey.yaml
3. Student-survey-lb.yaml
4) SWE645-HW2-Installation&SetupInstructions.pdf
5) ReadMe Project Links :
1. AWS URL of our homepage
Link for Student Survey Form(Part 2): https://ec2-44-197-169-25.compute-1.amazonaws.com/studentSurveyForm/
2. GitHub Repository
https://github.com/averma-24/
3. Video Demonstration
https://gmuedu-my.sharepoint.com/personal/averma24_gmu_edu/_layouts/15/stream.aspx?id=%2Fpersonal%2Faverma24%5Fgmu%5Fedu%2FDocuments%2FSWE645%2DHW2%2DREC%2Emp4&ga=1
4. Creating a Docker Image and pushing it to DockerHub
https://hub.docker.com/r/averma24/studentsurveyassignment/tags
5. Setting up Rancher on an EC2 Instance (FirstEC2)
34.194.61.172
6. Deploying a Kubernetes Cluster with Rancher on an EC2 Instance (SecondEC2)
52.5.160.67
7. Steps to create a deployment in a Kubernetes cluster: (3 Replicas)
34.194.61.172
8. Steps to deploy Jenkins on AWS EC2
44.194.15.192:8080
9. Creating a CI/CD Pipeline in Jenkins
44.194.15.192:8080
10. Setting up the Jenkinsfile
44.194.15.192:8080
11. Running the Jenkinsfile
44.194.15.192:8080
12. Accessing URL path & Kubernetes service in Rancher
https://34.194.61.172/k8s/clusters/c-w2vxb/api/v1/namespaces/default/services/http:student-survey-lb:8080/proxy/studentSurveyForm/
Note : Since the AWS EC2 is deployed using AWS Learner Lab, this link would not be accessible at the time this document would be viewed.
Conclusion :
By following these steps we were able to
1. Containerize the Web application we developed in Homework 1 – Part 2, using Docker
container technology.
2. Deployed the containerized application on the open source container orchestration platform
Kubernetes to enable scalability and resiliency of the application with baseline configuration of
at least three pods running all the time.
3. Used Rancher (https://rancher.com/docs) to set up the Kubernetes cluster.
4. Established a CI/CD pipeline that includes a Git source code repository at GitHub, and Jenkins
for automated build and for the automated deployment of our application on Kubernetes.
References :
HW2 Related - Creating EC2 instances in AWS Learner Lab
HW2 Related - CI/CD Setup Reference Guide https://medium.com/@pra4mesh/deploy-war-in-docker-tomcat-container-b52a3baea448 https://linuxize.com/post/how-to-install-jenkins-on-ubuntu-20-04/ https://www.jenkins.io/doc/book/pipeline/docker/
