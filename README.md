Ansiible Lab
What I want to do in these labs is have a disposable environments that embrace the two ways of working in provisioning and maintenence of infrastructure: declarative and proceedural paradigms. Using Terraform and Infrastructure as Code to create the scaffolding used in both learning and creating Migration Infrastructure.

Install Controller and tools
Prepare infra: create VPC (optional)
Create Lab nodes app1-app3 install software,SGs, NACLS, ingress/egress, object storage, monitoring, logging
Validate infrastructure, test operaability, health-check
Enable visibility by deploying monitoring stack (enable cloudwatch eventing)
*There are many ways to do the above. Another pattern, and inexpensive way would be to use Vagrant to create small infra vms to do the same locally. The key part is that the environment is using a declarative knowable method with

## Roman Stack
Terraform on a stick. Rolled up with Hashicorp goodness of Terraform and pre-configured deployments for hyperscalers (providers and modules hosted in public/private registries) as well as local and remote-provisioners combined with modules for easy deploy on VMs.  

- Deploy Terraform node with prereqs and tools (Deployment model: on-prem vmware/nutanix, air-gapped, cloud-native on all hyperscalers). Create Modules checked into the registry for these 
- Deploy build runtime (docker/podman/buildah) 
- Config data resides in git, data persisted locally, in object storage, with SaaS hosted/manuaged/unmanaged backend for state.



Deploy Terraform node with prereqs and tools (Deployment model: on-prem vmware/nutanix, air-gapped, cloud-native on all hyperscalers). Create Modules cheched into the registry for these
Deploy build runtime (docker/podman/buildah)
Config data resides in git
Miniature Easily Deployable Commodity Infrastructure For Migration
Deploy build runtime (docker/podman/buildah) Use containerd runtime on a utility vm.

Small deployments of custom tools run in an automated pipeline and published to a container registry

Break projects into smaller composable parts for the tooling

Terraform configurations as standard for deployment of Utility container runtimes that will host the deployments.

This is housed in a GHE repo. Can use private Git or hyperscaler container registry.

Platforms: VMWare, AWS,Azure (w ARM/Bicep templates),GCP, Nutanix, bare metal

These can be for places like $ACCOUNTNAME apps. Maybe an Operator within a CRD (Custom Resource Definition)

Observability ToolKit
Create an easily deployed OSS Toolchain using BPF capabilities of the Linux Kernel. Write tooling that focuses on existing migration challanges.

Build containerized deployments of tooling



########
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


## Version Control and Why It is Important
Once we provide our infrastructure as code, it is in a place where it can be de-coupled, separated away from many of the difficult well-known aspects of traditional enterprise infrastructure management. These were designed, and operate within, their contexts with flawed feedback mechanisms and assumptions. Injecting version control and high visibility within this context can super-charge the speed of change. 
## Automated Governance 
Spoken more about in the DevOps Automated Governance Reference Architectures (Kim, Willis, Kissler, Nygard et al.) looking to how CapitalOne this is a prime-mover 


## Labels: What's in A Name?
Sometimes I feel like that person who just got the Brother P-touch, labelling everything I can like a nut. The part that I miss is the power of having simplicity and meaning in applying these abstractions is a necessity. 

- In traditional datacenter oriented views the inventory and CMDB are widely understood as are the current enterprisey SNOW models. One part that is missing is the data cleansing and curation of this data outside the SOR. 
