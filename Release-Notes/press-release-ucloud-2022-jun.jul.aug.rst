uCloud - Press Release June|July|August - 2022
===============================================

.. figure:: /figuras/ucloud.png
   :alt: Logo uCLoud
   :scale: 60 %
   :align: center
   
----

.. centered:: Português_     -     Español_     -     English

.. _Português: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Release-Notes/nota-de-lançamento-ucloud-2022-jun.jul.ago.html 

.. _Español: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Release-Notes/notas-de-publicación-ucloud-2022-jun.jul.ago.html

====

2022.06-08
++++++++++

Press Release: uCloud
=====================
Period: June | July | August 

Version: `Update tags 5.3-b56 and 1.0-account88`

====

Introduction
============

Ustore renews the uCloud platform in line with the continuous evolution of innovations in the cloud computing industry, a dynamic environment that allows remote access to softwares, files storage and data processing via the Internet.

This release evokes the principle of the ISO 9001 standard, prepared by the International Organization for Standardization (known in Brazil as ABNT NBR ISO 9001). The objective of which is to establish consistent standards that increase the quality of the applied processes and result in continuous improvement and adjustments in functionalities, in the pursuit of quality management and business excellence.

The improvements presented below refer to the quality management principle mentioned in the ISO 9001 standard, carried out during the months of June, July and August of the current year.

====

News
====

This press release discloses the thirty-three global improvements made to some of the portal’s functionality menus, fourteen adjustments made to cloud changes and the seven new implementations. They are categorized into:

* Public and private clouds;

* uCloud Platform Enhancement in Account, uCloudOPS and Billing;

* New implementations.

====

Public and Private Clouds
=========================

Amazon Web Services (AWS)
-------------------------

Regarding the interaction with the Amazon Web Services (AWS) public cloud service provider:

* From this note, the Container Import can be performed solely for invoicing.

Microsoft Azure (Azure)
-----------------------

Regarding the interaction with the AZURE Microsoft public cloud service provider, three improvements can be listed:

* Changing the graphical interface of the Scaling Group creation button;

* For the best user experience, the option is to hide the Security Group field from VDCs;

* Perform Container Import only for billing.

Google Cloud Platform (GCP)
---------------------------

Concerning the interaction with the Google Cloud Platform (GCP) public cloud service provider, there were eight improvements listed below:

* The button to associate the disk with the VM receives a new graphic interface;

* Improved standard user agreement when creating a DBVM;

* Added the loadbalancers breakdown of a Scaling Group;

* Adaptation of Google-type Container Import;

* Inclusion of new regions, they are:

  * Melbourne, Victoria, Oceania: australia-southeast2.

  * Delhi,  National Capital Territory, Asia: asia-south2.

* Selection refinement to associate subnet with the Container Import;

* Zone binding when creating VM;

* New invoicing filters:

  * **Discount**: The discount credit type is used for amounts received after a contractual spend limit has been reached. In the Cloud Billing reports available in the console, this is listed as “Discounts based on (contractual) spend”.

  * **Free tier**: Some services offer “free use of resources up to specified limits”. In these services, credits are applied to implement the free tier usage.

  * **Promotion**: Promotional credit type includes “Google Cloud free trial and marketing campaign credits of other grants for  using Google Cloud”. When available, promotional credits are considered a form of payment and are automatically applied to reduce the total invoice. 



VMware 6.5 or superior (vCenter/vSphere)
----------------------------------------

Regarding the interaction with the VMware hypervisor 6.5 or superior, the following improvement is related:

* The scheduling policy for Scaling Group allows the user to create the policy that defines when to create new machine(s).

====

uCloud Platform Enhancement in Account, uCloudOPS and Billing
=============================================================

At Ustore, the practice of continuous improvement adopted to improve the uCloud platform, associated with productivity, results in the following list:

* User creation in Account: Shortcut to create a user directly in the Administration menu, Account submenu.

* Alphabetical listing of container and VDC on security group creation screen: when listing the VDCs on security group creation, the display is in alphabetical order.

* Listing in alphabetical order of container and VDC on the screen of a creating network: The screen of creating a network presents the list in alphabetical order of container and VDC.

* Listing in alphabetical order by container and VDC when creating the Public IP: When creating the Public IP, the list presented, of the container and the VDC, is in alphabetical order.

* uCloud interface security enhancement: Security improvements were made to the uCloud Front-End.

* The user’s language can be switched at the account level, in addition to the existing user level: therefore an account can have a language and be seen by the language that the user determines.

* Persistence of the user language switching: the platform maintains the language chosen on first access. 

* Language persistence when sending emails within the portal: The platform maintains the chosen language when sending emails.

* Adaptation of the list of permission and visualization profiles in the graphical interface: the list of profiles appears above the modal, making visualization easier.

* Creation of Virtual Tags with the same key, but with different values: this improvement allows the creation of one or more Tags with the same keys and different values.

* uCloud CORE.sql update: Significantly speeds up the environment response.

* Quotas update across the entire uCloud platform: The unification of quotas in all environments standardizes the visualization of user quotas in the contract and group functionalities.

* In the Configuration functionality menu, the General submenu includes the addition of the button (ON/OFF) in automatic activation and uCloud v.2, this button indicates that the function is enabled or disabled.

* Updated password recovery format.

* Improvement in the customization of branding in the billing features menu for the mobile version, in order to ensure the best view in the light and dark mode options.

* In the Tasks menu, in the list of tasks in operation, the “Actions” column allows the user to cancel or pause a Task regardless of its status, as long as the percentage is below 99%.

* Update on the “Checkbox” functionality associating all VMs in the contract and in the group.

* In the Administration Menu, when clicking on the Contracts submenu and selecting a specific Contract from the list, it is allowed to "Add Administrators" either user or user group. To facilitate the search, a search bar has been added, which returns the name of a user or a group as a result.

* Quota creation by quantity of VM/Instance per contract.

* Workflow adaptation to support the chaining of several tasks (sequentially and/or parallel form, with no maximum number) of existing workflows in the portal.

* Task approval when exceeding quota: When a user exceeds the existing quota in the contract automatically the administrator realizes that the user needs more quota. Thus, the administrator may approve or nor this request.

* New presentation of the Financial Report in the Billing data interface.

* CentOS7 option for ResourceKey creation: Cloud requirement met with the addition of CentOS7 as Operating System to tag USN.

* Kubernetes to create ResourceKey: addition of Kubernetes as Operating System as a Google requirement for tagging Kubernetes machines.

* The Virtual Tag Profile menu enhances the user experience by allowing similar names in virtual tag profiling and preventing the use of special characters.

* Increment of the Virtual Tag Profile by including the uCloudIdentifier blank that is used as a reference. It is applied in container and ticketing operations.

* The Services Catalog menu after refactoring the transmission point and receiving 'endpoint' information details the result only when the user requests the search.

* Associate the same USN Tag price for various contracts: removed tag restriction for only one contract.

* The Tasks menu receives the update of the record of tasks in the activities occurred in Billing within the portal.

* Adding variables when creating a virtual tag.

* Improved consumption monitoring Report: Addition of the Universally Unique Identifier - UUID of the container, optimizes the closing of the contract invoice that monitors consumption.

* The detailed invoice Summary screen increases data loading and makes the delivery of the request result faster in your interface

* Improved visualization of invoice closing with multi-contract users: A user linked to more than one contract has the option to see the invoice closing with the expenses of each specific contract individually.

====


New Implementation
==================

In this report, Ustore discloses the seven new innovations that occurred in the uCloud platform, briefly described below:

1. **Budget**: Corresponds to a consumption-based report that aims to define the total budget for a given period, whether it is monthly, quarterly, semiannual or annually. This report makes it possible to monitor the Budget usage.

2. **Contract-level branding customization**: Multicloud portal branding is allowed through contract-defined customization. The user client can select the characteristics of his brand (Company) represented in the Multicloud portal such as colors, logo, among others.

3. **Dimension**: To avoid the same resources being tagged differently, the dimension was created to group the distinct tags to resources of the same context. For this, logical operations and filters were created, in order to identify in Billing which resources belong to a given dimension.

4. **Import and Export of service offers in (XML + YAML)**: In this new functionality it is possible to import and export the same offer from any cloud, as long as it is linked to the uCloud Portal. Before, it was possible to import and export files in JSON format, then it was added the options of importing and exporting files in XML and YAML as well.

5. **Import of Google Credentials in AWS Secret Manager**: Secret Manager is a repository where information that only the user has access to is stored. To import this user’s Google credentials data, the action must be done through the uCloud so these are transferred to the hidden AWS repository.

6. **Account Level Permissions**: This new functionality optimizes the user’s permission process. In this account-level permission mode, the user can perform actions from the permission profile created for them, whether basic or advanced. This user has the power to administer several contracts linked to an account, according to the permissions granted to them.

7. **Consumption Monitoring Report V1**: New uCloud functionality that deals with the complete breakdown of expenses, divided by Clouds, Contracts and Resources. Different types of reports are generated, for each type of division (Cloud/Contract/Resource), separating them one at a time and organizing them from the largest to the smallest consumption. In addition to comparing the expenses of previous months, providing the customer with the necessary information so that they can assess whether there has been a decrease or increase in expenses.

In summary, the document presents the fourteen (14) improvements made in the public and private clouds category due to the demand in adapting to changes in these providers. The thirty-three (33) global enhancements to the uCloud platform. In addition to the seven (7) new implementations. Thus, the document is concluded with the release notes for this quarter corresponding to the months of June, July and August of the current year.