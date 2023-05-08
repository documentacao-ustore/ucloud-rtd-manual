

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

After inserting the address correctly, the user’s login screen is similar to the image below: 



.. image:: /figuras/fig_mangue/001_mangue_login.png
    :alt: Login screen 
    :scale: 80 %
    :align: center
=====


The credentials for the login and password are the same as those of the uCloud platform, which the Mangue.io platform is integrated with. Every user provisioned on the uCloud can automatically use their credentials to gain access to Mangue.io. 

After inserting the access credentials (login and password) and performing the login procedure, a similar figure may be presented to the user, in case of existing a cluster associated with the user’s in the Mangue.io contract. 


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

The moment the user selects the cluster and namespace, the values on the Overview screen are changed with the specific data of the user’s selection. 

====

Home screen
===========

The Overview home screen displays some graphs referring to the consumption values of computing resources specific to the user’s selection, the details of the graphs follow below:


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

For this purpose, the user must click on the “Trash Bin” |icone_lixo| icon. The Mangue.io platform requests a confirmation from the user for the action displaying the screen below: 


.. image:: /figuras/fig_mangue/005_mangue_deletar_bilhetador.png
    :alt: Delete financial data from the Ticket Cluster 
    :scale: 80 %
    :align: center
=====


For the user to confirm the action of deleting all financial data (values) of consumption referring to the selected cluster in the “Browsing Settings” tab, click on the green-colored button ``Delete``. 

With this action all cluster consumption values are removed and a new period of information collection is started, losing all the information accumulated (the historic series) of the selected cluster. 


Cálculo do Valor do Consumo do Cluster
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

On this screen, it is also possible to visualize the CPU usage, in millicores, of each Kubernetes resource, for this, the user has to specify the namespace and the resources they wish to view the CPU consumption, and click on the “Magnifying Glass” icon |icone_lupa|, to do the search, returning the last thirty minutes of CPU and Memory consumption.


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


Some menu options have a submenu, which are presented when the user places the mouse over the indication (less than sign “<”). When clicking on this icon |icone_menor|, the interface presents this option’s submenu to the user, see the example in the figure below.


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

* **# actionable column:** This column presents an alternative way to remove (delete) multiple rows with a single command. Each row is represented by a selectable icon |icone_selecionavel|. When the user selects a line or several, the Mangue.io platform presents the icon(s) above this column, they represent user actions to be performed at once in all selected lines. In this case three icons with very distinct actions are displayed:
  
  * **Rollback |icone_reversao|:** This option allows the user to perform an action of reversing the current version of the selected deployment(s) for its immediate previous version to the existing one on the Mangue.io Platform. 
  
  * **Scale |icone_escalar|:** The function of this screen allows the user to inform the number (full) desired to increment the application (deployment) replica number.
   
  * **Trash bin |icone_lixo_vermelho|:** This option allows the user to remove all the selected items with a single command.
  
  * **Change version |icone_alterar|:** This option allows the user to update multiple deployments at once, to which the user can inform the next version of each of them.
  
* **Deploys:** It is the representation of the *deployment.d name*;
  
* **Labels:** These are the deployments’ identifiers, they are used to link to a service;
  
* **Instances:** Presents the number of replicas that are operational of a deployment, and the total number of operational replicas desired for this deployment. They are divided by a slash (“/”) where the values found before the slash are the operational replicas, and the values after the slash represent the expected amount of operational replicas;
* 
* **Status:** The status of a deployment identifies the current state of the deployment. They can be presented by Running, Pending or “!” (exclamation mark):
  
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


     B. **Add Service**
     The second option of this submenu allows the user to add a service, when clicked the following modal interface screen is opened:


.. image:: /figuras/fig_mangue/017_mangue_add_servico.png
    :alt: Add Service Deployment
    :scale: 80 %
    :align: center
=====



On this modal, the user must fill in the following blanks:

      * **Name of the service:** The user must fill out with the service name they want to create;
  
      * **Deployment Labels:** The user must inform which labels are associated with this service;
  
      * **Types of access to the service:** Internal, External or *LoadBalancer:*
  
          * **Internal:** Services that can only be accessed from inside the cluster;
  
          * **External:** Corresponds to services that allow access from outside the cluster. A TCP-IP port between 30,000 –– 32,767 is provided;
  
          * **LoadBalancer**: Integrated straight with the Cloud Providers (AWS, AZURE, GOOGLE) creating a LAYER 7 *loadbalancer* for the respective app;
  
      * **Source port:** Inform the TCP-IP port number of the container allocated to the service;
  
      * **Destination port for the service:** Inform the TCP-IP source port in the container, the service will receive the request on the source port and forward it to the destination port;
  
      * **Select the protocol:** TCP or UDP.
  
      * ``Add`` **button:** If the service needs to expose more than one port, the user must return to the SourcePort/Destination  Port,  and add as many source/destination ports as necessary. 

To confirm all the options informed above, the user must click with the mouse on the ``Create Service`` button and wait for the creation feedback.

        C. **Delete Deployment** 

        The third option of this submenu allows the user to remove definitely a Deployment from the cluster and from the namespace that was selected in the **Configurations** tab; when clicked, the following modal interface screen is opened, requesting confirmation from the user:


.. image:: /figuras/fig_mangue/018_mangue_deletar_deployment.png
    :alt: Delete Deployment 
    :scale: 80 %
    :align: center
=====

This action is immediate and irreversible, the Mangue.io Platform removes the deployment selected by the user from the contract/cluster/namespace.

Just click over the button ``Delete`` to confirm the action and the Mangue.io Platform deletes the deployment from the selected environment.


    .. note:: This action **does not** remove any additional components external to this deployment - e.g.: an associated *PersistentVolume*, therefore if an external file exists, it continues to exist on the destination volume. This action only removes the deployment from the environment, but does not remove any other additional files from the computing environment. 

    D. **Edit Deployment**
    Some information cannot be edited through the Mangue.io forms. Elements, such as: 

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
        The function of this screen allows the user to inform the number (full) desired to increment the number of replicas of the application (deployment), which starts automatically after the confirmation with the click of the mouse over the ``Scale`` button.


.. image:: /figuras/fig_mangue/020_mangue_escalar_deployment.png
    :alt: Scale Deployment
    :scale: 80 %
    :align: center
=====

It is important to highlight that there is an increase in the usage consumption of CPU and cluster memory to support the simultaneous execution of the replicas of this application in the cluster infrastructure. 

        G. **Migrate Deployment** 

In the sixth option of the Deployment actions menu, there is the option to migrate the deployment between different clusters configured in the Mangue.io Platform.

The user must select which cluster integrated with Mangue.io they wish to migrate the chosen deployment. The recipient cluster blank is a “dropdown list” type, when the user clicks on it, the list of available clusters associated with the chosen contract in the configuration menu is presented.

To do the migration, the user just needs to click on the ``Migrate`` button and wait for the action feedback from the Mangue.io Platform. As a result of this action, a “Success” alert will be displayed on the upper right menu of the screen.


.. image:: /figuras/fig_mangue/021_mangue_migrar_deployment.png
    :alt: Migrate Deployment 
    :scale: 80 %
    :align: center
=====

        H. **Modify Version** 
    
After clicking on “Update Application Version” the platform presents the image “Update Deployment Version”. Through this control, the user can generate a “new version” for any deployment existing on the Mangue.io Platform. 


.. image:: /figuras/fig_mangue/022_mangue_atualizar_deployment.png
    :alt: Update deployment version 
    :scale: 80 %
    :align: center
=====

This blank is alphanumeric and the user can enter the desired information to identify the new version of the selected deployment. The new versions are under the sole control of the user, as they refer to the offers created by this user. 

After filling with the desired information, the user must click on the ``Send`` button to confirm the action to create a version for the deployment.


.. attention:: These new versions are not necessarily related to any version of the composing softwares, or any software that was used to compose the offer, different versions can be found outside of the Mangue.io platform.

        J. **Rollback**

This option allows the user to perform the action of reverting the deployment version to its version immediately prior to the existing version on the Mangue.io Platform.

This action in particular does not activate any additional confirmation screen, its action is immediate.

.. important:: By selecting this option, the Mangue.io Platform performs the reversal of the version immediately without requesting any confirmation from the user.

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

This section displays three graphs, two being of performance and one of value:

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


        C. **Section: PODs**

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


        E. **Section: Events**

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