## Ansiible Lab
*What I want to do in these labs is have a disposable environments that embrace the two ways of working in provisioning and maintenence of infrastructure: declarative and proceedural paradigms. Using Terraform and Infrastructure as Code to create the scaffolding used in both learning and creating Migration Infrastructure.*

- Prepare infra: create VPC (optional)
- Install Controller and tools. Use cloud-init and/or user_data functionality. This app stack will also be deployed to a cluster via helm.
- Create Lab nodes app1-app3 install software,SGs, NACLS, ingress/egress, object storage, monitoring, logging
- Validate infrastructure, test operaability, health-check 
- Enable visibility by deploying monitoring stack (enable cloudwatch eventing) 

*There are many ways to do the above. Another pattern, and inexpensive way would be to use Vagrant to create small infra vms to do the same locally. The key part is that the environment is using a declarative method with a way to manage what is provisioned. 


