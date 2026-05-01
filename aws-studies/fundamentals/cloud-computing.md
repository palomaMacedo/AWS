<img width="914" height="819" alt="Cloud-computing" src="https://github.com/user-attachments/assets/c97b54c0-86fb-40f4-a3d8-975baa6bd3fc" />


## AWS BENEFITS
* Scalability for growing applications
* Reduced costs with pay-as-you-go
* Access to innovative tools and services

## MAIN CHARACTERISTICS
* High-availability global infrastructure
* Security and compliance with rigorous standards
* Support for multiple programming languages

## Why Use AWS 
* Access to scalable resources for your project
* Flexibility in cloud services meets different needs
* Support for multiple programming languages for developers
* Integration with popular market tools that makes work easier

## Practical Tips
* Scalability: grows alongside your project
* On-demand cost: pay only for what you use
* Dev tools: SDKs, CLI, IaC
* Agility: from idea  to deploy in minutes
* Global-grade security, ready to use
* Massive ecosystem: docs, community, examples

## Sure! Here it is:
* 🔍 Did you know that Elasticsearch exists? It's a search and data analysis tool from an independent company!
* ⚡ It's different from the Elastic in EC2 — which refers to the ability to scale computing resources in the cloud ☁️
* 🤝 But Elasticsearch works great inside AWS! One more example of the platform's powerful ecosystem 🚀

##  REGIONS AND GLOBAL ARCHITECTURE
Here we aim to explore the Regions, Availability Zones and how they connect to AWS's global architecture, highlighting their importance for scalability and resilience.
REGION BENEFITS

* Increases service availability
* Improves infrastructure resilience
* Allows redundancy and disaster recovery

##  IMPORTANT CONSIDERATIONS

* Choosing the right region is crucial
* Understanding the available Availability Zones
* Evaluating latency and compliance requirements

##  AWS REGIONS

* AWS has hundreds of global regions.
* Each region is made up of several AZs.
* This structure ensures high availability and redundancy.
* The architecture is scalable and flexible to meet demands.
---
**AZ** = Availability Zone


## AVAILABILITY

* Redundant infrastructure across multiple AZs
* Minimizes interruption risks
* Scalability for variable demands

## IMPORTANCE

* High availability guarantee
* Geographic distribution of resources
* Protection against local failures


## PRACTICAL TIPS FOR CHOOSING REGIONS

### Latency and Performance
* Impact on user experience
* The choice of region can minimize latency and improve performance.

### Region Considerations
* Available services and reliability
* Check if the region offers the necessary services and has high availability.


## USER MANAGEMENT

* Create and manage users in IAM
* Define appropriate permissions and access
* Monitor user activities and history

## GROUPS AND POLICIES

* Organize users into groups for management
* Apply policies for access control
* Integrate Region information for security


## WHAT IS IAM?

* Identity Management is essential.
* Helps control access and permissions.
* Users and groups are fundamental for security.
* Policies configure access rules across regions.

## USERS AND GROUPS

* Organize users in IAM easily
* Create groups to simplify management
* Assign appropriate permissions to each group


## ACCESS POLICIES

* Define effective permissions and restrictions
* Manage secure access to resources
* Simplify user and group administration

## IAM REGIONS
* The importance of regions in IAM management and their influence on security

* IAM (Identity and Access Management) is not regional.
* Users, groups, policies and roles exist at a global level.
* A single AWS account → valid identities across all regions.



☁️ Summary — AWS Fundamentals
1. Cloud Providers and Scalability
Cloud Providers like AWS allow automatic migration between regions in case of failures, ensuring high availability — something difficult to achieve with local servers.
2. IaaS vs PaaS

IaaS — you control everything: RAM, CPU, OS. Ex: EC2
PaaS — you just write the code, the provider manages the infrastructure. Ex: Elastic Beanstalk

3. Lambda vs EC2

EC2 — charges for running time, even without receiving requests
Lambda — charges per request + execution time. If it doesn't run, you don't pay

4. AWS S3
Secure and scalable storage service. Stores any type of file (PDFs, code, Terraform) and allows access at any time. One of the most used AWS services.
5. Multi-Region Architectures
They are complex because each region has different prices, configurations and services. Requires data synchronization and backup across regions.
6. AWS Cloud Shell
Terminal integrated into the AWS console with AWS CLI already installed — allows executing commands directly, without local setup.
7. Multiple Regions
Increase the availability and resilience of the application. If one region goes down, another takes over automatically.
8. Region Selection
Always consider the proximity to end users to minimize latency and improve performance.
9. Region vs AZ

Region — geographic location (ex: São Paulo, Virginia)
AZ (Availability Zone) — physical data center within a region
Both are used for normal operations, not just backup

10. IAM is Global
IAM is not regional — users, groups, policies and roles apply to all regions of the same AWS account.
11. What is IAM
Service to manage identities and access in AWS. Controls who can access what, through users, groups, policies and roles.
12. CLI vs Web Console
Both have access to the same services. The CLI stands out for automation, productivity and scripting.

**IAM** = Identity and Access Management
