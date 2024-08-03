                                          # Jenkins CI/CD Pipeline with Ansible, Docker
 ![image](https://github.com/user-attachments/assets/11c62fbb-3263-4008-997a-7720a9e86386)
 
 #What is each tool?

GitHub Repository: Contains the code for the Docker web application.

GitHub Webhooks: Configured to send payloads to Jenkins whenever changes are pushed to the repository. 

Jenkins CI/CD Pipeline: Triggered by GitHub webhooks, the pipeline orchestrates the build, test, and deployment of the Docker image. 

Ansible: Used within the Jenkins pipeline to automate the pulling of the code from GitHub, build the Docker image, and deploy the container.

Docker: Image is rebuilt and the container is deployed automatically in response to changes pushed to the GitHub repository.

# These are the basic commands used in this project
sudo apt update 
sudo apt upgrade
ssh-keygen 
ssh-copy-id <username@<Docker private.ip.address> 

# Jenkins Job Cammands
scp -r /var/lib/jenkins/workspace/<pipeline name/* root@<ip address>:~<project directory>

ansible-playbook /var/lib/jenkins/playbooks/<playbook yaml file>

