

.. image:: /figuras/ucloud.png
   :alt: logo ucloud
   :align: center

----

.. centered:: Português_     -     Español_     -     English

.. _Português: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/usr-manual.html

.. _Español: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuales/ucloud-usuario.spa.html 

====

User manual
+++++++++++

Information technology solutions that make it possible to implement a scalable, solid and reliable computing architecture in a hybrid cloud.

====

Presentation
============

This document has as objective to explain the uCloud portal usage, a Cloud Service Broker Platform that allows the administration of several cloud service providers, whether they are private or public cloud providers.

In this manual are presented all the concepts, screens, functionalities and the usage commands for this product.


====


Introduction 
===========

The business organizations incorporate the cloud as a solution to manage their environments when using a combination of private and public clouds, the current great challenge is the management of these hybrid multi-cloud environments.

To reach a unified vision, as well as obtaining a control of the financial costs in a centralized way, since each business organization has a necessity and faces different challenges. 

The uCloud platform was developed for these scenarios, independently of how many providers (publics and/or privates) there are the user can interact with their platforms: 

* Infrastructure as a Service (IaaS);
* Platform as a Service (PaaS).


As previously mentioned, the uCloud is positioned with a Cloud Service Broker (CSB) platform that allows to manage multiple cloud services providers - privates as well as public cloud providers. 

A CSB platform such as the uCloud platform allows the organizations to act in five fundamentals points for the management of hybrid multi-cloud environments, they are:


====

Financial Governance
--------------------

Besides the infrastructure control, the uCloud platform allows the user companies of this application to establish goals, financial as well as quantitative resources (quotas). This financial or infrastructure limits, can be applied in three levels:


* For a general public provider (see the item Companies, in the Administration menu);

* For a group of users (see the item Groups, in the Administration menu);

* For a user/individual (see the item Users, in the Administration menu).


Therefore, the organization applies criteria of financial governance and expenses control, it also can follow the costs of its hybrid multi-cloud environment through a single interface.

The adoption of the financial limit (quotas) application and/or computing resources in which several levels reach the user level, as well as the expenses control is effective and allows to avoid that the organization's budget exceeds the limit and it is surprised with situations in which the computing infrastructure cost is exorbitant or above the pre-established values. 

Another aspect of the uCloud platform is the reduction of the certification cost and specialist training, in each one of the interfaces of each provider (public and/or private), seen as the application of a usage interface and single management is simple, it allows to extract more productivity from the cloud provider environment.

Even if the user does not have training or certification on the provider specific console (public and/or private), the uCloud platform makes it possible for the user to provision a computing resource on the desired environment in a simple and easy way.


====

Billing (Services Invoicing)
----------------------------


The uCloud platform provides the business organizations with the recurrent costs information, this consumption regards to the usage of the computing resources on the operation(s) in a hybrid multi-cloud environment. This is only one of the points that are part of the Cloud Financial Management (FinOps) practice.

It is important to highlight that, individually, the uCloud platform does not meet all the three pillars of the FinOps practice by default. The Ustore has other products that can be complementary and these products' set has the potential to act as an environment able to comprise and meet the FinOps practice.

The question supported by the uCloud is the Inform point, the other points of this better FinOps practice: the Optimization and Operation belong to the other products of the Ustore's portfolio that complements the uCloud platform.

It must be clarified that the uCloud platform does not create nor generate computing resource values, these amounts are generated in the public cloud providers which the uCloud application extracts (by downloading) the billing file (invoicing) of these providers. Then, add this information in their internal database. So that, according to the contract's commercial criteria can be applied and, later, these costs calculated and converted to the current currency in Brazil.

That way, the user stays informed of the costs evolution and can follow if these costs are found within the organization's financial governance criteria. 

Generally these costs are presented in non-structured text files (*Comma-separated Values* -  CSV) generated in each period (average of 8 hours). The uCloud platform adds the information of this *.CSV* file for its internal database, with the objective to speed up and simplify the presentation of these values on the user screen.

Exclusively, the users with a specific profile can *view costs* and stay informed of the total consumption values of their computing resources in each cloud provider (public and/or private). This allows the user to follow the active computing resources of the accumulated costs in the cloud services providers. 


====

Monitoring the Infrastructure
------------------------------

An important functionality of the uCloud platform is the recent implementation of the events management module (monitoring) that allows to collect occurrences and alarms that were generated on the cloud environments (public and/or private), activate notifications and create custom reports.

All this easiness reduces the costs for the organizations, once it eliminates the necessity of hiring providers monitoring services, since that service can represent high costs, which may impact negatively on the budget (exceed the limit) destined for the public cloud infrastructure.

This functionality allows integration to an environment of Service Desk management for IT Service Management control.


====

Inventory (Assessment)
----------------------

The uCloud platform connects with the cloud providers through the registering of specific access credentials of each cloud service supplier (public and/or private). For this purpose the companies must provide credentials of “operative” mode.

This operative credential is provided by the cloud service administrator and they are authorizations generated on the providers' account that only have permission to interact with a cloud public provider console through an API, they are not regular licenses with default login and password. That way, the security and the information security regulamentation rules are previewed and met in its totality.

Once the operative credentials are configured on the uCloud platform, the first activity is to synchronize the configuration and the computing resources inventory existing in the provider (virtual machines - workloads). This list is extracted and added to the uCloud database, in a way that the presentation on the user screen is fast.

With this inventory available directly inside the uCloud platform, the user can operate each one of the virtual machines, independently of which cloud provider this resource is provisioning. In the sequence, it is possible to view the operations to be applied to the computing resources existing in the cloud providers (public and/or private).

It is important to mention that the uCloud does not have any computing resources, these resources are in the public cloud service provider's clouds or in the virtualization environments (hypervisors) installed in its private Datacenter. Through the API Rest the uCloud platform sends actions (tasks) for the specific cloud environment (public and/or private) manager for those to execute the desired action.

The user can follow the result of any of those operation actions in the computing resources almost immediately, it is worth remembering that it is not the uCloud platform that executes the actions, but the environment where the virtual machine is (public and/or private). It is responsible for executing the task sent through the API Rest.

If the result reflects on the user's screen interface, the destination console can take a while to do this task and only after the end of its execution, the result is presented on the uCloud platform.

There is a menu option where the user can follow the percentage of the tasks' progress, their successful result or the error message regarding some restriction of the destination environment.

It is important to highlight that there can be restrictions applied to the user provisioned on the uCloud platform because they have exceeded the limit of their financial quota or computing resources. This way, the uCloud platform generates an error warning: **"quota limit exceeded"**, for example. These scenarios are described in the Tasks menu.


====

Infrastructure Operation
-------------------------

The term **operate** in this context is the user capacity to command certain actions directly in these virtual machines, with the basic operations to: 

* Shutdown;

* Restart;

* Suspend;

* Delete.


Through the interface of the uCloud platform the user can send commands for the consoles of each cloud provider, besides the actions listed above. It is also possible to view the specific configuration information of the virtual machine, as well as change or add some extra resource to it (for example: network card, disk, security group, snapshot, among others).

Regarding the public cloud service providers, the uCloud platform is prepared to connect with the following public cloud platforms:

* Amazon Web Services (**AWS**);

* Google Cloud Platform (**GCP**);

* Microsoft **Azure**;

* **IBM** Cloud;

* **Huawei** Cloud;

* **Oracle** Cloud Infrastructure.


Currently, the uCloud platform is prepared to connect with the following private cloud environment management platforms (hypervisors):

* **VMware** (vCenter Versions 5.0, 5.1, 5.5, 6.0, 6.7, 7.x or higher);

* **vCloud**;

* **Hyper-v** (Windows 2008R2, Windows 2012, Windows 2012R2 and Windows 2016, or higher);

* **Openstack**;

* **Xen Server**;

* **XCP-NG**;

* **KVM**.


The uCloud platform, besides the CSB (Cloud Service Broker) functions, still is a functionality aggregator that allows the user, in a simple and centralized way, the control of several virtualized environments managements consoles (hypervisors) whether it is from the on-premises private environment as well as from the public cloud providers environment.

It aggregates the monitoring, Cloud Workflow functionalities and makes it possible to implement a library repository centralized of files (playbooks) of reference for the usage of infrastructure tools as a code (Infrastructure as a Code).


====

Integration and Interoperability among platforms (API uCloud) 
---------------------------------------------------------------

Interoperability is the capability to interact and interchange data between two or more systems (computers, means of communication, networks, software and other information technology components) according to a defined method, with the purpose to obtain the expected result. Interoperability defines if two components of a system, developed with different tools and providers, can or cannot act together.

The communication between these "systems" is based on the consumption of an Application Programming Interface (API) that enables the sending and receiving of calls for execution of some activity or extraction of some type of stored information. The API is a set of norms that makes the communication between platforms through a series of standards and protocols possible.

Through the APIs, the developers can establish a communication standard (interoperability) between softwares and applications, that way the API usage expands the capacity of a software to communicate with other platforms.

The main example is the native and direct integration of the uCloud platform with the public cloud providers' console, all of it is executed through the interoperability via providers' consoles API.

Another really common example is the uCloud platform usage is the invoices emission ticketing for showback and chargeback systems, as well as the sending of information and alerts about the managed resources.

Our clients (and/or integrators) can use the API documentation of the uCloud with their internal platforms, in a way to complement or automate certain activities and/or actions that are beyond the native capacities of the uCloud platform.

For example: 

Consult and extract from the uCloud platform the values of the invoice costs of a public cloud provider through a financial/accounting application for the invoice emission.

The uCloud has its API documentation, the access to this complete documentation must be requested to your portal provider for it to be created and the access credential sent to the uCloud platform's documentation.

The Ustore team is ready to help, evaluate the demands of interoperability and integration between the uCloud platform, as well as the applications that have and allow the use of APIs for the interoperability.


====

uCloud Platform's Architecture
-------------------------------

In the sequence is presented a reference architecture for the uCloud platform with its components, providers and native integrations.


.. figure:: /figuras/ucloud_future_vision_small_2.png
   :alt: uCloud platform Reference Architecture
   :align: center

----


The uCloud platform communicates with the providers console through the API Rest, that way every action executed or configured on the uCloud screens sends actions (tasks) for the specific cloud (public and/or private) environment manager (console) for those to perform the desired action.

The Ustore is committed to maintain the constant development of its software platforms and apply the current IT market DevOps' best practices.

Our commitment regards the integration compatibility maintenance, so the most recent changes and implementations (new functionalities) result in the providers' console and of all the softwares which keep the interoperability. Therefore, the alteration must always be available through the uCloud platform interface.

*Ad hoc* a set of practices and projected tools are used to increase the capacity of an organization to provide applications and services more rapidly than the traditional processes of software development.


====

Access to the uCloud platform
=============================

----

Dashboard
===========

Section: Company billing quota
-------------------------------

Section: Shortcuts
------------------

**Virtual Machines**
~~~~~~~~~~~~~~~~~

**Virtual Datacenters**
~~~~~~~~~~~~~~~

**Billing**
~~~~~~~~

**Templates**
~~~~~~~~

Section: Recent tasks
-----------------------

Section: Quota information about services
------------------------------------------

CPU usage
~~~~~~~~~

Memory usage
~~~~~~~~~~~~

Disk usage
~~~~~~~~~~

Public IPs quota
~~~~~~~~~~~~~~~~~~~~

Virtual Machines quota
~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Administration Menu 
==================

Switch Roles
-------------

Switch Roles - Mock Scenario
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Mock Scenario (AWS):
~~~~~~~~~~~~~~~~~~~~~~

Mock Scenario (AZURE and AWS):
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Switch Roles - Using
~~~~~~~~~~~~~~~~~~~~~~~~~

*Account*
---------

With the addition of this functionality on the uCloud platform, the behavior on the Administration menu innovates by viewing the submenu allocated for Users, Groups, Companies and presents an Account functionality.

This new feature is located on the left side in the Administration menu, below Users, Group and Companies and will be described in detail throughout this document.

.. image:: /figuras/fig_adm_ing/001_ucloud_adm_submenu.png
  :alt: administration submenu
  :scale: 90%
  :align: center
-----

For the user to access this functionality it is just needed to click on the Administration menu > Account.

The home screen of this feature shows on the left side the uCloud platform functionalities, below the Administration menu Dashboard it is possible to create Users, Groups, Companies and Account, after creating it it is possible to edit, view, list, among other management activities.

In this example the image displays the Account feature, the user can view on the superior corner the three (3) symbols of: Company, Taks and the username that is logged in the portal. Then, it is possible to view the list of Accounts, the ``Refresh`` and ``+ Create Account`` buttons.

.. image:: /figuras/fig_adm_ing/002_ucloud_account.png
  :alt: administration submenu
  :scale: 90%
  :align: center
-----

Firstly, before starting the descriptive detail of the behavior and use of this functionality, the concept of Account  allocated in the Administration Menu listed after Users - Groups - Contracts will be characterized, the Account functionality can be viewed.

----

Introduction
~~~~~~~~~~~

The adoption of cloud as a solution to manage the environments of corporate organizations and the combination of private and public clouds is the great management challenge of these hybrid multi-cloud environments.

As previously mentioned in this document, the uCloud platform is developed for this scenario of hybrid environments, independently of how many providers (public and/or private) there are.  The user can interact with its Infrastructure as a Service (IaaS), Platform as a Service (PaaS).

In this context, the uCloud portal is positioned as a Cloud Service Broker - CSB platform that allows the management of multiple cloud service providers, as private as the public cloud providers. Consequently, the uCloud platform can be implanted in two different ways:

* Dedicated installation (on-premises)

For the dedicated installation scenario (on-premises) the **Account functionality** may not be applied, once the dedicated installation belongs to a single company, which does not share the uCloud platform between other organizations. Still in this scenario, it can be assumed that the uCloud platform installation will only be used in their own cloud(s), whether it is public or private.

* Installation shared as a service (SaaS - Software as a service)

The **Account** functionality was designed for the shared installation (SaaS) scenario, where the company (named *organization*) aims to provide the “Cloud Service Broker service” with the uCloud platform, among its various operations (regional or international) for their final-customers (multiples).

The scenario describe above about the uCloud platform SaaS is ideal to the connectivity/communication service provider (*organization*) which can share the uCloud platform among its regional operations and, also, between its final customers that wish the benefits of operation, financial governance and billing.

It makes it possible to organize and share the resources between the created "Accounts" besides applying service control policies to the **users, groups and companies**, optimizing the governance.

This new model inserts the layer "Account" in the **Administration** menu. It represents a new process to promote the alignment around this functionality and, therefore, to conduct the organizations to obtain a greater control of the hybrid environment, in a centralized manner, by its the business rule makes it possible to create the **Accounts**, and allocate the Companies, the Groups and their Users. Elements belonging to the Switch Roles universe. 

The **“Account”** functionality has as objective to deliver to the organization the viability of segmenting clients per size (virtual machine), per receipt volume (billing costs), assure the performance understanding per “Account” and filter its history by line of business.

To exemplify a way to charge for the *“service offering”* of Centralized Cloud Management by the uCloud platform, the example of “consumption levels” of computing infrastructure based on the number of Virtual Machines Managed by the uCloud platform, or by the monthly value to be invested, what happens first.

The Tiers represent the existing billing model in the **“Accounts”** functionality. The business rule created for this model establishes the accounting of the resources obtained and generated by a given account.

In the portal, the Tiers are categorized in levels from A to J (1 to 10) and calculated based on the rules established using two parameters: 

* Number of virtual machines **X** Determined monthly value
* Number of machines *versus* Cost/value

For example:

* In case of a created account, upon reaching one of the parameters, it immediately scales to the next level. The Tiers level description follows below: 

+-----------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+
| **Tier**              |  **A** |  **B** |  **C** |  **D** | **E**  |  **F**  |  **G**  |  **H**  |  **I**  |  **J**  |
+=======================+========+========+========+========+========+=========+=========+=========+=========+=========+
|| **Quantity of**      ||       ||       ||       ||       ||       ||        ||        ||        ||        ||        |
|| **Virtual Machines** || ≤ 20  || ≤ 30  || ≤ 50  || ≤ 75  || ≤ 100 || ≤ 150  || ≤ 200  || ≤ 250  || ≤ 300  || ≤ 500  |
+-----------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+
| **Monthly amount**    | $1.500 | $3.000 | $4.000 | $6.000 | $8.000 | $16.000 | $24.000 | $32.000 | $40.000 | $64.000 |
+-----------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+

.. attention:: All quantities and values presented above are merely illustrative, serving only as examples.

----

**Example Use Cases:** 
"""""""""""""""""""""

* Galaxy Company Contract (qty. VMs 20):

   In the Galaxy company “Account” there are 20 virtual machines (active and managed by the uCloud platform), therefore it fits in the Tier level “A” - that represents the monthly amount up to 1,500. If it goes past it (and it can depending on the virtual machines and other resources consumptions), the account fits the next Tier.


.. note:: In case the account only uses 18 machines, it keeps classified in the “A” Tier charging model - that in the example represents the lowest number or equal to 20 virtual machines and the monthly amount up to 1.500.* (applied according to the company’s established country).

----

Account Types
~~~~~~~~~~~~

There are two classification of **“Accounts”**, the accounts in the **Integrator** type and the **Producer** type, detailed next:

* Integrator Account:

      This account is responsible for creating the profiles of  the integrator and producer accounts, when creating these profiles, it feeds the tiers and the packages, in addition to establishing, the producer account its usage rule. 

       It works as a kind of cluster, aggregating and categorizing other corporations.

      For example: 

    An **Integrator** account adds the created accounts., it can be considered an “Integrator Account” for the countries that comprise it: Mexico, Brazil, Chile and Colombia.

    The account is responsible for creating other accounts and escalating the other users`. Its has as particularity the list of all the Producer accounts, the companies are associated to the accounts and each one of them receives the same business rules (tiers and packages).

* Producer Account:

       This producer account belongs to the organization which consumes the resource, represents a minor clustering unit and can operate the entire portal.

      For example: 

    Resuming the example above, this multinational corporation creates the “producer accounts” for the organizations that belong to it within a certain country listed below.

    In the case of this Producer Account A Country in Brazil:, the organization broadens the Company of the “A1 Brazil” Client.

    In the example, the company uses the account provider/cloud provider AWS Brasil. 

    The account provider has two (2) VDCs - DevOps Company A1 and NewApps Company A1.

    The groups and users are contained in the company (see figure below).

The following illustration is a representation of the **Account** functionality concept implemented in the uCloud platform. To describe this figure, it is notable the Integrator Account Country Brazil at the top.

The integrator account is [Country Brasil] which englobes the three (3) **Producer** accounts that are the Brazil Producer accounts: A, B and C.

In these producer accounts, their clients’ companies are allocated. Each company of the client has its virtual datacenter, Groups and Users.

  .. figure:: /figuras/figuras-release-notes-ingles-espanhol/ucloud_arquitetura_conceitual003-us-en.png
   :align: center
   
----

.. attention:: All the terms, names, denomination shown in this image are exclusively illustrative, as example.

-----

The accounts of the **Producer** type can have one or more administrators (in this level the profile of this user is one of System Administrator). The companies stop being created when the corporate resource ends, the viewing and permission profiles obey the business rule applied by the **Integrator Account**. 

The strategy of using the **Accounts**  functionality provides a better perception of value at the level of hierarchy, according to what wants to organize the data, within the context, by facilitating its transit at the operational, managerial and executive levels.

With the creation of this functionality, the administrator can manage the viewing and the permission of each *user* in each *group*, contained in a given *company*. Therefore, the access is denied **by default**, being granted only when the permissions specify “allow”. 

.. important:: The activities listed below are restricted only to the users credentials with the permissions of “platform Administrator” ‘role’ function. In case your user does not have this level of permission, please get in touch with your portal provider. By contacting them the authorized team can execute the needed customizations for your environment.

-----

Additionally, the **Accounts** functionality makes it possible to use the control policies that establish the protection barrier of permission and visualization to the users, depending on the characteristics of the type of user, group and company to which it belongs. 

By establishing these default permissions, access and resources visualization, it organizes and qualifies the privilege each user will have within the environment it belongs, creating then permission groups, different and necessary to create thorough controls in each account.

----

How to Access
~~~~~~~~~~~

Integrator and Producer accounts 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Account
----------

Main and Sub-Account
~~~~~~~~~~~~~~~~~

Creating Account 
~~~~~~~~~~~~~~~~~

Listing the Created Account
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Detailing the Account
~~~~~~~~~~~~~~~~~~~~~

Creating Sub-Account
~~~~~~~~~~~~~~~~~~~~~

How to view the Accounts List:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Users
-------

Viewing a User
~~~~~~~~~~~~~~

Creating New User
~~~~~~~~~~~~~~~~~

Groups
~~~~~~~

Viewing Group
~~~~~~~~~~~~~~

Creating New Group
~~~~~~~~~~~~~~~~~~~~

Company
--------

Financial Governance via Company
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Computing Resources Financial Isolation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Computing Resources Logical Isolation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Relate Budget to the Company 
~~~~~~~~~~~~~~~~~~~~~~~~~~

Budget
~~~~~~~~

Accessing Budget
~~~~~~~~~~~~~~~~~

Creating Budget and Sub Budget
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Quarterly Period
"""""""""""""""

Semiannual Period
"""""""""""""""

Annual Period
"""""""""""""""

Monthly Period
"""""""""""""""

Editing Budget 
~~~~~~~~~~~~~~~

Viewing Budget Cost Report
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Viewing Company
~~~~~~~~~~~~~~~

Section: General
""""""""""""""""

Section: Billing Rules
""""""""""""""""""""""

Section: Price Categories
""""""""""""""""""""""""""

Section: Alerts Policies
""""""""""""""""""""""""""

Section: Resources Price - Company
"""""""""""""""""""""""""""""""""""

Section: Company Quota
""""""""""""""""""""""""

Section: Primary Contact
""""""""""""""""""""""""""

Section: Administrators
""""""""""""""""""""""""""

Section: Business Data
""""""""""""""""""""""""""

Section: Conceded Virtual Datacenters
""""""""""""""""""""""""""""""""""""""""

Section: Users
"""""""""""""""

Section: Groups
""""""""""""""""

Section: Billing Data
"""""""""""""""""""""

Section: Permission Profiles
""""""""""""""""""""""""""""

Section: Products
"""""""""""""""""""

Section: Conceded Permissions
"""""""""""""""""""""""""""""""""

Section: Container Billing Profile
""""""""""""""""""""""""""""""""""

Provisioning Company
~~~~~~~~~~~~~~~~~~~~

----

Configuration Menu
===================

General
--------

Section: General
~~~~~~~~~~~~~~~~

Card: Synchronize Active Directory
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Apply profiles
""""""""""""""

Section: Resources Price
~~~~~~~~~~~~~~~~~~~~~~~~

Create default system cost
""""""""""""""""""""""""""

Section: LDAP Server Users Configurations
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section: Agreement Term upload
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Console
--------

Card: Console controllers
~~~~~~~~~~~~~~~~~~~~~~~~~~

Create console controller
"""""""""""""""""""""""""

Network
---------

Section: Network Configurations
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Card: SDN Controllers
~~~~~~~~~~~~~~~~~~~~~~

Creating a SDN controller
"""""""""""""""""""""""""

Public Subnets
---------------

Card: Public subnets
~~~~~~~~~~~~~~~~~~~~
                                 
Update
"""""""

Add subnet
"""""""""""

Subscriptions
-------------

Card: Subscriptions
~~~~~~~~~~~~~~~~~~

Creating subscription
"""""""""""""""""""""""

Flavor Billing Profile
-----------------------

Creating Flavor Billing Profile
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Permission Profiles
--------------------

View and Edit Permission Profile
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creating a Permission Profile
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Viewing Profiles
------------------

Creating Viewing Profile
~~~~~~~~~~~~~~~~~~~~~~~~

Editing Viewing Profile
~~~~~~~~~~~~~~~~~~~~~~~~

Billing Admin
--------------

Billing Administration
~~~~~~~~~~~~~~~~~~~~~~

Launch Accountant
""""""""""""""""""

Manage caches
""""""""""""""

Billing Admin LOG information
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Billing Admin LOG
~~~~~~~~~~~~~~~~~~

USN Tagging Resources
----------------------

Creation of a USN Tagging Resource
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Accounts management (new)
---------------------------

Card: Tiers List
~~~~~~~~~~~~~~~

Create Tier
"""""""""""""""

Section: Bundle list
~~~~~~~~~~~~~~~~~~~~

Create Bundle
"""""""""""""""

Card: Accounts list
~~~~~~~~~~~~~~~~~~~~

Edit Bundle
"""""""""""

Add and remove Tiers
""""""""""""""""""""

Environment settings (new)
---------------------------

Card: Environment settings
~~~~~~~~~~~~~~~~~~~~~~~~~

Add setting
""""""""""""

Section: Hidden elements
~~~~~~~~~~~~~~~~~~~~~~~~

Add setting
""""""""""""

Card: Exhibition elements
~~~~~~~~~~~~~~~~~~~~~~~~~~

Add setting
"""""""""""""

----

Security Menu
==============

Tickets (new)
-------------
			
Processes tickets (new)
~~~~~~~~~~~~~~~~~~~

Button: Open ticket
"""""""""""""""""

Button: Calendar
""""""""""""""

Button: Search
"""""""""""""

Card: Opened tickets - urgent
"""""""""""""""""""""""""""

Card: Opened tickets
""""""""""""""""""""

Card: Closed tickets
"""""""""""""""""""""

Tickets report (new)
~~~~~~~~~~~~~~~~~

Support dashboard
"""""""""""""""""""""

Button: Calendar
""""""""""""""

Button: Search
""""""""""""""

Assessments (new)
------------------

Auto assessment (new)
~~~~~~~~~~~~~~~~~~~

Card: Templates
""""""""""""""

Auto assessment Templates
""""""""""""""""""""""""

Create new Template
""""""""""""""

Card: Clients
""""""""""""""

Create new Client
""""""""""""""

Listing Client
"""""""""""""

Associating Template to the Client
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Auto assessment’s status forms
""""""""""""""""""""""""""""""""""

Generating graphs for viewing
""""""""""""""""""""""""""

.. CIS Control (new)
.. ~~~~~~~~~~~~~

.. Card: Assessment
.. """"""""""""""

.. New Assessment
.. """"""""""""""

Ethical Phishing
-----------------

User access: Admin Manager
~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

**Admin Manager Dashboard**
""""""""""""""""""""""""""

----

**My dashboard** 
""""""""""""""""""""""""""

----
    
**Companies Global Dashboard** 
""""""""""""""""""""""""""

----

**Company Dashboard** 
""""""""""""""""""""""""""

----

**Companies**
""""""""""""""

----

**Users**
""""""""""

----

**Campaigns**
"""""""""""""

----

**Contacts**
""""""""""""""

----

**Templates**
""""""""""""""

----

**Sending Profiles** 
""""""""""""""""""""

----

**Landing Pages**
""""""""""""""""""

----

User access: User 
~~~~~~~~~~~~~~~~~~

----

**Accessing**
""""""""""""

----

**Dashboard for the User User**
"""""""""""""""""""""""""""""""

----

**My Dashboard**
""""""""""""""""

----

**Company’s Dashboard** 
""""""""""""""""""""""""

----

**Campaigns**
""""""""""""

----

**Contacts**
""""""""""""

----

**Templates**
""""""""""""

----

**Landing Pages**
"""""""""""""""""

----

Virtual Machines Menu 
======================

Introduction
------------

Accessing a Virtual Machine
-----------------------------

Managing a Virtual Machine
----------------------------

Section General: Virtual Machines
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section: Instantaneous Performance
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   
Section: Metrics (**AWS** exclusive)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section: Network Interfaces
~~~~~~~~~~~~~~~~~~~~~~~~~

Section: Disk
~~~~~~~~~~~~~

Section: Snapshots
~~~~~~~~~~~~~~~~

Section: Subscriptions (**Exclusive Azure and Google Cloud Platform**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section: Performance History (**Exclusive Azure and GCP**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creating a Virtual Machine
---------------------------

Wizard Step 1 (Cloud Selection)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Step 2 (Virtual Machine basics information)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Step 3 (Virtual Machine basics information – cont.)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Step 4a (Virtual Machine security information)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Step 4b (Security Information – Exclusive Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Step 5a (User data)
~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Step 5b (**User data VMware**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Step 6 (View the virtual machine configurations)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Orchestrator Menu
=====================

Cluster
--------

Cluster Service
~~~~~~~~~~~~~~

----

Scaling Groups Menu
===================

Creating an AWS Scaling Group
------------------------------

Problems known with AWS Scaling Group
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creating an Azure Scaling Group
--------------------------------

Creating an Openstack Scaling 
------------------------------

Creating an vCloud Scaling 
---------------------------

----

Databases Menu
===================

Managing a Database
---------------------

Section General: Security Group 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section: Security Groups
~~~~~~~~~~~~~~~~~~~~~~~~~

Provisioning a Database 
~~~~~~~~~~~~~~~~~~~~~~~~~

Database creation (MySQL & AWS)
---------------------------------

Step 1 - Cloud Service Provider Selection (AWS) [level 4]
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 2 - Database Selection (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   
Step 3 - Database Specification (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 4 - Database configurations access (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 5 - Network and Security Specifications (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 6 - Security Copy Parameter (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Database creation (MySQL & Azure)
----------------------------------

Step 1 - Cloud Service Provider Selection (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 2 - Database Selection (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 3 - Database Specifications (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 4 - Database access configurations (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 5 - Network and Security Specifications (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 6 - Security Copy Parameter (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Database creation (MySQL & GCP)
--------------------------------

Step 1 - Cloud Service Provider Selection (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 2 - Database Selection (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 3 - Database Specifications (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 4 - Database access configurations (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 5 - Network and Security Specifications (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Step 6 - Security Copy Parameter (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Virtual Datacenters Menu 
=====================

Managing Virtual Datacenters
------------------------------

Section: General (new)
~~~~~~~~~~~~~~~~~~~~~~~
			
Section: Hosts (new)
~~~~~~~~~~~~~~~~~~~~~
			
Section: Networks (new)
~~~~~~~~~~~~~~~~~~~~~~~~
			
Section: Key Pair (new)
~~~~~~~~~~~~~~~~~~~~~~~~

Section: Security Group (new)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section: Templates (new)
~~~~~~~~~~~~~~~~~~~~~~~~~
			
Section: Flavors (new)
~~~~~~~~~~~~~~~~~~~~~~~

Section: Storages (new)
~~~~~~~~~~~~~~~~~~~~~~~~

Section: Catalog (new)
~~~~~~~~~~~~~~~~~~~~~~~

Section: Load balancers (new)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Section: Database (new)
~~~~~~~~~~~~~~~~~~~~~~~~

Section: Virtual machines (new)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Editing a Virtual Datacenter
------------------------------

Creating a Virtual Datacenter
-----------------------------

----

Billing Menu 
==============

Private Businesses
-------------------

Public Businesses (USN)
-----------------------

Corporate Environment
----------------------

----

**Billing Rules** 
-------------------

----

Invoicing Rule
~~~~~~~~~~~~~~

----

**Reports**
-------------

Consumption-Based Panels
-------------------------

Service History Report
~~~~~~~~~~~~~~~~~~~~~~~

Cadenced Billing Report
~~~~~~~~~~~~~~~~~~~~~~

Product Relational Cost Report
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Resource Viewing Report
~~~~~~~~~~~~~~~~~~~~~~~~~~

Budgets Costs Report
~~~~~~~~~~~~~~~~~~~~~~~~~~

Consumption Monitoring Report
~~~~~~~~~~~~~~~~~~~~~~~~~~

The Consumption Monitoring Report (v1) is a new functionality of the uCloud portal, which deals with the invoicing tracking and complete spending detail, categorized by Clouds (for example: AWS and AZURE) Contracts and Resources.

In this document, different types of indexes are generated, which can be tables, reports and graphs, for each type of class (Resource, Contract and Cloud). These are titled in topics as:

  1. Invoicing History; 
  2. Invoice per Contract/Project; 
  3. Major Variations on this Invoice and 
  4. Detailing TOP 3 Contract per Cloud.

.. attention:: |atencao| Each of those categories is separated and organized from the highest to the lowest consumption. 

----

In addition, the **Consumption Monitoring Report (v1)**, briefly named **CMR.v1**, compares the expenses of the current month with the previous month, providing the company with the necessary information to be able to evaluate the disbursement and have an efficient control of possible drops or increase in consumption. 

====

Accessing CMR.v1
""""""""""""""""

To generate the Consumption Monitoring Report (v1) on the uCloud portal, the user must access the ``Billing menu``, identified in the lower left corner. And then, click on the ``Reports submenu``.

.. figure:: /figuras/fig_ucloud_fin_rmcv1/1_Menu_Financeiro.png 
   :alt: Menu_Financeiro
   :align: center 
----

The screen below presents all the options related to accessing and managing invoices for groups or contracts that the user administers. 
  
.. figure:: /figuras/fig_ucloud_fin_rmcv1/2_Financeiro_painéis.png 
   :alt: Financeiro_painéis
   :align: center 
----

When clicking on the ``Reports submenu``, the topic “Consumption-Based Panel” provides access to reports related to consumption for the current month typed on the search by the user.

.. figure:: /figuras/fig_budget/17_painéis_consumo.png 
   :alt: Painéis_baseados_consumo
   :align: center 
----

It groups seven types of reports, one of them is the **Consumption Monitoring Report - CMR.v1**.

.. figure:: /figuras/fig_ucloud_fin_rmcv1/4_Descrição.png 
   :alt: Descrição
   :align: center 
----

By clicking on this option, the user can generate the desired document. 

====

Creating CMR.v1
""""""""""""""""

After clicking on **Consumption Monitoring Reports (v1) - CMR.v1**, a new screen opens, in which the user can select the month and year they desire to visualize, in addition to filtering the intended contracts. 

.. figure:: /figuras/fig_ucloud_fin_rmcv1/5_RMConsumo.png 
   :alt: Relatório Monitoramento Consumo v1 
   :align: center 
----

In this same modal, two buttons are displayed: 

* ``GENERATE REPORT`` Remains available for activation when at least one contract is selected. 
* ``SELECT ALL`` Refers to the contracts filter. There it is possible to note the scroll and search bar. 

.. figure:: /figuras/fig_ucloud_fin_rmcv1/6_Seleção_mês_e_ano.png 
   :alt: Seleção_mês_e_ano
   :align: center 
----

The scroll bar, located on the right side, helps the user to navigate through the modal in search for the desired contract. The search bar facilitates the search, the user just needs to type the initial letters of the contract.

.. figure:: /figuras/fig_ucloud_fin_rmcv1/7_Barras_rolagem_pesquisa.png 
   :alt: Barras_rolagem_pesquisa
   :align: center 
----

After clicking on Generate Report, a new screen opens, showing the month selected by the user and the ``DOWNLOAD`` and ``GENERATE NEW REPORT`` buttons. 

.. figure:: /figuras/fig_ucloud_fin_rmcv1/8_Download_recorte_RMCv1.png 
   :alt: Desbloquear_download
   :align: center 
----

The ``DOWNLOAD`` button is only unlocked when the data is compiled on the platform and it makes available the report for the period and the selected contract. 

In the example of the following screen, the platform informs that the “user does not have reports generated for the contracts and period selected” and asks the user to click on ``GENERATE NEW REPORT``.

To download the file, the user just needs to click on the referred button.

.. figure:: /figuras/fig_ucloud_fin_rmcv1/9_Gerar_relatório.png 
   :alt: Gerar_relatório
   :align: center 
----

In case there is no data, the reports become unavailable for the selected month, the ``DOWNLOAD`` button appears inactive (gray color) and the platform issues the message mentioned in the previous example and printed on the image above.

When there is data to be published on the period selected by the user, the platform informs that the report is in process of compiling the data. 

====

Following the status on the Tasks menu
"""""""""""""""""""""""""""""""""""""""

In the flow of creating the CMR.v1, the platform presents two types of situations, according to the user profile that is logged into the platform. The task status at the top of the screen differs, for each type of user, a procedure is described in the sequence:

**Case 1:** 

* **Admin user**: When opening the Tasks functionalities, it must be observed the “Pending Approvals” tab, which presents the columns: Operation, user, details, progress, start date, duration, status and actions.

**Case 2:** 

* **User user**: When creating the report, the user must request the administrator of their contract to carry out the approval of the requested task. 

**Procedure:**

In the “Actions” column located on the “Pending Approvals” tab **the admin user** of the contract must approve the action to “Generate Report”. In case of the “User user”, they must request the administrator of the contract to carry out or not the approval of the task.

.. figure:: /figuras/fig_ucloud_fin_rmcv1/10_Tarefas.png 
   :alt: Tarefas
   :align: center 
----

Next, they must wait for the “Status” to be updated, that can be: ``Running``, ``Failed`` or ``Success``. 

After successfully creating the new report, the data was compiled on the uCloud platform.

====

Enabling the CMR.v1’s download
"""""""""""""""""""""""""""""""""

When creating a new report successfully, the user must repeat the flow to download it once the data is compiled on the uCloud platform. 

In the sequence, it is necessary to select again, the same period and contracts that the user intends to search for previously created information. 

.. figure:: /figuras/fig_ucloud_fin_rmcv1/11_Fluxo.png
   :alt: Fluxo_gerar_relatório
   :align: center 
----

At this point, the user must observe if the ``GENERATE REPORT`` button is enabled (orange color), if so, it means that the flow to download the CMR.v1 continues, the data is previously prepared and can be extracted in the report format. 

In the course of this procedure, the platform presents the unlocking of the ``DOWNLOAD`` button, displaying it in green, according to the following image.

.. figure:: /figuras/fig_ucloud_fin_rmcv1/12_Relatório_gerado.png 
   :alt: Relatório gerado
   :align: center 
----

The user must check the message the platform presents: “Report generated for the contracts and selected period. They can download it or generate a new one with the same settings”. 

At the end of this sequence of activities, to download the desired CMR.v1 file, the user must click on the ``DOWNLOAD`` button.

====

Viewing CMR.v1
"""""""""""""""

After generating and downloading  the **Consumption Monitoring Reports (v1) - CMR.v1**, an example is presented and described: 

**Front Cover**

The document has a cover, which contains the following information:
 
1. Name of the company; 
2. Invoicing Date; 
3. Standardized text on the invoicing of consumptions in the clouds.

According to the picture shown below:

.. figure:: /figuras/fig_rmcv1_ing/13_consumption_cover.PNG 
   :alt: Consumption Cover
   :align: center 
----

**1 - Executive Summary** 

In the Executive Summary, an explicative text is presented, describing the variation of the values and the percentage that occurred in the current month’s invoice in comparison to the previous month, as shown in the example:

.. figure:: /figuras/fig_rmcv1_ing/14_consumption_summary.PNG 
   :alt: Consumption summary
   :align: center
----

**1.1 - Invoicing History**

Right after the executive summary, there is the Invoicing History, that presents a table with the period selected by the user, in which the value of the desired cloud in Reais (BRL) and Cloud Service Unit (Unidade de Serviço de Nuvem - USN -, in Portuguese) is shown , and the rate of change in percentage of the previous month as well as the current month.

.. attention:: |atencao| Cloud Service Unit (USN), is a pricing model for cloud services, assigned to companies that are associated with the government spheres. 


.. important:: |importante| USN aims to establish itself as a predictable, linear and flexible method to obtain a specific amount to be charged for cloud computational services.


.. note:: |nota| The USN metric consists of establishing a specific reference value for each type of cloud service, according to the individual metric associated with the resource consumption.

----

.. figure:: /figuras/fig_rmcv1_ing/15_consumption_clouds_history.PNG 
   :alt: consumption clouds history
   :align: center
----

According to the example above, the expenses of the current month are compared with the expenses of the previous month, showing if there was an increase or decrease in consumption for each specific contract, it also exhibits the percentage and possible variations from the previous month to the current month. 

In addition, this part of the implementation exposes a basic rule: only the 5 biggest expenses are specified, that is, the contracts that had the highest consumption during the current month are disclosed, together with the values of each one separately. 

This rule is intended to keep the document more compact, avoiding to extend it, according to the examples below:

* First AWS cloud example:

.. figure:: /figuras/fig_rmcv1_ing/16_consumption_aws_chart.PNG 
   :alt: consumption aws chart
   :align: center
----

For the sake of completeness and better visualization, this part of the document also generates a pie chart, containing the same information as the expenses of the table illustratively, separating the contracts by colors for better comprehension by the user.

* Second example of AWS cloud pie chart:

.. figure:: /figuras/fig_rmcv1_ing/17_consumption_aws_resources_chart.PNG 
   :alt: consumption aws resources chart
   :align: center
----

.. note:: |nota| In case of more than one cloud, the report follows the same pattern of presentation and information. 

----

* Third Azure cloud example:

.. figure:: /figuras/fig_rmcv1_ing/18_consumption_azure_chart.PNG 
   :alt: consumption azure chart
   :align: center
----

**2 - Invoice per Contract/Project**

In the Invoice per Contract/Project, the general expenses of the contracts of each cloud is first informed, as shown in the executive summary, with their values in BRL and USN.

.. figure:: /figuras/fig_rmcv1_ing/19_consumption_invoice_contract_project.PNG 
   :alt: consumption invoice contract project
   :align: center 
----

Following the table, a graph is presented containing the proportion of these consumptions in percentages, as shown below:

As in the Invoicing History, in the Invoicing per Contract/Project, a graph is also generated for complementation and better visualization of the user, containing the same information of the expanses of the table illustratively, demonstrating the proportion of expenses per cloud.

.. figure:: /figuras/fig_rmcv1_ing/20_consumption_chart_proportions_among_clouds.png 
   :alt: consumption chart proportions among clouds
   :align: center
----

After the chart, the following image exposes and specifies **all** contracts for each cloud (in addition to the top five displayed in the invoicing history), with the most recent projects being highlighted.

The example in the table below details the costs of the cloud, its contracts, and totals the value, presented in BRL and USN.

.. figure:: /figuras/fig_rmcv1_ing/21_consumption_invoice_contract_project.PNG 
   :alt: consumption invoice contract project
   :align: center
----

.. figure:: /figuras/fig_rmcv1_ing/22_consumption_invoice_contract_project.PNG 
   :alt: consumption invoice contract project
   :align: center 
----

.. note:: |nota| Note that in case of more than one cloud, the report follows the same pattern of presentation and information.

----

**3 - Major Variations in this Invoice**

In the “Major Variations on this Invoice" are presented in a table, all the variations of the contracts of the month of each specific provider, comparing the value of the previous month with the value of the current month, showing the variation of its total value in percentage, thus, this part of the document is a complementation to the “Invoice per Contract/Project”.

This table takes into account only the most relevant variations, with a cut containing, first, those greater than or equal to fifteen percent (>=15%), and therefore, those less than or equal to negative fifteen percent  (<= -15%). Here’s, the example:

.. figure:: /figuras/fig_rmcv1_ing/23_consumption_positive_variations.PNG 
   :alt: consumption positive variations
   :align: center
----

**Positive variations** (>=15%) are highlighted in a **bluish tone**, in the same way that the **negative variations**  (<= -15%) are highlighted in a **reddish tone**.

It is possible to notice that the greater the variation, the darker the tone.

.. figure:: /figuras/fig_rmcv1_ing/24_consumption_negative_variations.PNG 
   :alt: consumption positive variations
   :align: center
----

Furthermore, the contract with the highest variation value is highlighted, and presents the information of its resources detailedly. This chart are contains **all the contract resources** and their expenses, informing the changes in their consumption and its use. The graph also shows which were the resources that spent the most in the month, as exemplified in the following image:

.. figure:: /figuras/fig_rmcv1_ing/25_consumption_highest_aws.PNG 
   :alt: consumption highest aws
   :align: center
----

.. figure:: /figuras/fig_rmcv1_ing/26_consumption_aws_total_amount.PNG 
   :alt: consumption aws total amount
   :align: center 
----

.. figure:: /figuras/fig_rmcv1_ing/27_consumption_azure_highest.PNG 
   :alt: consumption azure highest
   :align: center
----

Right after the bar graph, a descriptive table is presented, with columns "Product" and "Total Amount" (BRL) of the quantities of each resource invested separately and specifically, from the highest number to the lowest.

.. figure:: /figuras/fig_rmcv1_ing/28_consumption_azure_resources.PNG 
   :alt: consumption azure resources
   :align: center
----

.. note:: |nota| In case of more than one cloud, the report follows the same pattern of presentation and information.

----

**4 - Detailing TOP 3 Contract per Cloud**

Finally, an index is exposed, containing the clipping of the three contracts that had the highest consumption in each cloud, and the resources that represent the greatest impact in each one of them. The report presets each of the clouds used by the company, the name of the contracts and their total values in BRL and USN, as presented on the next example:

.. figure:: /figuras/fig_rmcv1_ing/29_consumption_aws_contracts.PNG 
   :alt: consumption aws contracts
   :align: center
----

Next, the summary of how much each product costs the contract is presented in more detail, specifying them and showing the percentage of the total expenses of each contract. Such information is displayed from a illustrative graph, according to the example below:

.. figure:: /figuras/fig_rmcv1_ing/30_consumption_highest_aws_chart.PNG 
   :alt: consumption highest aws chart
   :align: center 
----

.. figure:: /figuras/fig_rmcv1_ing/31_consumption_aws_table.PNG 
   :alt: consumption aws table
   :align: center 
----

.. figure:: /figuras/fig_rmcv1_ing/32_consumption_aws_products_chart.PNG 
   :alt: consumption aws products chart
   :align: center
----

.. figure:: /figuras/fig_rmcv1_ing/33_consumption_aws_products_table.PNG 
   :alt: consumption aws products table
   :align: center
----

.. figure:: /figuras/fig_rmcv1_ing/34_consumption_highest_azure_chart.PNG 
   :alt: consumption highest azure chart
   :align: center
----

.. figure:: /figuras/fig_rmcv1_ing/35_consumption_azure_table.PNG 
   :alt: consumption azure table
   :align: center
----

.. attention:: |atencao| In case of more than one cloud, the report follows the same pattern of presentation and information.

----

Finally, is noticeable that the implementation **Consumption Monitoring Report (v1) CMR.v1**, helps to control the monthly expenses, presenting and comparing them with the previous month.

This update has a vast index, containing tables, reports and graphs that range from the most general to the most specific, granting the company and, consequently, the user all the necessary information and tools that allow total control over their investments and projects.

====


Cost limit based-Reports
~~~~~~~~~~~~~~~~~~~~~~~~~~

Defining the Reports
"""""""""""""""""""""

A. Cost Limit Reports
""""""""""""""""""""""
   
**New features:**


**Step by step:**


1. **Executing without saving**


**Steps for Configuration:**


**Periods Details:**


**Post-configuration procedures:**


**Cases in which the data are presented differently:**


2. **Saving a cost limit configuration (Creation)**


3. **Executing from a saved configuration**


4. **Editing a cost limit**


5. **Deleting a cost limit**


6. **Filtering by period**


7. **Generating projection for the following months**

----

.. centered:: Possible error messages:
----

B. Risk analysis
""""""""""""""""

**Step by step:**


1. **Executing a risk analysis**
   

2. **Generate cost limit report from the risk analysis**


3. **Generate risk analysis from the cost limit report**

  
Invoice based-panels
---------------------

My invoice
~~~~~~~~~~~~

Billing
~~~~~~~~~

.. * **Virtual Machines**:

.. * **Subscriptions**:

.. * **Snapshots**:

.. * **Public IPs**:

.. * **Load Balancers**:

.. * **DNS Zones**:

.. * **VPNs**:

.. * **Non-managed items**:


Consolidated Invoicing Report (CIR)
------------------------------------

Accessing the CIR
~~~~~~~~~~~~~~~

Selecting the CIR
~~~~~~~~~~~~~~~~~~

Following the CIR search
~~~~~~~~~~~~~~~~~~~~~~~~~~~
   
Listing the CIR companies
~~~~~~~~~~~~~~~~~~~~~~~

Detailing CIR actions
~~~~~~~~~~~~~~~~~~~~~~~
   
Use case: 
~~~~~~~~~~~~

Billing Trend Report (BTR)
----------------------------

Accessing the BTR
~~~~~~~~~~~~~~~~~~~

Creating a BTR
~~~~~~~~~~~~~~

How to download the file 
~~~~~~~~~~~~~~~~~~~~~~~~~~
   
Following the download on the Tasks Menu
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Viewing the BTR
~~~~~~~~~~~~~~~
   
Grouping by product name
~~~~~~~~~~~~~~~~~~~~~~~~~~

Grouping by Tag
~~~~~~~~~~~~~~~~~~

Filtering by anomaly
~~~~~~~~~~~~~~~~~~

Linked Accounts
----------------

**Utilitaries**
--------------
   
**Dimension**
~~~~~~~~~~~~


Dimension is a new implementation of the uCloud platform, and was created to group tags of different nomenclature, but that are part of the same context, that are tagged in distinct clouds. That way, it avoids equal resources being tagged differently.

For this, logical operations and a filter were elaborated, with the intention of identifying in Billing which resources belong to a certain dimension. To better understand the two points that build this concept, observe the following examples: 


1. It unifies a set of Tags that are different, but have the same meaning/role.

 * For example: 

   * product: ETC
   * Product: eTc
   * producT: CTE

It is noticeable that the Tags above express the same thing, although they differ in their written manners. It is important to remember that these can be **applied in different clouds**, but in the same resources, where they should behave equally.

Thus, when unifying this group of Tags in a dimension, it is possible to identify all the resources that are within that context, and that way have a new way of visualizing the Reports, Budget and Forecast.

1. Creates logical expressions.

 * For example:
 
   * product: EFG & department: IT

In the example above, the expression represents that this dimension desires all resources to have the Tags: “product: EFG & department:IT”. This expression is considered simple, nonetheless, something more complex can be built from what has been implemented. 

====


Creating a Dimension
"""""""""""""""""""""

To create a dimension, the user must click on the ``Financial menu``, and then on the ``Utilities submenu``, that displays two options presented on the next image:

1. **Dimension**; 
2. Virtual Tags.

.. image:: /figuras/fig_dimension_ing/01_dimension_billing_menu.png
   :alt: dimension billing menu
   :align: center
----

When selecting the “Dimension” option, the listing of dimensions generated previously is presented, as demonstrated in the figure below:
  
.. image:: /figuras/fig_dimension_ing/02_dimension_listing.png
   :alt: billing dimension listing
   :align: center
----

In case this is the first dimension to be created by the user, no list is displayed on the screen, as shown in the next image:

.. image:: /figuras/fig_dimension_ing/03_dimension_empty_listing.png
   :alt: billing dimension empty listing
   :align: center
----

On the superior left side of the screen, the ``Create Dimension`` button  is presented, which the user must press to start the creation process.

After clicking, the initial screen to create a “Dimension” is presented, as shown in the next figure:

.. image:: /figuras/fig_dimension_ing/04_dimension_start.png
   :alt: billing dimension start
   :align: center
----

To better understand the function of each blank, observe the detailing of these below:

* Dimension name: In this blank, the user must fill in the name of the dimension to be saved.

* ``Structure +`` : This button presents two options that the user can apply in the structure of their “Dimension”.

   * Tag Grouping;

   * Tag. 

.. attention:: |atencao| It is important to highlight that this structure must be a logical expression thought previously. Therefore, to group tags is necessary to put them in a group first.

----

* Structure: Corresponds to a block at the end of the screen, where the user has a better visualization of the structure that is being assembled.

* ``Save`` button: After completing the data, the user must press on the ``Save`` button so they are not lost.

====

Creating a Tag grouping
"""""""""""""""""""""""""

After filling in the “Dimension” name, the user must create a group for its structure. When hovering the mouse cursor over the “Tag Grouping” option, appears the following message:

.. image:: /figuras/fig_dimension_ing/05_dimension_message_grouping_expanded.png
   :alt: billing dimension message group expended
   :align: center
----

When selected, the group creation modal is shown, where the name of the group of Tags must be filled in and then saved.

.. image:: /figuras/fig_dimension_ing/06_dimension_create_grouping.png
   :alt: billing dimension create grouping
   :align: center
----

Once the action is performed, below the **”Structure +”** function, the name of the created group appears, and beside it there are two action buttons:

* Plus symbol “+” to create other group(s) or add Tag(s);

* Trash bin icon to delete the created group.

Next to these icons, the following information appears :

.. image:: /figuras/fig_dimension_ing/07_dimension_message_structure_expanded.png
   :alt: billing dimension message structure expanded
   :align: center
----

.. attention:: |atencao| It is important to note that in case the “Dimension” construction does not match the conditions presented in the message, the “Save” button is unavailable for activation. 

----

In the image below, it is also possible to notice that in the Structure function, at the bottom part of the screen, the group is represented by (   ).

.. image:: /figuras/fig_dimension_ing/08_dimension_grouping_structure.png
   :alt: billing dimension grouping structure
   :align: center
----

Creating Tag
"""""""""""""

By clicking on the plus icon ``+`` next to the created group and positioning the mouse cursor over the Tag option, the next message is shown:

.. image:: /figuras/fig_dimension_ing/09_dimension_message_tag_expanded.png
   :alt: billing dimension message tag expanded
   :align: center
----

When clicking on Tag, the Tag creation modal is presented:

.. image:: /figuras/fig_dimension_ing/10_dimension_modal_tag.png
   :alt: billing dimension modal tag
   :align: center
----

The first step for the user is to select one of the companies listed in the dropdown menu.

.. image:: /figuras/fig_dimension_ing/11_dimension_list_company.png
   :alt: billing dimension list company
   :align: center
----

After selecting the desired company, the ``Filter`` button, next to the dropdown menu, is available for activation, as exemplified in the image below:

.. image:: /figuras/fig_dimension_ing/12_dimension_filter.png
   :alt: billing dimension filter
   :align: center
----

In case the company already has existing Tags, a list of Tags with the keys and values of the last three months is exhibited. The screen displays the number of pages below the listing and the information retrieved in blocks of 10, 25, 50 or 100 lines.

.. image:: /figuras/fig_ucloud_findimensao/13_dimensão_company_tag.png
   :alt: Financeiro Dimensão_company_tag
   :align: center
----

The user must select the desired Tag, shown in the list, and the Keys and Tag Value created are automatically displayed.

.. image:: /figuras/fig_ucloud_findimensao/14_dimensão_company_tag_escolhida.png
   :alt: Financeiro Dimensão_company_tag_escolhida
   :align: center
----

When finishing filling the modal, the user must click on the ``Save`` button on the inferior right corner of the screen.

.. image:: /figuras/fig_dimension_ing/15_dimension_modal_second_tag.png
   :alt: billing dimension modal second tag
   :align: center
----

If a company does not have Tags and the user wants to create them, just type the Key and Value on the last blanks, as demonstrated on the image above, leaving the central blanks empty.

Once this is done, the “Dimension” screen creation should be displayed as follows: 

.. image:: /figuras/fig_dimension_ing/16_dimension_group_and_tag.png
   :alt: billing dimension group and tag
   :align: center
----

It can be seen, from the image above, that the “Dimension” has a hierarchy system, where first there is a group inserted in the structure, and only after the creation of the group do the Tags follow.
 
After the initialization of the process of creating a “Dimension”, it is necessary to add the other Tags of the same context to be part of the group.

To do so, the user must click on the plus sign “+” next to the Structure, which shows two **logical operators** </> OR and </> AND.

====

Using the logical operator
""""""""""""""""""""""""""""

Logical operators are a part of the programming language, and they are used for the purpose of creating true and false expressions. These are intended to join two divergent expressions and elaborate a more complex conditional expression. 

.. image:: /figuras/fig_dimension_ing/17_dimension_logical_operators_closeup.png
   :alt: billing dimension logical operators closeup
   :align: center
----

To better understand their application, information about the two operators used in the creation of “Dimension” is detailed below.

 * </> OR: In an expression, if only one of them is true, it is considered entirely true, and is executed. 

 * </> AND: In an expression, if one of them is false, it is considered entirely false, and is not executed.

To better understand its usage, the user must follow the creation process.

Resting the mouse cursor on the operator option </> OR, the following message is displayed:

.. image:: /figuras/fig_dimension_ing/18_dimension_operator_or_closeup.png
   :alt: billing dimension logical operator or closeup
   :align: center
----

That is, even if one of the Tags is non-existent, the action is still performed only with the existing Tag.

When hovering the mouse over the </> AND operator, the following message is presented:

.. image:: /figuras/fig_dimension_ing/19_dimension_operator_and_closeup.png
   :alt: billing dimension operator and closeup
   :align: center
----

That is, when searching for Tags, if only one of the Tags does not exist, the action is interrupted.

In this example, the operator “AND” was selected and the confirmation of the action is presented when both structures are changed:

.. image:: /figuras/fig_dimension_ing/20_dimension_operator_selected.png
   :alt: billing dimension operator selected
   :align: center
----

When finishing this first process of Tag creation, the user must create the second Tag, repeating the creation flow detailed above.

At the end of this step, the final structure of a dimension is displayed, and to store it, simply click on the ``Save`` button, located in the lower right corner of the screen, as presented in the image below:

.. image:: /figuras/fig_dimension_ing/21_dimension_structure_complete.png
   :alt: billing dimension structure complete
   :align: center
----

Upon completion of this action, the saved “Dimension” is shown in the dimension listing.

====

Listing Dimension
""""""""""""""""""

To list a newly created “Dimension”, usually the screen exhibits the listing. When consulting the “Listing Dimension” screen, if it does not update automatically, the user must click on the ``Refresh`` button in the superior right corner of the screen. 

Then, the screen shows a list that must present the created “Dimension”, as displayed on the figure below:

.. image:: /figuras/fig_dimension_ing/22_dimension_final_listing.png
   :alt: billing dimension final listing
   :align: center
----

The screen above “List of Dimensions” shows the contract name superior, the symbol of the “Tasks” functionality and the name of the logged-in user in the superior right corner.

On this screen, the user can opt between creating a new dimension, editing an existing dimension or deleting a created dimension. It presents the two buttons that allow to ``Create Dimension`` or ``Refresh`` the list of dimensions.

In this list, the columns of “Name” and “Actions” are presented, the information can be personalized and retrieved by clicking on the blocks of 10, 25, 50 or 100 lines. The “Actions” column allows the ``Edit`` and ``Delete`` operations.

====

Editing a Dimension
""""""""""""""""""""

To edit a Dimension, the user simply clicks on the ``Edit`` button in the “Actions” column in the “Dimension” list, as detailed below:

.. image:: /figuras/fig_dimension_ing/23_dimension_edit_button.png
   :alt: billing dimension edit button
   :align: center
----

Doing this, the screen with the assembled and finished structure is displayed, as exemplified below. This example, using a new dimension, contains Groups and multiple Tags. 

.. image:: /figuras/fig_dimension_ing/24_dimension_structure_complete.png
   :alt: billing dimension structure complete
   :align: center
----

When looking at the figure above, observe the trash can icon. That is, the user has the possibility to create other groups and add more Tags, as well as delete them.

It is also possible to realize that for each action performed, the Structure, located at the bottom of the page, is modified.

For the alteration to be confirmed, it is necessary for the user to press the ``Save`` button, next to the Structure function, located in the lower right corner of the page.

====

Where the "Dimension" is used
""""""""""""""""""""""""""""

Currently, this implementation groups Tags and gathers them in the “Dimension” created, facilitating the categorized visualization in other functionalities of the platform.

Furthermore, the “Dimension” is used in the modal “Create Budget” included in the card named “Sub Budget Details” in disambiguation_ .

.. _disambiguation: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Release-Notes/release.ing-ucloud-2022-jun.jul.aug.html#creating-budget-and-sub-budget

====

**Virtual Tags**
~~~~~~~~~~~~~~~~~

In a broad context, a TAG (a label) it’s a keyword that signs or identifies a particular computational resource (or service resulting from its existence) stored in a cloud provider, repository or database. The TAGs are a type of metadata, capable of providing information that describes the data, this facilitates automated search for information retrieval. A TAG is a label in which the user assigns a **Key** and a **Value** to a public cloud computing resource.

In the scenario of any type of cloud, the data contained in TAGs is used together with other forms of tagging that the cloud providers use to classify information about their resources. Thus, the TAGs help the research, organization, identification, management and, finally, the filtering of used resources in any cloud provider, for example: AWS, Azure, Google, among others. 

These TAGs (labels) after linking to a resource are used to categorize these resources so they can be classified by: purpose, property, criteria or location. For example: the user or the organization, can define a set of TAGs for the Amazon EC2 instances, of their account, to help track the owner and/or clustering level (stack values) of each computing resource of the public cloud consumed.

.. figure:: /figuras/figuras-release-notes-ingles-espanhol/ucloud_menu_configuracao_tags_virtual001-en-us.png
   :scale: 80%
   :align: center
----

.. note:: The picture above is an example and the information present is merely illustrative. 

In the picture above we use two Virtual Machines as an example of how to illustrate the link between TAG and resources. A detail that is mentioned very little is that the public cloud service providers don’t allow linking TAGs to all their products and/or services (check the provider documentation to know which resources are likely to have a TAG linked to the resource).

In the example above we link “two different TAGs” to the same resource (Virtual Machine) in this way we induce that the financial reports by TAG totaled the cost value of the TAG twice (the same value in each TAGs) and, for this example, in this situation double the cost within the same period.

But we must highlight that to the public cloud service provider’s environment, once a TAG is created, it will not automatically be linked to any resource (or services resulting from the resource existence). The user must first create the TAG(s) and then manually link the TAG(s) to the wished resource(s). Because it is a manual process and performed by a user at the cloud service provider console, the TAGs resources can be time consuming for the public cloud Cost Administrator. There may be too many rows in the billing/bucket file for the Cost Administrator to check. This verification and the TAGs linking process is continuous and manual.

.. important:: The fact that the TAGs are accessible to many services in cloud providers, it’s important to avoid adding private or confidential data to the Virtual TAGs, as for example: personal identification, confidential or sensitive information.

The uCloud Platform synchronizes and receives the content of the billing file (CSV) from the public cloud service provider and, consequently, receives all the TAGs existing in the provider.

----

uCloud’s platform Virtual Tags
""""""""""""""""""""""""""""""

We mentioned above that the process of linking a TAGs to a resource is manual, time consuming and, above all, it is not automatically repeated for new services of a resource that already has a linked TAG.

The new uCloud Platform Virtual TAGs functionality creates an automation for the TAGs linking process to existing resources in the public cloud service provider’s environment.
The uCloud Platform Virtual TAG process may automatically link a specific TAG to a resource to be selected based on Product Name and/or Product Family and/or Resource Identifier. 

.. attention:: The conjunction “and/or” shows the high granularity degree the user can select to attend to their specific use of their need.

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

----

Normalizing Virtual Tags
"""""""""""""""""""""""""

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

----

When to use
"""""""""""

Based on this new implementation, aimed at classifying, normalization and visualization of obtained information from the public cloud several providers, the new functionality “Virtual TAGs” enables to ticket/tag, that is, mark the resources that by some rule or definition, were not possible to find registered in the billing of a certain cloud provider used by the organization or user customer. 

Once, each cloud presents different reports of used resources, the difficulty for the IT professional to be able to normalize and understand the presented classification in several clouds, or even the suppressed information by TAGs absence that group the relevant format, valuable information, whether they are quantitative, qualitative or financial, facilitating the organization and/or its user customer the possibility of an assertive decision making, when using this new implementation called “Virtual TAGs”. Developed by the Ustore as a solution to attend this absence, it claimed in the reports that it has a similar behavior in the several cloud providers, such as AWS, Azure, Google, among others. 

The uCloud portal generates the financial report, this report retrieves information by product name or by TAG. It’s the uCloud portal that offers this unique service of “Virtual TAGs” that enables and/or facilitates the management and the classification of certain resources that no longer receive TAGs in the cloud, as mentioned previously, by rules or internal policies established by the providers themselves. 

It is necessary to use this new implementation, when the organization and the user customer need to retrieve information by TAG or product name in a distinct way, in several clouds, once each cloud provider, like Google, AWS and Azure treat the billing record report differently. And each one of them uses its own nomenclatures for each type of offered resource.

By applying the “Virtual TAGs” to the cloud resources (e.g: database and virtual machines) it is possible to create classification by cost centers divisions, projects and other types of groupings.

The new implementation from the uCloud portal enables users to present the information generated in the financial report according to what was classified or tagged by the user to group or identify information, whether it is by product name, purpose, property, criteria or location, among others.

.. note:: The keys and TAGs values may or may not be reflected in the billing report of several clouds. The TAGs don’t save semantic meaning in the Amazon EC2, they are interpreted as a character sequence.

Thus, resources imported from the public cloud billing file that, by any policies of these providers, fail to index the tag to the cloud service resource, may receive a “Virtual TAG” within the portal.

----

Tags restrictions
""""""""""""""""""

In case of the Virtual TAGs application, there are some tips and basic restrictions to be applied:

* **Maximum number of TAGs by resource**: 50

* **Maximum key size**: 128 characters

* **Maximum value size**: 256 characters

* **Allowed characters**: 
  
  * The allowed characters are: letters (a-z, A-Z), numbers (0-9) and representable spaces, besides the following characters: + - = . _ : / @.

  * To enable instance tags in metadata, the instance tags keys allow use of the letters (a-z, A-Z), numbers (0-9) and the following characters: + - = . ,  _ : @. Avoid spaces or / , and it can’t form only . (a dot), .. (two dots) or _index.

.. note:: For any resource, each key tag must be exclusive and can only have one value.

.. important:: The keys and TAGs values are Case Sensitive, in other words, differentiate **UPPERCASE from lowercase**. 

.. warning:: The **aws** prefix it’s reserved for the Amazon Web Service (AWS) use. It’s not possible to edit nor exclude the key or the value of a TAG when it has a key with this prefix. The TAGs with the aws prefix: don’t count to TAGs by resource limit.

----

How to use
""""""""""""

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

----

.. Cost Threshold
.. ~~~~~~~~~~~~~~

.. Billing Menu (USN)
.. ---------------------

.. Brazilian Govern Environment
.. ---------------------------

.. Billing Menu / USN Billing
.. =============================

----

Service Order Menu
====================

Using the Service Order
-------------------------

Creating the Service Order
--------------------------

Add Cost Estimate in USN and TSU
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Managing Service Order
-----------------------

Card: General
~~~~~~~~~~~~

Card: Cost Estimate (USN)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Card: Cost Estimate Configuration (TSU)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Card: Agreement
~~~~~~~~~~~~~~~~

.. Service Order Menu
.. =====================

.. Managing Service Order
.. ------------------------------

.. General Section - Service Order
.. ------------------------------

.. Estimate Cost Section (USN)
.. ------------------------------

.. Cost Estimate Configuration (TSU)
.. -----------------------------------

.. Agreement
.. ---------

----

Recommendation Menu (new)
=========================

----

Account Providers Menu
=======================

This menu is on the editing phase. Substituting to the menu below.

----

Containers Menu
==============

.. attention:: This menu is re-elaboration for updates, after the improvements occurred this month.

Managing a Container
---------------------

Creating New Container
----------------------

----

Hosts Menu 
==========

Create Hosts
-------------

Viewing a Host
----------------

----

Networks Menu 
=============

Networks
--------
  
Manage Network
----------------

Add “Subnet” in the AWS environment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Add  “Subnet” in the Azure environment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Add “Subnet” in GCP environment
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Add “Subnet” in the Private environment (VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create New Network
------------------

Create Network in Public Cloud Service Providers
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create Network in Private Network (On-Premisses)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create Network in Public Cloud Service Providers (AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create Network in Public Cloud Service Providers (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create Public Cloud Service Providers (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create Network in Private Environment (VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Public IPs
------------
   
Requesting a Public IP (**AWS and GCP**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Requesting a Public IP (**Azure**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Requesting a Public IP (private environment, e.g: **VMware vCenter**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Security Groups and ACLs
--------------------------

Manage Security Group
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Create Security Group
~~~~~~~~~~~~~~~~~~~~~~~~

Key Pair
-----------

Manage a Key Pair
~~~~~~~~~~~~~~~~~~

Creating a Key Pair
~~~~~~~~~~~~~~~~~~~~

Importing a Key Pair
~~~~~~~~~~~~~~~~~~~~~~

Load Balancers
----------------

Managing Load Balancer
~~~~~~~~~~~~~~~~~~~~~~~

Creating Load Balancer (Environments: AWS and GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creating Load Balancer (Environment: Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

vCloud Resources Group
----------------------

Create Resources Group
~~~~~~~~~~~~~~~~~~~~~~

.. DNS Zones
.. ---------

.. Manage Public DNS Zone
.. ~~~~~~~~~~~~~~~~~~~~~~~

.. Create Public DNS Zone (AWS and GCP)
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. Create Public DNS Zone (Azure)
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. Create Private DNS Zone - Observation
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

VPN
---

Create VPN in 3 Steps
~~~~~~~~~~~~~~~~~~~~~

Create Customer Gateway
~~~~~~~~~~~~~~~~~~~~

Create Private Gateway
~~~~~~~~~~~~~~~~~~~~~~

Create VPN Tunnel
~~~~~~~~~~~~~~~~~~

----

Storages Menu
=============

Create Storage
---------------

Viewing a Storage
-----------------------

----

Templates Menu 
=============

----

Flavors Menu 
============

Create Flavor
--------------

Viewing a Flavor
------------------

----

Workflows Menu 
==============
  
Direct Execution
----------------

Editing Workflow
-----------------

Creating Workflow
----------------

Definition of Workflow
~~~~~~~~~~~~~~~~~~~~~~~~
   
Inclusion of Associated Tasks
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creating Associated Task
--------------------------

Shutdown Task/Activation of Virtual Machine Programmer
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   
Create Snapshot Task
~~~~~~~~~~~~~~~~~~~~~~~

Script Task
~~~~~~~~~~~~~~~~

Client Server (Puppet)
----------------------
   
Provision a Puppet Server
~~~~~~~~~~~~~~~~~~~~~~~

Services Catalog
----------------

Resources: New Service
~~~~~~~~~~~~~~~~~~~~~~

Resources: Sending
~~~~~~~~~~~~~~~~~~

My previous services
~~~~~~~~~~~~~~~~~~~~

Marketplace: History of contracted services
"""""""""""""""""""""""""""""""""""""""

My contracted offers
""""""""""""""""

My registered offers
"""""""""""""""""""""

----

Tasks Menu
===========

Tasks tab
-----------

Pending Approvals Tab
-----------------------

Scheduled Tasks Tab
--------------------

----

Resources Inventory Menu
=======================

Create dynamic resources group
------------------------------

Native Tags Editor
--------------------

Tag
~~~~

Without Tag
~~~~~~~~~~
----

Colors and Custom Menu (new)
============================

Graphic interface Customization
-------------------------------

Theme info
~~~~~~~~~~

Identity
~~~~~~~~

Colors: Light mode
~~~~~~~~~~~~~~~~~~

Colors: Dark mode
~~~~~~~~~~~~~~~~~~

Registered themes
~~~~~~~~~~~~~~~~







.. |atencao| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/hand-stop-o.png?raw=true

.. |nota| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/hand-pointer-o.png?raw=true

.. |importante| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/warning.png?raw=true

.. |dica| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/asterisk.png?raw=true