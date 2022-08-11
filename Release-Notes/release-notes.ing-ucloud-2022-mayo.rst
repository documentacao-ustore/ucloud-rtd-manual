Release Note May – 2022
=======================

.. figure:: /figuras/ucloud_logo_peq.png
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

* New execution in the Listeners and Members of a Balancer functioning .

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

#. Update price table for flavors.

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

To exemplify a way to charge for the “service offering” of Centralized Cloud Management by the uCloud Platform, we will use the example of “consumption levels” of computing infrastructure based on the number of Virtual Machines Managed by the uCloud Platform, called “Tier. The Tiers represent the existing billing model in the “Accounts” functionality, the business rule created establishes the accounting of the resources obtained and generated by a given account.

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

Just for the purpose of exemplifying a scenario,we will describe the offer of services to use the uCloud Platform in the SaaS (Software as Service) modality to the Galaxy company, and in its “Account” there are 20 Virtual Machines (active and managed by uCloud Platform), it fits in the Tier level “A” - the monthly amount to be invested by the Galaxy Company will be R$1,500 reais or dollars (depends on which country the company will be established). An important observation, in case the account uses only 18 machines, it will still be classified in Tier “A”.

Segmentation by Accounts
------------------------

There are two classes of “Accounts”, they are categorized into two types, the accounts in the **Integrator** type and the **Producer** type, detailed below:

* \ A. \ **Integrator Account** This account is responsible for creating the profiles of  the integrator and producer accounts, when creating these profiles, it feeds the tiers and the packages, in addition to establishing, the producer account its usage rule. 

  * To exemplify:

  It works as a kind of cluster, agglomerating and categorizing other corporations.

  * For example: 

  In case of a multinational corporation using an Integrator account, it can be considered an “Integrator Account” for the countries that comprise it: Mexico, Brazil, Chile and Colombia.

  The corporation is responsible for creating other accounts and escalating the other users' permissions. Its particularity is the list of all the producer accounts, the list of all associated contracts and can apply business rules.

* \ B. \ Producer Account This producer account belongs to the organization which consumes the resource, represents a minor clustering unit and can operate the entire portal.

  * For example: 

  Resuming the example above, this multinational corporation creates the “producer accounts” for the organizations that belong to it within a certain country listed above, in Brazil, the organization has companies A and B which administers the contracts a1 and b1.

  Below is an illustration that represents the complete concept of the scope of the “Account” functionality implemented in the uCloud Platform. The names and denominations used are merely illustrative.

  .. figure:: /figuras/ucloud_arquitetura_conceitual003.png
   :align: center
   
----

The Producer Accounts can have one or more administrators (in this level the profile of this user is one of System Administrator - ex.: root), the contracts stop being created when the corporate resource ends, the visualization profiles and permission obey the business rule applied by the integrator account. 

The strategy of using the “Accounts”  functionality provides a better perception of value at the level of hierarchy that wants to organize the data within the context of organization, by facilitating its transit at the operational, managerial and executive levels.

With the creation of this functionality, the account administrator can manage the visualization and the permission of each user within each **group**, contained in a given **contract**. In this way, the access is denied by default, being granted only when the permissions specify “allow”. 

Additionally, the functionality “Accounts” makes it possible to use the control policies that establish the protection barrier of permission and visualization for users, depending on the characteristics of the type of user, group and contract to which it belongs. 

By establishing these defaults of permission, access and resources visualization, it organizes and qualifies the privilege each user will have within the environment the public cloud providers in each contract/group/user belongs, creating that way, different and necessary permissions to create minuncious controls in each account.

Description of Virtual TAGs 
===========================

In a broad context, a TAG (a label) it’s a keyword that signs or identifies a particular computational resource (or s service resulting from its existence) stored in a cloud provider, repository or database. The TAGs are a type of metadata, capable of providing information that describes the data, this facilitates automated search for information retrieval. A TAG is a label in which the user assigns a **Key** and a **Value** to a public cloud computacional resource.

In the scenario of any type of cloud, the data contained in TAGs is used together with other forms of tagging that the cloud providers use to classify information about their resources. Thus, the TAGs help the research, organization, identification, management and, finally, the filtering of used resources in any cloud provider, for example: AWS, Azure, Google, among others. 

These TAGs (labels) after linking to a resource are used to categorize these resources so they can be classified by: purpose, property, criteria or location. For example: the user or the organization, can define a set of TAGs for the Amazon EC2 instances, of their account, to help track the owner and/or clustering level (stack values) of each computacional resource of the public cloud consumed.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual001.png
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

.. figure:: /figuras/fig_release_note_maio_ing/ucloud_tabela_tag_virtal_maio_ing0001.png
   :align: center

----

