# Modernization of applications

## Intro
How to survive and thrive in this new cloud era?

Main focus is the way in which they structure and use their IT resources (*from CapEx to OpEx*). With Cloud, organizations can develop and build new applications to drive better engagement with customers and employees faster, securely, and at scale. It requires:
- New collaborative models
- Changing culture and processes
- Enabling team productivity and innovation.

IaaS: don`t manage physical infrastructure.
PaaS: don`t manage the infrastructure.


## Benefits
- **On demand self service**: Reduces the need for IT teams to act as gateway to techincal resources (net security, storage)
- **Broad network access**: Access to data & compute resources in *not limited* to a particular **geography**/location (low latency)
- **Resource pooling**: availability in case of service disruption/natural disaster
- **Rapid elasticity**: scale up or down instantly.
- **Measured service**: lower capital expenditure

## Compute options
**Computing**: machines's ability to process info to store, retrieve, compare and analyze it; automate tasks.

**Virtualization** multiple systems running on the same hardware.

**Virtual Machines** share the same pool of *computer processing, storage and networking resources*.

![Virtual Machines Structure](images/hypervisor.png)

A **hypervisor** sits on top of physical hardware and multiple VMs are built on top of it. It enables to have multiple applications to be running on a server.

**Containers** only recreate the OS, not the whole system (hardware). Both are ways to isolate environments to run software. The benefits are:
- Start faster
- Use less memory
- Predictable environments

**Kubernetes** open source cluster management system that provides automated container orchestration.

**Serverless computing** you put your data/app, the cloud provider takes care of everything behind the scene (deployments, management).

**Function-as-a-service**: run function on demand.

## Types of Cloud
**Private cloud**: org has virtualized servers in its own data centers.
**Hybrid cloud**: combination of on-premises/private cloud infra and public cloud services.
**Multi-cloud**: using multiple cloud providers.

**Cloud Bigtable**: manage database

**Anthos**: open application modernization platform
- Modernize your apps
- Build new ones
- Run them anywhere
- Build once, run anywhere

Secure network:
- 40% of thw world's internet traffic
- Operates over 200 countries & territories with 20 regions and over 130 points of access

Cloud strategy:
- Cost
- Security
- Openness
- Value of **available products & services**
- Environment

## Google Cloud compute solutions
**Compute Engine** computing & hosting service
- Create & Run VMs
- Scalable
- High performance

**Compute Engine VMs** (it is a ideal if you need complete control over the VM infrastructure)
- Boot quickly
- Persistent disk storage
- Consistent performance

Use cases:
- Software cannot easily be containerized
- You have existing VM images to move to the cloud

**Google Cloud VMWare Engine**: fully managed service that lets you run the VMWare platform in Google Cloud. You don't care about:
- Infrastructure
- Networking
- Managemtn services

**Bare Metal** enables you to migrate specialized workloads to the cloud while maintaining your existing investments and architecture.

**GKE** a managed env for deploying, managing, and scaling your containerized apps. It consists of multiple machines (Compute Engine instances) grouped together to form a cluster.
- Securely speed up app dev
- Streamline operations
- Manage infra

**App Engine**: PaaS and cloud computing for developing and hosting web apps
- Scalable web & mobile in any programming language
- Fully managed serverless platform
- Focus on writing code

**Cloud Run**: allows devs to build apps in their fav programming language with their fav dependencies & tools and deploy them in seconds. Containers.
- Automatically scaling up & down from zero instantly

**Cloud Functions** serverless exec env for building & connecting cloud services.
- Scalable
- Pay-as-you-go function as a service
- Zero server management

## Patterns to adopt the cloud
- Move apps first, then change them
- Change apps before move
- **Invent in greenfield**: building new infrastructure & applications in the cloud
- **Invent in brownfield**: replace an existing legacy application
- Move apps without changes

## Challenges in app dev
- A lot of work before writing code.
- Building code: design, build, test, integration, deploy.
- Decisions about: network architecture, choice of DB, type of server.
- Enables you to migrate specialized workloads to the cloud while maintaining your existing investments and architecture.

## Things to consider
- Avoid monolithic, use microservice
- Microservices benefits are:
    - Lower the risk of regressions
    - Debug issues quickly
    - Roll back to the last stable build if necessary



### GKE
Containerization allows developers to divide an application design into individual compartments. Parts of the code can be updated without affecting the whole application.

**Kubernetes** is an open source container orchestration system for automating computer application deployment, scaling, and management. GKE is the Google Cloud manage service for container orchestration.

### App Engine
It is a platfrom to build scalable Web apps and mobile back ends. It manages the infra for you.
- Auto-scaling

## APIs
Primary goals when doing digital transformation:
- Modernize IT systems
- Modernize apps
- Leverage APIs to unlock & create value for customers

### Benefits
APIs enable integration between systems. They expose data while protecting the integrity, securing and governing the access.

A **digital ecosystem** is a group of interconnected companies and products.

### Apigee
It is an API management platform.
API Services Layer: Runtime API gateway
Developer Services: Portal to utilize other APIs, register apps
Analytics Services: Measuring and tracking the performance of APIs.

## Legacy System challenges
The legacy system is mission critical, but often not equipped to deliver new services or upgrades at the speed and scale that users expect. Often cannot connect to new systems. They weren't developed to support the implementation and adoption of modern technologies such as the cloud or the Internet of Things or mobile applications. Are not designed to serve real time data.


