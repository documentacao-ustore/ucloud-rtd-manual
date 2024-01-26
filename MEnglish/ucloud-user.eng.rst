

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

Account
-----------------

Introduction
~~~~~~~~~~~

Account Type
~~~~~~~~~~~~

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

Accessing CMR.v1
""""""""""""""""

Creating CMR.v1
""""""""""""""""

Following the status on the Tasks menu
"""""""""""""""""""""""""""""""""""""""

Enabling the CMR.v1’s download
"""""""""""""""""""""""""""""""""

Viewing CMR.v1
"""""""""""""""

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

**Utilities**
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
~~~~~~~~~~~~~~~~~~~~

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
~~~~~~~~~~~~~~~~~~~~~~~~~

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
~~~~~~~~~~~~~

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
~~~~~~~~~~~~~~~~~~~~~~~~~~~

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
~~~~~~~~~~~~~~~~~

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
~~~~~~~~~~~~~~~~~~~~~

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
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Currently, this implementation groups Tags and gathers them in the “Dimension” created, facilitating the categorized visualization in other functionalities of the platform.

Furthermore, the “Dimension” is used in the modal “Create Budget” included in the card named “Sub Budget Details” in disambiguation_ .

.. _disambiguation: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Release-Notes/release.ing-ucloud-2022-jun.jul.aug.html#creating-budget-and-sub-budget

====

**Virtual Tags**
~~~~~~~~~~~~~~~~~
   
uCloud’s platform Virtual Tags
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
   
Normalizing Virtual Tags
~~~~~~~~~~~~~~~~~~~~~~~

When to use
~~~~~~~~~~~~~

Tags restrictions
~~~~~~~~~~~~~~~~~

How to use
~~~~~~~~~~~~

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