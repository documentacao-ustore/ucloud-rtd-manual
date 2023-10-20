.. image:: /figuras/fig_dci/014_dci_logomarca.png 
    :alt: logo dci 
    :scale: 80 % 
    :align: center 
======

.. centered:: Português_     -     Español     -     English_


.. _Português: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/dci-manual.html


.. _English: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/MEnglish/dci.eng.html

====

DCI - Manual de Funcionalidades  
===============================


Soluciones en tecnología de la información que posibilitan implementar una arquitectura computacional escalable, sólida y confiable en nube híbrida.


====


Introducción
----------

Este documento consiste en un manual con una breve descripción de las principales funcionalidades contenidas en el producto **Data Center Interconnect – DCI** de la plataforma uCloud.

----

Presentación
-------------

**Data Center Interconnect - DCI** es una solución de conectividad cuya red es definida por *software*.

La red definida por *software* (SDN) es una arquitectura que permite una gestión y un control más eficientes de los recursos de red, delimitando el plan de control del plan de datos.

En términos sencillos, la comunicación entre *datacenters* significa que las funciones de control y datos de la red están separadas, lo que permite una mayor flexibilidad y automatización en la gestión de la red.

----

Cómo conectarse al DCI
-------------------------

Para acceder a la plataforma es necesario haber realizado una “Primera compra” en el Panel del Cliente.

Tras esta compra, el usuario recibe sus credenciales de acceso, enviadas directamente a su correo electrónico registrado.

.. image:: /figuras/fig_dci_spa/001_acceso_DCI.png
    :alt: acceso
    :scale: 100 %
    :align: center
======

El usuario debe rellenar los campos ``Usuario`` y ``Contraseña`` con las credenciales recibidas del administrador de la plataforma. 

Pulsar el botón ``Entrar``.

Tras este procedimiento, la pantalla de inicio del Portal es presentada.

----

Visión General
---------------

Al principio, es importante comprender el impacto de algunas herramientas que aparecen en el menú superior derecho, que se muestra al usuario tras iniciar la sesión en el DCI.

La siguiente imagen es un fragmento del menú superior derecho, presentado en todas las pantallas disponibles para el usuario. Este menú muestra componentes relevantes como nombre, correo electrónico, configuraciones de cuenta, manual de funcionalidades y salir, cada uno descrito en detalle a continuación.


  * Nombre; 
  * Correo electrónico;
  * Configuraciones de Cuenta;
  * Manual de Funcionalidades;
  * Salir.


.. image:: /figuras/fig_dci_spa/002_vision_general_configuraciones.png
    :alt: visión general
    :align: center
======

**Icono de notificación** |icone_tarefas|   : Este icono es un punto importante para visualizar todas las actividades realizadas en el portal. Mediante este icono se pueden observar las acciones más recientes, reflejadas en forma de notificación en la pantalla "Tareas".

**Nombre**: Muestra el nombre del usuario conectado y su dirección de correo electrónico.
  
**Configuraciones de Cuenta**: Esta opción permite acceder a los detalles de la cuenta creada, donde se puede modificar la dirección de correo electrónico, el número de teléfono de contacto y gestionar los usuarios de su contrato. Este botón conduce al menú **Administración**.

**Manual de Funcionalidades**: Direcciona el usuario para el documento "Manual de Funcionalidades" almacenado en el ambiente de documentación online de Ustore Brasil.

**Salir**: Salir o cerrar la sesión de la aplicación.

----

Menú **Administración**
---------------------------

Para tener una visión completa de los servicios de DCI, existen algunos menús en la parte lateral izquierda de la plataforma, donde se puede encontrar informaciones valiosas de los productos.

Al acceder a este menú de Administración, es posible al usuario hacer uso de los submenús:

  * Usuarios;
  * Grupos;
  * Contratos.

.. image:: /figuras/fig_dci_spa/003_menu_administracion.png
    :alt: Menú Administración
    :scale: 80 % 
    :align: center
======


Menú **DCI**
------------

Este menú contiene tres submenús que posibilitan visualizar:

  * Puertos;
  * Circuitos;
  * Excursiones. 

A continuación, se detallan cada uno de estos submenús.


.. image:: /figuras/fig_dci_spa/004_menu_DCI.png
    :alt: Menú DCI
    :scale: 80 % 
    :align: center
======

Submenú Puertos
~~~~~~~~~~~~

Este submenú permite visualizar los recursos de los puertos, así como las acciones disponibles como mostrar recursos deshabilitados al listar, buscar información, actualizar la pantalla tras una modificación y seis columnas que categorizan cada uno de los puertos. 

Los puertos están conectados a través de Circuitos, éstos pueden o no tener circuitos, todos los puertos están dentro del *Datacenter*, cuando se adquiere el puerto, el cliente recibe la LOA (carta de autorización) necesaria para el flujo del proceso.


.. image:: /figuras/fig_dci_spa/005_submenu_puertos.png
    :alt: Submenú Puertos 
    :align: center
======

Se presentan tres funcionalidades:

  * El botón para ``Mostrar recursos deshabilitados``: Al pulsar este botón el usuario puede visualizar los recursos que están deshabilitados;
  * La acción de ``Buscar``: señalada por la lupa que indica al usuario la posibilidad de búsqueda;
  * El botón para actualizar la página cuando se hace clic en ``Actualizar``.

Las informaciones de los puertos se dividen en seis columnas y se presentan como se indica a continuación:

  * Designación;
  * *Status*;
  * Banda;
  * Tipo;
  * *Datacenter*;
  * *Golden Jumper*.

Al seleccionar un puerto, es posible visualizar todos los detalles por completo. La cabecera de esta nueva página muestra algunas opciones, que se activan mediante los botones ``Volver``, ``Descargar LOA``, ``Reenviar LOA`` y ``Confirmado``, en el cuerpo de la pantalla están distribuidos los *cards* que se describen a continuación.

.. image:: /figuras/fig_dci_spa/006_puertos_detalles.png
    :alt: Submenú puertos detalles 
    :align: center
======

El submenú Puertos exhibe tres *cards* que categorizan relevantes informaciones: 


  * General;
  * Vlans;
  * Historial.


----

*Card* General
""""""""""""

Este *card* se encuentra en el submenú Puertos, menú DCI. Muestra las principales informaciones de este puerto.


.. image:: /figuras/fig_dci_spa/007_puertos_card_general.png
    :alt: Puertos card General 
    :align: center
======

Una vez completados los catorce elementos que se enumeran a continuación, éstos deben mostrar un panorama general al usuario, incluyendo la fecha de creación y la asignación de este puerto, como se muestra en el ejemplo de arriba:

  * Usuario;
  * Nombre de la organización;
  * Número de identificación;
  * Designación;
  * Banda;
  * Enrutador;
  * Enrutador Puerto;
  * Posición DGO;
  * *Status*;
  * Datacenter;
  * Ciudad;
  * Tipo de puerto;
  * Fecha de creación;
  * Fecha de asignación.

----

*Card* Vlans
""""""""""""

El segundo *card* presentado en este submenú Puertos, situado a la derecha de la pantalla, contiene, además de las informaciones, un botón verde de acción.


.. image:: /figuras/fig_dci_spa/008_puertos_card_vlans.png
    :alt: Puertos card Vlans 
    :align: center
======

El *card* Vlans exhibe en la parte superior derecha una funcionalidad de actualización de la página que puede activarse a través del botón ``Actualizar``; a continuación, las informaciones se dividen en cuatro columnas:


  * Vlans en uso;
  * Circuito;
  * Banda;
  * Banda Base.

Las informaciones sobre Vlans se presentan en bloques de 10, 25, 50 o 100 líneas.

----

Submenú Circuitos
~~~~~~~~~~~~~~~~~~

Esta pantalla permite visualizar la lista de Circuitos, haciendo posible observar las acciones que deben realizarse con cada ítem, distribuidos en los botones y columnas.

.. image:: /figuras/fig_dci_spa/009_submenu_circuitos.png
    :alt: Submenú Circuitos 
    :align: center
======

En esta pantalla, inicialmente se pueden ver las acciones proporcionadas por la aplicación, como mostrar recursos deshabilitados, la búsqueda de informaciones, la actualización de la pantalla después de realizar un cambio y ocho columnas que categorizan las informaciones sobre cada uno de los circuitos.

Se presentan tres funcionalidades:
  
  * Botón ``Mostrar recursos deshabilitados``: Pulsando este botón, el usuario puede visualizar los recursos que están deshabilitados;
  * La acción de ``Buscar``: el signo de la lupa indica al usuario la acción de buscar algo;
  * Botón ``Actualizar``: indica que al pulsar este botón la página es actualizada.

De esta manera, la pantalla de circuitos presenta las ocho columnas informativas por separado, que se enumeran a continuación:

  * Designación;
  * Tipo;
  * Banda Base;
  * Banda Actual;
  * *Puerto - ID de Vlan*;
  * *Puerto - ID de Vlan*;
  * *Status*;
  * *Golden Jumper*.

Haciendo clic en cada circuito individualmente, es posible visualizar los detalles de las informaciones, empezando por el botón con la acción de ``Volver``, el *card* General, el *card* Configuraciones, el *card* Excursiones y, por último, el *card* Historial.

.. image:: /figuras/fig_dci_spa/010_detalles_circuito.png
    :alt: Detalles Circuito 
    :align: center
======

En este desglose del circuito listado, el usuario visualiza cuatro *cards* que categorizan informaciones distintas:

  * General;
  * Configuraciones;
  * Excursiones;
  * Historial.

----

*Card* General
""""""""""""

Este *card* está contenido en el submenú Circuito y presenta las principales informaciones del mismo.

.. image:: /figuras/fig_dci_spa/011_card_general_submenu_circuitos.png
    :alt: circuito card general
    :align: center


======

Compuesto por ocho elementos, como se muestra en el ejemplo de arriba, reflejan el panorama general del circuito al usuario, incluyendo los puertos que se conectan a través del circuito, que se enumeran a continuación:

  * Usuario;
  * Nombre de la organización;
  * Número de identificación;
  * Designación;
  * Fecha de creación;
  * Fecha de activación;
  * Puerto origen;
  * Puerto destino.

----

*Card* Configuraciones
""""""""""""""""""""

El segundo *card* del submenú Circuito muestra las principales informaciones acerca de éste.


.. image:: /figuras/fig_dci_spa/012_card_configuraciones_submenu_circuito.png
    :alt: circuito card configuraciones
    :align: center
======

El *card* Configuraciones ofrece en su parte superior derecha la funcionalidad de actualizar la página, que puede ser activada mediante el botón ``Actualizar``. Este *card* ofrece algunas informaciones como:


  * Status: “Activado”, seguido del botón ``Bloquear``;
  * Motivo de bloqueo:
         * Tipo y el botón ``Cambiar tipo``;
         * Banda actual;
         * Banda base;
         * Vlan Puerto Origen y a continuación el botón ``Cambiar Vlans``;
         * Vlan Puerto Destino.

----

*Card* Excursiones
"""""""""""""""""""""""

El tercer *card* del submenú Circuito muestra las principales informaciones sobre éste.


.. image:: /figuras/fig_dci_spa/013_card_excursiones_submenu_circuito.png
    :alt: circuito card excursiones
    :align: center
======

Al visualizar el *card* de Excursiones, se puede utilizar los dos botones situados a la derecha: ``+Crear Excursión`` y ``Actualizar``. Este *card* exhibe siete columnas que contienen informaciones tales como: 

* Banda;
* Fecha de inicio estimada;
* Fecha final estimada
* Fecha de inicio;
* Fecha final;
* Status;
* Acción.


----

*Card* Historial
""""""""""""""""

El último *card* del submenú Circuito muestra las siguientes informaciones sobre el historial de acciones realizadas:

.. image:: /figuras/fig_dci_spa/014_card_historial_submenu_circuito.png
    :alt: Circuito card historial
    :align: center
======

  * Operación;
  * Autor;
  * Fecha/Hora;
  * Status.

Al final, se muestra un bloque con la opción de seleccionar las informaciones en bloques de 10, 25, 50 o 100 líneas.

----

Submenú Excursiones
~~~~~~~~~~~~~~~~~~~~~~~~

*Card* General
""""""""""""

Este submenú posibilita la visualización de las Excursiones: finalizadas, interrumpidas, pendientes, programadas o activadas del usuario. 

Además del *status* de la excursión, es posible verificar la cantidad de banda a ampliar en el circuito y la banda base del mismo, con las fechas estimadas de inicio y fin y las fechas en las que la excursión efectivamente se realizó o finalizó. Los puertos y sus Vlans también están disponibles para visualización.

En esta pantalla se muestran las opciones para dos funcionalidades:

  * Botón ``Actualizar``: al hacer clic en este botón la página es actualizada;
  * Botón de acción ``+ Crear Excursión``: el signo de suma indica al usuario que haciendo clic es posible crear algo.

.. image:: /figuras/fig_dci_spa/015_excursiones_general.png
    :alt: excursiones
    :align: center
======

Para programar una excursión, es necesario hacer clic en el botón ``+ Crear Excursión`` y rellenar los campos en el modal presentado.

.. image:: /figuras/fig_dci_spa/016_crear_excursión.png
    :alt: crear excursión
    :align: center
======

Al visualizar este nuevo modal para crear excursiones, el usuario puede ver los siguientes espacios:
 
  * Fecha de inicio;
  * Fecha final;
  * Circuito.

En el área "fecha de inicio", el usuario selecciona la fecha deseada para programar el inicio de esta excursión y la fecha deseada para su finalización. Además de informar en el espacio siguiente sobre qué circuito se debe realizar la excursión. 

Una vez introducidos estos datos, se muestra al usuario la capacidad base del circuito seleccionado, así como la capacidad máxima posible para ese circuito y el campo "Banda", que permite seleccionar la banda estimada, tal y como se muestra en la siguiente imagen:

.. image:: /figuras/fig_dci_spa/017_crear_excursión_detalles.png
    :alt: crear excursión detalles
    :align: center
======

Cuando el usuario haya terminado de introducir los datos necesarios, puede hacer clic en el botón ``Crear Excursión`` y pasar a la siguiente etapa de este flujo.

.. note:: El botón ``Cancelar`` puede activarse en cualquier momento en caso de necesidad para anular la creación.

Una vez creada la excursión, la operación está completa. Ésta permite al usuario verificarla en el submenú "Excursión" con todas sus informaciones, junto con la opción de cancelar dicha excursión.

----

Menu **Tareas**
----------------

En la pestaña de tareas es posible monitorizar todas las operaciones realizadas dentro de la plataforma.

----

Panel de Tareas
~~~~~~~~~~~~~

Como ya se ha mencionado, la pantalla de tareas es importante para supervisar el progreso de los pedidos realizados en la plataforma.

.. image:: /figuras/fig_dci_spa/018_pantalla_tareas.png
    :alt: Pantallas Tareas 
    :align: center
======

Este menú posibilita visualizar cualquier caso de error, el seguimiento del *status* de los pedidos y cancelar algunas operaciones.


.. image:: /figuras/fig_dci_spa/019_cabecera_tareas.png
    :alt: Cabecera Tareas 
    :align: center
======

La pantalla de arriba presenta en la parte superior derecha el símbolo de tareas, el nombre del usuario conectado y, a continuación, las funcionalidades:

  * Botón ``Buscar``: Campo que facilita encontrar las informaciones rápidamente. 
  * Botón ``Actualizar``: Permite actualizar la página con un solo clic. 

Las tareas son presentadas en formato de lista, categorizadas en pestañas que contienen las informaciones sobre:

       * Tareas;
       * Tareas pendientes;
       * Tareas programadas.


.. image:: /figuras/fig_dci_spa/020_tareas_detalles.png
    :alt: Tareas detalles 
    :align: center
======

La pestaña "Tareas" presenta once tipos de informaciones divididas en columnas:

  * Operación; 
  * Solicitar ID;
  * Designación;
  * Razón social;
  * Autor;
  * *Error*;
  * Progreso;
  * Fecha de inicio;
  * Duración;
  * *Status*;
  * Acción.

Detallando la columna *status* que muestra tres estados distintos:

 * Son: ``Éxito``, ``Fallado`` o ``Aprobado``.

El objetivo de este estado es orientar la acción de seguimiento, de acuerdo con lo siguiente:

**Status de Éxito** - mostrado en color verde, significa que la operación se ha completado con éxito.
 
**Status de Fallado** - mostrado en rojo, significa que se ha producido algún problema durante la operación. En la propia tarea que falló, se puede observar el motivo de la incorrección en la columna "Error".

**Status de Aprobado** - mostrado en color verde, significa que la operación se ha realizado correctamente. Sin embargo, depende de alguna acción del usuario, ya sea "admin" o "user":

    * Para casos como "Primera Venta", queda pendiente al usuario la confirmación del *Golden Jumper* de ambos puertos.

    * Para casos de ventas subsiguientes de puertos, queda pendiente el *Golden Jumper* del puerto en cuestión.

====

Conclusión
---------

Este documento presenta la descripción de las funcionalidades contenidas en el producto **Data Center Interconnect – DCI**, desarrollado por Ustore.

====

**Equipo Ustore**

DCI Manual de Funcionalidades - v.5 - Actualización 28/09/2023 - Revisión 03/08/2023 - Creado el 08/02/2023.

.. |icone_tarefas| image:: /figuras/ucloud_icone_sino.png