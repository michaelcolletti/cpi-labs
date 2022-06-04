## Ansible Lab
*What I want to do in these labs is have a disposable environments that embrace the two ways of working in provisioning and maintenence of infrastructure: declarative and proceedural paradigms. Using Terraform and Infrastructure as Code to create the scaffolding used in both learning and creating Migration Infrastructure.*

- Install Controller and tools 
- Prepare infra: create VPC (optional)
- Create Lab nodes app1-app3 install software,SGs, NACLS, ingress/egress, object storage, monitoring, logging
- Validate infrastructure, test operaability, health-check 
- Enable visibility by deploying monitoring stack (enable cloudwatch eventing) 

*There are many ways to do the above. Another pattern, and inexpensive way would be to use Vagrant to create small infra vms to do the same locally. The key part is that the environment is using a declarative knowable method with 

## Roman Stack
- Deploy Terraform node with prereqs and tools (Deployment model: on-prem vmware/nutanix, air-gapped, cloud-native on all hyperscalers). Create Modules checked into the registry for these 
- Deploy build runtime (docker/podman/buildah) 
- Config data resides in git
- Encrypt at rest secrets in a vault
- 

## Miniature Easily Deployable Commodity Infrastructure For Migration 

- Deploy build runtime (docker/podman/buildah) Use containerd runtime on a utility vm.
- Small deployments of custom tools run in an automated pipeline and published to a container registry
- Break projects into smaller composable parts for the tooling

- Terraform configurations as standard for deployment of Utility container runtimes that will host the deployments. 
- This is housed in a GHE repo. Can use private Git or hyperscaler container registry.
- Platforms: VMWare, AWS,Azure (w ARM/Bicep templates),GCP, Nutanix, bare metal
- These can be for places like $ACCOUNTNAME apps. Maybe an Operator within a CRD (Custom Resource Definition) 

## Observability ToolKit
Create an easily deployed OSS Toolchain using BPF capabilities of the Linux Kernel. Write tooling that focuses on existing migration challanges.

- Build containerized deployments of tooling


