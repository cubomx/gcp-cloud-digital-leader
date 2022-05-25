# Data

Traditionally, data analysis could take days or months, is often incomplete, and complex reports were often done by specialized teams.

## Data Buckets
- User: all data from customers who use or purchase your services and products.
- Corporate: data about the company such as sales patterns and operations.
- Industry: data found outside an individual organization that everyone in the sector needs to view or access to gain knowledge about a specific domain.

## Data Types
- Images
- Audio files
- Social media interactions
- Tabular

Structured data: it is highly organized
- Customer records
- Easily stored in DB
- Quantitative

Unstructured: no org
- Audio, images, videos, documents
- Qualitative
- Objects: data, metadata, id
- BLOB: Binary Large Object

Use API 

## Data Consolidation & Analytics
Using a Cloud provider will make your data storage and compute powers elastic (scale up or down).

A database is an organized collection of data generally stored in tables and accessed electronically from a computer system. Databases efficiently ingest large amounts of real-time data.

Priorities:
- Data Integrity: accuracy & consistency
- Scale

**Cloud SQL**: fully managed RDBMS (integration with Google Kubernetes & Big Query). Offers security, availability, and durability, and storage scales automatically. For websites, e-commerces, report & chart creation.

**Cloud Spanner**-: fully managed DB service, designed to be globally scaled. Replicate over regions. Massive scalability. Mission-critcial RDB service. Scalable online transaction (OLTP). Strong consistency.

**Cloud Storage**: unified cloud storage, BLOB data (Binary Large OBject)
- any amount of data
- Low latency
- Access anywhere

Options:
- Multi-regional storage: serving content to user worldwide
- Regional: locally, internal use cases (Data analytics & ML)

Tier acces:
- Nearline (once per month access)
- Coldline (once per 90 days/quarter)
- Archive (once per year)

**Compute Engine**: compute power

**Data Warehouse**: data from multiple sources (even DBs). It enables rapid analysis of large and multidimensional datasets. Get insights, trends. Central Hub.

When combined with connector tools, data warehouses can transform unstructured data into semi-structured data that can be used for analysis


**Big Query**: fully managed data warehouse with downtime free upgrades
- Analyze PB of data (fast speeds & zero operational overhead)
- Serverless, pay for running job

Transform unstructured data:
- **Pub/Sub**: service for real-time ingestion of data analytics into  BigQuery with Dataflow
- **Dataflow**: large scale processing of data

**Data Lakes**: it stores structured, semi-structured, unstructured data. 
Functionality:
- Backup
- Storage for raw data.
- Historic data (not relevant to day-to-day business operations)


**Looker**: business intelligence solution, data platform:
- describe you data
- metrics

## Machine Learning
A. I. Describes any kind of machine capable of acting autonomously
M. L. 
- refers to computers that can learn from data without using a complex set of rules
- is a way to use standard algorithms or standard models to analyze data in order to derive predictive insights and make repeated decisions at scale

**Data quality**
The accuracy of those predictions, however, depend on large volumes of data that are free of bugs.

Qualities of good data:
- It has coverage (domain scope & all posible scenarios)
- Clean (dirt or inconsistency that prevents to make accurate predictions)
- Complete (sufficient data about the world to replace human knowledge): fractured data 

**Google Cloud AI Platform**: unified simply-managed platform that makes ML easy to adopt by analysts & devs.
- Generate your own tailored models
- Use pretrained models 
- Integration of analytics into apps

**Google Cloud AI Hub**: hosted repository of plug-and-play AI components
- Notebooks examples

**TensorFlow**: take advantage of TPUs (hardware to accelerate ML workloads with TensorFlow). Comprehensive, flexible ecosystem of tools, libraries, and community resources. Open-source software library for machine learning developed inside Google

Google's data such as **Vision API**. This offers powerful pretrained machine learning models using Google's data to automatically detect faces, objects, texts, and even sentiment in images.

**AutoML Vision API**. This API automates the training of your own custom machine learning models. GUI.


## Business Problems
- Replacing or simplifying rule-based systems
- Automating processes
- Understanding unstructured data
- Creating personalized customer experiences.

RankBrain, Google's deep neural network for search ranking.

