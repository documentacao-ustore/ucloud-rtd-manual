.. image:: /figuras/index/_ustore_pequena.png
    :alt: logo ustore
    :align: center
======


DCI - Manual de Funcionalidades  
===============================


Soluciones en tecnología de la información que posibilitan implementar una arquitectura computacional escalable, sólida y confiable en nube híbrida.

====


Introducción
------------


Este documento consiste en un manual con una breve descripción de las principales funcionalidades contenidas en el producto **Data Center Interconnect** - DCI de la plataforma Ustore.


----


Cómo conectarse al DCI
----------------------


Para acceder a la plataforma es necesario haber realizado una primera compra en el Panel del Cliente.


Tras esta compra, el usuario recibe sus credenciales de acceso, enviadas directamente a su correo electrónico registrado.



.. image:: /figuras/fig_dci/01_log_in.png
    :alt: login
    :align: center
======


El usuario debe rellenar los campos ``login`` y ``contraseña`` con las credenciales recibidas del administrador de la plataforma.


Haga clic en el botón ``Entrar``.


Tras este procedimiento, la pantalla de inicio del Portal es presentada.


----


Visión General
--------------


Al principio, es importante comprender el impacto de algunas herramientas que aparecen en el menú superior derecho.
  

Así, el recorte del menú superior que se muestra en la siguiente imagen presenta componentes relevantes, que se describen detalladamente a continuación.



.. image:: /figuras/fig_dci/02_qa_config_logout.png
    :alt: visão geral
    :align: center
======


 
**Icono de notificaciones**  |icone_tarefas|: Este icono es un punto relevante para la visualización de todas las actividades que se realizan en el Portal. A través de él, es posible observar las acciones más recientes, reflejando en forma de notificación la pantalla de Tareas.
  
**Configuración de la cuenta**: Permite acceder a los detalles de la cuenta creada, donde se puede cambiar el correo electrónico, teléfono de contacto y gestionar los usuarios en su Contrato. Este botón lleva al menú **Administración**.

----


Menú Administración
-------------------


Para tener una visión completa de los servicios de DCI existen algunos menús en la parte lateral de la plataforma, donde se puede encontrar informaciónes valiosas de los productos.
  


.. image:: /figuras/fig_dci/03_menu_adm.png
    :alt: menu administração 
    :align: center
======



**Menú DCI**
~~~~~~~~~~~


Este menú contiene submenús que permiten visualizar Puertos, Circuitos y Excursiones.

 
Submenú Puertos
~~~~~~~~~~~~~~~


En esta pantalla es posible visualizar sus recursos de puertos, así como las acciones que deben llevarse a cabo con cada ítem.


.. image:: /figuras/fig_dci/05_menu_portas.png
    :alt: Menu Portas 
    :align: center
======



Tres funcionalidades son presentadas: el botón para ``Exhibir recursos deshabilitados``, la acción de ``Buscar`` y la acción para actualizar la página ``Refresh``.


Las informaciones de los puertos se dividen en seis columnas y se presentan como se indica a continuación:


  * Designación
  * *Status*
  * Banda
  * Tipo
  * *Data Center*
  * *Golden Jumper*


Al seleccionar un puerto, es posible visualizar los detalles por completo. La nueva página presenta tres funcionalidades para ``Descargar LOA``, ``Reenviar LOA`` y el botón de ``Confirmado``.


.. image:: /figuras/fig_dci/06_menu_porta_bre.png
    :alt: Menu porta bre 
    :align: center
======


Además, se presentan también dos *cards* de informaciones: General y Vlans.


En el *card* de Vlans, la funcionalidad de actualización de página ``Refresh`` es presentada, y las informaciones se dividen en cuatro columnas:


  * Vlans en Uso
  * Circuito
  * Banda
  * Banda Base


Las informaciones sobre Vlans se muestran en bloques de 10, 25, 50 o 100.



Submenú Circuitos
~~~~~~~~~~~~~~~~~


Esta pantalla permite visualizar sus recursos de circuito, posibilitando observar las acciones que se deben efectuar con cada ítem.



.. image:: /figuras/fig_dci/07_menu_circuitos.png
    :alt: Menu Circuitos 
    :align: center
======



Tres funcionalidades son presentadas: el botón para ``Exhibir recursos deshabilitados``, la acción de ``Buscar`` y la de actualización de la página ``Refresh``.


Las informaciones de los circuitos se separan en ocho columnas y se presentan como se indica a continuación:


  * Designación
  * Tipo
  * Banda Base
  * Banda Actual
  * *Port - Vlan ID*
  * *Port - Vlan ID*
  * *Status*
  * *Golden Jumper*


Haciendo clic en cada circuito individualmente, es posible visualizar las informaciones del historial de acciones realizadas y su historial de excursiones en ese circuito, divididos en *cards* como se muestra en la imagen de abajo.


.. image:: /figuras/fig_dci/08_menu_circuito_04.png
    :alt: Menu Circuitos 
    :align: center
======


Además, es posible realizar algunas operaciones dentro del circuito, como por ejemplo, el cambio de VLAN o la modificación de tipo. 


----


Menú Tareas
-----------


En la pestaña de tareas es posible monitorizar todas las operaciones realizadas dentro de la plataforma.


Panel de Tareas
~~~~~~~~~~~~~~~

Como ya se ha mencionado, la pantalla de tareas es importante para supervisar el progreso de los pedidos realizados en la plataforma.


.. image:: /figuras/fig_dci/04_menu_tarefas.png
    :alt: Menu Tarefas 
    :align: center
======


Este menú posibilita visualizar cualquier caso de error, el seguimiento del *status* de los pedidos y cancelar algunas operaciones.


.. image:: /figuras/fig_dci/04_head_tarefas.png
    :alt: Cabeçalho Tarefas 
    :align: center
======


La pantalla de arriba presenta en la parte superior derecha el símbolo de tareas, el nombre del usuario conectado y, a continuación, las funcionalidades:


  * ``Búsqueda`` Campo de búsqueda que facilita encontrar informaciones rápidamente.
  * ``Refresh`` Campo que permite actualizar la página con un solo clic. 

Las tareas son presentadas en formato de lista, categorizadas en pestañas que contienen las informaciones sobre:


     * Tareas
     * Aprobaciones Pendientes
     * Tareas Programadas.


 .. image:: /figuras/fig_dci/04_lista_tarefas.png
    :alt: Lista de tarefas 
    :align: center
======


La pestaña "Tareas" presenta once tipos de informaciones divididas en columnas:


  * Operación
  * ID de pedido
  * Designación
  * Denominación social
  * Autor
  * *Error*
  * Progreso en porcentaje
  * Fecha de inicio
  * Duración
  * Estado
  * Acción


Detallando la columna *status* que muestra tres estados distintos:


  * Son: ``Éxito``, ``Fallo`` o ``Aprobado``.


El objetivo de este estado es orientar la acción de seguimiento, de acuerdo con lo siguiente:


**Status de Éxito** - mostrado en color verde significa que la operación se ha completado con éxito.
 
  
**Status de Fallo** - mostrado en color rojo significa que se ha producido algún problema durante la operación. En la propia tarea que falló, se puede observar el motivo de la incorrección en la columna "Error".

  
**Status de Aprobado** - mostrado en color verde significa que la operación se ha realizado correctamente. Sin embargo, depende de alguna acción del usuario, ya sea "admin" o "user":


     * Para casos como "Primera Venta", queda pendiente al usuario la confirmación del *Golden Jumper* de ambos puertos.


    * Para casos de ventas subsiguientes de puertos, queda pendiente el *Golden Jumper* del puerto en cuestión.


====


Conclusión
----------

Este documento presenta una breve descripción de las funcionalidades contenidas en el producto **Data Center Interconnect** - DCI, desarrollado por Ustore.


====


DCI Manual de Funcionalidades - Revisión y traducción: 03/03/2023.


.. |icone_tarefas| image:: /figuras/ucloud_icone_sino.png