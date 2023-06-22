

.. image:: /figuras/mangue-logo-peq.png
    :alt: Logo Mangue
    :scale: 50 %
    :align: center
=====

Mangue.io - User Manual
+++++++++++++++++++++++


Information technology solutions that make it possible to implement a scalable, solid and reliable computing architecture in a distributed cloud. 


====


Presentation
============

This document aims to explain the use of the Mangue.io Platform, an environment management platform for multiple container orchestrators. 

This manual introduces the concepts, screens, functionalities and commands for using this product. 


====


Introduction
============

Mangue.io is an environment management platform for multiple container orchestrators, which allows the orchestration, implantation (location and scheduling) and operationalization (execution) of application containers within one or more computing clusters (public or private) or among them.

The platform operates on a hybrid multicloud model and, this way, allows the organizations total control, support for sustaining backups, replication and environment migration. Centered on an agile, secure and productive approach to continuous application delivery for implantation, tests and updates with zero downtime and deployments rollback. 

The Mangue.io Platform supports the implantation and operationalization of image-based applications from a registry service. Besides, it also allows the creation of services for the applications (internal or external to the cluster to which the application belongs).

====


Access to the Platform
======================

The access to the platform is done through a website, the user must use an internet browser, after inserting the URL/link address they view the initial presentation screen. 

After starting a session in the chosen internet browser, the address/path to access the application must be filled out as displayed next: 

https://<mangueserver_IP_Address>:80

https://mangue_Server_Name.com/

After inserting the address correctly, the user's login screen is similar to the image below: 



.. image:: /figuras/fig_mangue/001_mangue_login.png
    :alt: Login screen 
    :scale: 80 %
    :align: center
=====


The credentials for the login and password are the same as those of the uCloud platform, which the Mangue.io platform is integrated with. Every user provisioned on the uCloud can automatically use their credentials to gain access to Mangue.io. 

After inserting the access credentials (login and password) and performing the login procedure, a similar figure may be presented to the user, in case of existing a cluster associated with the user's in the Mangue.io contract. 


.. image:: /figuras/fig_mangue/002_mangue_tela_inicial.png
    :alt: Home screen 
    :scale: 80 %
    :align: center
=====


The screen above represents an example of the home screen that the user views after entering valid credentials to access the Mangue.io platform. 

====


Browsing Settings
=================

On the upper right corner of the platform there is a configuration menu that is identified by a gear |icone_engrenagem| , in which the user has the option to select which contract, cluster and/or which namespace (namespaces are workspaces) they want to have access to.

By clicking on any of the blanks, the information on the screen changes automatically. 

.. image:: /figuras/fig_mangue/003_mangue_aba_selecao.png
    :alt: Configuration Selection tab 
    :scale: 80 %
    :align: center
=====



When selecting a contract, the options for selecting clusters are updated, listing only the ones that are associated to the selected contract, as well as the permissions that the logged in user has on these clusters - corresponds to the level of permission they have in the uCloud contract. 

The contracts that appear in this part are only those that already have some cluster integrated with the Mangue.io, in the sequence of this document the description of how to integrate and/or create a cluster in the application. On the selection occasion, the cluster that the platform is communicating with is changed and the information on the screen is updated for this new context. 

The moment the user selects the cluster and namespace, the values on the Overview screen are changed with the specific data of the user's selection. 

====

Home screen
===========

The Overview home screen displays some graphs referring to the consumption values of computing resources specific to the user's selection, the details of the graphs follow below:


Cluster Monthly Price Graph
---------------------------

This bar graph displays the cost evolution referring to the use of the computing infrastructure that supports and executes the applications.

On the vertical axis, you can follow the value and, on the horizontal axis, the value referring to the consumption of infrastructure on a daily basis is presented. It is possible to select the time gap to visualize the infrastructure consumption, being able to view the last 7 days, the last 20 days, the current month, the previous month, as well as customize a desired time interval. 

It is possible to observe that the values fluctuate due to the consumption of computing infrastructure resources to support all applications (deployments) that are active in the selected cluster. 


.. image:: /figuras/fig_mangue/004_mangue_preco_mensal_cluster.png
    :alt: Cluster Monthly Price Graph 
    :scale: 80 %
    :align: center
=====

This graph allows you to track the variation of the **actual infrastructure cost** required to maintain and support the running of a cluster, day by day. In the area: “Graph title” it is possible to know the total accumulated value, until the present day. 

These values are stored in an internal database of the Mangue.io platform, so the user can monitor the evolution of the value referring to the computing resources consumption to support an active and functional cluster. 

If the user wishes, this database (“Ticket”) can be cleared, removing all the information stored, in order to zero all the accumulated values. 

For this purpose, the user must click on the “Trash Bin” |icone_lata_lixo_preta| icon. The Mangue.io platform requests a confirmation from the user for the action displaying the screen below: 


.. image:: /figuras/fig_mangue/005_mangue_deletar_bilhetador.png
    :alt: Delete financial data from the Ticket Cluster 
    :scale: 80 %
    :align: center
=====


For the user to confirm the action of deleting all financial data (values) of consumption referring to the selected cluster in the “Browsing Settings” tab, click on the green-colored button ``Delete``. 

With this action all cluster consumption values are removed and a new period of information collection is started, losing all the information accumulated (the historic series) of the selected cluster. 


Cluster Consumption Value Calculation 
--------------------------------------

The values presented here are calculated based on the value/hour of vCPU and RAM Memory that is stored in the Mangue.io database. 

The Mangue.io Platform stores the resources consumption (CPU and Memory) of applications every minute; at the end of an hour (60 minutes), it  stores the total value of consumption in these 60 minutes. At the end of each day (24 hours) the Mangue.io Platform stores the value related to the consumption of computing resources, to keep all the applications active in each container. 

The CPU and Memory price used is the same price as the contract resources, the value is defined through uCloud, the contract price can be viewed on the Mangue through the **Permissions/ Contract** screen: 

.. image:: /figuras/fig_mangue/005.1_mangue_formula.png
    :alt: Mangue.io formula
    :scale: 80 %
    :align: center
=====


At the end of each 24-hours cycle, the total consumption value of the computing resources is stored in the Mangue.io Platform database and previously presented in the graph in: Cluster Monthly Price.


Total CPU Usage Graph
---------------------

On this screen, it is also possible to visualize the CPU usage, in millicores, of each Kubernetes resource, for this, the user has to specify the namespace and the resources they wish to view the CPU consumption, and click on the “Magnifying Glass” icon |icone_lupa_vermelha|, to do the search, returning the last thirty minutes of CPU and Memory consumption.


.. image:: /figuras/fig_mangue/006_mangue_uso_total_cpu.png
    :alt: Total CPU usage 
    :scale: 80 %
    :align: center
=====


Total Memory Usage Graph
------------------------

When searching for the Total CPU Usage Graph item, the platform retrieves information on the value of memory consumption, in MegaBytes, of the last thirty minutes of memory consumption corresponding to the namespace and selected resource.


.. image:: /figuras/fig_mangue/007_mangue_uso_total_memoria.png
    :alt: Total Memory Usage  
    :scale: 80 %
    :align: center
=====


User Menu
=========
The user menu bar is located on the left of the screen and, initially, is presented in expanded mode, as displayed on the picture below.


.. image:: /figuras/fig_mangue/008_mangue_menu_usuario_expandido.png
    :alt: User Menu (Expanded Mode) 
    :scale: 80 %
    :align: center
=====


Some menu options have a submenu, which are presented when the user places the mouse over the indication (less than sign “<”). When clicking on this icon |icone_sinal_menor|, the interface presents this option's submenu to the user, see the example in the figure below.


.. image:: /figuras/fig_mangue/009_mangue_submenu_workload.png
    :alt: Submenu Example 
    :scale: 80 %
    :align: center
=====


Workloads
=========

On this Workloads user menu option, the dashboard presents information about Deployments, *Daemonsets*, Horizontal Autoscaler, *StatefulSets* and Updates.


.. image:: /figuras/fig_mangue/013_mangue_submenu_workload.png
    :alt: Workloads Menu 
    :scale: 80 %
    :align: center
=====


A **Deployment** is a Kubernetes object, the orchestrator used by the Mangue.io, which is nothing else than an implantation controller that provides declarative updates for two other Kubernetes objects: Pods and *ReplicaSets*.

The **Pods** are the smallest implantable logical (computing) units that can be created and managed from within the Mangue.io. *ReplicaSet* has the objective to maintain a stable set of Pods replicas in execution at any moment. 

The **StatefulSet** is the workload API object used to manage applications in state. It is responsible for managing the implantation and dimensioning of a set of Pods and provides guarantees about their order and uniqueness. 

The **Daemonsets** manage a group of replicated pods. However, *DaemonSets* tries to adhere to a model of one pod per node, whether it is cluster-wide or on a subset of nodes. As the nodes are added to a cluster, the *DaemonSets* automatically add pods to new nodes as needed.

The **Horizontal Autoscaler** automatically dimensions the number of pods in a replication controller, replica set or stateful set based on observed CPU utilization (or supported by custom metrics, on some other metrics provided by the application). Note that the pod horizontal automated scaling does not apply to objects that can not be scaled, for example, *DaemonSets*.

====


Deployments
-----------

The Workload/Deployments menu presents all deployments of a cluster in a certain namespace.

A **Deployment** is a Kubernetes object, the orchestrator used by the Mangue.io, which is nothing more than an implantation controller that provides declarative updates for two other Kubernetes objects: Pods and *ReplicaSets*.


.. image:: /figuras/fig_mangue/014_mangue_workloads_deployments.png
    :alt: Workloads Deployments 
    :scale: 80 %
    :align: center
=====


On the table the following columns are presented with their respective information: 

* **# actionable column:** This column presents an alternative way to remove (delete) multiple rows with a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|. When the user choses a line or several, the Mangue.io platform presents the icon(s) above this column, they represent user actions to be performed at once in all selected lines. In this case three icons with very distinct actions are displayed:
  
  * **Rollback |icone_reversao|:** This option allows the user to perform an action of reversing the current version of the selected deployment(s) for its immediate previous version to the existing one on the Mangue.io Platform. 
  
  * **Scale |icone_escalar|:** The function of this screen allows the user to inform the number (full) desired to increment the application (deployment) replica number.
   
  * **Trash bin |icone_lixo_vermelho|:** This option allows the user to remove all the selected items with a single command.
  
  * **Change version |icone_alterar|:** This option allows the user to update multiple deployments at once, to which the user can inform the next version of each of them.
  
* **Deploys:** It is the representation of the *deployment.d name*;
  
* **Labels:** These are the deployments' identifiers, they are used to link to a service;
  
* **Instances:** Presents the number of replicas that are operational of a deployment, and the total number of operational replicas desired for this deployment. They are divided by a slash (“/”) where the values found before the slash are the operational replicas, and the values after the slash represent the expected amount of operational replicas;
 
* **Status:** The status of a deployment identifies its current state. They can be presented as Running, Pending or “!” (exclamation mark):
  
  * The **Running** status identifies that no error is happening with the deployment;
  
  * The **Pending** status identifies some transition state in the deployment. Whether it is by update, container process initialization or any other activity that identifies a transition state;
  
  * The **“!”** status (exclamation mark) identifies an alarm, in other words, that something went wrong with the deployment and its replicas. For example: the image of a container is passed with an inexistent version, thus, its download does not occur;
  
* **IP Access:** If the deployment has an associated service it is on this blank where the load balancer IP may be a service of type *loadbalancer*; port for access to the service if it is an external service (type *nodePort*) or the “intern IP” string in case it is an internal cluster service (type *ClusterIP*);
  
* **Image and Version:** In case there is more than one image or version of a container, they are listed one below the other, as in the example of the sixth deployment listed in the image of the deployment table;
  
* **Actions:** The last column presents a dropdown menu of actions that can be performed on the deployments:


.. image:: /figuras/fig_mangue/015_mangue_dropdown_menu_acoes.png
    :alt: Dropdown Actions Menu 
    :scale: 80 %
    :align: center
=====


A. **Add Persistent Volume Claim**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Applications that run in containers store their data in memory, and containers and pods that are run by Kubernetes can eventually die, which impacts the loss of data stored in memory. In case a user has sensitive information to persist, such as database volumes, a *PersistentVolumeClaim* must be created.



.. image:: /figuras/fig_mangue/016_mangue_add_pvc.png
    :alt: Add PersistentVolumeClaim 
    :scale: 80 %
    :align: center
=====


On this screen the user must fill out the blanks with the following information:

* **Name:** Inform the volume name the user wants to create.
  
* **Size:** The user must fill out a full number that represents a volume size file to be created.
  
* **Size Unit:** The user must select the size unit that will be used to create the volume. The options are:
  
      * **Kilo:** Kilobytes when the user wants to create a file with the previous value multiplied by 1,000;
  
      * **Mega:** Megabytes when the user wants to create a file with the previous value multiplied by 1,000,000;
  
      * **Giga:** Gigabytes when the user wants to create a file with the previous value multiplied by 1,000,000,000;
  
      * **Tera:** Terabytes when the user wants to create a file with the previous value multiplied by 1,000,000,000,000;
  
      * **Peta:** Petabytes when the user wants to create a file with the previous value multiplied by 1,000,000,000,000,000;


.. attention:: The Mangue.io Platform does not validate, previously, if there is an available disk space, in the informed size. No warning is presented to the user, if the computing environment does not have the necessary space, no error message is presented when creating this persistent volume with the informed characteristics.



.. note:: The user may verify an error indication, on the **Status** column on the menu Workloads / Deployments screen and consult the specific deployment, to which the *PersistentVolume* is associated with, as the previous image displayed on the Deployments topic.


* **StorageClass:** The user must select which NFS Storage volume are available in the presented list;
  
* **Access Mode:** This column presents the access configuration to this volume, there are three access mode, they are:
  
      * **ReadWriteOnce:** The volume is mounted and can only receive read and write instructions from a single node;

      * **ReadOnlyMany:** The volume is mounted and has read-only permissions, but from different nodes simultaneously, writing is not allowed;

      * **ReadWriteMany:** The volume is mounted and can read and write instructions simultaneously, but from different nodes;

* **Container:** When the user clicks on this location, the name of the application container will be displayed with a symbol similar to this “□”;

* **Mount Path**: Is the path where the volume is mounted in the container. If the application is based on a Linux environment, the volume mount path must use the operating system notation corresponding to the environment; if the application environment is based on an MS-Windows environment, the volume mount notation must be used with the corresponding operating system folders.

To confirm all the values and options informed, the user simply clicks on the ``Finish`` button to create the *PersistentVolume* and wait for the creation feedback in the upper right corner of the Mangue.io Platform screen.

====

B. **Add Service**
~~~~~~~~~~~~~~~~

The second option of this submenu allows the user to add a service, when clicked the following modal interface screen is opened:


.. image:: /figuras/fig_mangue/017_mangue_add_servico.png
    :alt: Add Service Deployment
    :scale: 80 %
    :align: center
=====



On this modal, the user must fill in the following blanks:

* **Name of the service:** The user must fill out with the service name they want to create;
  
* **Deployment Labels:** The user must inform the labels that are associated with this service;
  
* **Types of access to the service:** Internal, External or *LoadBalancer:*
  
      * **Internal:** Services that can only be accessed from inside the cluster;
  
      * **External:** Corresponds to services that allow access from outside the cluster. A TCP-IP port between 30,000 –– 32,767 is provided;
  
      * **LoadBalancer**: Integrated straight with the Cloud Providers (AWS, AZURE, GOOGLE) creating a LAYER 7 *loadbalancer* for the respective app;
  
* **Source port:** Inform the TCP-IP port number of the container allocated to the service;
  
* **Destination port for the service:** Inform the TCP-IP source port in the container, the service will receive the request on the source port and forward it to the destination port;
  
* **Select the protocol:** TCP or UDP.
  
* ``Add`` **button:** If the service needs to expose more than one port, the user must return to the SourcePort/Destination  Port,  and add as many source/destination ports as necessary. 

To confirm all the options informed above, the user must click with the mouse on the ``Create Service`` button and wait for the creation feedback.

====

C. **Delete Deployment**
~~~~~~~~~~~~~~~~~~~~~~~~

The third option of this submenu allows the user to remove definitely a Deployment from the cluster and from the namespace that was selected in the **Configurations** tab; when clicked, the following modal interface screen is opened, requesting confirmation from the user:


.. image:: /figuras/fig_mangue/018_mangue_deletar_deployment.png
    :alt: Delete Deployment 
    :scale: 80 %
    :align: center
=====

This action is immediate and irreversible, the Mangue.io Platform removes the deployment selected by the user from the contract/cluster/namespace.

Just click over the button ``Delete`` to confirm the action and the Mangue.io Platform deletes the deployment from the selected environment.


.. note:: This action **does not** remove any additional components external to this deployment - e.g.: an associated *PersistentVolume*, therefore if an external file exists, it continues to exist on the destination volume. This action only removes the deployment from the environment, but does not remove any other additional files from the computing environment. 

====

D. **Edit Deployment**
~~~~~~~~~~~~~~~~~~~~~~

Some information is not editable through the Mangue.io forms. Elements, such as: 

    * Container port;
    * Add some environment variable;
    * Remove some environment variable.

In meeting all edition demands for a Deployment, it is possible to directly edit the Deployment YAML in the Mangue.io Platform.

This option displays as example the image: Edit Deployment. Its content represents the JSON file with all the configurations of the deployment in Kubernetes, the user can edit whatever is necessary, confirm by pressing the ``Edit`` button and wait for the action feedback by the  Mangue.io Platform.

This functionality meets the users that have knowledge about the Kubernetes files format.


.. image:: /figuras/fig_mangue/019_mangue_editar_deployment.png
    :alt: Edit Deployment 
    :scale: 80 %
    :align: center
=====


E. **Change Tags**
~~~~~~~~~~~~~~~~~~

The function of this screen allows the user to change the Tags associated with the selected application. From there, it is possible to create a Tag, by clicking on the |icone_adicionar| icon, to be associated with the application.


.. image:: /figuras/fig_mangue/019.1_mangue_alterar_tag.png
    :alt: Change Tags 
    :scale: 80 %
    :align: center
=====

.. important:: To create a Tag is necessary to specify its key and value.

.. image:: /figuras/fig_mangue/019.2_mangue_criar_tag.png
    :alt: Create Tag 
    :scale: 80 %
    :align: center
=====

F. **Scale Deployment**
~~~~~~~~~~~~~~~~~~~~~~~~

The function of this screen allows the user to inform the number (full) desired to increment the number of replicas of the application (deployment), which starts automatically after the confirmation with the click of the mouse over the ``Scale`` button.


.. image:: /figuras/fig_mangue/020_mangue_escalar_deployment.png
    :alt: Scale Deployment
    :scale: 80 %
    :align: center
=====

It is important to highlight that there is an increase in the usage consumption of CPU and cluster memory to support the simultaneous execution of the replicas of this application in the cluster infrastructure. 

====

G. **Migrate Deployment**
~~~~~~~~~~~~~~~~~~~~~~~~~~

In the sixth option of the Deployment actions menu, there is the option to migrate the deployment between different clusters configured in the Mangue.io Platform.

The user must select which cluster integrated with Mangue.io they wish to migrate the chosen deployment. 

The recipient cluster blank is a “dropdown list” type, when the user clicks on it, the list of available clusters associated with the chosen contract in the configuration menu is presented.

To do the migration, the user just needs to click on the ``Migrate`` button and wait for the action feedback from the Mangue.io Platform. As a result of this action, a “Success” alert will be displayed on the upper right menu of the screen.


.. image:: /figuras/fig_mangue/021_mangue_migrar_deployment.png
    :alt: Migrate Deployment 
    :scale: 80 %
    :align: center
=====

H. **Modify Version**
~~~~~~~~~~~~~~~~~~~~~~

After clicking on “Update Application Version” the platform presents the image “Update Deployment Version”. Through this control, the user can generate a “new version” for any deployment existing on the Mangue.io Platform. 


.. image:: /figuras/fig_mangue/022_mangue_atualizar_deployment.png
    :alt: Update deployment version 
    :scale: 80 %
    :align: center
=====

This blank is alphanumeric and the user can enter the desired information to identify the new version of the selected deployment. The new versions are under the sole control of the user, as they refer to the offers created by this user. 

After filling with the desired information, the user must click on the ``Send`` button to confirm the action to create a version for the deployment.


.. attention:: These new versions are not necessarily related to any version of the composing softwares, or any software that was used to compose the offer, different versions can be found outside of the Mangue.io platform.


====

J. **Rollback**
~~~~~~~~~~~~~~~~

This option allows the user to perform the action of reverting the deployment version to its version immediately prior to the existing version on the Mangue.io Platform.

This action in particular does not activate any additional confirmation screen, its action is immediate.

.. important:: By selecting this option, the Mangue.io platform performs the reversal of the version immediately without requesting any confirmation from the user.

.. note:: Caution and attention are recommended, as this action creates some type of low performance to the deployment in which is being performed the action of rollback.

====

Deployment Information
----------------------

If the user clicks over a deployment name, the Mangue.io platform presents the deployment details screen, as shown in the picture below.

The user can note that this screen has several sections, each one described below respectively.


.. image:: /figuras/fig_mangue/023_mangue_overview_deployment.png
    :alt: Deployment overview 
    :scale: 80 %
    :align: center
=====


A. **Section:: Deployment Overview**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This section displays three graphs, two of performance and one of value:

* CPU;

* Memory;
  
* Price in the last 30 days.

They display the performance of the CPU (in millicores), Memory (in megabytes) and Price in the last 30 days, all regarding the deployment selected by the user. The red line on the price graphs indicates the tendency of the graph.

Interaction buttons are also displayed for the user, they can specify the period of CPU and Memory graphs.


.. image:: /figuras/fig_mangue/024_mangue_consumo_deployment.png
    :alt: Overview do consumo do deployment 
    :scale: 80 %
    :align: center
=====


B. **Section: ReplicaSet**
~~~~~~~~~~~~~~~~~~~~~~~~~~

The **Replicaset** section presents a table that lists all the presented *replicasets* for a deployment, on this list is shown information such as:

   * Name;
  
   * Number of pods available;
  
   * Number of total pods at a given moment;
  
   * Image along with its specified version;

   * Time (in days) since the creation of this *replicaset*;

   * A button with the option to delete it, as shown in the figure below.
  

.. image:: /figuras/fig_mangue/025_mangue_replicaset.png
    :alt: ReplicaSet 
    :scale: 80 %
    :align: center
=====


On this part, the Mangue.io platform presents the following information:

* **#**: Sequential number of the *replicaset* in this list;
  
* **Name**: This column presents the *replicaset* name, the user can verify that the Kubernetes environment generates unique names for each *replicaset*;
  
* **Available pods**: This column presents the number of pods for this *replicaset*;
  
* **Total Pods**: This column presents the total amounts of pods, configured for this *replicaset*;
  
* **Image**: This column presents the image file information used to create this deployment;

* **Duration**: This column presents the total of days this *replicaset* exists since the moment of its creation until the present day the user views this list.

====

C. **Section: PODs**
~~~~~~~~~~~~~~~~~~~~

In the **Pods** section there is a table with the list of all the pods present for the deployment, each one details their information such as:

    * Name;

    * Node in which it is being run;

    * Current status of the pod;

    * Image along with its version and duration.
  

.. image:: /figuras/fig_mangue/026_mangue_pods.png
    :alt: PODs 
    :scale: 80 %
    :align: center
=====


On this section, the Mangue.io platform presents the following information:

* **Name**: Deployment name that is established when it is created;

* **Node**: Presents the name of the Kubernetes node that is executing this deployment;

* **Status**: Presents the deployment status in its respective node. The status of a deployment identifies the current state. They can be represented by:

      * **Running** identifies that no errors are happening with the deployment;
  
      * **Pending** identifies some transition states in the deployment. Whether it is by update, container process initialization or any other activity that identifies a transition state;
  
      * **!** (exclamation mark) identifies an alarm, in other words, that something wrong happened with the deployment and its replicas. For example: the image of a container is passed with an inexistent version, thus, its download does not occur;

* **Image**: This column presents the information of the public image that was used for the creation of this deployment. This image can be found in public websites that contain technical information regarding the application itself, an example is the *Docker Hub* (https://hub.docker.com/);

* **Duration**: Presents the time (in days) elapsed since the creation of this deployment;

* **Actions**: This column presents the ``Actions`` button |icone_acao| when clicked, it displays the actions that can be performed on each listed pod, as shows the following picture:
  

.. image:: /figuras/fig_mangue/027_mangue_submenu_pods.png
    :alt: submenu PODs 
    :scale: 80 %
    :align: center
=====


Each of the options of this submenu is detailed and described below:

* **Delete Pod**: When clicking on the delete option, just wait for the action’s feedback. It generates an alert of “Success” or “Error” on the superior right menu. As the first option exists a pod deletion in question, when selecting this option the following modal appears:
  

.. image:: /figuras/fig_mangue/028_mangue_deletar_pod.png
    :alt: submenu actions Delete POD 
    :scale: 80 %
    :align: center
=====


* **Performance Graph**: The second option allows the user to observe the CPU and Memory graph performance of each pod, once this option is clicked, the screen below is presented to the user with the consumption graphs of CPU and memory of the selected pod.


.. image:: /figuras/fig_mangue/029_mangue_performance_pod.png
    :alt: submenu POD Performance  
    :scale: 80 %
    :align: center
=====


* **Log**: This third option allows the user to view the logs of a particular pod in a similar way to what one obtains with a SSH terminal console emulation session. The user is capable of filtering the number of records (rows) that they wish to see (options are: 10, 20, 50, 100, 300, 500, 1000, all). 
  
In case the pod has more than one container running, there is a dropdown where is possible to select which container the user wants to view the logs, as is shown in the following image:


.. image:: /figuras/fig_mangue/030_mangue_log_pods.png
    :alt: submenu Actions LOG several PODs 
    :scale: 80 %
    :align: center
=====


* **Command Line**: The fourth option offers the user to run command lines at the pod's operating system prompt, similar to what you get with an SSH terminal console emulation session. This functionality extends to one or more containers that existed within the pod in question. 


.. important:: To enable this function it is necessary to access the Integrations Menu and follow the steps corresponding to Container Execution. 


In case the pod has more than one container running, there is a dropdown that is possible to select which container the user wants to execute the commands, as shown in the following image:

.. image:: /figuras/fig_mangue/031_mangue_comando_pod.png
    :alt: submenu Actions Command Line other POD 
    :scale: 80 %
    :align: center
=====


D. **Section:: Volumes and Secrets**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

In this section are listed all the **Volumes** (files that store data) or **Secrets** (files, or authentication definitions when necessary), associated with the deployment selected.


.. image:: /figuras/fig_mangue/032_mangue_volumes_segredos.png
    :alt: Volumes and Secrets 
    :scale: 80 %
    :align: center
=====


The Mangue.io platform presents the following information in this section:

      * **#**: This column presents the sequential number of the volume or secret, shown in this list;

      * **Name**: This column displays the name of the volume or secret (operating system file) presented in this list;

      * **Type**: This column presents what is the type of item shown in this list, which can be a **volume** or **secret**

====

E. **Section: Events**
~~~~~~~~~~~~~~~~~~~~~~

In this section, all events linked to a deployment are listed. These events can be: due to an alteration in the quantity of Pods/Replicas, a change in the version of the deployment containers or any other change in its state.


.. image:: /figuras/fig_mangue/033_mangue_eventos.png
    :alt: Eventos de Deployment 
    :scale: 80 %
    :align: center
=====


The Mangue.io platform presents the following information in this section:

    * **#**: Event sequential number in the presented list;
  
    * **Created in**: Presents the total number of days, until the present date, since the event surge on the Mangue.io platform;
  
    * **Type**: Describes the type of event that occurred, and the following types of events can be listed:
  
      * **Normal**;
  
      * **Warning**.


    * **Object**: Describe which object configured in the Mangue.io platform was the source of the listed event. The identification of object type allows the user to identify this origin so they can have access to it and act in the event resolution, through its redefinition, or opt for its removal. Its type can be some of those listed below:

     * Deployments;
     * *Daemonsets*;
     * Horizontal Autoscaler;
     * Pods;
     * *Statefulsets*;
     * Updates;
     * Services;
     * Ingress;
     * *StorageClass*;
     * *PersistentVolumes*;
     * *PersistentVolumesClaim*.


  * **Message**: On this column the Mangue.io platform presents a list of messages that can help to identify the success of the event or the root cause of a potential problem, thus allowing the user to take some action to eliminate the root cause of the problem or being secure of the success of this event.
  

     * Pulled;
     * Created;
     * Started;
     * *NoPods*;
     * *FailedGetScale*;
     * *ProvisioningFailed*;
     * *FailedBinding*.
  
====

F. **Section: Pods Horizontal Autoscaler**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The Mangue.io platform allows the user to define the rules so the deployment performance is always the best possible, and the Mangue.io platform can increase the deployment processing in parallel, run several instances (replicas), to guarantee that users always have the best usage experience possible. 

It is worth mentioning that it is necessary to extract an instance of the Kubernetes Metrics Server active and operating in the cluster, for the Horizontal Pod Auto Scaler execution to occur. By default, the Mangue.io installation contemplates the installation of the metrics service.

In case the deployment does not have any Horizontal Autoscaler, the screen is presented as the example below:


.. image:: /figuras/fig_mangue/034_mangue_autoescalador_inexistente.png
    :alt: No horizontal autoscaler found
    :align: center
=====


For the user to create a **Scaler** rule, just click on the plus sign icon |icone_adicionar| by the example of the image above, for the interface to be presented where the user configures the rule(s) of how the platform should measure the infrastructure consumption of the deployment to start new replicas within the computing infrastructure so that the performance is met.


.. image:: /figuras/fig_mangue/035_mangue_criacao_autoescalador.png
    :alt: Horizontal Autoscaler - Creation 
    :align: center
=====

* **Minimum of Replicas**: Inform the minimum value of replicas of the deployment (a full number is mandatory - e.g: 1, 2) that the Mangue.io platform must keep active so the application has a minimum required performance, ensuring the user experience optimization. The minimum value for this blank is "one” (1);


* **Maximum of Replicas**: Inform the maximum value of replicas of the deployment (a full number is mandatory - e.g: 1, 2) that the Mangue.io platform must start for the application to support the growth in demand for users access and guarantee the optimization of the user experience. The maximum value for this blank is “fifteen” (15);


* **% Maximum of CPU usage**: The user must click on the green button with the plus sign ‘+’ for the platform to present the blank where the user informs the maximum percentage value (a full number is mandatory - e.g: 20, 22, 30) to be used by the Mangue.io as the maximum CPU allocation limit to execute a deployment replicas. This number is the maximum limit that the platform considers to start creating and running a new deployment replica. The maximum value for this blank is “one hundred percent” (100%).


* **% Maximum Usage Memory**: The user must click on the green button with the plus sign ‘+’ for the platform to present the blank where the user informs the maximum percentage value (a full number is mandatory - e.g: 20, 22, 30) to be used by the Mangue.io as a maximum limit  for a memory resource allocation to execute the replicas of a deployment. This number is the maximum limit that the platform considers to start creating and executing a new deployment replica. The maximum value for this blank is “one hundred percent” (100%).


It is important to highlight that when confirming the Horizontal Autoscaler event creation, there is a waiting time for it to appear on screen. This time comes from the need for the scaler to collect the metrics to become an active object in Kubernetes. 

The definition of “Scalability Rules” controls the increment/decrement in the number of replicas of the application, and, as consequence there is an increase/decrease in the computing resources consumption to run the largest/smallest number of active replicas. Therefore, there is an increase/decrease in the value of the infrastructure cost, during the time in which the several replicas are executed.

After the definition, or in case of an existing rule, the user sees the screen below:


.. image:: /figuras/fig_mangue/036_mangue_autoescalador_existente.png
    :alt: Horizontal Autoscaler - Existing
    :align: center
=====


* **#**: Horizontal Autoscaler sequential number in the presented list. 
  
* **Nome**: Identifies the name of the Autoscaler created, and normally, it must be the same name as the deployment;
  
* **Min. Replicas**: Identifies the parameter placed in the Autoscaler definition and corresponds to the minimum number of replicas that this scaler keeps active to guarantee the deployment performance.

* **Max. Replicas**: Indicates the parameter placed in the scaler, it corresponds to the maximum number of replicas maintained active to guarantee the deployment performance.

* **Number of Replicas**: Identifies the number of active replicas of the deployment at the present moment.
  
* **CPU Usage**: Presents the defined rule for the autoscaler, for the minimum and maximum limits of CPU usage. This rule must be interpreted as follows:
  
      * The first number is the current consumption of the CPU resource.
  
      * The second number is the maximum limit of CPU occupation, limit which the Mangue.io Platform **commissions** (activate) a new deployment replica.
  
* **Memory Usage**: Presents the defined rule to the autoscaler, for the minimum and maximum limits of memory allocation. This rule must be interpreted in the following way:
  
      * The first number is the current allocation consumption of the Memory resource.

      * The second number is the maximum memory allocation limit, which the Mangue.io Platform **commissions** (activate) a new deployment replica.

**Actions**: This column presents the ``Actions`` button |icone_acao| when clicked displays the actions that can be performed about the Horizontal Autoscaler, there are two options, they are:

      * Delete pods horizontal autoscaler;

      * Edit pods horizontal autoscaler.


.. image:: /figuras/fig_mangue/037_mangue_acoes_autoescalador.png
    :alt: submenu  actions Horizontal Autoscaler 
    :scale: 80 %
    :align: center
=====


By clicking on the “Delete” option the user confirms the removal of the scalability rules created and they are no longer applied to the deployment. 

.. attention:: An alert feedback is created on the superior right corner of the screen informing the success or error. 

The option to “Delete” from the Horizontal Autoscaler Actions menu presents the screen below:


.. image:: /figuras/fig_mangue/038_mangue_deletar_autoescalador.png
    :alt: submenu Actions Delete horizontal autoscaler
    :align: center
=====

By clicking over the “Edit” option, the Mangue.io platform presents the screen below, where it is possible for the user to change the existing values of the Horizontal Autoscaler. The following image “Horizontal Auto Scaler - Creation” presents options on how to change the values. 


.. image:: /figuras/fig_mangue/039_mangue_criar_autoescalador.png
    :alt: Rules of the Horizontal Autoscaler - Creation
    :align: center
=====

It is important to point out that the rules of the Horizontal Autoscaler described above are only associated with the deployment selected by the user.

Through the Workloads/Autoscaler Horizontal menu the user can view all the rules of the Horizontal Autoscaler, configured on the Mangue.io platform, associated with their respective deployments.

=====


G. **Section: Application Price in the Last Month**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This section displays the screen “Application price in the last month”, on it are listed the columns of currency, price per memory, price per CPU and total application price, on the sequence of each one of the columns is detailed:


.. image:: /figuras/fig_mangue/040_mangue_preço_deployment.png
    :alt: Application price (deployment)
    :align: center
=====

* **Currency**: Presents the name of the current currency referring to the values presented in the columns of this table; 
  
* **Price per Memory**: Presents the total value, of the current month, of the RAM memory resource consumption to keep the deployment running  (see the calculation formula);
  
* **Price per CPU**: Presents the total value, of the current month, of the CPU resource consumption to keep the deployment running (see the calculation formula);
  
* **Total APP price**: This column presents the sum of the two previous columns (Price per Memory and Price per CPU). With this information, the user can assess the **real infrastructure cost** necessary to maintain and support the execution of an active and functional 24 x 7 deployment.

====


Daemonsets
-----------

This section presents all the *Daemonsets* of a cluster in a certain namespace, in the following table we have information such as: 


.. image:: /figuras/fig_mangue/041_mangue_daemonsets.png
    :alt: List of Daemonsets
    :align: center
=====

* **#:** Sequential number of the *daemonset* on the presented list;

* **Name:** It's the representation of the *Daemonsets* name;

* **Labels:** *Daemonsets* identifiers, they are used to link to a service;

* **Instances:** Represents the number of operational replicas of a *Daemonsets*, and by the total quantity of operational replicas desired for this *Daemonsets*. They are divided by a slash (“/”) where the values found before the slash are operational replicas, and the values after the slash represent the expected amount of operational replicas;

* **Status:** A *Daemonsets* status identifies its current state. It can be presented by **Running**, **Pending** or **“!”** (exclamation mark):
  
      * The **Running** status identifies that no errors are happening with the  *Daemonsets*;

      * The **Pending** status identifies some transition state in the *Daemonsets*. Whether it is by update, container process initialization or any activity that identifies a transition state;

      * The **“!”** (exclamation mark) status identifies an alarm, in other words, that something wrong happened with the *Daemonsets* and its replicas. For example: the image of a container is passed with an inexistent version, thus, its download does not occur;

* **Access IP:** In case the *Daemonsets* has an associated service is in this blank where the load balancer IP can be a service of the loadbalancer type, port for access to the service can be an external service (*nodePort* type) or a string “intern IP” if it is a intern cluster service (*ClusterIP* type);
  
* **Image and version:**  In case there is more than one image or version of a container they are listed below the other, as in the example of the sixth *Daemonsets*, listed in the image of the *Daemonsets* table;
  
* **Duration:** Presents the duration  time of the *Daemonsets*.
  
* **Actions:** This column presents the ``Actions`` button |icone_acao| when clicked displays the following options:
  
 .. image:: /figuras/fig_mangue/041.1_mangue_acoes_daemonsets.png
    :alt: Edit and delete Daemonsets 
    :scale: 80 %
    :align: center
=====

      * **Edit DaemonSets:** This option presents the *daemonset* in JSON format, the user can edit what is necessary and select the edit option and wait for the action feedback from the Mangue.io Platform.
  
      * **Delete DaemonSets:** When selecting this action, the Mangue.io platform requests the confirmation from the user, as shown on the figure below:


.. image:: /figuras/fig_mangue/042_mangue_deletar_daemonsets.png
    :alt: Confirmation to delete Daemonsets
    :align: center
=====

**DaemonSet Information**
~~~~~~~~~~~~~~~~~~~~~~~~~~
 
If the user clicks on the name of any *Daemonsets* present on the list, the Mangue.io platform displays the screen with a *Daemonset* information, as shown in the example below:

.. image:: /figuras/fig_mangue/042.1_mangue_overview_daemonsets.png
    :alt: Overview Daemonsets
    :align: center
=====


Pods Horizontal Autoscaler 
--------------------------

The Mangue.io platform allows the user to define rules so the application performance is always the best possible and that deployment may increase the parallel processing, several instances of deployment (replicas), to guarantee that the users always have the best user experience possible.

The definition of ‘Scalability Rules’ controls the increment in the amount of replicas of a deployment, and consequently, there is an increase of the cost of the infrastructure, during the time in which the various replicas are running. In the table there is information such as:


.. image:: /figuras/fig_mangue/043_mangue_lista_autoescalador.png
    :alt: Horizontal Autoscaler
    :align: center
=====

* **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel| . When the user choses a line or several, the Mangue.io platform presents an icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. In this case the “Trash bin” icon |icone_lixo_vermelho| is presented, which allows to remove all the items indicated by the user with a single command;
  
* **Name:** Identifies the name of the Autoscaler created, and normally it must be the same name as the Deployment;
  
      * **Min. Replicas**: Identifies the parameter placed at the time of creation of the scaler, it corresponds to the minimum number of replicas which this scaler guarantees for the Deployment it is associated with;
  
      * **Max. Replicas:** Indicates the parameter placed at the time of creation of the scaler corresponding to the maximum number of replicas maintained active to guarantee that the Deployment is associated;

      * **Current Number of Replicas:** Identifies the current state of the number of replicas of the Deployment to which the scaler is associated with;

**Actions:** This column presents the button of ``Actions`` |icone_acao| when clicked displays the actions that can be performed on the Horizontal Autoscaler, there are two options:



.. image:: /figuras/fig_mangue/044_mangue_acoes_autoescalador.png
    :alt: submenu Actions - Horizontal Autoscaler 
    :scale: 80 %
    :align: center
=====

In the Horizontal Autoscaler “Actions” menu there is the option to delete, when selecting it, the following modal is shown:


.. image:: /figuras/fig_mangue/045_mangue_deletar_autoescalador.png
    :alt: Delete Horizontal Autoscaler 
    :align: center
=====

By clicking on the ``Delete`` button the Horizontal Autoscaler is removed, and the scalability rules created are no longer obeyed by the Deployment previously associated. 

.. attention:: A feedback  alert is created in the upper right corner of the screen informing the “success” or “error”.


PODs
-----

A Kubernetes **Pod** is a group of containers, implanted together, in the same host.

Pods operate at a higher level than the individual containers, because it is very common to have a group of containers working together to produce an artifact or to process a working set.

For example:

To illustrate what a pod is, by analogy, it is possible to use the sentence ‘a pod of whales’ that means “a group of whales” in this specific case, the term pod is related to the group of whales.

.. note:: A pod is a group of one or more containers, with shared storage/network resources and a specification of how to run the containers. 

The content of a pod is always put and scheduled together, then executed in a shared context. 

.. important:: A pod models an application-specific “logical host”. It contains one or more application containers that are relatively tightly coupled.

The Mangue.io platform can help the user create as many pods as needed for its Kubernetes environment, associating the Deployment with a Pod is described in another section of this manual, as well as the description of the process creation of a Pod.


.. image:: /figuras/fig_mangue/046_mangue_listagem_pods.png
    :alt: List of PODs
    :align: center
=====

The image above displays the listing of the created pods, followed by a description of the meaning of each one of the seven columns on this screen:

* **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|. When the user choses a line or several, the Mangue.io platform presents the icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. In this case the “Trash bin” icon |icone_lixo_vermelho| is presented, which allows to remove all the items indicated by the user with a single command;

* **Name**: Deployment name that is established in its creation;

* **Node**: Presents the name of the Kubernetes node that is running this Deployment;

* **Status**: Shows the status of the Deployment in its respective node. The status of a Deployment identifies the current state. It can be represented by:

      * **Running** identifies that no errors are happening with the Deployment;

      * **Pending** identifies some transition state in the Deployment. Whether it is by update, container process initialization or any activity that identifies a transition state;

      * **“!”** (exclamation mark) identifies an alarm, in other words, that something wrong happened with the Deployment and its replicas. For example: when the image of a container is passed with an inexistent version, thus, the download of this container does not occur;

* **Image:** This column presents the public image information that was used to create this deployment. This image can be found on public websites that contain technical information regarding the application itself, an example of one used is *Docker Hub* (https://hub.docker.com/);

* **Duration:** Presents the time (in days) elapsed since the creation of this Deployment;

* **Actions:** This column presents the ``Actions`` button |icone_acao| when clicked presents the actions that can be performed over each listed Pod, as shown in the following picture:


.. image:: /figuras/fig_mangue/027_mangue_submenu_pods.png
    :alt: submenu PODs 
    :scale: 80 %
    :align: center
=====

Each of the options of this submenu is described below:

* **Delete Pod**: When clicking on the **Delete** option, just wait for the action’s feedback. An alert of “Success” or “Error” is generated on the top right menu. As the first option exists a Pod deletion in question, when selecting this option, the following modal is shown:


.. image:: /figuras/fig_mangue/028_mangue_deletar_pod.png
    :alt: submenu Actions - delete POD 
    :scale: 80 %
    :align: center
=====

* **Performance Graph:** In the second option, the user is able to observe the CPU and Memory performance graphs of each Pod, once this option is clicked, the screen below is presented to the user with the consumption graphs of CPU and memory of the selected Pod.


.. image:: /figuras/fig_mangue/029_mangue_performance_pod.png
    :alt: submenu Performance of a POD
    :align: center
=====

* **Log**: On the third option, the user is capable of visualizing the logs of a particular Pod in a similar way to what one obtains with a SSH terminal console emulation session. The user is also capable of filtering the number of records (rows) that they wish to observe (options are: 10, 20, 50, 100, 300, 500, 1000, all). If Pod has more than one container running, there is a dropdown where is possible to select which container the user wants to view the logs, as it is shown in the following image:


.. image:: /figuras/fig_mangue/030_mangue_log_pods.png
    :alt: submenu Actions - log multiple pods 
    :scale: 80 %
    :align: center
=====


* **Command Line**: On the fourth option, the user is able to run command lines in the prompt Pod operating system, similar to what one obtains with a SSH terminal console emulation session. This functionality extends to one or more containers that existed within the Pod in question. 
  
.. important:: For this function to be enabled it is necessary to access the **Integrations Menu** and follow the steps corresponding to the **Container Execution**. 

If the Pod has more than one container running, there is a dropdown where is possible to select which container the user desires to execute the commands, as shown in the following image:


.. image:: /figuras/fig_mangue/031_mangue_comando_pod.png
    :alt: submenu Actions - command line other pod
    :align: center
=====

StatefulSets
------------

On this functionality the Mangue platform presents all *statefulsets* of a cluster in a certain namespace, on the following image is displayed information such as:


.. image:: /figuras/fig_mangue/048_mangue_statefulsets.png
    :alt: Listing of Statefulsets
    :align: center
=====

* **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|. When the user choses a line or several, the Mangue.io platform presents the icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. In this case the “Trash bin” icon |icone_lixo_vermelho| is presented, which allows to remove all the items indicated by the user with a single command;

* **Name**: It is the representation of the *Statefulsets* name;
  
* **Labels**: These are *Statefulsets* identifiers, they are used to link to a service;
  
* **Instances**: The values presented here indicate that the number of replicas of a *Statefulsets*. They are divided by a slash (“/”) where the values found on the left side of the slash are the values of active and operational replicas, and the values on the right side of the slash represent the maximum number of replicas that can be activated to maintain the desired *Statefulsets* performance. 
  
* **Status**: The status of a *Statefulsets* identifies the current state of each *Statefulsets* listed. They can be presented by **Running**, **Pending** or **“!”** (exclamation mark):
  
      * The status **Running** identifies that no errors are happening with the Statefulsets;
  
      * The status **Pending** identifies some transition states on the *Statefulsets*. Whether it is by update, container process initialization or any other activity that identifies a transition state;
  
      * The status **“!”** (exclamation mark) identifies an alarm, in other words, that something wrong happened with the *Statefulsets* and its replicas. For example: the image of a container is passed with an inexistent version, thus, its download does not occur;
  
* **IP**: In case the *Statefulsets* has an associated service, it is in this blank is where the load balancer IP if it is a service of the *loadbalancer* type, port for access to the service can be an external service (nodePort type) or the string “intern IP” if it is a internal cluster service (ClusterIP type);

* **Image and Version**: In case there is more than one image or version of a container, they are listed one below the other, as in the example of the sixth *Statefulsets* listed in the picture of the *Statefulsets* table;
  
* **Duration**: This column represents the time elapsed since the *Statefulsets* creation moment;
  
* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked displays two options as shown in the following picture:


.. image:: /figuras/fig_mangue/048.1_mangue_acoes_statefulsets.png
    :alt: Actions edit and delete statefulsets
    :scale: 80 %
    :align: center
=====

* **Edit Statefulsets**: This option presents a screen with a JSON file with all the *Statefulsets* configurations in Kubernetes, the user can edit whatever is necessary and select the edit option and wait for the action feedback from the Mangue.io Platform. This functionality attends the users that have knowledge about the Kubernetes files format. 

.. image:: /figuras/fig_mangue/049_mangue_editar_statefulsets.png
    :alt: Edit 
    :scale: 80 %
    :align: center
=====


* **Delete Statefulsets**: In the *Statefulsets* actions menu there is the option to delete, the user just needs to click on the button to confirm the action, as shown in the screen below:


.. image:: /figuras/fig_mangue/050_mangue_deletar_statefulsets.png
    :alt: confirmation message 
    :scale: 80 %
    :align: center
=====



Updates
--------

An Update is considered as an update event in a Kubernetes Cluster, its functionality has the purpose of facilitating the control and direct communication between the Kubernetes environment and Mangue.io interface. 


.. image:: /figuras/fig_mangue/051_mangue_update.png
    :alt: Update
    :align: center
=====

The image above displays the list of created updates, next the definition of each one of the eight columns:

* **#**: Event sequential number in the presented list;
  
* **Deployment Name**: Indicates the Deployment name;
  
* **Type**: Determines the type of update to be performed, there are two possible updates, they are:
  
      * **Update**- Occurs when the user determines which is the next version and the Deployment container;
  
      * **Rollback** - It is an operation that reverts the event for the previous version.
  
* **Status**: There are two possible status for an update, they are:
  
      * **UPDATED** -  This state corresponds to a performed update;
  
      * **OUTDATED** - Refers to a previous or old status, that waits for the update event through the Mangue.io platform;

* **Namespace**: Corresponds to the application Namespace to be updated and is being executed;
  
* **New Images**: Regards new images and versions of containers that are updated;
  
* **Duration**: Corresponds to the time the update was registered/executed;
  
* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked displays a single option:


.. image:: /figuras/fig_mangue/052_mangue_botao_atualizar.png
    :alt: action update 
    :scale: 80 %
    :align: center
=====

* **Update**: When selecting the option to update on the ``Actions`` button of the table, the Mangue.io platform presents a screen of confirmation for the operation:


.. image:: /figuras/fig_mangue/053_mangue_mensagem_atualizar.png
    :alt: message update 
    :scale: 80 %
    :align: center
=====

By clicking on the ``Update`` button the update event for the corresponding Deployment is released. 

The images and versions of containers contained on the “New Images” blank are used. An alert feedback is created on the superior right corner of the screen informing the “Success” or “Error”. 

Right above the table, there are three elements with which the user can act:


.. image:: /figuras/fig_mangue/053.1_mangue_pesquisar_atualização.png
    :alt: Search update
    :align: center
=====


* **The search action**: In case the list presented on this screen is too long (occupying more than one page), there is a blank where it is possible for the user to make a search with the desired Update name. It is just necessary to inform part of the name and type enter or click on the "Magnifying glass" icon |icone_lupa_verde|. As a result of this search only comes up the Updates that contains the key-word of the search;

* **The update action**: Just click on the icon |icone_update| for the Mangue.io to update the interface with the most recent values of the Updates table;

* **Create Integration with Updates**: Just click on the plus sign |icone_adicionar| for the user to register a new update for a Deployment in a certain Namespace. The Mangue.io platform presents the following screen for the user: 


.. image:: /figuras/fig_mangue/054_mangue_criar_integracao.png
    :alt: Create integration
    :align: center
=====

Next, follows the description of the blanks of this screen:

* **Token:** This blank is filled with a string of characters after the user clicks on the ``Generate Token`` button, the blank is filled with the token string that is informed for the communication with the Mangue.io API. This token must be saved and informed to authenticate the C.I. versions. When generating a token, it must be sent via API for the Mangue.io server, because it is responsible for guaranteeing the integrity of the requisition sent. 

* **Namespace:**When clicking on this blank, it is presented a list (dropdown) with all the existing Namespaces in the cluster selected on the “Configuration Selection” tab.

* **Deployment:** When clicking on the blank is presented a list (drop-down) with all the Deployment associated with the namespace selected on the previous blank. 

* **Create:** When the user configures all the blanks on this screen, with the correct criteria to add an update event (update), they must click over the ``Create`` button to add the update event on the Mangue.io platform. This new event is added to the list with the pending status. By clicking on the ``Create`` button a permission is generated for the user to register the updates on the platform through calls to the Mangue API. An alert feedback is created on the superior right corner of the screen informing of the “Success” or “Error”. 

.. note:: In case the event does not appear listed, immediately, the user must click on the  “” (update) icon to update the information on the screen. 


Below there are two examples of the benefits for the Updates functionality:

        **Example 1:**

        A user has a CI/CD pipeline that is executed and generates some stable versions per day. As the user has their cluster Kubernetes managed by the Mangue.io and its applications installed it is possible to register the updates on the platform through the CI/CD pipeline, and wait for the update event to be launched through the Mangue.io interface.

        **Example 2:**

        A user has a CI/CD pipeline that is executed and generates some stable versions per day. As the user has their cluster Kubernetes managed by Mangue.io and its applications installed it is possible to update the application directly through the CI/CD pipeline.


====

Catalog
=======

The Mangue.io platform allows the user to create applications (Deployments) in two different ways: the simplified way that guides the user through the sequence of screens and the elaborated one that allows uploading a text file. Next, the description of the two formats of how to create applications (deployments).

The first is simplified, it occurs when guiding the user using those screens as intermediate, that after all the filling and confirmation by the user, the informed data are converted in a file with ‘YAML syntax’, and this construction (practically with no errors) is used to generate the application.

The objective of this first approach is to minimize the potential YAML syntax errors to a Kubernetes environment. The creation of code in YAML syntax, in the Kubernetes environment, demands a high degree of specialization and knowledge of the developer. The syntax, correct for the environment must have all the needed dependencies to generate the desired result in the correct form and ready for use in the Kubernetes environment (e.g.: an application/ Deployment).

The other form is to allow the user to upload a text file, whose content is the application codification in YAML syntax, already adapted and prepared for a Kubernetes environment. If the developer (user) has enough practice to create their own scripts in YAML syntax, they may use them and bring this to the Mangue.io platform with the purpose to conduct in which Cluster, Pod, Node, this code/script is executed and managed. 

When the user accesses the Catalog menu, the Mangue.io platform presents the screen below, on the sequence the description of each one of the options from this menu flow.


.. image:: /figuras/fig_mangue/055_mangue_catalogo.png
    :alt: Catalog
    :align: center
=====



New application
----------------

This modality is the form the Mangue.io platform conducts the user through the screens, requesting the information in sequence so that, posteriorly, the Mangue.io platform makes the compilation of information generating the application within the Cluster and Namespace selected in the gear tab |icone_engrenagem| “Configuration Selection”.

Below are described the steps to fill the forms from the screens that guide the user.

A. **First Step: New application**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

For the creation of a new application (Deployment) the Mangue.io platform segments the process in two steps, the user must fill the following blanks:

.. image:: /figuras/fig_mangue/056_mangue_criar_deployment.png
    :alt: create deployment
    :align: center
----

* **Name**: This space is mandatory, the user must inform the application (Deployment) name with which this stays identified on Mangue.io platform;
* **Replicas**: This blank is mandatory, the user must inform the number (full)that they desire to allocate to execute the application (Deployment) as soon as created. This number is allocated in the computing infrastructure so that the user obtains a better performance experience, and the Mangue.io platform takes care of allocating these computing resources; 
* **Search Image**: This area is mandatory, an image search of an application is performed in the server of image register http://hub.docker.com. The user can inform a sequence of characters (even if partial) of any image cataloged on Hub Docker, and the Mangue.io platform does a search and presents a list that contains the characters sequence. See the example below, with the sequence search “wordp”, to search the application **Wordpress** image:

.. image:: /figuras/fig_mangue/057_mangue_pesquisar_imagem.png
    :alt: search image
    :align: center
----

The user just needs to click with the mouse cursor on the line of the desired image to select the best image available.

* **Container name**: This blank is mandatory, in it the name with which the user intends to identify it within the Mangue.io platform must be informed;
* **Block execution of privileged user**: On this space the user can block all the Deployment containers for it to be executed in a privileged way, with access to resources and Kernel capacities of the Host machine;
* **Specify user, group or system file ID**: On this area it is possible to indicate the user, group or system file ID the container is executed;
* **Application Tags**:On this blank the user can inform the application Tags, as well as create a Tag to be associated to the application;
* ``Add`` **button**: To create a new application (Deployment) the Mangue.io platform segments the process in two steps. After the user confirms the action with the ``Add`` button the user views the following screen:

.. image:: /figuras/fig_mangue/058_mangue_modal_imagem.png
    :alt: configure image
    :align: center
----

* **Image version**: This blank is mandatory on it the user must inform how the application (Deployment) is identified on the environment. This blank can be filled with numbers or characters, to attend to the user demand (e.g.: latest, last, 1.xx, 1.20);

* **ContainerPort**: This area is mandatory on it the user must inform which TCP-IP container port can be used for the application (Deployment) to be available to others users access;
  
      * **Maximum Resource to be used [CPU in millicores]**: On this space the user can inform the maximum of CPU resources that must be allocated, on the computing infrastructure of the Cluster to offer the maximum performance for this application (Deployment). This quantity must be informed with a full number, to support and execute the application (Deployment);
  
      * **Minimum Resource to be used [CPU in millicores]**: On this blank the user can inform the minimum of CPU resources that must be allocated, on the computing infrastructure of the Cluster to offer the minimum acceptable performance for this application (Deployment). This quantity must be informed with a full number, to support and execute the application (Deployment);
  
      * **Maximum Resource to be used [Memory in millicores]**: On this area the user can inform the maximum of RAM memory resources that must be allocated, on the computing infrastructure of the Cluster to offer the maximum performance to this application (Deployment). This quantity must be informed with a full number to support and execute the Deployment;
  
      * **Minimum Resource to be used [Memory in millicores]**: On this blank the user must inform the minimum of RAM memory resources that can be allocated, on the computing infrastructure of the Cluster to offer the minimum acceptable performance for this application (Deployment). This quantity must be informed with a full number, to support and execute the new application (Deployment);
  
* **Allow privileged execution**: On this blank the user must inform if the container has access to the resources and Kernel capacities of the Host machine;
  
* **Specify user, group or file system ID**: On this area it is possible to indicate the user, group or file system ID that the container is executed;
  
* **Registry Secret**: On this blank the user must inform the Secret name of the images server associated with this image. By clicking with the mouse over this blank, the Mangue.io platform presents a list file of Secrets available on the private image server; 
  
* ``Next`` **button**: When the user clicks on the ``Next`` button the Mangue.io platform presents the screen with the blanks respectives of Secrets and Environment Variables of the container. See the screen below:

.. image:: /figuras/fig_mangue/059_mangue_secrets_e_variaveis.png
    :alt: secrets and Variables
    :align: center
----

* Environment Variables:

      * Environment variable name;
      * Environment variable content;
      * ``Add`` button
* Secrets
      * Secret name;
      * Environment Variable;
      * Secret Key;
      * Secret Value;
      * ``Add`` button;
      * ``Create Secret`` button;
      * ``Back`` button
      * ``Finish`` button.

After clicking on the ``Finish`` button, the Mangue.io platform closes the sub screens and returns to the first step of the new application process, it presents the its configuration listed, as the example below:

.. image:: /figuras/fig_mangue/061_mangue_lista_aplicacao.png
    :alt: application list
    :align: center
----

Below  the content description of the columns presented on this list:

* **#**: Shows the container sequential number on the present list;

* **Container**: Displays the container name informed on the previous steps, the start of a new application creation process (Deployment);

* **Image**: Presents the image name of the application that was selected from the images register server (e.g.: http://hub.docker.com);
  
* **Version**: Displays the information of the application version (Deployment) informed on the previous steps;

* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked, it presents a submenu with the following options:

.. image:: /figuras/fig_mangue/062_mangue_acoes_submenu.png
    :alt: actions submenu
    :align: center
----

      * **Add PersistentVolumeClaim**: Through this screen the user may configure the file characteristics regarding the *PersistentVolumeClaim* (PVC). The Mangue.io platform simplifies the PVC configuration process, offering to the user options on the graphic interface that conduct the decisions regarding the PVC, as below:
  
.. image:: /figuras/fig_mangue/063_mangue_add_pvc.png
    :alt: add PVC
    :align: Center
----

          * **Size / 1Gi, 5Gi, 10Gi**: The user can select the volume size simply by clicking with the mouse cursor over the desired number, selecting the best size option for this PVC. The options are expressed in Gigabytes (1, 5, or 10);
          * **Size / Customized**: Another way of creating a PVC with a volume with a differing size from the previous options, the Mangue.io platform presents a slide bar that allows the user to select the PVC's desired size. Using the mouse cursor over the orange indicator, the user can move this indicator (left or right) to define the final desired size. The minimum size is 1 Gigabyte and the maximum of 100 Gigabytes;
          * **Storage Class**: This blank is a dropdown list that is composed only of NFS servers configured on the Mangue.io platform. The user must select the more adequate NFS server to receive the PVC file;
          * **Access Mode**: This column presents the access configuration to this volume, these access modes can be three, they are: *ReadWriteOnce*, *ReadOnlyMany*, *ReadWriteMany*;
          * **Mount Path**: On this space the user must inform the path where the volume is mounted on the container. If the application base is on a Linux environment, the montage volume path must use the notation of the Linux operating system;
          * **Volume name**: On this area the user must inform the name of the volume file that is created on the Cluster operating system.

      * **Add ConfigMap**: A *ConfigMap* is an API object used to store non-confidential data in key-value pairs. On this sub screen the user can include and configure the desired *ConfigMap(s)*  file(s) for their environment.
  
.. image:: /figuras/fig_mangue/064_mangue_add_configmap.png
    :alt: add ConfigMap
    :align: center
----

          * **ConfigMap Name**: This blank is mandatory, the user must inform the desired name to register in the Mangue.io platform and identify this *ConfigMap*;
          * ``Add`` **button**;
          * **Mount Path**: This space is mandatory the user must inform the path where the volume is mounted on the container. If the application base is in a Linux environment, the mount path of the volume must use the environment notation of the Linux operating system;
          * **File Name**: This area is mandatory the user must inform the file name that is created on the virtual machine operational system that uses the *ConfigMap*;
          * **File content**: This blank is mandatory and the user must fill in with the specific content of the *ConfigMap*;
          * ``Add ConfigMap`` **button**: After filling in all the previous blanks the user must press this button with the mouse cursor so the Mangue.io platform can promote the creation, configuration and recording of the *ConfigMap* for this new application (Deployment).
     * **Edit Container**: When selected this option the Mangue.io platform presents the screen regarding the **Fist Step: New Application**, so the user can edit the configurations on this container.
     * **Exclude Container**: This action is defined and when actioned the Mangue.io platform removes allo the container initial configuration, **no confirmation of this action is required.**
  
----

B. **Validate New Application**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

If the user clicks with the mouse over the container name the Mangue.io platform presents a screen with all the information about Container resources.

The Mangue.io platform identifies all the resources of *PersistentVolumeClaim*, *ConfigMap*, of the container the user configured for this application and list these resources according to the example of the screen below:

.. image:: /figuras/fig_mangue/065_mangue_recurso_container.png
    :alt: container resources
    :align: center
----


* **#**: This column presents the container sequential number in the presented list;
* **Name**: This column shows the name of the resource informed on previous steps;
* **Type**: This column displays the type of resource created on previous steps;.
* **Mount Path**: This column presents the information of the operational system directory according how it was configured on previous steps;
* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked, it presents a submenu with the following options:

.. image:: /figuras/fig_mangue/066_mangue_acoes_recursos.png
    :alt: actions resources
    :align: center
----

      * Attach to another container: A Mangue.io platform facility allows the user to attach this application to a different container than the one created since the beginning of this process. When loading this option the Mangue.io platform presents the following screen:

.. image:: /figuras/fig_mangue/067_mangue_criar_pcv.png
    :alt: create PVC
    :align: Center
----

When clicking over the containers blank a drop-down list is presented with the containers available and configured on the Mangue.io platform. The user just needs to select the desired container and confirm the action.

      * **Delete**: This action is definitive and by actioning it the Mangue.io platform removes all the container initial configuration;

.. attention:: There is no request confirmation on the "Delete" action.

----

C. **Second Step: Deploy on the Clusters**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This section enables the understanding of how to operate one of the greatest facilities of this platform. It allows the creation, launch and execution of this new application (Deployment) in more than one Cluster, simultaneously. 

The platform makes it possible to operationalize the selection of one (or more) Cluster (s) currently configured on the Mangue.io environment. The image and the description of this section is below:

.. image:: /figuras/fig_mangue/068_mangue_deploy_clusters.png
    :alt: deploy on the clusters
    :align: center
----

* **Clusters Available**: This blank when selected presents the drop-down list with all the configured Clusters on the platform. The user just needs to select which ones they want to launch and execute the application Deployment that is being created.
* ``Next`` **Button**: The user must click on this button to start the third and last step to create a new application (Deployment).

----

D. **Third Step: Enable Zero Down-time**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

As mentioned at the start of this topic, the objective of this first approach - Creation of New Application via screens/forms on Mangue.io - is to minimize the potential YAML syntax errors for a Kubernetes environment. 

The creation of a code in YAML syntax in the Kubernetes environment demands a high degree of specialization and knowledge from the developer. Thus the syntax correct for the environment, may have all the dependencies needed to generate the desired result and be integrated in the Kubernetes environment use (e.g.: an application/ Deployment).

The development of an application (Deployment) script with the YAML syntax in a Kubernetes environment can be very long, and the dependencies between script sections and with external elements (PVCs; *ConfigMaps*, environment variables, among others) can induce the script creation with errors or parameters absence failures, decorring of the little experience or attempt of using a script developed by another person.

For example:

A generic script found on the virtual environment may not make clear all the dependencies of environment variables and external files.

The scripts adaptation process (very little documented in the year of 2018) could be a great frustration and prevent the popularization of the Kubernetes environment, therefore the Mangue.io platform simplifies this process by guiding the user through screens and forms.

After the complete fill in (of this second part) of all the blanks of screens and forms regarding the application (Deployment) creation the Mangue.io platform generates the complete YAML script and, by consequence, its compilation with no errors. 

This document's reader can see below the description of the next screens that are part of the last step before the finalization and creation of the application (Deployment) that is executed and managed by the Mangue.io platform. 

.. image:: /figuras/fig_mangue/069_mangue_habilitar_downtime.png
    :alt: enable down time
    :align: center
----

* **MaxSurge**: On this space the user must inform the maximum quantity of replicas they wish to keep active on the Mangue.io platform. During the update process of the application (Deployment) version, this number is responsible for keeping a minimum of replicas to guarantee the user experience during an update process;
* **MaxUnavailable**: On this blank the user must inform the maximum quantity of replicas they wish to keep unavailable on the Mangue.io platform. During an update process of the application (Deployment) version, this number indicates to the Mangue.io the quantity of replicas that can be updated in a parallel mode;
* **Container**: This is a header of a section that indicates the container name that is being created for this new application (Deployment).
* **Section ReadinessProbe**: The Kubernetes environment uses *ReadinessProbe* to know when a container is ready to start to accept traffic. A Pod is considered ready when all its containers are concluded. On the blanks below the user must insert the values referring to the environment of *ReadinessProbe*.

      * **SuccessThreshold**: On this blank the user must inform a full number that defines the minimal quantity of containers that the Mangue.io platform must keep available during the process of update in a way to guarantee the user experience that is using the application (Deployment);
  
      * **FailureThreshold**: In this area the user must register a full number that defines the maximum quantity of containers that are unavailable during an update process of the application (Deployment) version. This number indicates to the Mangue.io platform the quantity of replicas that may be updates in a parallel manner;
  
      * **ReadinessPath**: On this space the user must indicate the path of the directory where is created a file register (log) that stores all the events during the process of container update;
  
      * **Request Headers**: On this subsection the user may configure the update events register file content layout that must be created, adding columns (headers) and the column content;
  
      * **Header name**: On this blank the user must inform the column name that is created within the update events register file (log).
  
      * **Header Value**: This space the user must indicate the initial value of the column that is created within the update events register file (log).
  
      * ``Add`` **button**: This button informs the Mangue.io Platform the set header/value must be configured in the update events register file (log). The user may add the quantity of columns that is made necessary, they just need to fill in the values on the previous blanks and press the ``Add`` button.
  
* **LivenessProbe**: The Kubernetes environment uses *LivenessProbe* to know when to restart a container. These probes are performed in intervals of time (seconds) defined by the user and after this period it is added a line on the log file. On the spaces below the user enters with the values referring to the *LivenessProbe* environment:
  
      * **PeriodSeconds**: On this blank the user must inform the full number that represents the period of seconds referring to the probe activity break (*livenessprobe*);
  
      * **ReadinessPath**: In this area the user must indicate the path to the directory where a register file (log) is created that stores all the events during the container update process.;
  
      * **Request Headers**: On this subsection the user may configure the update events register file content layout to be created, adding the columns (headers) and the column content;
  
      * **Header name**: On this blank the user must inform the column name that is created within the update events register file (log).
  
      * **Header Value**: This space the user must indicate the initial value of the column that is created within the update events register file (log).
  
      * ``Add`` **button**: This button informs the Mangue.io platform the set header/value must be configured in the update events register file (log). The user may add the quantity of columns that is made necessary, they just need to fill in the values on the previous blanks and press the ``Add`` button.
  
      * ``Back`` **button**: If the user needs to go back to a previous step, they must press this button. It is important to highlight that in this operation all the information filled on this screen by the user is lost, and the Mangue.io platform returns to the previous screen. 
  
      * ``Finish`` **button**: The user must press this button when the filling of all the blanks from the previous screens are concluded, when it's ready to start the application (Deployment). The Mangue.io platform compiles all the information on the blanks and generates a YAML script. By compiling this script and generating the application (and all its dependencies: PVCs, *ConfigMaps*, log files, among others) it is executed and managed within the Mangue.io platform environment.

At this point the Mangue.io platform ends the application (Deployment) screens creation and the user can find their new application installed on the **Workloads/Deployments** menu screen.

The user may have a larger quantity of information about its new application on the "Deployment Information" menu.

-----

Deploy via YAML
-----------------

This is the second approach the Mangue.io platform allows the user to upload a text file, whose content is the application codification in YAML syntax, already adapted and prepared for a Kubernetes environment.

The YAML stands for “Ain't a markup language”, according to https://yaml.org/, is an amicable data serialization default to any programming language. YAML was created in the belief that all data can be represented adequately as a combination of lists, hashes (maps) and scalar data (simple values).

The syntax is relatively simple and was projected considering that it is very readable, but that also was easily mapped for the common types of data in most high-level languages. Beyond that, YAML uses a notation based on indentation and a set of distinct characters of the ones used by XML, making that both languages are easily composed in one another. 

Any user with a YAML syntax knowledge can use the Mangue.io interface to create a: Deployment, Service, *Statefulsets*, Volume or Ingress.

The Mangue.io platform allows the user expert in YAML enters with their code in a free manner directly through the interface (data-entry), or upload a file in text format not formatted (ASCII) of a directory/folder of their computer to the Mangue.io platform.

When clicking over the Deploy via YAML Code option the Mangue.io platform presents the following screen:

.. image:: /figuras/fig_mangue/070_mangue_deploy_clusters.png
    :alt: deploy clusters
    :align: center
----

A. **Available Clusters**
~~~~~~~~~~~~~~~~~~~~~~~~

The user must click over the “Available Clusters” blank to open a drop-down list of all the configured clusters on the Mangue.io platform, then select the recipient Cluster in which the Deployment is created and executed.

There is a mensage present on the screen that is important to highlight for the Deployment via YAML creation process.

.. note:: In case no Cluster is selected, the deploy is made only on the Cluster being used currently.

----

B. **Template**
~~~~~~~~~~~~~~~~

On the sequence the user must select one of the YAML code model options (template) that is previously configured on the Mangue.io platform, this functionality adds productivity to the user, and each model type is an option on the drop-down list:

* **Default**: Allows the user to configure the YAML code in a free way. In this option the user must have a good YAML syntax knowledge to enter with the desired code. The user must start clicking with the mouse on the gray area beside the number “1”, before starting to type their YAML code. 

.. attention:: For each new line the user must use the ``Enter`` key to start a new line. 

The user must use their own development experience to structure the syntax of their code line by line. Through this option the user may enter with a YAML code to create, provision a new Pod on the Mangue.io platform.

* **Deployment**: In this option the Mangue.io platform presents a new YAML code template with the initial syntax to create a Deployment. The user may use the mouse to click on the  desired line and on the location, then start the typing of the specific parameter for the Deployment. Therefore, editing the YAML code template the platform presents.
* **Service**: On this option the Mangue.io platform presents a YAML code template with the initial syntax to create a Service. The user may use the mouse to click on the desired line and on the location, then start the typing of the specific parameters for the service. Therefore, editing the YAML code template the platform presents.
* **Statefulsets**: On this option the Mangue.io platform presents a YAML code template with the initial syntax to create a Statefulsets. The user may use the mouse to click on the desired line and on the location, then it is possible to start the typing of the specific parameters for the *Statefulsets*. Therefore, editing the YAML code template the platform presents;
* **Volume**: On this option the Mangue.io platform presents a YAML code template with the initial syntax to create a Volume. The user may use the mouse to click on the desired line and on the location, then start the typing of the specific parameters for the Volume. Therefore, editing the YAML code template the platform presents.
* **Ingress**: On this option the Mangue.io platform presents a YAML code template with the initial syntax to create a definition of Ingress. The user may use the mouse to click on the desired line and on the location, then start the typing of the specific parameters. Therefore, editing the YAML code template the platform presents.

The expert user in YAML may see that the use of templates increases productivity and keeps the code better documented and structured according to the best practices.

----

C. **Browse**
~~~~~~~~~~~~~~

This button allows the user to upload a text non formatted (ASCII) file type, with a YAML code previously created by the user. The user must click on the ``Browse`` button, in this action the Mangue.io platform to presents the "File Explorer" screen of your computer, then, it is necessary to select the folder/directory where the code file is located.

The Mangue.io platform is configured to identify and present all the files with extensions “.yaml and .yml” present on the folder/directory selected. In case the user has saved on their source code in a file with different extension, they must type the full name of the file on the blank “Name” or select the option “All files (*.*)” to locate and select the desired file.

.. image:: /figuras/fig_mangue/071_mangue_arquivo_yaml.png
    :alt: file Explorer
    :align: center
----

When the user selects the desired file, just click on the ``Open`` button, so the Mangue.io platform uploads the content from the selected file to the interface, at this moment the user visualizes that the Mangue.io platform numbers, sequentially, all the lines of the uploaded code.

At this point the user can edit the code directly through the Mangue.io platform interface, to personalize or correct any YAML code line present on the screen.

----

D. **Submit**
~~~~~~~~~~~~~~

When the user is concludes the insertion of all the YAML code content and is secure that this code is correct, the green button ``Submit`` must be clicked for the Mangue.io platform to perform the code load and its consequent compilation by make this code available as Deployment, Service, *Statefulsets*, Volume or Ingress.

At this point the Mangue.io platform closes the application (Deployment) creation screens, then the user can find their new application listed on the "Workloads/Deployments" screen.

The user can view a larger quantity of information about its new application on the "Deployment Information" menu.

----

E. **Server VS Code**
~~~~~~~~~~~~~~~~~~~~

.. image:: /figuras/fig_mangue/072_mangue_add_vscode.png
    :alt: add server vs code
    :align: center
----

To create a Visual Studio Code is necessary to click on the |icone_adicionar| button and fill in the blanks below:

* **Server VS Code name**: Server VS Code name to be created;
* **Server VS Code size**: Disk size to be made available for the Visual Studio Code. The size measure is defined on the “Type of Size” blank;
* **Type of Service**: The user may select the type of service to be attributed to the Visual Studio Code deployment. The available options are: Cluster IP, *NodePort*, Load Balancer and Ingress;
* **Port**: The user can select the port to be used in the service;
* **Type of Size**: Specifies the size unit. The available options are: Gi e Mi;
* **Ingress Class**: In case the type of service selected is Ingress it is necessary to select the Ingress CLass to be used for the service;
* **Server VS Code URL**: In case the type of service selected is Ingress it is necessary to specify its route path. Example: */vscode*;
* **Activate authentication**: The user can attribute a password that is necessary to access the server VS Code;
* **Servier VS Code password**: Password to be used to access the server VS Code.

----

ConfigMap
=========

In a simple way, it is possible to affirm the *ConfigMap* is a set of key-value pairs destined to the configuration storage, that is kept within files that can be consumed through pods. It is very similar to Secrets, but provides a work mode with strings that do not possess confidential data, like: passwords, keys, tokens and other sensitive data.

The *configMap* files, can be both complex files that have few rules, as well as files on JSON format complexes and full of rules.

It is important to highlight that a *configMap* file can contain the complex content of a JSON, the user just needs to fill the content of this file obeying the correct syntax of a JSON.

When selecting this option on the bar slide, the Mangue.io platform presents the following screen which contains a listing of all the *configMaps* registered on the platform.

.. image:: /figuras/fig_mangue/073_mangue_configmaps.png
    :alt: configMaps
    :align: center
----

Below the description of each column of this table:

* **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|. 

When the user choses a line or several, the Mangue.io platform presents the icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. 

In this case the "Trash bin" icon |icone_lixo_vermelho| is presented, which allows to remove all the items indicated by the user with a single command;

* **Name**: On this column is presented the *configMap* name added by the user. When clicking with the mouse over the name, the Mangue.io platform presents a screen with the content(s) of the *configMap* file(s). 

By default is presented only the visualization of a line from the file content, in case the content is bigger than the blank, the user can position the mouse on the inferior right corner, until the mouse cursor changes for a double diagonal arrow |icone_seta_diagonal|. Therefore, allowing the user to redimension the listed content space, and accommodate the size that is adequate for the user, for its better viewing.

.. image:: /figuras/fig_mangue/074_mangue_configmaps_arquivo.png
    :alt: configmaps file
    :align: center
----

It is important to highlight that this window does not allow the edition of the listed content.

* **Duration**: On this column is presented the time (in days) since the *configMap* creation moment.
* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked, it presents two options, as the following figure:

.. image:: /figuras/fig_mangue/075_mangue_acoes_configmap.png
    :alt: actions configmaps
    :align: center
----

      * **Delete configMap**: When the user selects this option the Mangue.io platform presents the screen below requesting the confirmation of the *configMap* removal option.

.. image:: /figuras/fig_mangue/076_mangue_deletar_configmap.png
    :alt: delete Configmap
    :align: center
----


.. note:: It is important to highlight that this action is definitive and removes the file from the operating system, not being able to restore it, thus all the references of this **configMap** on the Mangue.io platform are erased. Therefore, it is necessary to recreate the file from the beginning.


      * **Edit Configmap**: When selecting this option the Mangue.io platform presents the following screen, place where the user can perform the necessary alterations on the *configMap* file(s) content(s).

.. image:: /figuras/fig_mangue/077_mangue_add_configmap.png
    :alt: add configmap
    :align: center
----

The following image is a cutout of the elements positioned above the table, there are three different and available actions to the user:

.. image:: /figuras/fig_mangue/078_mangue_pesquisar_atualizacao.png
    :alt: search update
    :align: center
----

* **Search action**: In case the present list on this screen is too long (occupying more than one page), there is a blank where it is possible for the user to perform a search by the *ConfigMaps* desired name. The user just needs to inform part of the name and click ``Enter`` or click over the "Magnifying glass" icon |icone_lupa_verde|. As result of this search only the *ConfigMaps* that contain the key-word will come up on the search.
* **Update action**: Just click on the  |icone_update| icon for the Mangue.io to update the interface with the most recent values from this *ConfigMaps* table.
* **Action of adding a ConfigMap**: Just click on the plus sign |icone_adicionar| so the user can register a new *ConfigMaps*. The Mangue.io platform presents the following screen to the user:

.. image:: /figuras/fig_mangue/079_mangue_add_configmap.png
    :alt: add configmap
    :align: center
----

Below the description of the blanks on the screen above:

* **configMap name**: On this blank the user must type the desired *configMap* name, then click over the plus sign icon |icone_adicionar|, which results in the Mangue.io platform adding the blanks below:
  
      * **“n” File**: For each time the user clicks on the plus sign |icone_adicionar| the Mangue.io platform adds a gray line with the *configMap* file sequential number. In case the user needs to remove (erase) the file configured on the "Trash bin" icon |icone_lixo_vermelho| just opt for removing the **“n”** file from the *configMap*.
      * **File name**: On this space the user must inform the file name that is created on the recipient operational system that supports the deployment execution. It is important to remember that this name, and its respective extension, must follow the rules of file naming of the recipient operational system, therefore must contain only ASCII default characters. 


.. attention:: There must not be used the letters with accents (á, é, í, ã, õ, ç, among others), there may be an error on the file creation on the operational system.


      * **File content**: On this blank the user must type the named file content, on the previous blank. This content that must be informed according to the technical necessity and the objective of this *configMap*.
  
By default is presented only the visualization of some lines on the file content, in case the content is bigger than the blank, the user can position the mouse on the inferior right corner, until the mouse cursor changes to a double diagonal arrow |icone_seta_diagonal|. Therefore, allowing the user to redimension the space of the listed content and, accommodate the size that is adequate to the user, for better viewing this blank.

      * ``Add configMap`` **button**: After the user informs the necessary *configMap* file(s), the user must click with the mouse over the button ``Add configMap``, for the Mangue.io platform to perform the creation of the referred file(s) on the recipient operating system environment. After this action over this button the platform closes this window and returns to the screen where the *configMap* list is presentes.

====

Cluster Events
===============

Through this menu option, the Mangue.io platform presents all the events that occurred on the cluster and namespace selected on the gear tab |icone_engrenagem| "Configuration Selection". For each selection of contract/cluster/namespace the events list is automatically updated. 

.. image:: /figuras/fig_mangue/080_mangue_cluster_events.png
    :alt: cluster events
    :align: center
----

Below the content description of each column presented on the list:

* **#**: Event's sequential number on the presented list;
* **Name**: Event name the Mangue.io platforms generated for the deployment;
* **Type of event**: 

    Describes the type of event occurred, and can be listed the following types of events:

      * Normal;

      * Warning.
  
* **Type of object**: Describes which configured object on the Mangue.io platform originated the listed event. The identification of the type of object, allows the user to identify this origin so it can have access to the object and act on the event resolution. It can be through the object redefinition, or opt for its removal. The types of object can be some of the listed below:
  
      * Deployments;

      * *Daemonsets*;
  
      * Horizontal Autoscaler;
  
      * Pods;

      * *Statefulsets*;
  
      * Updates;
  
      * Services;
  
      * Ingress;
  
      * *StorageClass*;
  
      * *PersistentVolumes*;

      * *PersistentVolumesClaim*.
  
* **Object name**: Name of the event resource.
* **Mensage**: 

      * Pulled;

      * Created;

      * Started;
  
      * *NoPods*;
  
      * *FailedGetScale*;

      * *ProvisioningFailed*;
  
      * *FailedBinding*.
  
* **Executed in**: Informs how long ago the event happened.

The following image is a cutout of the elements positioned above the table, there are three actions different and available to the user:

.. image:: /figuras/fig_mangue/081_mangue_pesquisar_evento.png
    :alt: search event
    :align: center
----

* **Search action**: In case the list presented on this screen is too long (occupying more than one page), there is a blank where it is possible for the user to make a search with the desired event name. 

They just need to inform part of the name and click ``Enter`` or click on the icon with the "Magnifying glass" |icone_lupa_verde|. 

As a result of this search only comes up the events that contains the searched key-word;

* **Update action**: Just click on the icon |icone_update| so the Mangue.io update the interface with the most recent values of the events table;

====

Cron Jobs, Jobs
===============

On this menu option, the user can observe two distinct functions of the Mangue.io platform, they are jobs and cron jobs. The user views the list of all jobs and cron jobs, the list presents what is programmed for the contract, cluster and namespace selected on the gears tab |icone_engrenagem| "Configuration Selection". For each contract/cluster/namespace selection the list is automatically updated.

----

A. **Cron Jobs**
~~~~~~~~~~~~~~~~

The Cron Jobs are useful to create periodic and recurring tasks (jobs), such as execute backups or send emails. The Cron Jobs can schedule individual tasks for a specific time,  as well as programming a job for when its cluster is probably idle. 

The Mangue.io platform lists all the cron jobs configured in its environment:

.. image:: /figuras/fig_mangue/082_mangue_cronjobs.png
    :alt: cron jobs
    :align: center
----

Below the content description for every column presented on the list:

* **#**: Cron job's sequential number on the presented list;
* **Name**: Cron job name the Mangue.io platform generates for the deployment;
* **Schedule**: Shows the schedule configuration (date and time) programmed for executing this cron job;
* **Duration**: Presents the cron job duration time;
* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked, displays the option to delete CronJob as shown in the following picture:

.. image:: /figuras/fig_mangue/083_mangue_deletar_cronjobs.png
    :alt: delete cron job
    :align: center
----

B. **Jobs**
~~~~~~~~~~~~

A job creates one or more pods and guarantees that one of their specific numbers is closed with triumph. As the pods are successfully concluded, the job tracks the well successful conclusions. When a specified number of well successful conclusions is reached, the task (that is, Job) is concluded. Excluding a job cleans all the created pods.

The user can also configure a job for it to be executed, in parallel, in various pods.

.. image:: /figuras/fig_mangue/084_mangue_jobs.png
    :alt: jobs
    :align: center
----

Below the content description of each column presented on the list:

* **Name**: Job name the Mangue.io platform generates for the deployment;
* **Status**: This column presents three possible values, “COMPLETED”, “IN PROGRESS” AND “FAILED”:

      * **COMPLETED**:  Job executed with success;
  
      * **IN PROGRESS**: Job being executed;

      * **FAILED**: Job failed on the execution.

* **Parallelism**: Number of pods for parallel execution;
* **Conclusions**: Well successful conclusions;.
* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked, it displays the option to delete the job, as shown in the figure:

.. image:: /figuras/fig_mangue/085_mangue_deletar_job.png
    :alt: delete job
    :align: center
----

Invoicing
=========

This Mangue.io platform option is a great ally to the companie's Financial Governance. Few tools available on the market currently present the computing infrastructure consumption in real values, to support a serverless environment based in containers (Kubernetes).

The term serverless may take a false notion that this environment does not generate computing infrastructure costs, but any software application always needs a computing resource (CPU, memory, disk, operating system - OS).

For this software to be executed each item loads its cost of use, storage licensing (OS and softwares) and must be calculated day to day, for it to meet the criteria and policies of the Cost Governance and Financial Governance.

The Mangue.io platform has a database that accumulated month-to-month infrastructure consumption values, since the moment of its installation. This database is calculated day-to-day and accumulated the consumption values, according to the formula calculation presented on the topic "Cluster Consumption Value Calculation".
By selecting this menu option the Mangue.io platform presents the following screen:

.. image:: /figuras/fig_mangue/086_mangue_faturamento_cluster.png
    :alt: cluster Invoicing
    :align: center
----

The Mangue.io platform presents the cluster and namespace values selected on the gears tab |icone_engrenagem| "Configuration Selection". For each selection of a new contract/cluster/namespace the values and graphs are automatically updated.

This screen is divided in two different sections, next is the detailing of each section.

----

Consolidated Report
--------------------

This screen presents information about the monthly consumption of clusters, the user can view the price of each cluster on the pie graph present on the image below. As well as it is possible to view the consumption per user, this only occurs when the deployment is created through the Mangue.io, once it is stored on the deployment the responsible user information for its creation.

.. image:: /figuras/fig_mangue/087_mangue_overview_financeiro.png
    :alt: invoicing overview
    :align: center
----

By selecting a cluster the information on the screen is reloaded according to the selected cluster, this includes both the graphs that inform the price per cluster and user, as well as the table with details about the application costs.

By default the consult is done considering all the cluster namespaces, but the user can filter by a specific namespace clicking on ``Select a namespace`` the information on the screen are reloaded as it is on the previous item, distinguishing for returning only the selected namespace values.

Still on this screen is possible to visualize a details list about the application costs, as can be seen on the image below:

.. image:: /figuras/fig_mangue/088_mangue_lista_aplicacoes.png
    :alt: application list
    :align: center
----

* **Name**: This column presents the deployment name, reminding that for the deployment to appear here it needs to be in a cluster with the “ticket” enabled;
* **User**: This column presents the user responsible for the application creation;.
* **Namespace**: This column presents the namespace which the application belongs;
* **CPU price**: This column presents the cost per application CPU corresponding to the selected month;
* **Memory price**: This column presents the cost per application Memory corresponding to the selected month;
* **Total price**: This column presents the sum of CPU and Memory price.

There is still the possibility to export the information corresponding to the table above, in csv format, through the functionality “export to csv” represented by the following button |icone_exportar|, that when clicking the user can download the file right after.

----

History
--------

The CPU resources and cluster memory consumption is presented in a graph format named as “Cluster Invoicing History”, as the following image:
 
.. image:: /figuras/fig_mangue/089_mangue_historico_faturamento.png
    :alt: invoicing History
    :align: center
----

A. **Monthly Cluster Invoicing History** 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This section presents a graph with the evolution of CPU and cluster Memory resource consumption value, to support and execute all the Workloads contents (Deployments, *Statefulsets*, Horizontal Autoscaler, Pods, *Statefulsets*). 

The user may select the period which they desire to visualize the values, just needing to select the month and year presented right above the graph:

.. image:: /figuras/fig_mangue/090_mangue_mes_ano.png
    :alt: month and year
    :align: center
----

By clicking on the calendar icon, the Mangue.io platform presents an annual selection screen, where the user may choose which year they wish to view:

.. image:: /figuras/fig_mangue/091_mangue_ano.png
    :alt: year
    :align: center
----

As soon as the calendar is clicked, it is possible to select the desired year on the Mangue.io platform, according to the image of the screen above. Next, the user may select the month they wish to visualize and its accumulated values:

.. image:: /figuras/fig_mangue/092_mangue_mes.png
    :alt: month
    :align: center
----

As soon as the user selects the month, the Mangue.io platform indicates the process of search and value calculation of month and year selected. This process may take a few seconds and the user may follow this process evolution, monitoring a “black line” that appears from the left to the right on the top of the internet browser area.

The minute the line fills in at the top of the browser area, the Mangue.io platform updates the graph of the screen with daily values of the month and year selected.

It is important to mention the daily values presented reflect until the current day, in other words, if the user desires to consult the month values, and current month is found (for example) on the first fortnight, the graph represents only from the first until the 15th day of the current month. 

This graph represents an evolution line of the computing infrastructure consumption value and can be comprehended as a mathematical progression. In other words, is the consumption value of the previous day added to the current day consumption and, then, successively. 

For each beginning of the month, the value is “zeroed” starting a new calculation cycle of the computing infrastructure for the month period, until the current day. This way, the value of the first day of the month can not be presented immediately, because the Mangue.io platform needs to compute the value of the day after 24 hours of the first day - the value of the current day is presented after 24 hours.

The graph line may present “peaks” and “valleys” due to several factors, therefore must be taken into consideration the environment in its totality. Consumption increase can be recurring with the launch of Horizontal Autoscalers, Migrations, Updates, Cron Jobs creation of new applications, deployment among others.

All the situations listed above are potential causes of computing infrastructure consumption increase and the evolution due to total values of this graph.

----

B. **Cluster Invoicing History**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This graph presents the month-to-month accumulated consumption of the last four (04) months of the period the user is found.

.. image:: /figuras/fig_mangue/093_mangue_historico_cluster.png
    :alt: cluster invoicing History
    :align: center
----

On the figure above, can be seen the example of how the Mangue.io platform presents the cluster infrastructure consumption values. This graph exhibits the last four months of consumption.

The current month's accumulated value represents the consumption of the first day of the month until the consult day; this way, in case the current day is the first week of the month, the accumulated value represents the week's consumption.

It is important to mention, the Mangue.io platform ZEROES all the values of the month on the first day of each month. And starts the sum (mathematical progression) until the last day of the month (day 30 or 31 - except the month of February).

On the vertical axis, are presented the maximum rounded value for the next value above the maximum, in a period. For the user to identify the correct value, just position the mouse pointer over the bar of the desired month, for the Mangue.io platform may present the detailed value of the month in which the mouse cursor is positioned. 

----

C. **By Tags**
~~~~~~~~~~~~~~

The Mangue.io platform allows the Kubernetes application to have Tags, composed by a set of key and value, with the objective to group similar applications and the objective of viewing their invoicing. 

The Tags can be created or associated with an application during the creation process of an application, according to the demonstration on the "New Application" section on Catalog, or in an already existing application, demonstrated on the "Change Tags" section in Deployments. 

The Invoicing by Tags screen is separated in two sections: 

* Monthly invoicing by tags history;
* Tags details.

.. image:: /figuras/fig_mangue/94_mangue_historico_tags.png
    :alt: tags history
    :align: center
----

On the Monthly Invoicing by Tags History section, the user must first select a Cluster, so the platform can load the Cluster Tags. After that, the user may select the desired invoicing period and the Tags to be exhibited in graph and on the Tags Details section.

.. image:: /figuras/fig_mangue/95_mangue_detalhes_tag.png
    :alt: tags details
    :align: center
----

On the Tags Details section, is exhibited a list with all of them or only the selected Tags on the Monthly Invoicing by Tags History section. On the Tag detailing, is presented a list of applications with Tag and a graph with the Tag invoicing in the last 30 days.

The user can exclude a Tag clicking on the |icone_lata_lixo_preta| button, on the Tag detailing.

----

D. **Alerts** 
~~~~~~~~~~~~~~

Through alerts, it is possible for the user to be notified when reaching the established budget for a deployment or set of deployments, when grouped in tags. Besides being able to configure the actions that must be executed when the budget for these resources is achieved. This makes it possible for the user to have more control over the cost of each service. 

As viewed on the following images, a card displays "Alerts" and the other "Webhooks", the details of each one of them are described on the sequence:

.. image:: /figuras/fig_mangue/96_mangue_alertas_webhooks.png
    :alt: alert webhooks
    :align: center
----

* **Alerts**: Shows an alert list, with the following columns:

      * **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|.
  
When the user choses a line or several, the Mangue.io platform presents the icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. 

In this case the "Trash bin" icon |icone_lixo_vermelho| is presented, which allows to remove all the items indicated by the user with a single command;

      * **Name**: This column presents the alert name defined on its creation moment. When selecting this blank is presented the information screen about the alert, on it the user can visualize a progress bar, actions and webhooks selected in the creation moment. As can be seen on the image below:

.. image:: /figuras/fig_mangue/97_mangue_alert.png
    :alt: alert
    :align: center
----

      * **Progress bar**: Corresponds to the current value of the deployments associated with the alert, having as 100% the alert budget value;
  
      * **Actions**: Action executed in the moment in which the deployments associated to an alert reach the budget price;
  
      * **Webhooks**: Webhook executed in the moment in which the deployments associated to an alert reach the budget price;
  
      * **Application**: This column presents the deployment or set of deployments selected for the corresponding alert in the moment of the alert creation;
  
      * **Status**: This column presents two possible values, “DONE” and “PENDING”:
  
          * **DONE**: Indicates the alert has already reached the budget price and that was executed, shooting the webhooks and configured actions;

          * **PENDING**:Indicates the alert was not executed;

      * **Date**: This column presents the creation date of the alert;
  
      * **Alert quota**: This column presents the budget price defined for the alert;

      * **Actions**: This column presents the action button |icone_acao| when clicked, it presents a single option to delete the alert.
	
.. image:: /figuras/fig_mangue/98_mangue_deletar_alerta.png
    :alt: delete alert
    :align: center
----
	
          * **Delete Alert**: When the user selects this action the Mangue.io platform requires a confirmation from the user to remove (erase) the desired alert from the platform database:


.. image:: /figuras/fig_mangue/99_mangue_aviso_deletar.png
    :alt: warning delete
    :align: center
----

On this alert sections it is possible to visualize the add alert icon, as the following example |icone_adicionar|, by clicking on the button is presented a form with blanks for the user that enable the creation of an alert, following a flow of three steps, details, webhooks and actions:

* **Details**: On this step is required information about the alert specifically: 

      * **Name**: Blank corresponding to the alert name;
  
      * **Description**: Blank corresponding to the alert description;
  
      * **Type**: There are two possible values for the type, by Tag to select a set of deployments, and by Deployment to select only one deployment. By selecting a tag or deployment occurs a search of the total cost value corresponding to the deployment or selected tag, this value is presented on the Current Cost blank presented on the screen;
  
      * **Deadline**: This blank may be defined a deadline for the alert execution, the alerts with the pending status are not executed after the deadline established for the alert;
  
      * **Budget**: On this blank may be informed the alert budget price, when the total cost of the selected deployments sum reaches the value informed the alert is executed. 
  

.. attention:: The Budget Value needs to be bigger than the Current Cost value.

.. image:: /figuras/fig_mangue/100_mangue_alerta_detalhes.png
    :alt: details modal
    :align: center
----

* **Webhook**: On this step there is a list of webhooks, the user can select none or several. When selecting a webhook it is listed below for the user to inform the type of return executed, being able to choose between HTTP or e-mail. 

.. image:: /figuras/fig_mangue/101_mangue_alerta_webhook.png
    :alt: webhook modal
    :align: center
----

* **Actions**: On this step it is possible to select an action to be executed in the moment of alert execution, there are three values the user can select for action, as the example on the image below:

.. image:: /figuras/fig_mangue/102_mangue_alerta_acoes.png
    :alt: alert actions
    :align: center
----

      * **Application Escalation**: This action allows the user to configure the switch of quantity of replicas in execution of the selected application. The moment in which the alert is executed, makes it possible to decrease/increase the quantity of instances of an application, in an aligned way to the current cost of the same application. Example on the following image:

.. image:: /figuras/fig_mangue/103_mangue_escalonamento_aplicacao.png
    :alt: application Escalation
    :align: center
----

      * **Change Request and Limits**: This action allows the user to change the request and limit of the selected applications, by the moment in which the alert is executed. Example on the following image:

.. image:: /figuras/fig_mangue/104_mangue_alterar_request_limit.png
    :alt: change request limit
    :align: center
----

      * **Stop Application**: It is also possible to stop the selected application, by the moment in which the alert is executed. For that, it is necessary to click on ``Confirm application stop``.

.. image:: /figuras/fig_mangue/105_mangue_parar_aplicacao.png
    :alt: stop application
    :align: center
----

.. note:: At least one webhook or one action must be informed to enable the alert creation.

* **Webhooks**: The webhook is a form of sending information to some recipient when an event happens, in this case when the deployments related to the alert reach the budget price defined on the alert creation, the Webhook shoots the information. The Mangue.io provides two forms of sending information: through the HTTP protocol, and/or through the email.

.. image:: /figuras/fig_mangue/106_mangue_webhooks.png
    :alt: webhooks
    :align: center
----

      * **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|. 
  
When the user choses a line or several, the Mangue.io platform presents an icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. 

In this case the "Trash bin" icon |icone_lixo_vermelho| is presented, which allows to remove all the items indicated by the user with a single command;

      * **Name**: This column presents the webhook name defined in the creation moment;

      * **Method**: This column presents the HTTP method selected in the webhook creation moment, there may be the following values: “GET”, “POST”, “PUT”, “DELETE”, “PATCH”;
  
      * **Url**: This column presents the recipient url to send the message;
  
      * **Body**:This column presents the HTTP requisition body;

      * **Email**: This column presents the recipient email to send the message to the corresponding webhook;

      * **Alerts**: This column presents an alerts list that are related to the corresponding webhook;

      * **Actions**: This column presents the ``Action`` button |icone_acao| when clicked, it presents the following options:

.. image:: /figuras/fig_mangue/107_mangue_acoes_webhook.png
    :alt: actions webhook
    :align: center
----

          * **Delete Webhook**: When the user selects this action the Mangue.io platform requires confirmation from the user to remove (erase) the desired alert from the database: 

.. image:: /figuras/fig_mangue/108_mangue_deletar_webhook.png
    :alt: delete webhook
    :align: center
----

          * **Edit Webhook**: When the user selects this action the Mangue.io platform presents the form present on the image below with the webhook information, for the user to edit.

.. image:: /figuras/fig_mangue/109_mangue_editar_webhook.png
    :alt: edit webhook
    :align: center
----

* **Name**: The webhook name must be informed;
* **Method**: Indicates the HTTP requisition method;
* **URL**: Informs the HTTP requisition url;
* **Body**: Communicates the HTTP requisition body;
* **Email**: Indicates the email to send messages;.
* **Menssage**:  Expresses the message that is sent to the email informed on the previous blank.

On this webhook section it is possible to visualize the add icon, as the following example |icone_adicionar|.

.. attention:: The webhook addition form is the same one presentes for edition.

====

Recommendations
===============

The Mangue.io platform may make recommendations to optimize the CPU and Memory usage of the Cluster applications, with the objective to avoid waste. On Kubernetes makes the resource allocation to an application using the following concepts:

* **Request**: Minimal quantity of allocated resources to the application. Example: an application with memory request of 256 MB always has allocated that memory quantity, even if the application always use only 20MB;
* **Limit**: In case the application needs to use more resources than specified on Request, the Kubernetes tries to allocate more resources in case the machine does not have it available. It is possible to limit the resource quantity the Kubernetes tries to allocate the application using Limit. Example: an application request of 256 MB always has 256 MB allocated, if it needs more memory it can be allocated until 512MB and in case it is not enough the application runs out of memory, causing slowness or instability on the application.

The platform makes the optimization by analyzing the history metrics of CPU and memory usage, therefore verifying if an application is with more resources allocated than necessary or with insufficient resources to keep the stability. 

   .. image:: /figuras/fig_mangue/110_mangue_recomendacoes.png
    :alt: recommendations 
    :scale: 80 %
    :align: center
=====

The recommendations page is exhibited in a list with the applications on namespace and current Cluster, and it is possible to search recommendations through the application name. 

Below is described the information presented on the scheduled tasks table.

* **#**: Sequential number recommendation registered on Mangue.io platform;.
* **App**: Application name with the recommendation;
* **CPU Current /Ideal Request**: Indicates the current value and recommended CPU Request. In case there is no recommendation on this column “- / -” is exhibited; 
* **CPU Limit Atual/Ideal**: Indicates the current value and recommended CPU Limit. In case there is no recommendation on this column “- / -” is presented; 
* **Memory  Request Current /Ideal**:Indicates the current value and recommended Memory Request. In case there is no recommendation on this column “- / -” is shown; 
* **Memory Limit Current /Ideal**: Indicates the current value and recommended Memory Limit. In case there is no recommendation on this column “- / -” is presented; 
* **Actions**: This column has the following elements: 

      * ``Apply`` button, when clicked applies the recommended values on the application;
      * ``Action`` button |icone_acao| when clicked, it presents the following option:

.. image:: /figuras/fig_mangue/111_mangue_descartar_recomendacao.png
    :alt: discard recommendation 
    :scale: 80 %
    :align: center
=====

          * **Discard the current recommendation**: When selecting the option to discard, the recommendation selected is removed, and a previous recommendation is shown, in case there is one. 
          * ``More Suggestions`` **button**: when clicked redirects to a page where is presented a list with all the recommendations generated previously.

.. image:: /figuras/fig_mangue/112_mangue_historico_recomendacao.png
    :alt: recommendation suggestion history 
    :scale: 80 %
    :align: center
=====

Permissions
============

All the points described on this segment are stored on the database that supports the Mangue.io platform installation. This database, and its content, must be managed and changed at the servers Linux operating system prompt (virtual machines) that support the Mangue.io platform infrastructure.

During the process of default implementation on the Mangue.io platform, it is installed a database manager (MariaDB / MySQL) and the content of this database and its registers referring to Clusters, Permissions, Billing, Contracts, *ClusterRole*, *ClusterRoleBinding*, Service and *ServiceAccount*, are populated during the post-installation software process.

It is not object of this document do described the inclusion process of new registers on the Mangue.io platform database, get in touch with the Ustore support area so you can have access to the document “Mangue.io Installation Manual (see item: Default Content from the Database)”.

On the next screens are described how the platform interface presents the database content through the Mangue.io HTML interface.


Contract
---------


Below is the screen that presents information about the contract selected on the configuration menu, it is possible to visualize the information about the contract and information about the users of the contract.

.. image:: /figuras/fig_mangue/113_mangue_informacoes_contrato_user.png
    :alt: contract information
    :align: center
----

A. **Contract information**
~~~~~~~~~~~~~~~~~~~~~~~~~

 It is possible to visualize the contract administers, price per CPU and price per memory defined for the contract.

B. **Users information**
~~~~~~~~~~~~~~~~~~~~~~~~

On this section are listed the information about the contract users, and the level of permission of each user. The permissions per user reflect the level of permission attributed to a user on the uCloud, following the example of the table below:

.. image:: /figuras/fig_mangue/114.1_mangue_eng_table.png
    :alt: table uCloud
    :align: center
----

In case some permission change had happened in some of the users whether it is a user removed from the contract, user added to the contract, or even the same level of permission altered, there is a routine to synchronize the users permissions with the uCloud, reflecting such changes on the Mangue.io. 

Nonetheless, in case there is interest of executing the permissions  synchronization in that exact moment, there is a icon on the right side |icone_sync|, when clicked it is executed the same function to synchronize permissions that would have been by the routine. 

Through this users list it is possible to extract the following information:

* **Login**: This blank presents the user login that was provisioned on the Mangue.io platform database;
* **Role**: This column presents the authorization profile (role) of the provisioned user;
* **Service Account**: This column presents the service account associated to the user;
* **Cluster Role**: This column presents the cluster role associated to the user; 
* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked, it displays the following option:

.. image:: /figuras/fig_mangue/115_mangue_deletar_permissoes.png
    :alt: delete permissions
    :align: center
----

      * **Delete Permissions**: By selecting this action the corresponding user to the selected line permissions is removed. The platform requests a confirmation to delete the user permission on the Mangue.io, as the image below:

.. image:: /figuras/fig_mangue/116_mangue_aviso_permissao.png
    :alt: warning permission
    :align: center
----


Roles
------

Access control based on functions/profile (Role Based Access Control - RBAC) is a method of regular access to computer resources or networks based on the functions of individual users in its organization.

A RBAC role (permission/profile) or *ClusterRole* contains rules that represent a set of permissions. 

.. note:: A role always defines permissions in a specific namespace; when creating a rule it must specify the namespace to which it belongs.


A. **Section: Roles**
~~~~~~~~~~~~~~~~~~~~~~

In this section the user may see a list of all the existing roles in the cluster that was selected on the gears tab |icone_engrenagem| "Configuration Selection".

.. image:: /figuras/fig_mangue/117_mangue_roles.png
    :alt: roles
    :align: center
----

* **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|. 

When the user choses a line or several, the Mangue.io platform presents the icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. 

In this case the “Trash bin” icon |icone_lixo_vermelho| is presented, which allows to remove all the items indicated by the user with a single command;
* **Name**: On this column it presents the role name added by the user;
* **Labels**: Labels are used to specify the objects attributes identification that are significant and relevant and present on the role yaml syntax;
* **Duration**: This column presents the elapsed time in days since the moment of the initial application of this role;
* **Actions**:This column presents the ``Action`` button |icone_acao|  when clicked, it displays two options: 

.. image:: /figuras/fig_mangue/118_mangue_acoes_role.png
    :alt: actions role
    :align: center
----

      * **Delete Role**: When the user selects this action they remove the role from the cluster that was selected on the gears tab |icone_engrenagem| "Configuration Selection". It is worth remembering that this action is irreversible and definite. The Mangue.io platform requires the user confirmation to remove (erase) the desired group from the database:

.. image:: /figuras/fig_mangue/119_mangue_deletar_role.png
    :alt: delete role
    :align: center
----

In case the user had executed this action by mistake, it is necessary to register the group on the Mangue.io platform database through any SSH tool; The action of including configuration on the database is made through the command line on the virtual machine Linux operating system that supports the execution of the Mangue.io platform.

      * **Edit Role**: It is recommended that only users experts in YAML syntax make the alterations in a role, because the codification (or alteration) of the syntax in a wrong form may result in the access lost to all the existing clusters' environment.
This option opens a screen of role edition using the YAML syntax code, as on the example of the screen below.

.. image:: /figuras/fig_mangue/120_mangue_editar_role.png
    :alt: edit role
    :align: center
----

The user must start clicking with the mouse on the gray area next to the number of the line they wish to edit, before starting to type their YAML code. For each new line the user must use the ``Enter`` key to start a new line, using their own development experience to structure their syntax code line by line. Through this option the user can enter (or edit) with a YAML code to create, edit the role on the Mangue.io platform. 

After editing a role the user must click on the green button ``Send`` for all the code to be sent and applied to the cluster that was selected on the gears tab |icone_engrenagem| "Configuration Selection".

----

B. **Section: Role Bindings**
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A linking of function/profile (*rolebinding*) concedes the permissions defined in a role to a user or set of users. It contains a list of subjects (users, groups or service accounts) and a reference to the role that is being conceded. A *RoleBinding* concedes permissions within a specific namespace, while a *ClusterRoleBinding* concedes this access to the whole cluster.

A *RoleBinding* may make reference to any role in the same namespace. As an alternative, a *RoleBinding* may make reference to a *ClusterRole* and link a *ClusterRole* to the *RoleBinding* namespace. If you wish to link a *ClusterRole* to all the namespaces in its cluster, use a *ClusterRoleBinding*.

.. image:: /figuras/fig_mangue/121_mangue_bindings.png
    :alt: role Bindings
    :align: center
----

* **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|. 

When the user choses a line or several, the Mangue.io platform presents the icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. 

In this case the “Trash bin” icon |icone_lixo_vermelho|  is presented, which allows to remove all the items indicated by the user with a single command;
* **Name**: On this column is presented the *rolebinding* name added by the user. When clicking with the mouse over the name, the Mangue.io platform presents a screen with the content(s) of the *configMap* file(s). 

By default it presents only the visualization of a line from the file content, in case the content is bigger than the blank, the user can position the mouse on the inferior right corner, until the mouse cursor changes for a double diagonal arrow |icone_seta_diagonal|, that allows the user to redimension the listed content blank size, for a better view of this blank.
* **Labels**: Labels are used to specify the objects attributes identification that are significant and relevant and present on the role yaml syntax;
* **Duration**: This column presents the time elapsed in days since the moment of its initial application of this *rolebinding*;
* **Actions**: This column presents the ``Action`` button |icone_acao| when clicked, it presents two options:

.. image:: /figuras/fig_mangue/122_mangue_acoes_bindings.png
    :alt: actions Bindings
    :align: center
----

      * **Delete RoleBinding**: When the user selects this action they remove the *rolebinding* from the cluster that was selected on the gears tab  |icone_engrenagem| "Configuration Selection". It is worth remembering that this action is irreversible and definite. The Mangue.io platform requests the user confirmation to remove (erase) the desired *rolebinding* from the database:

.. image:: /figuras/fig_mangue/123_mangue_aviso_bindings.png
    :alt: warning role Bindings
    :align: center
----

In case the user had executed this action by mistake, it is necessary to register the *rolebinding* on the Mangue.io platform database through any SSH tool; The action of including configuration on the database is made through the command line on the virtual machine Linux operating system that supports the execution of the Mangue.io platform.

      * **Edit Rolebinding**: It is recommended that only users experts in YAML syntax make the alterations in a *rolebinding*, because the codification (or alteration) of the syntax in a wrong form may result in the access lost to all the existing clusters' environment.

This option opens a *rolebinding* edition screen using the YAML syntax code, as the example of the screen below:

.. image:: /figuras/fig_mangue/124_mangue_editar_binding.png
    :alt: edit role binding
    :align: center
----

The user must start clicking with the mouse on the gray area next to the number of the line they wish to edit, before starting to type their YAML code. For each new line the user must use the ``Enter`` key to start a new line, using their own development experience to structure their syntax code line by line. Through this option the user can enter (or edit) with a YAML code to create, edit the *rolebinding* on the Mangue.io platform. 

After editing the rolebinding the user must click on the green button ``Send`` for all the code to be sent and applied to the cluster that was selected on the gears tab |icone_engrenagem| "Configuration Selection".

----

Service accounts
-----------------

When a user accesses the cluster, they are authenticated by *APIServer* as a specific user account (currently, generally is admin, unless the cluster administrator has personalized their cluster). The process in containers within the PODs can also get in touch with *APIServer*. When they do, they are authenticated as a specific service account (for example, default).

.. image:: /figuras/fig_mangue/125_mangue_service_account.png
    :alt: service account
    :align: center
----

* **# actionable column**: This column presents an alternative way to remove (erase) various rows in a single command. Each row is represented by a selectable icon |uCloud_icone_coluna_acionavel|. 

When the user choses a line or several, the Mangue.io platform presents the icon(s) above this column, they represent the user's actions to be executed once for all the selected lines. 

In this case the “Trash bin” icon |icone_lixo_vermelho| is presented, which allows to remove all the items indicated by the user with a single command;
* **Name**: On this column, it is presented the *serviceaccount* name added by the user;
* **Namespace**: Informs the namespace in which the *serviceaccount* was created;
* **Duration**: On this column presents the time elapsed in days since the moment of the initial application of this *serviceaccount*;
* **Actions**: This columns presents the ``Action`` button |icone_acao| when clicked, it presents a single option:

.. image:: /figuras/fig_mangue/126_mangue_aviso_service_account.png
    :alt: warning service account
    :align: center
----

      * **Delete ServiceAccount**: When the user selects this action they remove the *serviceaccount* of the cluster that was selected on the gears tab |icone_engrenagem| “Configuration Selection”. It is important to remember that this action is irreversible and definitive. The Mangue.io platform requests confirmation from the user to remove (erase) the *serviceaccount* desired from the database:

.. image:: /figuras/fig_mangue/127_mangue_cluster_role.png
    :alt: cluster role
    :align: center
----

In case the user had executed this action by mistake, it is necessary to register the *serviceaccount* on the Mangue.io platform database through any SSH tool; The action of including configuration on the database is made through the command line on the virtual machine Linux operating system that supports the execution of the Mangue.io platform.

----

Cluster Role
------------



.. |icone_engrenagem| image:: /figuras/fig_mangue/icone_engrenagem.png

.. |icone_lata_lixo_preta| image:: /figuras/fig_mangue/icone_lixo.png

.. |icone_lupa_vermelha| image:: /figuras/fig_mangue/icone_lupa_vermelha.png

.. |icone_sinal_menor| image:: /figuras/fig_mangue/icone_sinal_menor.png

.. |uCloud_icone_coluna_acionavel| image:: /figuras/uCloud_icone_coluna_acionavel.png

.. |icone_reversao| image:: /figuras/fig_mangue/icone_reversao.png

.. |icone_escalar| image:: /figuras/fig_mangue/icone_escalar.png

.. |icone_lixo_vermelho| image:: /figuras/fig_mangue/icone_lixo_vermelho.png

.. |icone_alterar_versao| image:: /figuras/fig_mangue/icone_alterar_versao.png

.. |icone_adicionar| image:: /figuras/fig_mangue/icone_adicionar.png

.. |icone_acao| image:: /figuras/fig_mangue/icone_acao.png

.. |icone_adicionar_vermelho| image:: /figuras/fig_mangue/icone_adicionar_vermelho.png

.. |icone_lupa_verde| image:: /figuras/fig_mangue/icone_lupa_verde.png

.. |icone_update| image:: /figuras/fig_mangue/icone_update.png

.. |icone_seta_diagonal| image:: /figuras/fig_mangue/icone_seta_diagonal.png

.. |icone_exibir| image:: /figuras/fig_mangue/icone_exibir.png

.. |icone_exportar| image:: /figuras/fig_mangue/icone_exportar.png

.. |icone_load_balancer| image:: /figuras/fig_mangue/icone_loadbalancer.png

.. |icone_rotulo| image:: /figuras/fig_mangue/icone_rotulo.png

.. |icone_engrenagem_azul| image:: /figuras/fig_mangue/icone_engrenagem_azul.png

.. |icone_sync| image:: /figuras/fig_mangue/icone_sync.png

