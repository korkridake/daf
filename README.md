# Table of Content

<!-- vscode-markdown-toc -->
* 1. [Define Purpose of DAF](#DefinePurposeofDAF)
* 2. [Understand Data & AI Maturity Framework](#UnderstandDataAIMaturityFramework)
* 3. [Deploy Enterprise Data Estate](#DeployEnterpriseDataEstate)
* 4. [Additional Resources](#AdditionalResources)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

# CAF - Data Adoption Framework

##  1. <a name='DefinePurposeofDAF'></a>Define Purpose of DAF

The Data Adoption Framework (DAF) helps you identify key cloud adoption activities and objectives to accelerate your journey to the cloud. For successful cloud adoption, organizations need to capitalize the four capabilities: (1) Learn (2) Lead (3) Scale (4) Secure.

##  2. <a name='UnderstandDataAIMaturityFramework'></a>Understand Data & AI Maturity Framework 

Data is a broad definition, including all the types of information your organisation collects, stores, analyses, and uses. It can be recorded in many formats: numbers, text, images, video, maps. Data maturity is a measurement of how advanced a company’s data analysis is. A high level of data maturity is the stage reached when data has woven its way deeply into the fabric of an organization and when data has become incorporated in every decision that an organization makes. Some great examples of advanced data maturity are early data innovators that are already proving to be dominant in their industries. Companies like AirBnb, Uber and Netflix take data so seriously that it’s more accurate to call them data companies than to consider them traditional competitors in the hospitality, transportation or entertainment industries.

I would like to introduce Data & AI Maturity Framework by University of Chicago Center for Data Science & Public Policy consists of the following considerations:

1. Problem Identification - Problem Definition, Impact, Available Data, Data Fields, Size, and Target Population.
2. Data Governance Capability - Ownership, Physical Accessibility, Data Security Policy (HIPPA, FERPA etc.)
3. Implementation and Maintanance - Technical Implementation, Data Infrastructure, Maintenance.
4. Data Readiness - Accesibility, Storage, Integration, Relevance & Sufficiency, Quality, Collection Frequency, Granularity, History, Privacy Policies, Documentation.
5. Organization Readiness - Staff Buy In, Data Collector Buy In, Leadership Buy In, People Resources, Data Use Policy, Intervenor Buy In, Funder Buy In.

* [Data Maturity Framework by University of Chicago Center for Data Science & Public Policy](https://docs.google.com/spreadsheets/d/1UUOCau_xxVReQqbdI7GP321rrRSD0yozu22kROp1u8s/edit#gid=1662346894)

A range of variation on data maturity assessment are available:

* [GCP Cloud Maturity Assessment](https://digitalmaturitybenchmark.withgoogle.com/cloud/)
* [AWS Maturity Model](https://d0.awsstatic.com/whitepapers/AWS-Cloud-Transformation-Maturity-Model.pdf)

##  3. <a name='DeployEnterpriseDataEstate'></a>Deploy Enterprise Data Estate

Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently. Terraform can manage existing and popular service providers as well as custom in-house solutions.

Configuration files describe to Terraform the components needed to run a single application or your entire datacenter. Terraform generates an execution plan describing what it will do to reach the desired state, and then executes it to build the described infrastructure. As the configuration changes, Terraform is able to determine what changed and create incremental execution plans which can be applied.

The key characteristics of Terraform are:

1. Infrastructure as Code (IaaC)
2. Execution Plans
3. Resource Graph
4. Change Automation

Let's implement and deploy Azure Data Services using Terraform ([rlevchenko/terraform-azure-data: Terraform script to deploy almost all Azure Data Services](https://github.com/rlevchenko/terraform-azure-data)). In particular, we are going to deploy:

* Azure Service Bus (Standard, namespace,topic,subscription, auth. rules)
* Azure Data Lake Storage (ZRS, Hot, Secured, StandardV2)
* Azure Data Factory (w/Git or without)
* Azure Data Factory linked with Data Lake Storage
* Azure Data Factory Pipeline
* Azure DataBricks WorkSpace (Standard)
* Azure EventHub (Standard, namespace)
* Azure Functions (Dynamic, LRS storage, Python, w/App.Insights or without)
* Azure Data Explorer (Kusto, Standard_D11_v2, 2 nodes)
* Azure Analysis Server (backup-enabled,S0, LRS, Standard)
* Azure Event Grid (domain, EventGridSchema)
* Azure SQL Server (version 12.0)
* Azure SQL Database (ElasticPool, 5 GB max data size)
* Azure SQL Elastic Pool (StandartPool, LicenseIncluded, 50 eDTU, 50GB max data size)

This extensive list of Azure Data Services is customizable according to your environment. Therefore, please feel free to add or remove the services as needed for your project. 

##  4. <a name='AdditionalResources'></a>Additional Resources

* [AWS Cloud Adoption Framework](https://aws.amazon.com/professional-services/CAF/)
* [Microsoft Cloud Adoption Framework for Azure - Cloud Adoption Framework | Microsoft Docs](https://docs.microsoft.com/en-us/azure/cloud-adoption-framework/)
* [Cloud Adoption Framework  |  Google Cloud](https://cloud.google.com/adoption-framework)
* [Deploy Azure Data Services with Terraform – UseIT | Roman Levchenko](https://rlevchenko.com/2020/09/15/deploy-azure-data-services-with-terraform/)
* [rlevchenko/terraform-azure-data: Terraform script to deploy almost all Azure Data Services](https://github.com/rlevchenko/terraform-azure-data)
* [Introduction - Terraform by HashiCorp](https://www.terraform.io/intro/index.html)
* [Data Maturity Framework – Center for Data Science and Public Policy](http://www.datasciencepublicpolicy.org/home/resources/datamaturity/)