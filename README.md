# jenkins-project




TASK 1: Automate Code Deployment Using CI/CD Pipeline (GitHub Actions)
•	Objective: Set up a CI/CD pipeline to build and deploy a web app.
In this project, we leverage Jenkins to create a robust CI/CD pipeline that integrates tools like Docker,  and OWASP Dependency Check to deliver secure and high-quality software.
Tools used:
1.	GitHub
2.	Jenkins
3.	Docker Hub
4.	Docker
5.	nodeJS




GITHUB:
 GitHub is a platform for hosting and sharing code using Git. It helps developers collaborate by tracking changes, managing versions, and reviewing code. You can create repositories(repos) to store and organize projects. It also offers features like issue tracking and CI/CD workflows.

 
 


 JENKINS:
Jenkins is an automation tool for building and deploying software. It uses pipelines to automate tasks like testing, building, and deploying code. It supports plugins to integrate with various tools. Jenkins makes Continuous Integration and Continuous Delivery (CI/CD) easy.




DOCKER:
Docker is a tool to create, share, and run lightweight virtualized environments called containers. Containers package code and dependencies together for consistent behavior across systems. It simplifies app deployment and avoids “it works on my machine” issues. Docker images are reusable blueprints for containers.




NODE.JS:
Node.js is a runtime that lets you run JavaScript outside the browser. It’s great for building fast and scalable server-side applications. Node.js uses non-blocking, event-driven programming for high performance. It’s commonly used for web servers, APIs, and real-time apps.





CI/CD WORKFLOW:
•	The pipeline automates build, test, and deploy processes, making it efficient and reliable.
•	Security and quality checks are seamlessly integrated into the pipeline, ensuring every release is both secure and robust.





STEP-1: Launch EC2 Instance with below Configurations
1.	AMI : Amazon Linux Kernel 5.10
2.	Instance Type: T2.small
3.	EBS Volume : 28 GB
4.	Security Groups : All Traffic


STEP-2: Install Jenkins




STEP-3: Install Docker & GIT


#chmod 777 ///var/run/docker.sock



STEP-4: Install the following dependencies on Jenkins
1.	NodeJS (version 16.2.0)
2.  Docker Pipeline
3.  pipeline stageview


STEP-5: Integrate all the tools to Jenkins


STEP-6: Add Dockerhub Credentials


STEP-7: Create a Jenkins Job


STEP-8: Docker hub registry image

STEP-9:   Finally Deployed website with public IP and port number.
http://18.232.116.59:3000/



![Screenshot (65)](https://github.com/user-attachments/assets/33d2d249-247b-438f-a614-7b6b8c687a79)

![Screenshot (67)](https://github.com/user-attachments/assets/0e21c5f1-ed13-46c7-9d34-7b6057d5d927)


![Screenshot (68)](https://github.com/user-attachments/assets/98eb4090-9229-406e-9e69-857309165e05)
![Screenshot (69)](https://github.com/user-attachments/assets/40e7b786-614a-4ca1-8301-cd8fac891750)






![Screenshot (72)](https://github.com/user-attachments/assets/f3a9b53c-89b8-41ec-9d21-71ff09fafa0f)




![Screenshot (74)](https://github.com/user-attachments/assets/6b484649-e27e-4884-af9e-8fce01c5e7b8)





