# Review

## Bringing your own licenses
You can bring images with existing licenses in any region that supports **sole-tenant nodes**
- no additional charge for bringing images with existing licenses
- still pay for your licenses according to your agreements.

## Preemptible instances
Preemptible VM instances are available at much *lower price—a 60-91%* discount—compared to the price of standard VMs. However, Compute Engine ***might stop (preempt)** these instances if it needs to reclaim the compute capacity for allocation to other VMs. Preemptible instances use excess Compute Engine capacity, so their availability varies with usage.

After 24 hours Compute Engine stops instances. Might not always be available.

## Organization Policy Service
Centralized & programmatic control over your organization's cloud resource.
- **Organization policy admin**: able to configure contraints across your entire *resource hierarchy*

IAM focuses on **who**, authorization. Organization Policy focuses on **what**, set restrictions on specific
resources to determine how they **can be configured**.

Common Use Cases:
- Limit resource sharing based on domain
- Limit the usage of **IAM** service accounts
- Restrict the physical location of newly created resources

## Partner Interconnect 
Connectivity between your *on-premises* network and your VPC network

## Active Directory SSO
To be able to removed people who has acces from AD.

## Storage Access
**Google Cloud Coldline** is cold-tier for achival data with access frequency of less than one per year.

## Cloud Functions
- Access to Firebase & Google Cloud events
- Scalable computing power

Use cases:
- Notify users
- Perform DB sanitization & maintenance
- Exec intensive taks in the cloud
- Integrate with third-party

## Cloud Bigtable
Fully managed, scalable NoSQL DB servie for large analytical & operational workloads (up to 99.999&).
- sub-10ms latency
- Personalization, ad tech, fintech, digital media, IoT

## Cloud Data Fusion
Fully managed, cloud-native data integration at any scale. Make your disparate data silos more unified.
Easily transform and map data (pipelines). GUI.

## Firestore
Flexible, scalable NoSQL cloud DB to store & sync data for client-side and server-side dev.

## Dataflow
After you construct a pipeline (Apache  Beam), you can use Dataflow to deploy and execute it. 
Automatically spinning up & tearing down the necessary resources. 

## Data Catalog
Fully managed & scalable metadata management service that allows orgs to quickly discover, manage
and understand all their data.
- Data discovery with search inteface
- Flexible & powerful cataloging system
- Auto-tagging mechanism for sensitive data

## Cloud Build
Build, test, and deploy in a serverless CI/CD platform. 
- All programing languages
- 15 machine types, hundreds of concurrent builds per pool
- Envs: VMs, serverless, Kubernetes, Firebase

## Cloud Scheduler
Fully managed cron job service:
- Batch
- Big data jobs
- Cloud infra ops


## Cloud Deployment Manager
Infrastructure deployment service that automates the creation & management of Google Cloud resources.

## Cloud Code
Set of IDE plugin for popular IDEs that makes easier to create, deploy and integrate apps with Google Cloud.

## Cloud VPN
Securely extends your peer net yo Google's net through an *IPsec VPN tunnel*. Traffice encrypted and 
travels over the public internet. Low-volume data connections.

## Direct peering
Establish a *direct peering* connection between your business net and Google's edeg net & exchange
high-throughput cloud traffic. Exists outside of Google Cloud.

## Cloud Interconnect
Extends on-premises net to Google's net:
- HA
- Low latency
- Doesn't traverse the public internet.

## AutoML Tables
Collaborative automatic implementation of Machine Learning models (struct data, high speed & scale).

## Private Google Access
To have VM wiht only internal IP addresses.

## Google Cloud Armor
Protect your apps/webs against DoS.Google Cloud Armor security policies are available only for backend 
services behind an external HTTP(S) load balancer. The load balancer can be in Premium Tier or Standard Tier.

## Secret Manager
Store API keys, passwords, certificates, and other sensitive data.

## Transfer
- *Storage Transfer Service*: TBs
- *gsutil*: up to 1 TB
- *Transfer Appliance*: not enough

## Anthos
Unifies the *management* of infra & apps across on-premises, edge, and multiple clouds. 

## [BigQuery Data Transfer Service](https://cloud.google.com/bigquery-transfer/docs/introduction?hl=en)
Moving data:
- Google: Google Ads, Google Merchant Center, YouTube
- External: Amazon S3, Teradata, Amazon Redshift


## Paid support
- Standard
- Enhanced
- Premium

Basic included with your Google Cloud subscription which cover only Case, phone, and chat support for billing issues only

**Support Hub** is the reference page for GCP support.

## Cloud Security Scanner
Identifies vulnerabilities in:
- App Engine
- GKE
- Compute Engine

It follows all public URLs, crawling your app and attempts the most interaction possible.

## Compliance Webpages resources
- GDPR Home Page
- Compliance Offerings
- Compliance Reports Manager

## Project
A Project facilitates organization of services and objects and also use this method of segmentation for billing and accounting. 

You can only create 5 networks per project.


## Compute Engine 
It provides machine type recommendations to help you optimize the resource utilization of your virtual machine (VM) instances: Rightsizing Recommendations