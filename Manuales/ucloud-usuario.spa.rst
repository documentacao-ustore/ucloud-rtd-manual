Manual de Administración y Operación de uCloud
++++++++++++++++++++++++++++++++++++++++++++++


.. image:: /figuras/ucloud_logo_peq.png
   :alt: logo ucloud
   :align: center

----

Soluciones de tecnologías de la información que permiten implementar una arquitectura de cómputo escalable, sólida y confiable en una nube distribuida.


-----

Presentación
============

Este documento tiene como objetivo explicar el uso de la Plataforma *uCloud*, una plataforma de Cloud Service Broker (broker de servicios en nube) que permite administrar múltiples proveedores de servicios de nube, tanto privados como proveedores de nube pública. 

En este manual se presentan los conceptos, las pantallas, las funcionalidades y los comandos de uso de este producto.

----

Introducción
============

Las organizaciones empresariales han adoptado la nube como solución para administrar sus entornos y adoptan una combinación de nubes privadas y públicas, el gran desafío actual es la gestión de estos entornos híbridos de múltiples nubes *(hybrid multi-cloud)* con el fin de lograr una visión unificada, así como obtener un control centralizado de los costos financieros, ya que cada organización empresarial tiene una necesidad y se enfrenta a diferentes desafíos.

La Plataforma de uCloud ha sido desarrollada para estos escenarios, independientemente de cuantos proveedores (públicos y/o privados) existan, el usuario podrá interactuar con sus plataformas de Infraestructura como Servicio *(Infrastructure as a Service - IaaS)*, Plataforma como Servicio *(Platform as a Service - PaaS)*.

Como se mencionó anteriormente, uCloud está posicionado como una plataforma de **Cloud Service Broker - CSB** *(Broker de servicios en la nube)* que permite administrar múltiples proveedores de servicios en la nube, tanto privados como proveedores de nube pública.

Una plataforma **CSB** como la Plataforma uCloud permite a las organizaciones actuar en cinco puntos fundamentales para la gestión de entornos híbridos multi-nube, son:


Gobernanza Financiera
---------------------

Además del control de la infraestructura, la Plataforma de uCloud permite a las empresas usuarias de esta plataforma establecer límites, tanto financieros como cuantitativos de recursos (cuotas). Estos límites financieros o de infraestructura pueden aplicarse en tres niveles:

  * Para un proveedor público en general (ver el elemento Contratos, en el Menú Administración);
  * Para un grupo de usuarios (ver el elemento Grupos en el menú Administración);
  * Para un usuario/individuo (ver el elemento Usuarios, en el Menú Administración).

De esta forma, la organización aplicará criterios de gobernanza financiera y control de costos, como también podrá acompañar los costos de su entorno híbrido de multi-nube a través de una única interfaz.  

La adopción de la aplicación de límites (cuotas) financieros y/o recursos computacionales en diversos niveles alcanza el nivel de usuario, Así el control de costos será efectivo y permitirá evitar que el presupuesto de la organización sorprenda en situaciones que el costo de la infraestructura computacional sea exorbitante o por encima de los valores preestablecidos.

Otro aspecto de la Plataforma de uCloud es la reducción de costos de certificación y capacitación de los especialistas, en cada una de las interfaces de cada proveedor (público y/o privado), ya que el empleo de una interfaz de uso y gestión única y sencilla permite extraer más productividad del entorno del proveedor de la nube. Incluso si el usuario no cuenta con capacitación o certificación en la consola específica del proveedor (pública y/o privada), la plataforma uCloud permitirá al usuario aprovisionar un recurso informático en el entorno deseado de manera sencilla y fácil.

Billing (Facturación de los Servicios)
--------------------------------------

La Plataforma de uCloud proporciona a las organizaciones empresariales información sobre los costes recurrentes relacionados con el uso de los recursos computacionales en la(s) operación(es) en un entorno multinube híbrido. Este es solo uno de los puntos que forma parte de la práctica de **Cloud 
Financial Management - FinOps** (Gestión financiera de la nube).

Es importante resaltar que, individualmente, la Plataforma de uCloud no atiende a los tres pilares de la práctica de *FinOps* por *default*. Ustore posee otros productos que pueden ser complementarios y el conjunto de productos tiene potencial para actuar como un entorno capaz de englobar y atender la 
práctica de *FinOps*.

El requisito soportado por uCloud es el punto de **Información** *(Inform)*, los otros puntos de esta mejor práctica de *FinOps*: la **Optimización** y la **Operación** pertenecen a los otros productos de la cartera de Ustore que complementa la Plataforma de uCloud.

Se debe aclarar que la Plataforma de uCloud no crea ni genera valores de recursos computacionales, estos valores se generan en los proveedores de nube pública de los que la Plataforma de uCloud **extrae** *(descargar)* el archivo de **Billing** *(facturación)* de estos proveedores y añade esta información en sus 
bases de datos internas. Para que, posteriormente, de acuerdo con los criterios comerciales del contrato puedan ser aplicados y estos costos calculados y convertidos para la moneda corriente en Brasil.

De esta forma, el usuario permanece **informado** de la evolución de los costos y podrá seguir si estos costos se encuentran dentro de los criterios de la gobernanza financiera de la organización.

Generalmente estos costos se presentan en archivos de texto no estructurados **(Comma-separated Values - CSV)** generados cada período (promedio de 8 horas) y la Plataforma de uCloud agrega la información de este archivo **CSV** a su base de datos interna para agilizar y simplificar la presentación de estos valores en la pantalla del usuario.

Exclusivamente, los usuarios con un perfil específico pueden 'visualizar costos' y permanecer **informados** de los valores de consumo de sus recursos computacionales totales en cada proveedor de la nube (pública y/o privada). Esto permite que el usuario pueda realizar un seguimiento de los costos acumulados de los recursos informáticos activos en los proveedores de servicios en la nube.

Monitoreo de la Infraestructura
-------------------------------

Una funcionalidad importante de la Plataforma de uCloud es la reciente implementación del módulo de gestión de eventos (monitoreo) que permite recopilar eventos y alarmas que se han generado en los entornos de nube (público y/o privado), activar notificaciones y crear informes personalizados. 

Todas estas facilidades reducen los costos para las organizaciones, una vez que elimina la necesidad de contratación de servicios de monitoreo de los proveedores, pues tal servicio puede representar altos costos los cuales pueden impactar de forma negativa en el presupuesto (sobrepasar el límite) 
destinado a infraestructura de nube pública. 

Esta funcionalidad permite integrar a un entorno de gestión de Service Desk 
para control *IT Service Management* (gestión de servicios de TI).

Inventario *(Assessment)*
-----------------------

La plataforma de uCloud se conecta a los proveedores de la nube mediante el registro de credenciales de acceso específicas de cada proveedor de servicios en la nube (público y/o privado). Para ello, las empresas deben proporcionar credenciales de modo **"operativo"**.

Esta credencial operativa es proporcionada por el administrador del servicio en la nube y son credenciales que se generan en las cuentas de los proveedores que solo tienen permiso para interactuar con la consola del proveedor público en la nube a través de una API, no son credenciales normales con información estándar de inicio de sesión y contraseña. De esta forma, la seguridad y las 
normas de regulación de seguridad de la información están previstas y atendidas en su totalidad.

Como las credenciales *operativas* se configuran en la Plataforma de uCloud, la primera actividad es sincronizar la configuración y el inventario de recursos informáticos existentes en el proveedor (máquinas virtuales - cargas de trabajo). Este inventario de máquinas virtuales se extrae y se agrega a las bases de datos de uCloud para que la presentación en la pantalla del usuario sea rápida.

Con este inventario disponible directamente dentro de la Plataforma de uCloud, el usuario podrá operar cada una de las máquinas virtuales, independientemente de cuál sea el proveedor de la nube que esta función está aprovisionada. Vea a continuación las posibles operaciones a aplicar a los 
recursos computacionales existentes en los proveedores de nube (público y/o privado).

Es importante mencionar que la Plataforma de uCloud no tiene recursos computacionales, estos recursos existen en las nubes de los proveedores de servicios de nube pública o en los entornos de virtualización *(hypervisors)* instalados en su DataCenter privado. A través de la API Rest, la Plataforma de uCloud, envía acciones (tareas) al administrador de entorno de nube específico (público y/o privado) para que realicen la acción deseada.

El usuario podrá seguir el resultado de cualquiera de las acciones de operación en los recursos computacionales de forma casi inmediata, vale recordar que no es la Plataforma de uCloud la que **ejecuta** las acciones, sino el entorno donde la máquina virtual existe (ya sea público y/o privado). Este es el encargado de ejecutar la tarea enviada a través de la API Rest.

Si el resultado no se refleja en la interfaz de la pantalla del usuario, la consola de destino puede tardar un cierto tiempo en realizar esta tarea y solo después de que finalice la ejecución de la tarea se mostrará el resultado en la interfaz de uCloud.

Existe una opción de menú donde el usuario podrá seguir el porcentaje de progreso de estas tareas, su resultado de éxito o el mensaje de error referente a alguna restricción del entorno destino.

Es importante resaltar que pueden existir restricciones aplicadas al usuario aprovisionado en la Plataforma de uCloud, restricciones al usuario porque puede haber agotado su límite, su cuota financiera o de recursos computacionales, de esta forma la Plataforma de uCloud generar un aviso de 
error: **"límite de cuota excedido"** por ejemplo. Estos escenarios se describen en el menú Tareas.

Operación de la Infraestructura
-------------------------------

La mención operar significa al lector que es la capacidad del usuario comandar ciertas acciones directamente en estas máquinas virtuales, como acciones de:

 * Parar (shutdown)
 * Reiniciar (restart) 
 * Suspender (suspend)
 * Remover (delete)
 * para citar algunas operaciones básicas.

A través de la interfaz de la Plataforma de uCloud, el usuario puede enviar comandos a las consolas de cada proveedor de la nube, además de las acciones mencionadas anteriormente. También puede ver la información de la configuración específica de la máquina virtual, así como cambiar o agregar algunas características adicionales a esta máquina virtual (por ejemplo: tarjeta de red, disco, grupo de seguridad, snapshot, entre otros).

En cuanto a los proveedores de servicios de nube pública, la Plataforma de uCloud está preparada para conectarse con las siguientes plataformas de nube pública:

* ** Amazon Web Services *(AWS)*
* ** Google Cloud Plataform *(GCP)*
* ** Microsoft *Azure*
* ** IBM Cloud
* ** Huawei Cloud
* ** Oracle Cloud Infrastructure *(OCI)*

Actualmente, la plataforma uCloud está lista para conectarse con las siguientes plataformas *(hypervisors)* de administración de entornos de nube privada:

* ** VMware *(vCenter Versões 5.0, 5.1, 5.5, 6.0, 6.5, 6.7, 7.x ou superior)*
* ** vCloud
* ** Hyper-v *(Windows 2008R2, Windows 2012, Windows 2012R2 e Windows 2016 ou superior)*
* ** Openstack
* ** Xen Server
* ** XCP-NG
* ** KVM

La plataforma uCloud, además de las funciones CSB *(Cloud Service Broker)*, también es un agregador 
de funcionalidades que permite a los usuarios, de forma sencilla y centralizada, controlar varias consolas de administrador de entornos virtualizados *(hypervisors)* desde el entorno local privado *on-premises* o desde el entorno del proveedor de nube pública. Agrega monitoreo, flujo de trabajo en la nube *(Cloud Workflow)* y le permite implementar un repositorio ‘biblioteca’ centralizado de archivos de referencia *(playbooks)* para el uso de herramientas de infraestructura como código
*(Infrastructure as a Code)*.


Integración e Interoperabilidad Multiplataforma *(API de uCloud)*
=================================================================

La interoperabilidad es la capacidad de dos o más sistemas (ordenadores, medios de comunicación, redes, programas informáticos y otros componentes de la tecnología de la información) para interactuar e intercambiar datos según un método definido, con el fin de obtener los resultados esperados. La interoperabilidad define si dos componentes de un sistema, desarrollados con diferentes herramientas, de diferentes proveedores, pueden o no actuar juntos.

La comunicación entre estos "sistemas" se basa en el consumo de una interfaz de programación de aplicaciones *(API)* que permite enviar y recibir llamadas para la ejecución de alguna actividad o la extracción de algún tipo de información almacenada. Las siglas API provienen de la expresión inglesa *Application Programming Interface* que, traducida al portugués, puede entenderse como interfaz de programación de aplicaciones. En otras palabras, la API es un conjunto de reglas que permite la comunicación entre plataformas a través de una serie de normas y protocolos.

A través de las API, los desarrolladores pueden establecer comunicación (interoperabilidad) entre programas y aplicaciones capaces de comunicarse con otras plataformas.

El principal ejemplo es la integración nativa y directa de la Plataforma uCloud con la consola de los proveedores de nubes públicas, todo ello mediante la interoperabilidad a través de la API de las consolas de los proveedores.

Otro ejemplo muy común de uso de la Plataforma uCloud es la emisión de facturas para los sistemas de showback y chargeback, así como el envío de información y alertas sobre los recursos gestionados.

Nuestros clientes (y/o integradores) pueden utilizar la documentación de la API de la Plataforma uCloud con sus plataformas internas para complementar o automatizar ciertas actividades o acciones que están más allá de las capacidades nativas de la Plataforma uCloud. Por ejemplo: *consultar y extraer de la Plataforma uCloud el coste de la factura de los objetos de valor de un proveedor de la nube pública a través de una aplicación financiera/contable para la emisión de facturas*.

La Plataforma uCloud dispone de documentación de su API, pero el acceso a la documentación completa debe solicitarse al Equipo de Atención al Cliente *(contato@usto.re)* para que se cree y envíe una credencial de acceso a la documentación de la Plataforma uCloud.

El Equipo de Ustore está preparado para ayudar y evaluar las demandas de interoperabilidad e integración entre la Plataforma uCloud y las plataformas que tienen y permiten el uso de APIs para la interoperabilidad.



Arquitectura de Referencia de la Plataforma uCloud
==================================================

A continuación presentamos una arquitectura de referencia para la Plataforma uCloud con sus componentes, proveedores e integraciones nativos.

.. figure:: /figuras/uCloud_future_vision-small.jpg
   :alt: Arquitectura de Referencia de la Plataforma uCloud
   :align: center

----

La Plataforma uCloud se comunica con la consola de los proveedores a través de la API Rest, por lo que cada acción realizada o configurada en las pantallas de uCloud envía acciones (tareas) al administrador (público y/o privado) del entorno de nube (consola) específico para que puedan realizar la acción deseada.

Ustore se compromete a mantener el constante desarrollo de sus Plataformas de Software y aplicar las mejores prácticas *(best practices)* de *DevOps* vigentes en el mercado de TI en la actualidad.

Nuestro compromiso es mantener la compatibilidad de integración, para que los últimos cambios e implementaciones en la consola de proveedores y todo el software que mantenemos mantengan la interoperabilidad, para que la nueva funcionalidad esté siempre disponible a través de la interfaz de la Plataforma uCloud.

Se utiliza un conjunto de prácticas y herramientas diseñadas para aumentar la capacidad de una organización para entregar aplicaciones y servicios más rápido que los procesos tradicionales de desarrollo de software.

Consulte la documentación específica acerca de roadmap de evolución de la plataforma uCloud o en el sitio web de Ustore (www.ustore.com.br).


Acceso a la plataforma uCloud
=============================

Dashboard
---------

Sección Contenedores
--------------------

Sección de Gráficos de uso de recursos
--------------------------------------

Sección Últimas Tareas
----------------------

Sección Máquinas Virtuales
--------------------------

Accesos directos de la sección a los menús principales
------------------------------------------------------

Solicitud de Nueva Contraseña
-----------------------------

Usuario no aprovisionado
------------------------

Menú de Usuario
===============

Menú de Administración
======================

Switch Roles
------------

Switch Roles - Escenario de Ejemplo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Escenario de Ejemplo *(AWS)*:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Escenario de Ejemplo *(AZURE y AWS)*:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Switch Roles - Utilizando
~~~~~~~~~~~~~~~~~~~~~~~~~

Menú Administración / Usuarios
------------------------------

Visualización de un Usuario
---------------------------

Creación de Usuario
-------------------

Administración / Grupos
-----------------------

Viendo Grupo
------------

Creando Grupo
-------------

Administración / Contrato
-------------------------

Gobernanza Financiera a través del Contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Aislamiento Financiero de Recursos Informáticos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Aislamiento Lógico de Recursos Computacionales
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Viendo Contrato
---------------

Sección General
---------------

Sección Reglas de Facturación
-----------------------------

Sección Categorías de Precio
----------------------------

Sección Políticas de Alertas
----------------------------

Sección Precio de los Recursos - Contrato
-----------------------------------------

Sección Cuota del Contrato
--------------------------

Sección Contacto Principal
--------------------------

Sección Administradores
-----------------------

Sección Datos de la Empresa
---------------------------

Sección Virtual Datacenters Otorgados
-------------------------------------

Sección Usuarios
----------------

Sección Grupos
--------------

Sección Datos de Facturación
----------------------------

Sección Perfiles de Permisos
----------------------------

Sección Productos
-----------------

Sección Permisos Concedidos
---------------------------

Sección Perfil de Facturación de Contenedores
---------------------------------------------

Aprovisionamiento de Contrato
-----------------------------


Menú Configuración / General
============================

Sección General
---------------

Sección Precio de los Recursos
------------------------------

Sección de Configuraciones de Usuarios del LDAP Server
------------------------------------------------------

Menú Configuración / Red
========================

Sección Configuración de Red
----------------------------

Sección Controlador SDN
-----------------------

Menú Configuración / Sub-redes Públicas
=======================================

Menú Configuración / Firmas
===========================

Creando Firma
-------------

Menú Configuración / Flavor Billing Profile
===========================================

Creando un Flavor Billing Profile
---------------------------------

Menú Configuración / Perfiles de Permisos
=========================================

Ver y Editar un Perfil de Permisos
----------------------------------

Creando un Perfil de Permisos
-----------------------------

Menú Configuración / Perfiles de Visualización
==============================================

Botón Crear Perfil de Vista
---------------------------

Editar Perfil de Vista
----------------------

Menú Configuración / Billing Admin
==================================

Información de Registro *(LOG)* de Billing Admin
------------------------------------------------

.. Etiqueta de Recursos USN
.. ------------------------

.. Creación de una Etiqueta de Recursos USN
.. ----------------------------------------

.. Una vez creado el perfil es posible editar
.. ------------------------------------------



Menú Máquinas Virtuales
=======================

  *1. **Gobernanza Financiera**

  *2. **Billing (Facturación de los Servicios)**

  *3. **Supervisión de la Infraestructura**

  *4. **Inventario (*Assessment*)**

La plataforma de uCloud se conecta ...

  *5. **Operación de la Infraestructura**

Con el inventario disponible ...

Menú Máquinas Virtuales
-----------------------

Administración de una Máquina Virtual
-------------------------------------

Sección General / Máquinas Virtuales
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sección de Rendimiento Instantáneo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sección Metrics (exclusivo AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sección Interfaces de Red
~~~~~~~~~~~~~~~~~~~~~~~~~

Sección Disco
~~~~~~~~~~~~~

Sección Snapshots
~~~~~~~~~~~~~~~~~

Sección Signatures *(Exclusivo Azure y Google Cloud Platform)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sección Historial de Rendimiento *(Azure y GCP)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creando una Máquina Virtual
---------------------------

Wizard Paso 1: *Selección de la Nube*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Paso 2: *Información básica de la máquina virtual - parte 1*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Paso 3: *Información básica de la máquina virtual - parte 2*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Paso 4a: *Informaciones de seguridad de la máquina virtual*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Paso 4b: *Información de seguridad -Exclusivo Azure*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Paso 5a: *User data*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Paso 5b: *User data VMware*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Paso 6: *Ver la configuración de la máquina virtual*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Monitoreo de Máquina Virtual
----------------------------

Performance
~~~~~~~~~~~


Menú Scaling Groups
===================

Creando un Scaling Group AWS
----------------------------

Problemas Conocidos con el Grupo de Escalabilidad AWS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creando un Scaling Group Azure
------------------------------

Menú Base de Datos
==================

Administración de una Base de Datos
-----------------------------------

Sección General / Grupo de Seguridad
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sección Grupos de Seguridad
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Aprovisionamiento de una Base de Datos
--------------------------------------

Creación de Bases de Datos *(MySQL & AWS)*
------------------------------------------

Paso 1: Selección del Proveedor de Servicios en la Nube *(AWS)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 2: Selección de la Base de Datos *(MySQL & AWS)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 3: Especificaciones de la Base de Datos *(MySQL & AWS)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 4: Configuraciones de acceso a la Base de Datos *(MySQL & AWS)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 5: Especificaciones de Red y Seguridad *(MySQL & AWS)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 6: Parámetro de Copia de Seguridad *(MySQL & AWS)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creación de Bases de Datos *(MySQL & Azure)*
--------------------------------------------

Paso 1: Selección del Proveedor de Servicios en la Nube *(Azure)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 2: Selección de la Base de Datos *(MySQL & Azure)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 3: Especificaciones de la Base de Datos *(MySQL & Azure)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 4: Configuraciones de acceso a la Base de Datos *(MySQL & Azure)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 5: Especificaciones de Red y Seguridad *(MySQL & Azure)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 6: Parámetro de Copia de Seguridad *(MySQL & Azure)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creación de Bases de Datos *(MySQL & GCP)*
------------------------------------------

Paso 1: Selección del Proveedor de Servicios en la Nube *(GCP)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 2: Selección de la Base de Datos *(MySQL & GCP)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 3: Especificaciones de la Base de Datos *(MySQL & GCP)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 4: Configuraciones de acceso a la Base de Datos *(MySQL & GCP)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 5: Especificaciones de Red y Seguridad *(MySQL & GCP)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Paso 6: Parámetro de Copia de Seguridad *(MySQL & GCP)*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Menú Virtual Datacenters
========================

Gestionando Virtual Datacenters
-------------------------------

Editando un Virtual Datacenter
------------------------------

Creando un Virtual Datacenter
-----------------------------

Menú Financiero
===============

Entorno Corporativo
-------------------

.. Entorno Gobierno Brasileño
.. --------------------------

Menú Financiero (Entorno Corporativo)
=====================================

Sección Mi Factura
------------------

Sección Factura Actual
~~~~~~~~~~~~~~~~~~~~~~

Sección Máquinas Virtuales
~~~~~~~~~~~~~~~~~~~~~~~~~~

Sección IP Pública
~~~~~~~~~~~~~~~~~~

Sección Equilibradores
~~~~~~~~~~~~~~~~~~~~~~

Sección Elementos No Administrados
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sección ‘X’ Contratos
---------------------

Sección de Factura del Contrato ‘xyz’
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Sección Grupos
~~~~~~~~~~~~~~

Factura de Grupo en el Contrato
-------------------------------

Facturación del Usuario
-----------------------

.. Menú Financiero (USN)
.. =====================

.. Entorno Gobierno Brasileño
.. --------------------------

.. Menú Financiero / USN Billing
.. -----------------------------

.. Menú Financiero / Informe Consolidado de Facturación
.. ----------------------------------------------------

.. Orden de Trabajo
.. ================

.. Administrar la Orden de Trabajo
.. -------------------------------

.. Sección General
.. ~~~~~~~~~~~~~~~

.. Sección Estimación de Costos (USN)
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. Configuración de Estimación de Costos (UST)
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. De Acuerdo
.. ~~~~~~~~~~

Menú Contenedores
=================

Gestión de un Contenedor
------------------------

Creando un Nuevo Contenedor
---------------------------

Menú Hosts
==========

Menú Red
========

Redes
-----

Agregar *Subred* en el entorno AWS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Agregar *Subred* al entorno de Azure
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Agregar *Subred* al entorno GCP
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Agregar *Subred* al entorno Privado (ejemplo: VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Crear Red en Proveedores de Servicios de Nube Pública
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Crear Red en Entorno Privado (On-Premises)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Crear Red en Proveedores de Servicios de Nube Pública (AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Crear Red en Proveedores de Servicios de Nube Pública (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Crear Red en Proveedores de Servicios de Nube Pública (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Crear Red en Entorno Privado (ejemplo: VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Menú IPs Públicos
=================

Solicitar una IP Pública (AWS y GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Solicitar una IP Pública (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Solicitar una IP Pública (entorno privado VMware vCenter)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Menú Grupos de Seguridad y ACLs
===============================

Administrar Grupo de Seguridad
------------------------------

Crear Grupo de Seguridad
------------------------

Menú Par de Claves
==================

Administrar un Par de Claves
----------------------------

Crear un Par de Claves
----------------------

Importando un Par de Claves
---------------------------

Menú Equilibradores
===================

Administrando Equilibrador
--------------------------

Creando Equilibrador (entornos AWS y GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creando Equilibrador (entorno Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Menú Zona DNS
=============

Administrar Zona DNS Pública (AWS y GCP)
----------------------------------------

Crear Zona DNS Pública (Azure)
------------------------------

Crear Zona DNS Privada (observación)
------------------------------------

Menú VPN
========

Crear la VPN en 3 pasos
-----------------------

Crear Customer Gateway
----------------------

Crear Private Gateway
---------------------

Crear Túnel VPN
---------------

Menú Storage
============

Visualización de un Storage
---------------------------

Menú Templates
==============

Menú Flavors
============

Visualización de un Flavor
--------------------------

Menú Workflows
==============

Workflows / Direct Execution
============================

Editando Workflows
------------------

Creando Workflow
----------------

Creando Tareas Asociadas
------------------------

Tarea de iniciar y detener máquinas virtuales
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tarea de crear imagen de disco (instantánea)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tarea de Script
~~~~~~~~~~~~~~~

Workflows / Cliente Server (Puppet*)
====================================

Workflows / Catálogo de Servicios
=================================

Comprando Oferta - Catálogo de Servicio
=======================================

Creando Oferta / Catálogo de Servicio
=====================================

Creación de oferta a través de Menús de la Plataforma uCloud
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Creación de oferta a través de la carga de Archivo JSON
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. Menú Workflows / Catálogo de Servicios
.. ======================================

Menú Trabajos
=============

Pestana Trabajos
----------------

Pestana Aprobaciones Pendientes
-------------------------------

Pestana Trabajos Programados
----------------------------

Menú Inventário de Recursos
===========================

Editor de Etiquetas *(tags)* Nativo
-----------------------------------

Conclusión
----------










































 

