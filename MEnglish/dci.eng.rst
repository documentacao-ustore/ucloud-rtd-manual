.. image:: /figuras/index/_ustore_pequena.png
    :alt: logo ustore
    :align: center
======



DCI - Functionalities Manual
============================

Information technology solutions that make it possible to implement a scalable, solid and reliable computing architecture in a hybrid cloud.

====


Introduction
------------


This document consists of a manual with a brief description of the main functionalities contained in the **Data Center Interconnect - DCI** product, from the Ustore platform.

----

Presentation
----

**Data Center Interconnect - DCI**

How to login on DCI
------------------


To have access to the platform it is necessary to have made a first purchase on the Customer Panel.

After this purchase the user receives their access credentials, sent directly to their registered email.


.. image:: /figuras/fig_dci/01_log_in.png
    :alt: login
    :align: center
======

The user must fill out the ``login`` and ``password`` blanks, with the credentials received from the platform's administrator.
 
Click on the ``Login In`` button.

After this procedure, the initial screen of the portal is presented.

----

General view
------------


At first, it is important to understand the impact of some tools existing on the top right menu.

For that, the top menu cut out shown on the following image, displays relevant components, described in detail on the sequence.



.. image:: /figuras/fig_dci/02_qa_config_logout.png
    :alt: visão geral
    :align: center
======


**Notification icon** |icone_tarefas|: This icon is a relevant point for viewing all the activities done on the portal. Through it, it is possible to observe the most recent actions, reflecting as a notification on the Tasks screen.

**Account configuration**: Makes it possible to access the created account details, where it is possible to change the email, phone and manage users in your Company. This button directs to the Administration menu.

----

Administration menu
-------------------

For the complete view of the DCI services there are some menus on the side of the platform, in them it is possible to find valuable information to the product.



.. image:: /figuras/fig_dci/03_menu_adm.png
    :alt: menu administração 
    :align: center
======


DCI Menu
--------

This menu contains a submenu that makes it possible to view Ports, Circuits and Excursioning.


Ports submenu
~~~~~~~~~~~~

On this screen it is possible to view the ports resources, beyond that, it is possible to observe the actions to be taken with each item.



.. image:: /figuras/fig_dci/05_menu_portas.png
    :alt: Menu Portas 
    :align: center
======



Three functionalities are presented: the button to ``Show deactivated resources``, the ``Search`` action and the option to ``Refresh`` the page.

The ports information, are divided in six columns and presented, as mentioned above:

  * Designation
  * Status
  * Band
  * Type
  * Data Center
  * Golden Jumper

By selecting a port, it is possible to view the details completely. The new page presents three functionalities to ``Download LOA``, ``Resent LOA`` and the ``Confirmed`` button.

.. image:: /figuras/fig_dci/06_menu_porta_bre.png
    :alt: Menu porta bre 
    :align: center
======


Two information cards are shown: General and Vlans.

On the Vlans card, the update functionality of the page ``Refresh`` is presented, and information are divided into four columns:

  * Vlans in Use
  * Circuit
  * Band
  * Baseband

The information about the Vlans are shown in blocks of 10, 25, 50 or 100.



Circuits submenu
~~~~~~~~~~~~~~~~



This screen allows to view the circuit's resources, making it possible to observe the actions to be taken with each item.


.. image:: /figuras/fig_dci/07_menu_circuitos.png
    :alt: Menu Circuitos 
    :align: center
======



Three functionalities are presented: the button to ``Show deactivated resources``, the ``Search`` action and the option to ``Refresh`` the page.

The information about the circuits, are separated into eight columns and presented, as mentioned below:

  * Designation
  * Type
  * Baseband
  * Current Band
  * Port - VLAN ID
  * Port - VLAN ID
  * Status
  * Golden Jumper

When clicking in each circuit individually, it is possible to view the information of the actions done and its excursioning history in this circuit, divided into cards, as shown on the image below.

.. image:: /figuras/fig_dci/08_menu_circuito_04.png
    :alt: Menu Circuitos 
    :align: center
======

Besides that, it is allowed to make some operations within the circuit, as for example, the VLAN alteration or the change of type, found on the Configurations card.

----

Task menu
---------

On the task tab it is possible to track all the operations performed within the platform.


Task panel
~~~~~~~~~~

As mentioned above, the tasks screen is important to track the progress of the orders made on the platform.

.. image:: /figuras/fig_dci/04_menu_tarefas.png
    :alt: Menu Tarefas 
    :align: center
======

This menu makes it possible to view each error case, track the order status and cancel some operations.

.. image:: /figuras/fig_dci/04_head_tarefas.png
    :alt: Cabeçalho Tarefas 
    :align: center
======


The screen above presents on the right top part the tasks symbol, the username logged in, and the functionalities next:

  * ``Search`` Search blank that makes it easier to find information with agility.
  * ``Refresh`` Blank that allows to update the page with a click.


The tasks are presented in a list format, categorized in tabs containing the information about

  * Tasks
  * Pending approvals
  * Scheduled tasks


 .. image:: /figuras/fig_dci/04_lista_tarefas.png
    :alt: Lista de tarefas 
    :align: center
======

The "Tasks" tab shows eleven types of information divided into columns:

  * Operation
  * Order ID
  * Designation
  * Company name
  * Author
  * Error
  * Progress in percentage
  * Start date
  * Duration
  * Status
  * Action

Detailing the *status* column that shows three different states.

  * They are ``Success``, ``Fail`` or ``Approved``.


The objective of this status is to direct the tracking action, according to the following:

**Success status** - shown in green, means that the operation was concluded with success.

**Fail status** - displayed in red, means that an error occurred during the operation. On the failed task itself it is possible to verify what was the  reason for the irregularity, through the "Error" column.

**Approved status** - presented in green, means that the operation occurred with success. Although it depends on a user action, whether it is **admin** or **user**.

    * For cases such as "First Sale", the Golden Jumper confirmation of both ports is pending from the user.

    * For the cases of subsequent sales of ports, the Golden Jumper of the port in question is pending.

====


Conclusion
----------

This document presented a brief description of the functionalities contained on the **Data Center Interconnect - DCI** product, developed by the Ustore.


====

DCI Functionalities manual - February 8th, 2023 - Review on March 2nd, 2023.



.. |icone_tarefas| image:: /figuras/ucloud_icone_sino.png 


