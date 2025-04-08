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



In Jenkins, **webhooks** are commonly used to trigger Jenkins jobs based on events occurring in external systems, such as GitHub, GitLab, or Bitbucket. Webhooks allow Jenkins to automatically start a build when certain events, like code pushes, pull requests, or branch updates, happen on the external system.

### Setting up Webhooks in Jenkins:

1. **Install the necessary plugins:**
   To use webhooks, ensure you have the appropriate plugins installed in Jenkins. For Git-based systems, this typically involves:
   - **GitHub Plugin**
   - **GitLab Plugin**
   - **Bitbucket Plugin**
   These plugins handle the integration between Jenkins and the respective platform.

2. **Create or configure a Jenkins job:**
   You’ll need to create or configure a Jenkins job (usually a pipeline or freestyle job) that will be triggered by the webhook. This job typically contains the steps that Jenkins will execute when the event occurs.

3. **Configure the webhook on your external system (e.g., GitHub):**
   - For **GitHub**, go to the repository’s settings > Webhooks > Add webhook.
   - In the **Payload URL**, enter the Jenkins webhook URL. This will generally be something like:  
     ```
     http://<jenkins-server>/github-webhook/
     ```
   - Set the content type to `application/json`.
   - Choose which events should trigger the webhook (e.g., push events, pull requests, etc.).
   - Finally, save the webhook.

4. **Configure Jenkins to handle the webhook:**
   Jenkins will need to listen for incoming webhooks, and this is usually done using the **GitHub Plugin** or **GitLab Plugin**. Once you have set up your Jenkins job:
   - Go to the job configuration.
   - Under **Build Triggers**, enable the trigger option that corresponds to the external service, such as **GitHub hook trigger for GITScm polling** or similar options for GitLab or Bitbucket.

5. **Test the webhook:**
   Once everything is set up, push changes to the external system (e.g., commit code to GitHub). The webhook should notify Jenkins, and it should automatically trigger the configured job.

### Example: GitHub Webhook in Jenkins

1. Install the **GitHub plugin** in Jenkins.
2. Create a Jenkins job (e.g., a Freestyle or Pipeline job).
3. In the Jenkins job configuration, under **Build Triggers**, check **GitHub hook trigger for GITScm polling**.
4. Copy the webhook URL generated by Jenkins (it should look like: `http://<your-jenkins-server>/github-webhook/`).
5. In your GitHub repository, navigate to **Settings > Webhooks**.
6. Add a new webhook, set the Payload URL to the Jenkins webhook URL, and select the events that should trigger the webhook (usually "Push events").
7. Save the webhook, and now Jenkins will automatically trigger a build whenever the selected event occurs on GitHub.

### Use Cases:
- **Continuous Integration (CI):** Automatically trigger builds when new code is pushed.
- **Pull Request Builds:** Trigger builds when a pull request is created or updated.
- **Branch Builds:** Trigger builds when changes are made to specific branches.

By using webhooks, you can integrate Jenkins with external platforms to automatically trigger builds and streamline your CI/CD pipeline.





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


STEP-9: attach web hooks to trigger

STEP-9:   Finally Deployed website with public IP and port number.
http://18.232.116.59:3000/



![Screenshot (65)](https://github.com/user-attachments/assets/33d2d249-247b-438f-a614-7b6b8c687a79)

![Screenshot (67)](https://github.com/user-attachments/assets/0e21c5f1-ed13-46c7-9d34-7b6057d5d927)


![Screenshot (68)](https://github.com/user-attachments/assets/98eb4090-9229-406e-9e69-857309165e05)
![Screenshot (69)](https://github.com/user-attachments/assets/40e7b786-614a-4ca1-8301-cd8fac891750)






![Screenshot (72)](https://github.com/user-attachments/assets/f3a9b53c-89b8-41ec-9d21-![Screenshot (75)] 

(https://github.com/user-attachments/assets/b8742aac-8225-4211-8532-8ae7173995ec)
71ff09fafa0f)


![Screenshot (75)](https://github.com/user-attachments/assets/5acbc124-abef-4a6a-a34e-030870d0e67d)




![Screenshot (74)](https://github.com/user-attachments/assets/6b484649-e27e-4884-af9e-8fce01c5e7b8)





