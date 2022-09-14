uCloud - Release Note May – 2022
================================

.. figure:: /figuras/ucloud.png
   :alt: Logo uCLoud
   :scale: 50 %
   :align: center
   
----

uCloud platform version: *update tag 5.2-b35*

Introduction
============

In general, the IT infrastructure professional uses several consoles to provision computational resources, whether it is within the organization (private data center) or in a cloud provider. The computation in cloud is an evolution of information technology’s services and products on demand, called Computing Utility by Brantner et.al., 2008, to which the objective is to provide basic components such as: storage, processing and network bandwidth through specialized providers with a low cost per unit used. In contemporaneity, keeping up to date and prepared, in all the consoles is a challenge for this professional.

In an attempt to increase productivity and reduce the degree of dependence on these consoles, the market developed the concept of Infrastructure as a Code (Iaac). This concept only addresses the moment of initial provisioning (even with the use of scripts for installing patterns and softwares), there may be demands in which the IT professional must connect to the environment console, to perform some intervention in the infrastructure that is not possible through the IaaC concept. Being connected and alternate between the several cloud consoles demands a great specialization and knowledge from the IT professional.

The CSB (Cloud Service Broker) platforms were developed to occupy this niche and concentrate the inventory of computational resources from public and private clouds in a single interface that transfers control and operation of these multi-cloud resources to the user. 

As mentioned, the market itself developed provisioning computacional resources methodologies through automated scripts (also called playbooks). Among these formats there are some that the world market has adopted more widely, such as Ansible, Terraform and Puppet.

The market has also created the demand for programming the execution of a several scripts sequence within a controlled and linked flux, so that an error in one of these scripts can interrupt the entire flow to avoid provisioning an infrastructure without its due quality. 

Alert to the constant evolution in the Brazilian market and to our users demands, the Ustore introduces new implementation, corrections, integrations, updates in the functionality menu and its detailed description.

In addition to expanding the existing concept, this release notes details the updates occurred in the uCloud Platform, included in (*tag.5.2-b35*) attending to the several market demands of our clients, capable of transforming the public and private clouds management form with the uCloud platform.

New implementations 
===================

The news presented below were categorized into:

* Corrective actions to adapt to changes occurred in the cloud providers;

* The integrations executed in the portal;

* Global updates in some functionalities menu from the portal.

In addition to the most robust innovations, listed in three themes. These new implementations will be described, in detail, through this document.

#. Account 

#. Virtual TAGs 

#. Oracle Cloud Infrastructure

Corrective Actions
==================

In this release notes are listed all the corrective actions implemented, motivated by certain situations reported to our development team.

Amazon Web Services (AWS)
-------------------------

Regarding the interaction with the AWS public cloud service provider, there have been no alterations, fixes, new implementations or new functionality.

Microsoft Azure (Azure)
-----------------------

Regarding the interaction with the Microsoft Azure public cloud service provider, we can list the following alterations:

#. Adaptation of the Scaling Group to suit the update in the response model sent by the cloud. After this implementation, by creating a Scaling Group the process automatically creates an Instance Group, to be managed by this Scaling Group.

#. Adjustment to the model for handling the deletion of disks associated with Virtual Machines. This improvement was necessary because there was a change in the way the deletion is done in the cloud. Adaptation in the PMC to accompany this improvement.

Google Cloud Platform (GCP)
---------------------------

Regarding the interaction with the Google Cloud Platform (GCP) public cloud service provider, we can list the following alterations:

* New execution in the Listeners and Members of a Balancer functioning.

* Addition to the support by creating the Balancer using the HTTP protocol.

* UDP (User Datagram Protocol) rule application to Security Groups.

* New region inclusion, such as:

  * Columbus, Ohio, North America: us-east-5
  * Dallas, Texas, North America: us-south1
  * Madrid, Spain, Europe: europe-southwest1
  * Milan, Italy, Europe: europe-west8
  * Paris, France, Europe	: europe-west-9

Huawei Cloud (Huawei)
---------------------

Regarding the interaction with the Huawei Cloud public cloud service provider, there was no alteration, correction, nem implementation or new functionality. 

IBM Cloud
---------

Regarding the interaction with the IBM Cloud public cloud service provider we can list the following alteration:

#. Implementation of the business rule to disable editing the single NIC (Network Interface Cloud) of the Virtual Machine.

VMware 6.5 or superior (vCenter/vSphere)
----------------------------------------

Regarding the integration with the VMware 6.5 (or superior) private cloud hypervisor, we can list the following alterations:

#.	Update on how to create a subnet to suit the new uSDN version.

#.	Anomalous behavior corrected, multiple connections opened at the same time.

VMware vCloud
-------------

Regarding the interaction with the VMware 6.5 (or superior) private cloud hypervisor, we can list the following alterations:

* Container importation correction.

* API update to version 35.0.

Integrations
------------

* There was one implementation and improvement of communication with the monitoring agent (Mangue/uCloud)

Updates
-------

Below is the update list that have been implemented on the uCloud Platform:

#. Expansion of the coverage of translations of portal elements or items, both into Spanish and English.

#. Update price table for Flavors.

#. Review of communication in portal exception messages, focus on user interaction with content and user experience.

Virtual Datacenter Menu (VDC)
-----------------------------

#. Reduction of loading time within the VDC editing screen of a container.

Visualization Profiles Menu 
---------------------------

#. Addition of uLog and uMonitor modules as selection option in Visualization Profiles.

Description of New Implementations
==================================

Below is described the technical and operational characteristics of three new implementations that were applied to this new uCloud Platform version/release. In this chapter are listed the new implementations and they will be clarified in the course of this document.

#.	Account 

#.	Virtual TAGs 

#.	Oracle Cloud Infrastructure (OCI) - Operation functionalities only. 

Account Description
===================

The uCloud Platform can be implanted in two different ways:

\ A. \ Dedicated installation (on-premises)

For the dedicated installation scenario (on-premises) the Account functionality may not be applied, probably this installation only belongs to a single company, and this company will not share the uCloud Platform between other organizations. Still in this scenario, we will assume that the installation of the uCloud Platform will only be used in their own cloud(s) (public and/or private).

\ B. \ Installation shared as a service (SaaS - Software as a service)

The Account functionality was designed for the shared installation (SaaS) scenario, where the company (we will call it **organization**) aims to provide a Cloud Service Broker service with the uCloud Platform between its various operations (regional or international) and for its several final-customers.

The scenario uCloud Platform SaaS described above is ideal to the connectivity/communication service provider (**organization**) which can share the uCloud Platform among its regional operations and, also, between its final customers that wish the benefits of an operation, financial governance and billing.

This functionality helps the management and the organization environment control, in a centralized manner, by its the business rule makes it possible to create the “Accounts” and allocate the Contracts, the Groups and its Users (elements belonging to the Switch Roles” universe). 

It makes it possible to organize and share the resources between the created “Accounts”, besides applying the service control policies to **contracts**, **groups** and **users**, optimizing the governance upgrade. This new model inserts the layer “Account” in the **Administration** menu which represents a new process to promote the alignment around the “Accounts” functionality and, that way, to conduct the organizations to obtain a greater control.

This functionality “**Accounts**” has the objective to provide to the organization the possibility of segmenting customers by size (Virtual Machines), by revenue volume (financial costs), makes it possible to understand the development by “Account” and filter its history by line of business.

To exemplify a way to charge for the “service offering” of Centralized Cloud Management by the uCloud Platform, we will use the example of “consumption levels” of computing infrastructure based on the number of Virtual Machines Managed by the uCloud Platform, called "Tier". The Tiers represent the existing billing model in the “Accounts” functionality, the business rule created establishes the accounting of the resources obtained and generated by a given account.

In the portal, the Tiers are categorized in levels from A to J (1 to 10) and calculated based on the rules established using two parameters: - certain numbers of Virtual Machines generates a determined maximum cost (number of machines versus cost/value). In case of a created account, upon reaching one of the parameters, the application immediately scales to the next level. The Tiers level follows below: 

+-----------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+
| **Tier**              |  **A** |  **B** |  **C** |  **D** | **E**  |  **F**  |  **G**  |  **H**  |  **I**  |  **J**  |
+=======================+========+========+========+========+========+=========+=========+=========+=========+=========+
|| **Quantity of**      ||       ||       ||       ||       ||       ||        ||        ||        ||        ||        |
|| **Virtual Machines** || ≤ 20  || ≤ 30  || ≤ 50  || ≤ 75  || ≤ 100 || ≤ 150  || ≤ 200  || ≤ 250  || ≤ 300  || ≤ 500  |
+-----------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+
| **Monthly amount**    | $1.500 | $3.000 | $4.000 | $6.000 | $8.000 | $16.000 | $24.000 | $32.000 | $40.000 | $64.000 |
+-----------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+

.. attention:: All quantities and values presented above are merely illustrative, serving only as examples.

Example Use Cases:
------------------

* Galaxy Company Contract (qty. VMs 20):

Just for the purpose of exemplifying a scenario, we will describe the offer of services to use the uCloud Platform in the SaaS (Software as Service) modality to the Galaxy company, and in its “Account” there are 20 Virtual Machines (active and managed by uCloud Platform), it fits in the Tier level “A” - the monthly amount to be invested by the Galaxy Company will be R$1,500 reais or dollars (depends on which country the company will be established). An important observation, in case the account uses only 18 machines, it will still be classified in Tier “A”.

Segmentation by Accounts
------------------------


There are two classes of “Accounts”, they are categorized into two types, the accounts in the **Integrator** type and the **Producer** type, detailed below:

* \ A. \ **Integrator Account** This account is responsible for creating the profiles of  the integrator and producer accounts, when creating these profiles, it feeds the tiers and the packages, in addition to establishing, the producer account its usage rule. 

  * To exemplify:

  It works as a kind of cluster, agglomerating and categorizing other corporations.

  * For example: 

  In case of a multinational corporation using an Integrator account, it can be considered an “Integrator Account” for the countries that comprise it: Mexico, Brazil, Chile and Colombia.

  The corporation is responsible for creating other accounts and escalating the other users` permissions. Its particularity is the list of all the producer accounts, the list of all associated contracts and can apply business rules.

* \ B. \ **Producer Account** This producer account belongs to the organization which consumes the resource, represents a minor clustering unit and can operate the entire portal.

  * For example: 

  Resuming the example above, this multinational corporation creates the “producer accounts” for the organizations that belong to it within a certain country listed above, in Brazil, the organization has companies A and B which administers the contracts a1 and b1.

  Below is an illustration that represents the complete concept of the scope of the “Account” functionality implemented in the uCloud Platform. The names and denominations used are merely illustrative.

  .. figure:: /figuras/figuras-release-notes-ingles-espanhol/ucloud_arquitetura_conceitual003-us-en.png
   :align: center
   
----

The Producer Accounts can have one or more administrators (in this level the profile of this user is one of System Administrator - ex.: root), the contracts stop being created when the corporate resource ends, the visualization profiles and permission obey the business rule applied by the integrator account. 

The strategy of using the “Accounts”  functionality provides a better perception of value at the level of hierarchy that wants to organize the data within the context of organization, by facilitating its transit at the operational, managerial and executive levels.

With the creation of this functionality, the account administrator can manage the visualization and the permission of each user within each **group**, contained in a given **contract**. In this way, the access is denied by default, being granted only when the permissions specify “allow”. 

Additionally, the functionality “Accounts” makes it possible to use the control policies that establish the protection barrier of permission and visualization for users, depending on the characteristics of the type of user, group and contract to which it belongs. 

By establishing these defaults of permission, access and resources visualization, it organizes and qualifies the privilege each user will have within the environment the public cloud providers in each contract/group/user belongs, creating that way, different and necessary permissions to create minuncious controls in each account.

Description of Virtual TAGs 
===========================

In a broad context, a TAG (a label) it’s a keyword that signs or identifies a particular computational resource (or service resulting from its existence) stored in a cloud provider, repository or database. The TAGs are a type of metadata, capable of providing information that describes the data, this facilitates automated search for information retrieval. A TAG is a label in which the user assigns a **Key** and a **Value** to a public cloud computacional resource.

In the scenario of any type of cloud, the data contained in TAGs is used together with other forms of tagging that the cloud providers use to classify information about their resources. Thus, the TAGs help the research, organization, identification, management and, finally, the filtering of used resources in any cloud provider, for example: AWS, Azure, Google, among others. 

These TAGs (labels) after linking to a resource are used to categorize these resources so they can be classified by: purpose, property, criteria or location. For example: the user or the organization, can define a set of TAGs for the Amazon EC2 instances, of their account, to help track the owner and/or clustering level (stack values) of each computacional resource of the public cloud consumed.

.. figure:: /figuras/figuras-release-notes-ingles-espanhol/ucloud_menu_configuracao_tags_virtual001-en-us.png
   :align: center

----

.. note:: The picture above is an example and the information present is merely illustrative. 

In the picture above we use two Virtual Machines as an example of how to illustrate the link between TAG and resources. A detail that is mentioned very little is that the public cloud service providers don’t allow linking TAGs to all their products and/or services (check the provider documentation to know which resources are likely to have a TAG linked to the resource).

In the example above we link “two different TAGs” to the same resource (Virtual Machine) in this way we induce that the financial reports by TAG totaled the cost value of the TAG twice (the same value in each TAGs) and, for this example, in this situation double the cost within the same period.

But we must highlight that to the public cloud service provider’s environment, once a TAG is created, it will not automatically be linked to any resource (or services resulting from the resource existence). The user must first create the TAG(s) and then manually link the TAG(s) to the wished resource(s). Because it is a manual process and performed by a user at the cloud service provider console, the TAGs resources can be time consuming for the public cloud Cost Administrator. There may be too many rows in the billing/bucket file for the Cost Administrator to check. This verification and the TAGs linking process is continuous and manual.

.. important:: The fact that the TAGs are accessible to many services in cloud providers, it’s important to avoid adding private or confidential data to the Virtual TAGs, as for example: personal identification, confidential or sensitive information.

The uCloud Platform synchronizes and receives the content of the billing file (CSV) from the public cloud service provider and, consequently, receives all the TAGs existing in the provider.


The uCloud Platform Virtual Tags
--------------------------------

We mentioned above that the process of linking a TAGs to a resource is manual, time consuming and, above all, it is not automatically repeated for new services of a resource that already has a linked TAG.

The new uCloud Platform Virtual TAGs functionality creates an automation for the TAGs linking process to existing resources in the public cloud service provider’s environment.
The uCloud Platform Virtual TAG process may automatically link a specific TAG to a resource to be selected based on Product Name and/or Product Family and/or Resource Identifier. It’s important to highlight the conjunction “and/or” shows the high granularity degree the user can select to attend to their specific use of their need.

See below how the new Virtual TAGs implementation allows to automate the TAGs link in resources.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual002.png
   :align: center

----

.. note:: The picture above is an example and the present information is merely illustrative.

In the example above, every time the uCloud Platform performs the billing/bucket CSV file synchronization, the TAGs will be linked automatically to all resource records (rows) in the billing file in which the Product Name or Product Family or Resource Identifier correlation is found.

The Virtual TAGs are applied in cloud resources (for example: virtual machines, databases) so it’s possible to create classification by projects, divisions by cost center, among other types of groupings.These keys and TAG values may or may not be reflected in the billing reports available to consultation only through the public cloud provider’s console. Thus, the resources imported from the bucket/billing file existing in the public cloud providers that by any policy these providers fail to index the tag to the cloud service resource, may receive a “Virtual TAG”. But it’s very important to highlight that these “Virtual TAGs” only exist in the uCloud Platform database, not being written (or synchronized) to the bucket/billing that exists in the public cloud service provider’s environment.

This is a unique service and it’s available with the new uCloud Platform implementation to facilitate the used resource classification in the **several clouds** through the “Virtual TAG”. The Virtual TAG must be created by the client organization, it can be based on the categorization profile, according to the used resource and the identification needed in the financial report, whether it is by purpose, property, criteria or location, among others. 

The Virtual TAG must be applied by the user client within the uCloud portal, in order to enable the resource automated identification that is no longer tagged by the several cloud providers with different rules and internal policies of each one of them. After the Virtual TAG application as a uCloud Platform resource and then, applying through the virtual-tag-applier Accountant, and their normalization, using the virtual-tag-normalizer Accountant. This way, the information visualization will be easier for the decision making, recorded in the financial reports, regarding the used resources provided by the several clouds that were not previously tagged by the cloud itself.

The organizations that use the automated processes to manage the infrastructure include the additional TAGs specific for automation, in general they create relevant grouping to organize the resources in technical, commercial and security dimensions.

Virtual TAGs Normalization
--------------------------

It’s important to mention the continuous existence of a cloud service provider resource, it generates new services or products resulting from the public cloud service provider resource existence/maintenance (ex.: snapshots).

When a client requests a creation of a backup copy of the new disk image (snapshot) a new snapshot may, not necessarily, receive the link of a TAG in the Virtual TAGs process.

To cover this gap there is a new **Virtual TAGs Normalization** functionality. 

This process performs a comparison of each row of the billing file and when it finds a resource with “no Virtual TAG” but this row is a new service/product of a resource with a Virtual TAG, this process MAKES A COPY of the Virtual TAG from the main resource even if its ProductName, ProductFamily, Resource Identifier combination were not able to link the Virtual TAG.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual003.png
   :align: center

----

.. note:: The table above is an example and the present information is merely illustrative.


This process may take a while, because it is performed with the string comparison of characters of each billing row individually.

With this process, the uCloud Platform complements the new Virtual TAGs functionality, but it must be executed only when the Cost Administrator user identifies that there are resources with no Virtual TAGs.

When to use
-----------

Based on this new implementation, aimed at classifying, normalization and visualization of obtained information from the public cloud several providers, the new functionality “Virtual TAGs” enables to ticket/tag, that is, mark the resources that by some rule or definition, were not possible to find registered in the billing of a certain cloud provider used by the organization or user customer. 

Once, each cloud presents different reports of used resources, the difficulty for the IT professional to be able to normalize and understand the presented classification in several clouds, or even the suppressed information by TAGs absence that group the relevant format, valuable information, whether they are quantitative, qualitative or financial, facilitating the organization and/or its user customer the possibility of an assertive decision making, when using this new implementation called “Virtual TAGs”. Developed by the Ustore as a solution to attend this absence, it claimed in the reports that it has a similar behavior in the several cloud providers, such as AWS, Azure, Google, among others. 

The uCloud portal generates the financial report, this report retrieves information by product name or by TAG. It’s the uCloud portal that offers this unique service of “Virtual TAGs” that enables and/or facilitates the management and the classification of certain resources that no longer receive TAGs in the cloud, as mentioned previously, by rules or internal policies established by the providers themselves. 

It is necessary to use this new implementation, when the organization and the user customer need to retrieve information by TAG or product name in a distinct way, in several clouds, once each cloud provider, like Google, AWS and Azure treat the billing record report differently. And each one of them uses its own nomenclatures for each type of offered resource.

By applying the “Virtual TAGs” to the cloud resources (e.g: database and virtual machines) it is possible to create classification by cost centers divisions, projects and other types of groupings.

The new implementation from the uCloud portal enables users to present the information generated in the financial report according to what was classified or tagged by the user to group or identify information, whether it is by product name, purpose, property, criteria or location, among others.

.. note:: The keys and TAGs values may or may not be reflected in the billing report of several clouds. The TAGs don’t save semantic meaning in the Amazon EC2, they are interpreted as a character sequence.

Thus, resources imported from the public cloud billing file that, by any policies of these providers, fail to index the tag to the cloud service resource, may receive a “Virtual TAG” within the portal.

TAGs Restrictions
-----------------

In case of the Virtual TAGs application, there are some tips and basic restrictions to be applied:

* **Maximum number of TAGs by resource**: 50

* **Maximum key size**: 128 characters

* **Maximum value size**: 256 characters

* **Allowed characters**: the allowed characters are: letters (a-z, A-Z), numbers (0-9) and representable spaces, besides the following characters: + - = . _ : / @.

* To enable instance tags in metadata, the instance tags keys allow use of the letters (a-z, A-Z), numbers (0-9) and the following characters: + - = . ,  _ : @. Avoid spaces or / , and it can’t form only . (a dot), .. (two dots) or _index.

.. note:: For any resource, each key tag must be exclusive and can only have one value.

.. important:: The keys and TAGs values are Case Sensitive, in other words, differentiate **UPPERCASE from lowercase**. 

.. warning:: The **aws** prefix it’s reserved for the Amazon Web Service (AWS) use. It’s not possible to edit nor exclude the key or the value of a TAG when it has a key with this prefix. The TAGs with the aws prefix: don’t count to TAGs by resource limit.

How to use
----------

This new implementation allows to tag the missing marking resources in the cloud ticketing, either by rule or definition. This results in relevant information gained from those resources that would no longer be categorized and retrieved. 

There are some common marking strategies that help identify and manage resources in the cloud, to organize resources and to allocate costs, beyond several marking categories in the cloud, AWS for example: 

* Techniques

* Automation

* Commercials

* Safety

The additional TAGs present better efficiency by creating groupings, TAGs techniques, TAGs for automation, commercial TAGs, safety TAGs. We can mention some among them: Name, Applicative ID, Applicative Function, Cluster, Environment, Version, Date/Time, Accept/Refuse/ Safety, Project. Owner, Cost Center/ Business Unit, Customer, Confidentiality and Conformity.

.. note:: The TAG behavior in the AWS cloud: the TAGs created by the system that start with aws: are reserved for the AWS use, it’s not possible to edit or exclude a TAG that starts with the aws prefix. Regarding the creation TAG limit, each resource can have a maximum of 50 TAGs created by the user.

We can summarize the Virtual TAGs functionality use process in two distinct moments:

#. **Creation and Automation in the Virtual TAGs use**;

  \ a. \ Provision an identification name for a single Virtual TAGs profile with all the TAGs links based on the Product Name and/or Product Family and/or Resource Identifier combination.

  \ b. \ Virtual TAGs Link Profile to the cloud identifier (container).

  \ c. \ Perform Billing/Bucket file processing and synchronization.

  \ d. \ Visualization of Financial reports on the uCloud Platform using totalization by **TAGs**.

  \ e. \ If its identified that there are still resources with NO TAGs (remember there are resources the public cloud service provider does not link to any TAG; or that the Product Name, Product Family, Resource Identifier combination was not enough to associate the totality of rows of the billing file), the uCloud Platform allows to address the TAGs absence with the next process.

2. **Virtual TAGs normalization**;

  \ a. \ This process should only be applied when the existing combination in the Virtual TAGs Profile cannot apply TAGs to all the resources.
  
  \ b. \ This process must be executed ONLY ONCE a month as it demands a certain time to complete the normalization of all the billing rows in the current month period. This process must be started manually and normalizes the virtual TAGs just for a single period, it’s not recurring or automatic.

The picture below presents the new implementation in the uCloud portal:

.. figure:: /figuras/fig_release_note_maio_ing/ucloud_menu_configuração_tag_virtual_ing001.png
   :align: center

----

With the addition of the new functionality in the portal and the possibility to use the Virtual TAGs to retrieve information previously tagged from the used resource in any cloud provider, uniquely, where the use can occur in two flows, detailed next:

#. Linking  a TAG to a cloud resource through the specification of a character sequence that identifies a [**ProductName**], [**ProductFamily**] and/or [**Cloud Identifier**].

  \ a. \ For this flow, the user can specify, for example, that the resource belonging to the ProductName Amazon Elastic Compute Cloud, in the [ProductFamily] **Data Transfer**, linked to the cloud identifier i-0e85640d78d096974 has the TAGs specified  in the form, even if these TAGs are not provided by the cloud.

.. figure:: /figuras/fig_release_note_maio_ing/ucloud_menu_configuração_tag_virtual_ing002.png
   :align: center

----

.. figure:: /figuras/fig_release_note_maio_ing/ucloud_menu_configuração_tag_virtual_ing003.png
   :align: center

----

  \ b. \ Virtual TAGs Link Profile created, to the cloud (container) provisioned on the uCloud Platform.

.. figure:: /figuras/fig_release_note_maio_ing/ucloud_menu_configuração_tag_virtual_ing004.png
   :align: center

----

2. Normalization of TAGs for resources where TAGs are not returned by the cloud in the product family.

  \ a. \ For this flow, it will be possible to enable that in the act of the cloud ticketing data collection, the obtained resources do not come by default with the cloud provider TAG, they will be normalized with the TAGs that are associated with this resource.

  * If there already is a TAG with the same key on the other side, the TAG will not be overwritten. 
  
  * All the hyper Identifiers that belong to the same [productName].

When exporting the billing report, the “Virtual TAGs” return to normal, according to the resources used in the TAGs.


.. figure:: /figuras/fig_release_note_maio_ing/ucloud_menu_configuração_tag_virtual_ing005.png
   :align: center

----

The picture above presents the Virtual TAGs application, by the virtual-tag-applier Accountant, and its normalization, using the virtual-tag-normalizer Accountant.

Oracle Cloud Infrastructure (OCI)
=================================

With the organizations needing to maintain a consistent performance, they tend to adopt the strategy of using multiple public cloud providers. To attend to this demand, the Ustore launches the new implementation “Oracle Cloud Infrastructure (OCI), integrating the OCI public cloud with the uCloud portal.

This new release of the uCloud Platform, provides only the OCI infrastructure operation functionalities, according to the list below.

From this release notes, our portal to give support to the cloud, available the resources and functionality of **embitne Operation** OCI listed next: 

.. figure:: /figuras/fig_release_note_maio_ing/ucloud_tabela_oracle_ing0002.png
   :align: center

----

It should be noted that the current list of functionalities above is directly related to the availability of functionalities present in the current Software Development kit (SDK) published by Oracle, and was used by the Ustore DevOps team (May/2022) for integration with the Oracle Cloud Infrastructure.

The continuous development of both the DevOps team at Ustore, as well as the expansion of new functionalities present in other evolutions of the Oracle SDK, provides the evolution of releases and/or versions of the uCloud Platform, which will be listed in the future Release Notes of the uCloud Platform.

.. note:: In the present moment of this Release note (May, 2022) the API and the SDK for the OCI still does not allow the complete support to the collect implementation and billing infrastructure calcule present in the OCI environment. We await the SDK and API Oracle Cloud Infrastructure evolution to implement the billing functionality for OCI.

This set of new functionalities implemented and described, contained in this document, generated the development of this new version (update tag.5.2-b35). Thus, Ustore reaffirms its constant commitment to evolving the platform and aligning it with the needs of the market and its customers.