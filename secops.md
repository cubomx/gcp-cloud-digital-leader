# Sec Ops

## Financial Governance
Managing cloud costs:
- Planning & budgeting
- Monitor & control
- Optimizing accurately forecast future costs

Top pain points when managing cloud environments:
- Unpredictable costs
- Lack of visibility and transparency

Three lenses:
- People 
- Process
- Technology

Close collaboration between technology and line of business teams. 
Partnership across finance, technology, and business functions. 
Central team consist of *several experts* who ensure the best practices and 
there's visibility into the ongoing cloud spend. This group would be able to 
make real time decisions.

Having a culture of accountability in place across teams helps organizations spot waste, 
quickly take action to eliminate it, and ensure they're maximizing their cloud investment.

- Gain greater visibility
- Drive a culture of accountability for cloud spending across the organization
    - Ownership fro projects & sharing cost views
- Control costs to reduce to risks of overspending
    - Policies & permissions to control spending
    - Creating budgets & alerts
- Provide intelligent recommendations to optimize cost and usage.

TCO: hardware, software, management & support, communications, 
user expenses, the cost of service downtime, training, and other productivity losses. 
The cloud improves efficiency, reliability, and security, enabling greater productivity 
and innovation for businesses.

Best practices:
- Identify the individual or team that will manage costs
- Learn the diff between invoices & cost tools (An invoice and Google Cloud tools are 
not the same thing)
- Use cost management tools for accountability and to gain visibility, control, and intelligence

**An invoice** simply tells you how much you're spending over a period of time.

Get insight of costs:
- Built-in reporting tools
- Custom dashboards
- Pricing calculator: see how changing usage will affect their costs.


## Security
**Privacy**: data an org/individual has access to and who they can share it.

**Security**: policies, procedures, and controls.

**Compliance**: meeting standars set by a third party (regulatory authority or international standards organization) 

**Availability**: prevent unauthorized access but, still make available when needed. How much time the 
*cloud service provider* **guarantees** data and services are running/accesible.

Google's data statement:
- **You own your data**, not Google.
- **Google does not sell customer data** to third parties, neither fro advertising purposes.
- **All customer data is encrypted by default**
- **Google Cloud guards against insider access to your data**
- **We never give any gov entity "backdoor" access to your data**
- **Our privacy practices are audited** against international standards
    - ISO 27-0-17, covers the protection of personally identifiable information (PII) in cloud services

Threats:
- Constant criminal attacks 
- Physical damage (natural disasters, physical hardware, power losses)
- Malware, viruses (data lost, damaged, destroyed), and ransomware attacks (blocked until pay)
- Unsecured third party systems
- Lack or expert knowledge

### Shared responsibility
Cloud provider process your data.
You are the data controller.

**Defense in depth**: multiple built in security layers.
- Customer's core responsibility is to secure access to data.
- Cloud provider is responsible for securing the underlying infrastructure.

Three components:
- Sharding (fragmentation/division)
- Encryption keys
- Key encryption key

Google Cloud's multilayer approach to security:
- Hardware: Google designs own servers, storage, networking gear
    - Titan chip checks the integrity when boot up
- Software: Servers are not allowed onto the net, until the health is confirmed
    - Titan continues to verify the OS and the rest of the deploy software stack
- Storage: encryption at rest
    - Data is broken into pieces (chunks) in memory
    - The pieces are encrypted with their own data encryption key (DEK)
    - These DEKs are then encrypted or wrapped, generating a key encryption key (KEK)
    - Encrypted chunks & wrapped encryption keys are distributed across Google's infra
- Identity: zero trust model; strongly authenticate.
- Network: encryption in transit; protect against DDoS attacks.
- Operations: Google's experts

Customer Responsibility:
- Understanding of who can access what data

| Action | Frontend user | Manager | Super user | Admin |
| ---- | ---- | ------- | ----- | ------- |
| View logs| | | x | x |
| Modify settings | | | | x |
| Modify users | | x | | x |
| Modify applications | | x | | x |
- Enable MFA protect against phishing
- Security keys
- IT Teams & business decision makers need to ensure that **they have visibility** (logging & monitorig tools)
    - What's happening
    - Who is accessing what data
    - When
- A open and blameless culture
- Be ready if something happens
- Google Cloud has the following for controlling data access, maintain visibility, preparing for breaches:
    - Best practices
    - Templates
    - Products
    - Solutions


### Identity & access management

The **Cloud identity** helps organization control & manage access to resources:
- Security
- Integrity
of data & systems.

An **Identity Access Management** policy (IAM) is made of:
- who (Google account, Google group, service account, Google workspace or Cloud Identity domain)
- can do what (IAM role)
    - Primitive (Owner, Editor, Viewer)
        - Account Administrator: apply primitive roles to a Google Cloud project
        - Viewer: examine but not change state
        - Editor: Viewer + change state
        - Owner: Editor + manage roles & permissions on the resource 
    - Predefined: each role is a collection of permissions
    - Custom: more granular roles, least privileged model (minimal amount of privilege)
- on which resource

You can group people and grant permissions per group.

### Resource hierarchy
- **Resource**: any Google Cloud service
- **Project**: 
    - Enabling & using Google Cloud capabilities (managing APIs)
    - Enabling APIs
    - Adding & removing collaborators
    - Enabling other Google/Alphabet services
- **Folder**: contain projects, other folders, or combination of both
- **Organization**: managed through the Cloud Console; lets admins see & control Google Cloud resources & permisssions
- **Domain**: handled through Cloud identity; manage user profiles

Permissions can be inherited from any folders above it or from the organization.

2 other roles for *resource management* are:
 - **Cloud Billing** accounts:
    - Live under the org and track any charges for associated projects.
    - User can associate projects and see spend
    - Admins are able to unlink projects, set budgets, contact billing support
 - **Payment profiles**:
    - Sits outside of Google Cloud
    - Pay for all Google services (Google Cloud, Google ads, Chrome licenses)      

## Monitoring Cloud IT Services & Operations
Challenges:
- Devs are expected to continuously improve customer facing services. 
    - Schedule system downtimes (monthly, quarterly, yearly)
    - Be agile:
        - Release new functions frequently
        - Increase business value with new features
        - Release fixes fast
- Operators ensure that systems & apps operate reliably
    - Prefer to work slowly to ensure reliability and consistency
- Working in silos; avoid it, promote collaboration
- If a problem occurs, it can be very difficult to identify the source of the problem and
resolve it quickly. 
- Accountability between the teams is not always clear.

What to do?
- Adjust expectations for service availability not to be 100%
- Adopt DevOps & SRE bes pratices to work more collaboratively with clearer
accountability

### Service Availability:
- Cloud Providers define service availability in a SLA (Service Level Agreement), service 
level objectives and service level indicators.
- **SLA** is a contractual commitment betwen the cloud service provider and the customer.
    - Quality, availability and reliability of the service.
    - If not met, the cloud provider would incur a cost usually paid out to the customer.
- **SLO** it's the goal for the cloud service perfomance level, a key element inside a SLA
    - Shared between the cloud provider and the customer
    - Above, everyone is happy
    - If below the SLO and above the SLA, its give a signal to the cloud provider to reduce 
    service outages and increase service reliability
- **SLI** is a measure of the service provided
    - Reliability & errors
    - **Error Budget**: amount of error over a certain period of time before end users start
    feeling unhappy. It is like a pain tolerance for availability, latency.

### DevOps & SRE
DevOps:  philosophy that seeks to create a more collaborative and accountable culture 
within developer and operations teams.
- Reduce silos: break down barriers across teams
- Accept failure as normal
- Implement gradual change: easier to review
- Leverage tooling and automation
- Measure everything

SRE: a discipline that applies aspects of Software Engineering to operations.
- Create ultra-scalable & highly reliable software systems.
- Write code and run production systems.

SRE Best Practices:
- Shared ownership of production between devs and ops.
    - Define SLOs 
    - Calculate error budgets
    - Determine reliability
    - Order work priorities
- Accept failure as normal: blameless lessons learned discussion
- Implement gradual changes: rolling out changes to a small % of users before making them
generally available
- Leverage tooling and automation: toil automation, reduce the amount of manual repetitive work.
- Measure everything: tracking everything related to toil, reliability, and the health of their
 systems

A culture of:
- Goal setting
- Transparency
- Data-driven decision making

### Resource Monitoring tools
**Google Cloud's operations suite** tools help to:
- Monitor
- Troubleshoot
- Improve app performance

Tools fall into two major categories:
- **Operation-focused tools**
    - Cloud monitoring
    - Cloud logging
    - Error reporting
    - Service monitoring
- **Application performance management tools**
    - Cloud Debugger
    - Cloud Trace
    - Cloud Profiler

**Monitoring**: gathering predefined sets of metrics/logs.
- **Cloud Monitoring**: foundation for SRE; provides visibility into performance, 
uptime, and overall health of cloud applications. Use of charts, dashboards, manage
alerts. Also, can evaluate the entire infra on a modular level.
- **Cloud Logging**: a log file contains the OS write events. Get insight and identify 
the root cause of issues. The service is fully managed (performs at scale). It can ingest 
app & system log data as well as custom log data from GKE, VMs, other services. 
Automatically ingest audit and platform logs.
- **Cloud monitoring**: view of all Google Cloud metrics at 0$ and integrates with
a variety  of providers (non-Google)
- **Cloud Debugger**: monitor app perfomance. Inspect the state of running app in real time.
- **Cloud Trace**: monitoring app perfomance. Find bugs in app that is chunked into small pieces
(containers/microservices). It helps devs to debug or fix and optimize the code.
