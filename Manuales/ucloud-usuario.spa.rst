

.. image:: /figuras/ucloud.png
   :alt: logo ucloud
   :align: center

----

.. centered:: Português_     -     Español     -     English_

.. _Português: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/usr-manual.html

.. _English: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/MEnglish/ucloud-user.eng.html 

====

Manual del usuario
++++++++++++++++++


Soluciones de tecnologías de la información que permiten implementar una arquitectura de cómputo escalable, sólida y confiable en una nube distribuida.

====


Presentación
============

Este documento tiene como objetivo explicar el uso de la plataforma *uCloud*, una plataforma de *Cloud Service Broker* (broker de servicios en nube) que permite administrar múltiples proveedores de servicios de nube, tanto privados como proveedores de nube pública. 

En este manual se presentan los conceptos, las pantallas, las funcionalidades y los comandos de uso de este producto.

====

Introducción
============

Las organizaciones empresariales han incorporado la nube como solución para administrar sus ambientes virtuales y adoptan una combinación de nubes privadas y públicas, el gran desafío actual es la gestión de estos ambientes híbridos de múltiples nubes *(hybrid multi-cloud)* con el fin de lograr una visión unificada, así como obtener un control centralizado de los costos financieros, ya que cada organización empresarial tiene una necesidad y se enfrenta a diferentes desafíos.

La plataforma uCloud ha sido desarrollada para estos escenarios, independientemente de cuantos proveedores (públicos y/o privados) existan, el usuario podrá interactuar con sus plataformas:

   * Infraestructura como Servicio *(Infrastructure as a Service - IaaS)*;
   * Plataforma como Servicio *(Platform as a Service - PaaS)*.

Como se mencionó anteriormente, uCloud está posicionado como una plataforma de *Cloud Service Broker - CSB* *(Broker de servicios en la nube)* que permite administrar múltiples proveedores de servicios en la nube, tanto privados como proveedores de nube pública.

Una plataforma *CSB* como la plataforma uCloud permite a las organizaciones actuar en cinco puntos fundamentales para la gestión de ambientes híbridos multi-nube, son:

====


Gobernanza Financiera
---------------------

Además del control de la infraestructura, la plataforma uCloud permite a las empresas usuarias establecer límites, tanto financieros como cuantitativos de recursos (cuotas). Estos límites financieros o de infraestructura pueden aplicarse en tres niveles:

  * Para un proveedor público en general (ver el elemento Contratos, en el menú Administración);
  * Para un grupo de usuarios (ver el elemento Grupos en el menú Administración);
  * Para un usuario/individuo (ver el elemento Usuarios, en el menú Administración).

De esta forma, la organización aplica criterios de gobernanza financiera y control de gastos, como también puede acompañar los costos de su ambiente híbrido de multi-nube a través de una única interfaz.  

La adopción de la aplicación de límites (cuotas) financieros y/o recursos computacionales en diversos niveles alcanza el nivel de usuario. Así el control de costos es efectivo y permite evitar que el presupuesto de la organización sorprenda en situaciones que el gasto de la infraestructura computacional sea exorbitante o por encima de los valores preestablecidos.

Otro aspecto de la plataforma uCloud es la reducción de costos de certificación y capacitación de los especialistas, en cada una de las interfaces de cada proveedor (público y/o privado), ya que el empleo de una interfaz de uso y gestión única y sencilla permite extraer más productividad del ambiente del proveedor de la nube. 

Incluso si el usuario no cuenta con capacitación o certificación en la consola específica del proveedor (pública y/o privada), la plataforma uCloud permite al usuario aprovisionar un recurso computacional en el entorno deseado de manera sencilla y fácil.

====


Billing (Facturación de los Servicios)
--------------------------------------

La plataforma uCloud proporciona a las organizaciones empresariales información sobre los costos recurrentes relacionados con el uso de los recursos computacionales en la(s) operación(es) en un ambiente multinube híbrido. Este es solo uno de los puntos que forma parte de la práctica de *Cloud Financial Management - FinOps* (Gestión financiera de la nube).

Es importante resaltar que, individualmente, la plataforma uCloud no atiende a los tres pilares de la práctica completa *FinOps*. Ustore posee otros productos que pueden ser complementarios y el conjunto de productos tiene potencial para actuar como un ambiente capaz de englobar y atender la práctica de *FinOps*.

El requisito soportado por uCloud es el punto de *Información* *(Inform)*, los otros puntos de esta mejor práctica de *FinOps*: la *Optimización* y la *Operación* pertenecen a los otros productos de la cartera de Ustore que complementa la plataforma uCloud.

Se debe aclarar que la plataforma uCloud no crea ni genera valores de recursos computacionales, estos montos se generan en los proveedores de nube pública, la aplicación uCloud *extrae* *(descarga)* el archivo de *Billing* *(facturación)* de estos proveedores. 

Despues añade esta información en sus bases de datos internas para que, posteriormente, de acuerdo con los criterios comerciales del contrato puedan ser aplicados y estos costos calculados y convertidos para la moneda corriente en Brasil.

De esta forma, el usuario permanece *informado* de la evolución de los valores y puede acompañar si estos costos se encuentran dentro de los criterios de la gobernanza financiera de la organización.

Generalmente estos costos se presentan en archivos de texto no estructurados *(Comma-separated Values - CSV)* generados cada período (promedio de 8 horas) y la plataforma uCloud agrega la información de este archivo *CSV* a su base de datos interna para agilizar y simplificar la presentación de estos valores en la pantalla del usuario.

Exclusivamente, los usuarios con un perfil específico pueden `visualizar costos` y permanecer informados de los valores de consumo de sus recursos computacionales totales en cada proveedor de la nube (pública y/o privada). Esto permite que el usuario pueda realizar un seguimiento de los costos acumulados de los recursos informáticos activos en los proveedores de servicios en la nube.

====


Monitoreo de la Infraestructura
-------------------------------

Una funcionalidad importante de la plataforma uCloud es la reciente implementación del módulo de gestión de eventos (monitoreo) que permite recopilar acontecimientos y alarmas que se han generado en los ambientes híbridos de nube (público y/o privado), activar notificaciones y crear informes personalizados.

Todas estas facilidades reducen los costos para las organizaciones, una vez que elimina la necesidad de contratación de servicios de monitoreo de los proveedores, pues tal servicio puede representar altos costos los cuales pueden impactar de forma negativa en el presupuesto (sobrepasar el límite) destinado a infraestructura de nube pública.

Esta funcionalidad permite integrar a un entorno de gestión de Service Desk para control *IT Service Management* (gestión de servicios de TI).

====

Inventario (*Assessment*)
-------------------------

La plataforma de uCloud se conecta a los proveedores de la nube mediante el registro de credenciales de acceso específicas de cada fornecedor de servicios en la nube (público y/o privado). Para ello, las empresas deben proporcionar credenciales de modo *operativo*.

Esta credencial operativa es proporcionada por el administrador del servicio en la nube y son autorizaciones que se generan en las cuentas de los proveedores que solo tienen permiso para interactuar con la consola del proveedor público en la nube a través de una API, no son calificaciones normales con información estándar de inicio de sesión y contraseña. De esta forma, la seguridad y las normas de regulación de seguridad de la información están previstas y atendidas en su totalidad.

Como las credenciales *operativas* se configuran en la plataforma de uCloud, la primera actividad es sincronizar la configuración y el inventario de recursos informáticos existentes en el proveedor (máquinas virtuales - cargas de trabajo). Esta lista de máquinas virtuales se extrae y se agrega a las bases de datos de uCloud para que la presentación en la pantalla del usuario sea rápida.

Con este inventario disponible directamente dentro de la plataforma de uCloud, el usuario puede operar cada una de las máquinas virtuales, independientemente de cuál sea el proveedor de la nube que esta función está aprovisionada. Vea a continuación las posibles operaciones a aplicar a los recursos computacionales existentes en los proveedores de nube (público y/o privado).

Es importante mencionar que el uCloud no tiene recursos computacionales, estos recursos existen en las nubes de los proveedores de servicios de nube pública o en los entornos de virtualización *(hypervisors)* instalados en su Datacenter privado. A través de la API Rest, la plataforma uCloud, envía acciones (tareas) al administrador de ambiente de nube específico (público y/o privado) para que realicen la acción deseada.

El usuario puede seguir el resultado de cualquiera de las acciones de operación en los recursos computacionales de forma casi inmediata, vale recordar que no es la plataforma uCloud la que *ejecuta* las acciones, sino el entorno donde la máquina virtual existe (ya sea público y/o privado). Este es el encargado de ejecutar la tarea enviada a través de la *API Rest*.

Si el resultado no se refleja en la interfaz de la pantalla del usuario, la consola de destino puede tardar un cierto tiempo en realizar esta tarea y solo después de que finalice la ejecución de ella, se mostra el resultado en la interfaz de uCloud.

Existe una opción de menú donde el usuario puede seguir el porcentaje de progreso de estas tareas, su resultado de éxito o el mensaje de error referente a alguna restricción del ambiente destino.

Es importante resaltar que pueden existir restricciones aplicadas al usuario aprovisionado en la plataforma uCloud, porque ello puede haber agotado el límite de su cuota financiera o de recursos computacionales, de esta forma la plataforma uCloud genera un aviso de error: **"límite de cuota excedido"** por ejemplo. Estos escenarios se describen en el menú Tareas.

====


Operación de la Infraestructura
-------------------------------

El término **operar** neste contexto puede ser visto como la capacidade del usuario comandar directamente en estas máquinas virtuales acciones de:

 * Parar (*shutdown*);
 * Reiniciar (*restart*); 
 * Suspender (*suspend*);
 * Remover (*delete*).

A través de la interfaz de la plataforma uCloud, el usuario puede enviar comandos a las consolas de cada proveedor de la nube, además de las acciones mencionadas anteriormente. También es possible ver la información de la configuración específica de la máquina virtual, así como cambiar o agregar algunas características adicionales a esta (por ejemplo: tarjeta de red, disco, grupo de seguridad, snapshot, entre otros).

En cuanto a los proveedores de servicios de nube pública, la aplicación uCloud está preparada para conectarse con las siguientes plataformas de nube pública:

  * Amazon Web Services (**AWS**);
  * Google Cloud Plataform (**GCP**);
  * Microsoft **Azure**;
  * **IBM** Cloud;
  * **Huawei** Cloud;
  * **Oracle** Cloud Infrastructure.

Actualmente, la plataforma uCloud está lista para conectarse con las siguientes plataformas *(hypervisors)* de administración de entornos de nube privada:

  * **VMware** *(vCenter Versões 5.0, 5.1, 5.5, 6.0, 6.5, 6.7, 7.x ou superior)*;
  * **vCloud**;
  * **Hyper-v** *(Windows 2008R2, Windows 2012, Windows 2012R2 e Windows 2016 ou superior)*;
  * **Openstack**;
  * **Xen Server**;
  * **XCP-NG**;
  * **KVM**.

La plataforma uCloud, además de las funciones CSB *(Cloud Service Broker)*, también es un agregador 
de funcionalidades que permite a los usuarios, de forma sencilla y centralizada, controlar varias consolas de administrador de ambientes virtualizados *(hypervisors)* desde el local privado *on-premises*, o desde el proveedor de nube pública. 

Agrega monitoreo, flujo de trabajo en la nube *(Cloud Workflow)* y le permite implementar un repositorio centralizado de archivos de referencia *(playbooks)* para el uso de herramientas de infraestructura como código *(Infrastructure as a Code)*.

====

Integración e Interoperabilidad entre plataformas (*API uCloud*)
------------------------------------------------------------------


La interoperabilidad es la capacidad de dos o más sistemas (ordenadores, medios de comunicación, redes, programas computacionales y otros componentes de la tecnología de la información) para interactuar e intercambiar datos según un método definido, con el fin de obtener los resultados esperados. La interoperabilidad define si dos componentes de un sistema, desarrollados con herramientas e diferentes proveedores, pueden o no actuar juntos.

La comunicación entre estos "sistemas" se basa en el consumo de una interfaz de programación de aplicaciones *(API)* que permite enviar y recibir llamadas para la ejecución de alguna actividad o la extracción de algún tipo de información almacenada. 

Las siglas *API* provienen de la expresión inglesa *Application Programming Interface* que, traducida al español, puede entenderse como interfaz de programación de aplicaciones. En otras palabras, la *API* es un conjunto de reglas que permite la comunicación entre plataformas a través de una serie de normas y protocolos.

A través de las API, los desarrolladores pueden establecer comunicación (interoperabilidad) entre programas y aplicaciones capaces de comunicarse con otras plataformas.

El principal ejemplo es la integración nativa y directa de la plataforma uCloud con la consola de los proveedores de nubes públicas, todo ello mediante la interoperabilidad a través de la API de las consolas de los proveedores.

Otro ejemplo muy común de uso de la plataforma uCloud es la emisión de facturas para los sistemas de showback y chargeback, así como el envío de información y alertas sobre los recursos gestionados.

Nuestros clientes (y/o integradores) pueden utilizar la documentación de la API del uCloud con sus plataformas internas para complementar o automatizar ciertas actividades o acciones que están más allá de las capacidades nativas de la plataforma uCloud. 

Por ejemplo: 

Consultar y extraer de la plataforma uCloud el coste de la factura de los objetos de valor de un proveedor de la nube pública a través de una aplicación financiera/contable para la emisión de facturas.

El uCloud dispone de documentación de su *API*, pero el acceso a la documentación completa debe solicitarse al Equipo de Atención al Cliente *(contato@usto.re)* para que se pueda crear y enviar una credencial de acceso a la documentación de la plataforma uCloud.

El equipo de Ustore está preparado para ayudar, evaluar las demandas de interoperabilidad e integración entre la plataforma uCloud, bien como las aplicaciones que tienen y permiten el uso de las *APIs* para la interoperabilidad.

====

Arquitectura de la plataforma uCloud
--------------------------------------

A continuación presentamos una arquitectura de referencia para la plataforma uCloud con sus componentes, proveedores e integraciones nativos.

.. figure:: /figuras/ucloud_future_vision_small_2.png
   :alt: Arquitectura de Referencia de la plataforma uCloud
   :align: center

----

La plataforma uCloud se comunica con la consola de los proveedores a través de la API Rest, por lo que cada acción realizada o configurada en las pantallas de uCloud envía acciones (tareas) al administrador (público y/o privado) del entorno de nube (consola) específico para que puedan realizar la acción deseada.

Ustore se compromete a mantener el constante desarrollo de sus plataformas de software y aplicar las mejores prácticas *(best practices)* de *DevOps* vigentes en el mercado de TI en la actualidad.

Nuestro compromiso es mantener la compatibilidad de integración, para que los últimos cambios e implementaciones en la consola de proveedores y todo el software que mantenemos mantengan la interoperabilidad, para que la nueva funcionalidad esté siempre disponible a través de la interfaz de la plataforma uCloud.

Para este caso, se utiliza un conjunto de prácticas y herramientas diseñadas para aumentar la capacidad de una organización para entregar aplicaciones y servicios más rápido que los procesos tradicionales de desarrollo de software.

.. Consulte la documentación específica acerca de *roadmap* de evolución de la plataforma uCloud o en el sitio web de Ustore (www.ustore.com.br).

====


Acceso a la plataforma uCloud
=============================

El acceso a la plataforma se realiza a través de una dirección de Internet, el usuario debe utilizar un navegador de Internet *(Internet browser)* e introducir la dirección URL/enlace, para que el usuario vea la pantalla de presentación inicial. Los navegadores de Internet 
compatibles con la plataforma uCloud son: Microsoft Edge versión 86.x, Google Chrome versión 85.x, Firefox verano 80.x u Opera versión 71.x.

La plataforma uCloud está adaptada para que su interfaz se presente en **Portugués (nativo), Español e Inglés**. Esta configuración la realiza el usuario. En su perfil es posible seleccionar el idioma de presentación de la interfaz, sin tener que cambiar la configuración de idioma de su sesión de navegador de Internet.

.. figure:: /figuras/ucloud_idioma_plataforma_001.png
   :alt: Idioma de la plataforma uCloud
   :scale: 50 %
   :align: center

----

.. attention::
    *Es importante tener en cuenta que la plataforma uCloud **no es compatible con Microsoft Internet Explorer (IE)** en ninguna versión, ya que las tecnologías de este navegador están desactualizadas y no soportan la evolución de las páginas HTML actuales.*

Después de iniciar sesión en un Internet browser, la dirección/ruta de acceso para la aplicación debe rellenarse como ejemplo a continuación, de la siguiente manera:

  * Ejemplo de enlace con dirección IP: ``http://<ucloudserverTCP_IP_Address>:80``

  * Enlace de ejemplo con el nombre del servidor: ``http://ucloud_Server_Name.com/``

Después de ingresar la dirección correctamente, la pantalla del usuario será similar a la figura a continuación:

.. figure:: /figuras/ucloud_acesso_plataforma_000.png
   :alt: Pantalla de inicio de sesión de la plataforma uCloud
   :align: center

----

Las credenciales de inicio de sesión y la contraseña deben haber sido aprovisionadas previamente en la plataforma uCloud por un usuario con un perfil de administrador (u otro usuario con este permiso).

El usuario debe informar sus datos de inicio de sesión y contraseña en los campos y hacer clic en el cursor del mouse en el botón **Entrar**.

Si las credenciales de acceso no han sido aprovisionadas, no existen o en el último caso, el usuario no recuerda la información correcta de sus credenciales, no tendrá acceso a la plataforma. Ver el Item **Solicitud de Nueva Contraseña**, en caso de que el usuario oscurezca algún tipo de información para proceder con el inicio de sesión de acceso a la plataforma uCloud.

Después de ingresar sus credenciales de acceso (nombre de usuario y contraseña), realice el procedimiento de inicio de sesión, al usuario se le presentará la pantalla a continuación:

* 1a parte de la pantalla

.. figure:: /figuras/ucloud_acesso_plataforma_001.png
   :alt: Dashboard uCloud
   :align: center

------

* 2a parte de la pantalla

.. figure:: /figuras/ucloud_acesso_plataforma_002.png
   :alt: Dashboard uCloud
   :align: center

----

La siguiente es una descripción detallada de las características de la pantalla de inicio *(Dashboard)* de la plataforma uCloud.


Dashboard
=========

Después de informar al usuario y la contraseña, puede ver la pantalla principal del portal de uCloud, como se muestra en la pantalla a continuación, tiene un menú en el lado izquierdo con una lista de opciones, y cada opción representa una pantalla de administración de uCloud, algunas pantallas solo estarán disponibles de acuerdo con el nivel de acceso del usuario.

El usuario puede notar que la pantalla del panel de control está dividida en secciones, que se describen a continuación:


Sección: Cuota de facturación del contrato
-------------------------------------------

----

Sección: Atajos
---------------

----

**Máquinas Virtuales**
~~~~~~~~~~~~~~~~~~~~~~

**Datacenters Virtuales**
~~~~~~~~~~~~~~~~~~~~~~~~

**Financiero**
~~~~~~~~~~~~~~

**Modelos**
~~~~~~~~~~~~~

----

Sección: Tareas recientes
---------------------------

----

Sección: Informaciones de cuota sobre los servicios
-----------------------------------------------------

----

Uso de la CPU
~~~~~~~~~~~~~~

Uso de la Memoria
~~~~~~~~~~~~~~~~~~

Uso del Disco
~~~~~~~~~~~~~~

Cuota de IPs públicas
~~~~~~~~~~~~~~~~~~~~~~

Cuota de Máquinas Virtuales
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----


.. Sección Contenedores
.. --------------------

.. En esta sección se presentan todos los proveedores de la nube (públicos y /o privados) donde cada contenedor está representado con un "botón" en la interfaz, como se muestra a continuación:

.. .. figure:: /figuras/uCloud_acesso_platafform_003.png
   :alt: sección contenedores dashboard
   :align: center

.. ----

.. Con cada necesidad de buscar información del contenedor el usuario interesado, debe seleccionar con el mouse el "botón" que representa el contenedor. 

.. Por lo tanto, para que el usuario pueda verificar sus cuotas y asignación de recursos, simplemente seleccione el contenedor elegido en la sección Gráficos de Uso de Recursos. Luego, al final de la selección, se cambiará la imagen de la pantalla y mostrará como resultado la representación de la asignación respectiva que se refiere al contenedor seleccionado.

.. Debido a que la plataforma uCloud es un entorno híbrido de múltiples nubes, se mostrarán tantos botones como sea necesario para representar todas las nubes (públicas y/o privadas) que se hayan configurado en el entorno de uCloud.

.. En el caso de que solo haya un botón, esto significa que el cliente tiene un único proveedor de servicios en la nube configurado en su entorno.

.. Consulte el elemento **Contenedores** para comprender los procesos de cómo configurar un proveedor de servicios en la nube (público y/o privado) en la plataforma uCloud.

.. Sección de Gráficos de uso de recursos
.. --------------------------------------

.. En esta sección el usuario puede comprobar la cantidad de recursos computacionales disponibles (cuota límite) y los valores totales que ya han sido utilizados/consumidos por ella:

.. .. figure:: /figuras/uCloud_acesso_platafform_004.png
   :alt: sección graficos de uso de recursos
   :align: center

.. ----

.. Estos límites (cuotas) han sido definidos y/o asignados al usuario, siguen los estándares y reglas de negocio de la organización, que estaban asociados con este usuario en el momento del aprovisionamiento de sus credenciales en la Plataforma uCloud.

.. Consulte los elementos Grupos y Usuarios para configurar o cambiar los límites (cuotas) de recursos computacionales o financieros, tanto para grupos como para un límite individual para un usuario específico.


.. Sección Últimas Tareas
.. ----------------------

.. La plataforma uCloud es un entorno que se comunica con las consolas de los proveedores de la nube o con el hipervisor utilizado internamente en Datacenter en su organización a través de la API Rest. De esta forma, todas las acciones -actividades- funciones solicitadas a través de la plataforma uCloud se 'encapsulan' como si fueran un `mensaje` y se envían a la consola de destino para que la consola realice las ´tareas´ enviadas.

.. .. figure:: /figuras/uCloud_acesso_platafform_005.png
   :alt: sección últimas tareas
   :align: center

.. ----

.. En consecuencia, la sección Tareas presenta la última lista de acciones - actividades - roles solicitados por el usuario que está registrado y activo (login) en la plataforma uCloud.

.. En esta sección, se presentará una lista de algunas tareas, que demuestran el porcentaje realizado y lo(s) resultado(s) respectivo(s) de esta(s) acción(es), ya sea para acciones completas exitosas o incompletas, debido a algún error recibido como respuesta de la consola de destino (pública y/o privada).

.. Consulte otros detalles en el elemento **Tareas**.

.. Sección Máquinas Virtuales
.. --------------------------

.. En esta sección, se enumerarán las máquinas virtuales que han experimentado interacciones o cambios recientes a través de la interfaz de la plataforma uCloud.

.. .. figure:: /figuras/uCloud_acesso_platafform_006.png
   :alt: sección últimas tareas
   :align: center

.. ----

.. Importante destacar un punto: Máquina virtual que ha sido cambiada en cualquiera de sus características, a través de la consola del proveedor de servicios en la nube (pública y/o privada), esta máquina virtual no formará parte de esta lista. La plataforma uCloud enumera solo las máquinas virtuales que han sido cambiadas por usuarios registrados y activos (inicio de sesión) en la plataforma uCloud.

.. Consulte el elemento **Menú de Usuario** para comprender las funcionalidades de cada opción de menú hacer.


.. Accesos directos de la sección a los menús principales
.. ------------------------------------------------------

.. En esta sección se presentan accesos directos a las características más frecuentes de la plataforma uCloud, de una forma más accesible y directa.

.. .. figure:: /figuras/uCloud_acesso_platafform_007.png
   :alt: sección últimas tareas
   :align: center

.. ----

.. Se puede acceder a todos los accesos directos presentados hasta ahora a través de sus respectivas funciones en el Menú de Usuario, que se coloca en la barra lateral izquierda en la interfaz de la plataforma uCloud.

.. Es importante tener en cuenta que el usuario activo (login) puede tener restricciones en ciertas opciones de menú, dependiendo del perfil asociado a ese usuario, determinado por la organización a la que está asociado el usuario. 

.. De esta forma, se enumerarán los accesos directos correspondientes al perfil del usuario al que se permitirá el acceso.

.. Solicitud de Nueva Contraseña
.. -----------------------------

.. Si el usuario no recuerda sus datos para iniciar sesión en la plataforma uCloud, la aplicación le permite recuperar la contraseña de acceso durante el proceso de inicio de sesión o si el usuario recibe el mensaje en la esquina superior de la pantalla con una advertencia emergente **"Usuario o contraseña incorrectos"** como se muestra en la figura a continuación:

.. .. figure:: /figuras/uCloud_nova_senha_001.png
   :alt: solicitud de nueva contraseña
   :align: center

.. ----

.. El usuario debe hacer clic en el cursor del mouse en la opción **"¿Olvidó su contraseña?"** como se detalla en la siguiente figura:

.. .. figure:: /figuras/uCloud_nova_senha_002.png
   :alt: solicitud de nueva contraseña
   :align: center

.. ----

.. Si la información de inicio de sesión del usuario existe, pero si necesita ingresar una nueva contraseña, la plataforma uCloud presentará al usuario el formulario para el cambio.

.. .. figure:: /figuras/uCloud_nova_senha_003.png
   :alt: solicitud de nueva contraseña
   :align: center

.. ----

.. En el primer campo, el usuario informa la dirección de correo electrónico que está registrada y en el segundo campo debe rellenar con la información de inicio de sesión del usuario que se aprovisionó en la plataforma uCloud.

.. Después de informar un correo electrónico válido y una cuenta de usuario para el acceso, el usuario debe hacer clic en el cursor del mouse en el botón verde `Edición`, la interfaz mostrará el siguiente mensaje:

.. .. figure:: /figuras/uCloud_nova_senha_004.png
   :alt: solicitud de cambiar contraseña
   :align: center

.. ----

.. El usuario debe comprobar el recibimiento de un mensaje en su buzón de correo electrónico con las instrucciones para restablecer la contraseña. El usuario debe proceder como se describe en el correo electrónico y restablecer su contraseña de acceso.

.. .. figure:: /figuras/uCloud_nova_senha_005.png
   :alt: solicitud de cambiar contraseña
   :align: center

.. ----

.. Debe verificar que el dominio "@ucloud.usto.re" esté bloqueado en su lista de mensajes no deseados (spam) para permitirle recibirlo.

.. Cuando el usuario hace clic en el cursor del mouse sobre el enlace/url presente en su correo electrónico, el usuario será llevado a una sesión de su navegador *(browser)* de Internet conectado a la plataforma uCloud, se mostrará la pantalla a continuación:

.. .. figure:: /figuras/uCloud_nova_senha_006.png
   :alt: solicitud de cambiar contraseña
   :align: center

.. ----

.. Después de que el usuario informe de la nueva cadena en el campo **Nueva Contraseña**, el usuario debe volver a introducirla en el siguiente campo **Confirmar Contraseña** igual a la notificada en el campo anterior.

.. Después de confirmar la nueva contraseña, el usuario debe hacer clic en el cursor del mouse en el botón **Guardar**, la interfaz mostrará el siguiente mensaje:

.. .. figure:: /figuras/uCloud_nova_senha_007.png
   :alt: cambiar contraseña
   :align: center

.. ----

.. Después de este procedimiento, el usuario puede realizar el proceso de inicio de sesión utilizando la información del usuario y la nueva contraseña. La nueva contraseña estará disponible de inmediato, y no tiene que esperar ningún período para la vigencia de la misma.


.. Usuario no aprovisionado
.. ------------------------

.. Si la información de inicio de sesión del usuario no se ha registrado previamente o la combinación de datos de correo electrónico e inicio de sesión, la plataforma uCloud mostrará un mensaje *pop-up*, en la esquina superior derecha de la pantalla, con la información de que los datos informados para cambiar la contraseña no existen en la plataforma uCloud.

.. .. figure:: /figuras/uCloud_user_nao_provisionado_001.png
   :alt: usuario no aprovisionado
   :align: center

.. ----

.. En este caso, simplemente póngase en contacto con el administrador de la plataforma uCloud de su organización para que puedan aprovisionar sus datos para el inicio de sesión. Solo un usuario correctamente aprovisionado tendrá su acceso efectivo.


.. Menú de Usuario
.. ===============

.. La barra de menú del usuario se encuentra a la izquierda de la pantalla y se muestra inicialmente en modo expandido, como en la figura a continuación:

.. .. figure:: /figuras/uCloud_menu_usuario_001.png
   :alt: menú de usuario modo expandido
   :align: center

.. ----

.. Algunas opciones de menú tienen un submenú, que se presenta cuando el usuario coloca el mouse sobre la indicación (signo inferior "<"). Al hacer clic en este icono, la interfaz presenta el submenú de esta opción al usuario, vea el ejemplo en la figura a continuación:

.. .. figure:: /figuras/uCloud_menu_usuario_002.png
   :alt: ejemplo de un submenú
   :align: center

.. ----

.. Es posible que el usuario elija reducir la presentación de la barra de Menú de Usuario al modo Solo icono, para tener un área de presentación más grande. Para cambiar entre el Modo Expandido del Menú de Usuario y los Iconos del Modo de Menú de Usuario, hay un gráfico verde con tres barras , fácil de identificar para el usuario. Este elemento estará presente en cualquier pantalla de la plataforma uCloud.

.. Cuando el usuario hace clic en este elemento, la barra de Menú de Usuario se cambiará a los Iconos de Modo, como se muestra en la figura a continuación:

.. .. figure:: /figuras/uCloud_menu_usuario_003.png
   :alt: menú de usuario modo iconos
   :align: center

.. ----

.. Cuando la barra de Menú de Usuario está en modo de icono, los submenús se mostrarán como se muestra a continuación:

.. .. figure:: /figuras/uCloud_menu_usuario_004.png
   :alt: abrir un submenú en modo icono 
   :align: center

.. ----

.. Las siguientes páginas detallan cada una de las opciones del menú de usuario y su funcionalidad.


Menú Administración
======================

Al presentar algunos conceptos sobre el entorno de administración de uCloud, es importante aclarar algunos puntos sobre la plataforma uCloud, en los conceptos existen tres términos que serán ampliamente utilizados en el entorno de uCloud:

  * **Contrato:** Es la forma en la que se define la relación *'comercial'* entre el prestador y la empresa que te contrató. En el contrato se definen los costos, el margen financiero, la tasa de conversión de moneda, los costos de recursos (opcional) y la cuota general (límite) que puede ser una cuota financiera o una cuota de recursos computacionales.

  * **Grupo:** Es una forma lógica definida únicamente dentro de la plataforma uCloud que puede definir un grupo de usuarios (por ejemplo, DevOps), un departamento (por ejemplo, ventas), una iniciativa (por ejemplo, VDI), a la que se asocian múltiples usuarios como parte integral de este grupo. Estos "grupos" no existen en los proveedores de nube (públicos y/o privados) existen solo dentro de la plataforma uCloud.

  * **Usuario:** Un usuario es la entidad que ha identificado el acceso a la plataforma uCloud para tomar medidas sobre los recursos informáticos de los proveedores (públicos y/o privados).

La siguiente figura ejemplifica, en una imagen, la relación entre estos tres términos y es fundamental que el usuario utilice esta figura como referencia para entender los enlaces.

.. figure:: /figuras/ucloud_arquitetura_conceitual001.png
   :align: center

----

Es importante entender que un **Contrato** puede tener múltiples usuarios y varios grupos; cada **Grupo** puede contener estos usuarios. Sin embargo, la plataforma uCloud permite que un Usuario forme parte de un solo contrato y un grupo, y un solo Grupo está vinculado a un solo contrato.

En el siguiente documento se describe que al configurar las cuotas (límites financieros o de recursos) del contrato, estos límites serán compartidos/divididos por cada uno de los grupos existentes, y por lo tanto los usuarios se limitan a las cuotas del grupo al que están incluidos.

Es posible señalar, en la figura anterior, que el término *Virtual DataCenter (VDC)* este término es una asignación lógica de máquinas virtuales que permite a las organizaciones definir uno (o más) grupos de servidores que forman parte de una nube. Un VDC puede representar un departamento, una subsidiaria o un grupo de usuarios, y otra información en el elemento **Virtual DataCenter**.

El término 'Administración' varía en función del perfil del usuario que está accediendo al sistema en ese momento. uCloud tiene cinco perfiles diferentes, que generalmente podemos describir a continuación:

  #. **Usuarios del sistema:** son usuarios habituales los que acceden al sistema para consumir recursos. Existe la posibilidad de *Usuarios con perfil de solo lectura*, quienes pueden designar usuarios regulares o habituales que solo pueden acceder a la plataforma uCloud para ver la información.

  #. **Usuarios Administradores de Contrato:** son los usuarios que están asociados a un contrato y en este contrato pueden definir reglas de boletería, provisión y cambio de otros usuarios en la plataforma.

  #. **Usuarios Administradores de Grupo:** son usuarios que están asociados a un grupo de usuarios, pueden aprovisionar y cambiar a otros usuarios en la plataforma.

  #. **Usuario Administrador Financiero:** son usuarios con un perfil para acceder a la información financiera de uCloud.

  #. **Usuario Administrador:** son usuarios con perfil de acceso completo y pueden realizar intervenciones globales en la configuración de la plataforma. Este perfil de usuario es exclusivo de Ustore o de un perfil de usuario único de la organización que compró las licencias de la plataforma uCloud. Este usuario administrador tiene permiso para administrar todas las funciones y recursos globales que ofrece la plataforma. 


.. note::
  |atencao| *El perfil de administrador no se tratará en este documento. Por favor, póngase en contacto con su punto focal en Ustore para obtener el documento específico: Manual del Administrador de la plataforma uCloud. Por seguridad, las mejores prácticas indican que  solo debe haber un usuario aprovisionado con este tipo de perfil.*

----


Switch Roles
------------

Cuando un usuario de infraestructura multinube necesita cambiar entre varias consolas de proveedores de nube, el proceso de inicio de sesión de varias credenciales en varias consolas lleva tiempo y puede incurrir en errores tipográficos de inicio de sesión y contraseña.

La plataforma uCloud como entorno multinube permite al usuario interactuar con los recursos informáticos existentes a través de múltiples proveedores de nube diferentes simultáneamente.

Cuando inicia sesión en la plataforma uCloud (inicio de sesión), el usuario obtiene un conjunto específico de permisos para realizar acciones que pertenecen al contrato al que está vinculado el usuario. Los usuarios pertenecen a un Grupo y los Grupos pertenecen a un contrato. Por lo tanto, las credenciales de acceso de usuario están vinculadas a uno o más contratos, este acuerdo puede aprovisionarse para tener acceso a una (o más) credenciales de acceso a los entornos de proveedores de nube pública y/o privada.

Vea la siguiente figura, que muestra el enlace del usuario a uno o más contratos:

.. figure:: /figuras/ucloud_arquitetura_conceitual001.png
   :align: center

----

El primer aspecto de la figura anterior es que podemos comprobar que este cliente tiene dos contratos diferentes. El **Contrato A** está asociado con un solo proveedor de nube pública (por ejemplo, *AWS*) y el **Contrato B** está asociado con dos proveedores de nube pública diferentes (por ejemplo, *AWS* y *Azure*).

----


Switch Roles - Escenario de Ejemplo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

En la figura anterior podemos ver que los usuarios Maria, João y Carlos pertenecen a un solo contrato y este contrato tiene un solo proveedor (por ejemplo, *AWS*).

El usuario **Josué** está asociado con dos acuerdos diferentes, y para evitar que este usuario tenga que cambiar entre diferentes sesiones de inscripción (terminando una sesión e iniciando otra con otra credencial), Ustore ha desarrollado e implementado la funcionalidad **Switch Roles**.

De esta manera, **solo** el usuario Josué, a través de la funcionalidad de *Switch Roles* puede cambiar entre los contratos a los que está vinculado, simplemente cambiando entre los contratos vinculados.

El usuario **Josué** es responsable de administrar completamente la infraestructura del entorno de Azure, pero en el entorno de AWS, solo puede ver los recursos computacionales porque no tiene permiso para operar estos recursos informáticos (por ejemplo, *Read Only*).

A través de la funcionalidad *Switch Roles* será posible aplicar este cambio de rol, sin necesidad de intercambio de usuarios, esto se hará a través de la selección de contrato y/o contenedor al que este usuario quiera acceder.

También para ilustrar este ejemplo, con la nueva implementación de Perfil de Permisos, puede crear diferentes conjuntos de permisos y vincular cada conjunto (Perfil de Permisos) a cada usuario y aprovisionar un nivel muy específico de granularidad.

----


Escenario de Ejemplo (AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


+----------------------------+---------+--------------------+-----------+
| Perfil de Permisos         | Usuario | Virtual Datacenter | Permiso   |
+============================+=========+====================+===========+
| AWS DevOps Full            | Maria   | DevOps             | Full      |
+----------------------------+---------+--------------------+-----------+
| AWS DevOps *Read Only*     | João    | DevOps             | Read Only |
| AWS Homolog Full           |         | Homolog            | Full      |
+----------------------------+---------+--------------------+-----------+
| AWS Homolog Full           | Carlos  |  Homolog           | Full      |
+----------------------------+---------+--------------------+-----------+
| AWS Infra Full             | Josué   | Infra              | Full      |
+----------------------------+---------+--------------------+-----------+


Actualmente puede aprovisionar cuatro (04) Perfiles de Permisos diferentes y vincular cada perfil a un usuario específico. 

En el ejemplo de la tabla anterior, puede ver que el usuario **João** tiene dos conjuntos diferentes de permisos que son específicos de cada conjunto de infraestructuras virtuales *(Virtual Datacenter-VDC)* al que este usuario puede acceder. Se concluye que el usuario João tiene acceso sin restricciones a VDC Homolog, y solo visualización a VDC DevOps.

Considere el ejemplo a continuación del usuario **Josué** que tiene diferentes características para cada contrato.

----

Escenario de Ejemplo (AZURE y AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


+----------------------------+---------+--------------------+-----------+
| Perfil de Permisos         | Usuario | Virtual Datacenter | Permiso   |
+============================+=========+====================+===========+
| Azure Infra RO             | Josué   | Infra Azure        | Read Only |
| AWS Infra Full             |         | Infra AWS          | Full      |
+----------------------------+---------+--------------------+-----------+

Este es un ejemplo de la simplicidad y transparencia que proviene de expandir y cambiar el nuevo Perfil de Permissionization, que le permite vincular diferentes conjuntos de permisos al mismo usuario, que están vinculados a diferentes contratos. Podemos verificar que el usuario de **Josué** tiene acceso sin restricciones *(full)* a la infraestructura de VDC Infra AWS (Contrato AWS) y acceso de solo lectura *(read only)* al VDC de Infra AZURE (Contrato Azure).

Anteriormente, el usuario tenía dos credenciales diferentes (por ejemplo, `josue.aws/passwordABC` y `josue.azure/password123``) y, por lo tanto, realizaba varias sesiones de inicio de sesión diferentes en la Plataforma uCloud.

Con la combinación del nuevo Perfil de Permisos en conjunto con la funcionalidad *Switch Roles* será posible aplicar este cambio del tipo de permisos, sin necesidad de intercambio de usuarios, esto se hará a través de la selección del contrato y/o contenedor al que este usuario quiera acceder.

----

Switch Roles - Utilizando 
~~~~~~~~~~~~~~~~~~~~~~~~~~~

La funcionalidad de Switch Roles se encuentra en la esquina superior derecha de la interfaz de la Plataforma de uCloud (junto al nombre de usuario) - ver la siguiente pantalla:

.. figure:: /figuras/ucloud_dashboard_switch_roles001.png
   :align: center

----

Simplemente haga clic en el usuario con el cursor del mouse sobre el nombre del contrato y la Plataforma uCloud muestra una ventana pop-up, que resulta el usuario de la lista de contratos a los que está vinculado el usuario para que seleccione el contrato deseado.

.. figure:: /figuras/ucloud_dashboard_switch_roles002.png
   :scale: 60 %
   :align: center

----

Al seleccionar el contrato deseado, la Plataforma uCloud actualizará la información presentada en la esquina superior derecha de la sesión del usuario.

Es importante tener en cuenta que esta ventana pop-up enumera solo los contratos a los que está vinculado el usuario. Si hay otros acuerdos aprovisionados en la Plataforma uCloud, no tendrá acceso a ninguno de estos otros acuerdos.

.. figure:: /figuras/ucloud_dashboard_switch_roles003.png
   :align: center

----

La función Switch Roles permite a un usuario cambiar tanto su nivel de acceso como obtener acceso a diferentes contratos con diferentes reglas de permisos para cada contrato sin tener que cerrar sesión en la Plataforma uCloud.

Con esta nueva funcionalidad, un solo usuario puede acceder, por ejemplo, a la nube de Azure y a la nube de AWS con la capacidad de tener responsabilidades, permisos y niveles de acceso completamente diferentes y específicos para cada uno de los entornos de proveedores de nube pública.

La personalización de los permisos de actividad que puede tener el usuario se aclarará en el tema **Perfil de Permiso** de este documento.

----


Cuenta *(Account)*
-----------------

----

Introducción
~~~~~~~~~~~~~~

----

Tipo de Cuenta (`Account`)
~~~~~~~~~~~~~~~~~~~~~~~~~~

----

¿Cómo Acceder?
~~~~~~~~~~~~~~~

----

Cuentas Integrador y Productor
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Cuentas 
--------

----

Principal y Subcuenta
~~~~~~~~~~~~~~~~~~~~~~

----

Creando una Cuenta
~~~~~~~~~~~~~~~~~~~~~~

----

Listando la Cuenta Creada
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Detallando la Cuenta
~~~~~~~~~~~~~~~~~~~~~~

----

Creando la Subcuenta
~~~~~~~~~~~~~~~~~~~~~~

----

¿Cómo visualizar la Lista de Cuentas?
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Usuarios
----------

.. attention:: Este menú está siendo reelaborado para ser actualizado, tras las mejoras y nuevas implantaciones realizadas este trimestre.

La plataforma uCloud tiene sus propias bases de datos que almacenan la información de los usuarios, como el inicio de sesión y la contraseña, de manera segura y encriptada. La pantalla de inicio del **Menú de Administración** muestra la lista de usuarios aprovisionados, la información de inicio de sesión de un usuario, el grupo al que está asociado el usuario y el tipo de perfil para este inicio de sesión.

Dependiendo del tipo de perfil de usuario que esté accediendo al sistema, la Plataforma uCloud solo presentará la relación de usuario que el perfil que está registrado y activo puede gestionar o administrar.

   .. figure:: /figuras/uCloud_menu_administracao_usuario_001.png
   :scale: 80 %
   :align: center

----

Para proceder con el acceso a la Plataforma uCloud, debe aprovisionar (registrar) a un usuario con su respectivo nombre de usuario y contraseña de acceso.

A continuación se presentan las columnas presentadas en esta lista de usuarios:

* **Botón Crear Usuario**: Cuando se selecciona este botón, el proceso se describe en el elemento **Crear Nuevo Usuario**.

* **Login**: Esta columna presenta las credenciales de login del usuario. Como una forma de simplificar la visualización, si hace clic en el botón del mouse en el título de esta columna, la plataforma uCloud ordena la lista de inicio de sesión de los usuarios alfabéticamente de forma ascendente (a - z) o descendente (z - a).

* **Nombre**: Esta columna muestra el nombre del usuario que se informó durante el proceso de aprovisionamiento en la plataforma uCloud. Como una forma de simplificar la visualización, si hace clic con el botón del mouse en el título de esta columna, la plataforma uCloud ordena la lista de nombres de usuario alfabéticamente de forma ascendente (a – z) o descendente (z – a).

* **Grupo**: Esta columna presenta el grupo principal del usuario que fue informado durante el proceso de su aprovisionamiento en la plataforma uCloud. Como una forma de simplificar la visualización, si hace clic en el botón del mouse en el título de esta columna, la plataforma uCloud ordena la lista de grupos de usuarios alfabéticamente (a - z) o descendente (z - a).

* **Perfil**: Esta columna muestra el perfil del usuario que fue informado durante el proceso de su aprovisionamiento en la Plataforma uCloud. Como una forma de simplificar la visualización, si hace clic en el botón del mouse en el título de esta columna, la plataforma uCloud ordena la lista de perfiles de usuario alfabéticamente (a - z) o descendente (z - a).

* **Búsqueda Rápida**: El usuario puede notar que justo debajo del nombre de cada columna hay un campo 'en blanco', este campo le permite realizar una búsqueda rápida del contenido del listado para reducir y reducir la cantidad de incidencias de esta lista de eventos de inicio de sesión. Simplemente complete el campo 'blanco' con una cadena que pueda ser relevante, y la plataforma uCloud actualizará la pantalla para representar ese patrón de búsqueda.

* **Columna de perfil**: El campo de búsqueda rápida en la columna Perfil tiene un control avanzado en forma de *"dropdownlist"* que le permite aplicar un **filtro** de 'tipo de perfil' para que la lista presentada esté restringida solo a la opción seleccionada. Para hacer esto, simplemente haga clic en el cursor del mouse en este campo, la Plataforma uCloud muestra las opciones de filtrado.

.. figure:: /figuras/uCloud_menu_administracao_usuario_002.png
   :align: center

----

Un usuario, aprovisionado, debe estar vinculado a solo uno de los seis **Tipos de Perfiles** disponibles, esta definición se deriva del rol con el que se puede asociar este usuario. De estos seis tipos, solo *dos (02)* perfiles (perfil de *usuario* y perfil de *auditor*) se utilizan en las operaciones diarias en la plataforma uCloud.

El perfil de **Auditor** tiene un papel muy estrecho pero muy importante en el control y la gestión de los costes del entorno de recursos de computación en la nube (público y/o privado).

El perfil de Usuario es el más fundamental y flexible, ya que puede asumir diferentes niveles de permisos y funciones de operación, gestión y administración del entorno empresarial en uCloud.

A continuación se muestra la descripción de los cuatro tipos básicos del perfil de usuario en la plataforma uCloud, que son:

* **Usuario**: es el perfil universal y todo otro perfil tiene como premisa ser aprovisionado como un usuario de la Plataforma de uCloud y que debe estar vinculado a un grupo y está limitado los permisos (acceso a menús) y cuotas (límites financieros o de recursos) que pueden ser individuales o compartidas por el grupo. Es importante destacar que cualquier otro perfil descrito a continuación, son variaciones de este perfil inicial.
  * Este usuario no tiene permiso para cambiar ninguno de sus permisos, los cuales se establecieron durante su aprovisionamiento. Solo un usuario con el perfil de administrador de grupo y/o de acuerdo puede restablecer los límites (cuotas) y permisos de este perfil de usuario.
  * Este usuario está identificado en el listado con la marca gráfica (flag): ``user``

* **Usuario Administrador de Contrato**: es un usuario, anteriormente provisionado, que está registrado en el campo Administrador en la pantalla de Contratos. Este perfil de usuario tiene permiso para aprovisionar nuevos usuarios, así como cambiar algunos campos de la pantalla de Contrato.

  * Este usuario tiene el privilegio de cambiar algunos de sus permisos establecidos durante su aprovisionamiento, así como cambiar algunos de sus propios permisos, así como los permisos de otros usuarios. Solo un usuario con el perfil de administrador de grupo y/o de acuerdo puede restablecer los límites (cuotas) y permisos de este perfil de usuario.

  * Este usuario está identificado en el listado con la marca gráfica (flag): ``user`` - el término **User +** una estrella parcialmente rellenada - indica que este usuario es un Administrador de Contrato.

* **Usuario Administrador de Grupo**: es un usuario, previamente aprovisionado, que está registrado en el campo Administrador del Grupo en la pantalla de Grupos. Este usuario tiene permiso para cambiar algunos de sus permisos establecidos durante su aprovisionamiento, así como cambiar algunos de sus propios permisos, así como los permisos de otros usuarios. Solo un usuario con el perfil de administrador de grupo y/o de acuerdo puede restablecer los límites (cuotas) y permisos de este perfil de usuario.

  * Este usuario está identificado en el listado con la marca (flag) gráfica: ``user`` - el término **User +** una estrella no rellena - indica que este usuario es un Administrador de Grupo.

* **Usuario Administrador de Contrato y Administrador de Grupo**: La Plataforma de uCloud permite que un usuario pueda estar asociado como Administrador de un Grupo y, simultáneamente, Administrador de un Contrato este usuario está identificado en la lista con la marca (flag) gráfica: ``user`` y una estrella estará completamente llena indicando que este usuario es un Administrador de Grupo y de Contrato.
  
 * Esta doble asociación de perfil permite a este usuario un alto nivel de control y administración del entorno de la empresa.
  
* **Auditor**: es un usuario que tiene acceso al menú de la Gestión Financiera y realiza el seguimiento de la facturación del portal, así como define las reglas de fijación de precios del contrato.

  * Este usuario, por premisa básica, no está asociado a ningún permiso para operación y alteración de cualquiera que sea el recurso computacional, en uno u otro proveedor de servicio de nube (público y/o privado). Este perfil tiene acceso únicamente al análisis financiero y de costos del contrato al que este usuario está vinculado, por intermedio de un grupo.
  * Este usuario está identificado en el listado con la marca (flag) gráfica: ``user`` el término indica que este usuario es un Auditor del Contrato.

Los otros cuatro perfiles (**Administrator, Service, VDI User, VDI Administrator**) son perfiles internos de la Plataforma de uCloud, no estarán cubiertos en este documento. Póngase en contacto con su punto focal en Ustore para obtener los documentos específicos: *Manual del Administrador de la Plataforma uCloud y 
.. Manual del Entorno VDI Ustore*

----

Visualizando un usuario
---------------------------

.. attention:: Este menú está siendo reelaborado para ser actualizado, tras las mejoras y nuevas implantaciones realizadas este trimestre.

En la lista de usuarios es posible ver la información de un usuario, simplemente haga clic con el mouse sobre la línea en la que se presenta el usuario, la Plataforma de uCloud mostrará la pantalla con toda la información del usuario aprovisionado en la plataforma. En esta pantalla es posible añadir nuevas configuraciones al perfil de un usuario. 

La pantalla de visualización de detalles de un usuario se divide en secciones y se describe a continuación:

.. figure:: /figuras/uCloud_menu_administracao_usuario_003.png
   :scale: 60 %
   :align: center

----

* **Sección General**: La primera sección de esta pantalla muestra los datos generales del perfil de usuario aprovisionado en la Plataforma uCloud. Por medio de esta pantalla será posible cambiar algunos campos referentes al usuario.

  * **Botón de Eliminar Usuario:** Este botón se puede utilizar para eliminar de forma definitiva e irreversible al usuario aprovisionado en la Plataforma de uCloud. Solo el usuario haga clic con el cursor del mouse sobre el botón, se mostrará la pantalla solicitando la confirmación de la acción, como se muestra a continuación:

.. figure:: /figuras/uCloud_menu_administracao_usuario_004.png
   :align: center

----

Tras la confirmación de la Eliminación del usuario, este usuario y sus credenciales de acceso no estarán disponibles de forma **irreversible de inmediato** y no será posible recuperar la información de este usuario. Si la eliminación es accidental, este usuario debe ser aprovisionado de nuevo, ver el elemento **Crear Nuevo Usuario**.

  * **Icono de Edición Activo** |icone_edita_on|: Todos los campos que tienen el icono de edición activo pueden cambiar su contenido.
  
  * **Icono de Edición Inactivo** |icone_edita_on|: Todos los campos que tienen el icono de edición inactivo o no son susceptibles de tener su contenido alterado a través de esta pantalla (ej.: valores de las cuotas de grupo) o el perfil del usuario que está registrado y accediendo a esta pantalla, no tiene permiso para cambiar el contenido del (de los) campo(s).

  * **Icono de Confirmación** |icone_conf_verde|: Cuando el usuario confirma su intención de cambiar el contenido del campo deseado, la Plataforma de uCloud muestra un icono de confirmación. Después de haber finalizado el cambio del contenido del campo el usuario debe hacer clic con el cursor del mouse en el botón verde para confirmar el cambio. Después de esta acción la información del campo se modificará permanentemente en las bases de datos de la Plataforma de uCloud.

  * **Icono de Cancelación** |icone_cancela_vermelho|: En caso de que el usuario haya hecho clic sobre el icono de edición por error o no desee que el cambio se almacene (grabada) permanentemente, basta con que el usuario haga clic con el cursor del mouse sobre el icono rojo. El icono rojo cancela los cambios y el contenido del campo vuelve a los valores iniciales antes de realizar cualquier relleno o cambio.

  * **Barra de Desplazamiento**: Esta sección posee un gran conjunto de campos, para la completa visualización de todo el usuario debe utilizar la barra de desplazamiento al lado derecho de esta sección. Si el usuario desplaza el mouse, la pantalla se desplaza hacia abajo y muestra los campos que no se estaban visualizando, como se muestra a continuación:

.. figure:: /figuras/uCloud_menu_administracao_usuario_005.png
   :alt: menú administración usuario 
   :align: center

----

  * **Solo Lectura**: Este campo configura a un usuario que no tiene permiso para realizar ninguna acción a través de la Plataforma de uCloud, pero su inicio de sesión está activo y tiene la capacidad de ver todas las pantallas que tiene permiso.

.. important:: Este es un campo tipo *"checkbox"* que el usuario puede actuar para alternar su modo actual, `siempre que su perfil permita proceder a cambio`. Si el icono está en color rojo, simplemente haga clic con el cursor del mouse y el campo se activará para el color verde. Si el icono está en color verde, simplemente haga clic con el mouse y el campo se desactivará poniéndose en color rojo.

* **Autenticación Multifactor**: Este campo indica si este usuario tendrá su proceso de autenticación en la plataforma (login) siendo verificado doblemente, antes de aprobar que este usuario tenga acceso a la Plataforma de uCloud. Para ello, se enviará un mensaje en el número de servicio móvil del celular registrado.

.. important:: Este es un campo tipo *"checkbox"* que el usuario puede actuar para alternar su modo actual, `siempre que su perfil permita proceder a cambio`. Si el icono está en color rojo, simplemente haga clic con el cursor del mouse y el campo se activará para el color verde. Si el icono está en color verde, simplemente haga clic con el mouse y el campo se desactivará poniéndose en color rojo.

* **Activar Cuota de Facturación**

* **Aprobación del Administrador**: Este campo configura que todas las acciones y solicitudes realizadas en la interfaz de la Plataforma de uCloud, de este usuario, deberán ser aprobadas por un usuario Administrador del Grupo. Esta es una funcionalidad para aumentar el control de gobernanza de costos y operaciones.

.. important:: Este es un campo tipo *"checkbox"* que el usuario puede actuar para alternar su modo actual, `siempre que su perfil permita proceder a cambio`. Si el icono está en color rojo, simplemente haga clic con el cursor del mouse y el campo se activará para el color verde. Si el icono está en color verde, simplemente haga clic con el mouse y el campo se desactivará poniéndose en color rojo.


* **Sección Permisos de Usuario**: Cuando se crea el usuario, hereda/recibe todos los permisos definidos en el grupo al que pertenece (ver la siguiente sección), así como los permisos establecidos en el Acuerdo. Esta tabla es opcional, pero permite añadir o revocar los permisos que este usuario tiene para realizar acciones, o acceder a menús, en la Plataforma de uCloud.

.. figure:: /figuras/uCloud_menu_usuario_006.png
   :align: center

----

  * **Botón Editar**: Para agregar o revocar permisos para el usuario, el Administrador (o usuario con autorización) debe hacer clic en este botón para que la Plataforma de uCloud pueda mostrar la pantalla que es posible realizar el procedimiento de agregar o eliminar permisos específicos para este usuario. Vea el siguiente ejemplo:

.. figure:: /figuras/uCloud_menu_usuario_005.png
   :align: center

----

Esta pantalla tiene dos columnas distintas:

  * A la izquierda son los permisos previamente añadidos al usuario. Al lado de cada permiso existe un campo del tipo *"checkbox"* que al ser seleccionado elimina (revoca) el respectivo permiso de este usuario.

  * A la derecha están los permisos disponibles en la Plataforma de uCloud que se pueden agregar al perfil individual de este usuario. Al lado de cada permiso existe un campo del tipo *"checkbox"* que, cuando se selecciona, agrega el respectivo permiso de este usuario.
  
  * **Usar los permisos predeterminados**: Al seleccionar este campo *"checkbox"* y confirmar la acción, el usuario recibirá todos los permisos de usuario disponibles en la Plataforma de uCloud.
  
  * **Botón Aplicar**: Después de verificar que todos los cambios necesarios han sido configurados (inclusiones o exclusiones), el usuario debe hacer clic con el mouse en el botón **Aplicar** para confirmar los cambios - de forma definitiva e inmediata - para el usuario que está viendo/cambiando. Terminada esta acción la Plataforma de uCloud cerrará esta pantalla y volverá a la pantalla anterior, con su contenido actualizado, presentando la nueva relación de permisos del usuario.

* **Sección Políticas de Permisos de Usuario (eventual)**: Esta sección solo se mostrará a los usuarios que han sido aprovisionados en la Plataforma uCloud con el *"checkbox"* **Crear Usuario en la Nube** habilitado. En esta sección se muestran todas las directivas de permisos específicas y únicas del entorno del proveedor de servicios de nube pública. Estas políticas se “importan” durante el proceso de sincronización del contenedor, y permiten un alto nivel de control granular de las capacidades (permisos) que el usuario puede realizar dentro del entorno del proveedor de servicios en la nube. Cuando el usuario es recién aprovisionado, este puede estar asociado a ninguna directiva de permisos, será necesario configurar manualmente los permisos.

.. figure:: /figuras/uCloud_menu_usuario_007.png
   :align: center

----
  
  * **Botón Editar** Este botón permite al usuario Administrador (o usuario autorizado) agregar o revocar las políticas de permisos del entorno del proveedor de servicios en la nube. Para ello, se debe hacer clic en el botón **'Editar'** desde allí se le permitirá al usuario administrador agregar o eliminar permisos específicos para el usuario deseado. Vea el siguiente ejemplo:

.. figure:: /figuras/uCloud_menu_usuario_008.png
   :align: center

----

Esta pantalla tiene dos columnas distintas:

  * A la izquierda son los permisos previamente añadidos al usuario. Al lado de cada permiso existe un campo del tipo *"checkbox"* que al ser seleccionado elimina (revoca) el respectivo permiso de este usuario.

  * A la derecha están los permisos disponibles en la Plataforma de uCloud que se pueden agregar al perfil individual de este usuario. Al lado de cada permiso existe un campo del tipo *"checkbox"* que, cuando se selecciona, agrega el respectivo permiso de este usuario.


  * **Botón Aplicar**: Después de verificar que todos los cambios necesarios han sido configurados (inclusiones o exclusiones), el usuario debe hacer clic con el mouse en el botón **Aplicar** para confirmar los cambios - de forma definitiva e inmediata - para el usuario que está viendo/cambiando. Terminada esta acción la Plataforma de uCloud cerrará esta pantalla y regresará a la pantalla anterior, con su contenido actualizado, presentando la nueva relación de permisos del usuario.

* **Sección Permisos de Grupo**: Esta sección solo muestra los permisos definidos en la configuración del grupo al que está vinculado este usuario. La Plataforma de uCloud no permite que los permisos listados aquí puedan ser cambiados a través de esta pantalla. Para tener contacto y conocer los permisos definidos en el grupo, vea el elemento Administración / Grupos.

Si se requieren cambios de cualquier permiso que se enumeran aquí, estos cambios deben realizarse en la configuración del Grupo.

.. figure:: /figuras/uCloud_menu_usuario_009.png
   :align: center

----

* **Sección Grupos Secundarios**: En esta sección es posible asociar un usuario a más de un grupo en la Plataforma de uCloud. En la sección **General**, puede comprobar el grupo principal al que está vinculado el usuario.

.. figure:: /figuras/uCloud_menu_usuario_010.png
   :align: center

----

  * **Botón Editar**: Para vincular a este usuario a un grupo secundario, o desvincular a este usuario de un grupo secundario, el Administrador (o usuario con autorización) debe hacer clic en este botón **Editar** para que la Plataforma de uCloud pueda mostrar la pantalla que permite desvincular al usuario de grupos secundarios. Vea el siguiente ejemplo:

.. figure:: /figuras/uCloud_menu_usuario_011.png
   :align: center

----

  * A la derecha están listados los grupos que están vinculados al contrato del grupo principal al cual este usuario fue provisionado originalmente. La Plataforma de uCloud enumera solo los grupos que están vinculados al contrato vigente. Al lado de cada grupo existe un campo del tipo *"checkbox"* que, cuando seleccionado, vincula el grupo seleccionado a este usuario.
  
  * A la izquierda están listados los grupos secundarios que este usuario está vinculado. Al lado de cada grupo existe un campo del tipo *"checkbox"* que, cuando se selecciona, desvincula el grupo seleccionado de este usuario.

  * **Botón Aplicar**: Después de certificar que todas las vinculaciones, o remoción, han sido configuradas, el usuario debe hacer clic en el botón Aplicar para configurar los cambios, de forma definitiva e inmediata, para el usuario que se está visualizando/alterando. Después de esta acción la Plataforma de uCloud cierra esta pantalla y vuelve a la pantalla anterior con su contenido presentando la nueva relación de permisos de usuario.

* **Sección de Perfiles de Visualización**: Esta sección permite al administrador del contrato seleccionar qué opciones del Menú de Usuario puede ver este usuario. A través de esta funcionalidad, el administrador puede personalizar la forma en que este usuario interactúa con la plataforma uCloud. Puede seguir el proceso de definición de estos perfiles en el elemento **Configuración / Perfiles de Visualización**. Esta configuración elimina o añade las opciones de la barra de **Menú de Usuario**, de modo que para el usuario no hay forma de saber que existe tal funcióny. La posibilidadde saberlo, sería acompañar a otro usuario que utiliza la plataforma con otras opciones de **Menú de Usuario** visibles.

.. figure:: /figuras/uCloud_menu_usuario_012.png
   :align: center

----

  * **Botón Add**: Para agregar este usuario a un perfil de vista previa, o desvincular a este usuario de un grupo secundario, el Administrador (el usuario creado) debe hacer clic en este botón **Add** para que la Plataforma uCloud pueda mostrar la pantalla que permite asociar al usuario con uno de los perfiles de visualización configurados en la plataforma. Vea el ejemplo a continuación:

.. figure:: /figuras/uCloud_menu_usuario_013.png
   :align: center

----

Puede ingresar parte del nombre de un grupo y hacer clic en el cursor del mouse (o en la tecla Enter) para que la plataforma uCloud presente una lista de todos los grupos que tienen la misma cadena reportada. Este campo distingue entre mayúsculas y minúsculas y/o minúsculas, solo enumera los perfiles de vista previa que coinciden exactamente con la parte del texto que se escribió (si no aparece nada, escriba texto con otra combinación de mayúsculas o minúsculas).

.. note:: *Es importante tener en cuenta que los perfiles enumerados en la pantalla de muestra no existen y se crearon solo con fines ilustrativos*.

* **Botón Guardar**: Después de asegurarse de que ha vinculado al usuario al perfil de vista correcto, el usuario debe hacer clic con el botón del mouse en el botón **Guardar** para configurar los cambios, de forma definitiva e inmediata, para el usuario que está viendo/cambiando. Tras esta acción la Plataforma uCloud cierra esta pantalla y vuelve a la pantalla anterior con su contenido presentando la nueva relación de permisos de usuario.

* **Sección Últimos Logins**: En esta sección se enumerarán todos los eventos en los que este usuario ha iniciado sesión (login) en la Plataforma uCloud. Vea la pantalla de ejemplo a continuación:

.. figure:: /figuras/uCloud_menu_usuario_014.png
   :align: center

----

  * **Fecha de `Login`**: Este campo muestra la fecha y la hora en que el usuario inicia sesión en una Plataforma uCloud utilizando su inicio de sesión (login). La información se presenta en formato de fecha en la norma brasileña (Día/Mes/Año Hora:Minuto:segundo).
  * **Fecha de `Logout`**: Este campo muestra la fecha y la hora en que el usuario cierra sesión en la plataforma uCloud con su inicio de sesión. La información se presenta en formato de fecha en la norma brasileña (Día/Mes/Año Hora:Minuto:segundo).
  * **Tiempo de Sesión**: Este campo muestra la cantidad total de tiempo que este inicio de sesión de usuario permanece conectado a la plataforma uCloud, en el formato de horas, minutos y segundos (por ejemplo, 6h 18m 33s).
  * **IP Remota**: Este campo muestra el número de la dirección TCP-IP con la que el usuario estaba asociado cuando inició sesión con la Plataforma uCloud.

.. note:: Es importante tener en cuenta que los inicios de sesión enumerados en la pantalla de ejemplo no existen y se crearon solo con fines ilustrativos.

* **Búsqueda Rápida**: El usuario nota que justo debajo del nombre de cada columna hay un campo 'en blanco' que le permite realizar una búsqueda rápida del contenido del listado para reducir y reducir la cantidad de incidencias de esta lista de eventos de inicio de sesión (login). Simplemente complete el campo en blanco con una cadena que pueda ser relevante, y la Plataforma uCloud actualizará la pantalla para representar este patrón de búsqueda.

* **Sección Máquinas Virtuales**: Esta sección presenta una lista de máquinas virtuales (VMs) o cargas de trabajo *(workloads)* creadas por este usuario durante una sesión activa en la Plataforma uCloud.

.. figure:: /figuras/uCloud_menu_usuario_015.png
   :align: center

----

.. note:: Es importante tener en cuenta que las máquinas virtuales enumeradas en la pantalla de ejemplo no existen y se crearon solo con fines ilustrativos.

* **Búsqueda Rápida**: Es posible que el usuario no pueda notar que justo debajo del nombre de la columna hay un campo 'en blanco' que le permite realizar una búsqueda rápida sobre el contenido del listado para reducir y reducir la cantidad de incidencias de esta lista de máquinas virtuales *(VMs)* de este usuario. Simplemente complete el campo en blanco con una cadena que pueda ser relevante, y la plataforma uCloud actualiza la pantalla para representar este patrón de búsqueda.

----

Creando un Nuevo Usuario
--------------------------

Antes de tratar con la creación de un usuario, es importante establecer que para la Plataforma uCloud un Usuario está vinculado a un Grupo y un Grupo está vinculado por un Contrato [Usuario<Grupo<Contrato].

De esta forma, antes de empezar a crear un nuevo usuario, es importante comprobar la existencia del grupo al que estará asociado este usuario. Para crear un usuario debe seleccionar la opción **'Crear Usuario'** como se indica a continuación.

.. figure:: /figuras/uCloud_menu_usuario_022.png
   :align: center

----

Para aprovisionar a un usuario en la Plataforma uCloud, segue la descripción detallada de la correcta finalización de los campos, son:

.. figure:: /figuras/uCloud_menu_usuario_017.png
   :align: center

----

* **Grupo**: Este campo es obligatorio y el usuario debe informar a un grupo previamente aprovisionado en la Plataforma uCloud, ya que no será posible seguir registrando un usuario sin vincular a este nuevo usuario a un grupo existente.

  * Puede ingresar parte del nombre de un grupo y hacer clic en el cursor del mouse (o en la tecla Enter) para que la Plataforma uCloud pueda mostrar una lista de todos los grupos que tienen la misma cadena informada, vea el ejemplo a continuación:
  * Cuando encuentre el Grupo al que este nuevo usuario debe estar vinculado, simplemente selecciónelo y el campo se llenará con el grupo específico.
  * Es importante tener en cuenta que puede asociar este usuario con más de un grupo si es necesario. Pero estos grupos deben estar vinculados por un solo Contrato.

* **Nombre**: Este campo es obligatorio y debe rellenarse con el nombre del usuario que está provisionando.

* **Login**: Este campo es obligatorio y debe rellenarse con la cadena que se utilizará para identificar al usuario durante el proceso de inicio de sesión *(login)* de uCloud.

* **Contraseña**: Este campo es obligatorio y debe rellenarse con la cadena de contraseña del usuario. Es importante tener en cuenta que esta secuencia debe ser mayor que cuatro (04) caracteres alfanuméricos. Debe seguir la recomendación de usar contraseñas "seguras y de alta complejidad", de acuerdo con la documentación que se encuentra en el sitio web de Azure. La recomendación es de al menos ocho (08) y un máximo de setenta y dos (72) caracteres y debe contener caracteres de tres de las siguientes categorías:

  * Letras mayúsculas y minúsculas (A a Z)
  
  * Números base 10 (de 0 a 9)

  * Caracteres no alfanuméricos (caracteres especiales): (~! @ # $% ^& * -+ = '|\\() {} \ []:; "' <>,.? /) 

.. note:: *Es importante tener en cuenta que los símbolos de moneda como el euro o la libra esterlina no se cuentan como caracteres especiales para esta configuración de política*.

  * **Confirmar Contraseña**: Este campo es obligatorio y debe rellenarse con la misma cadena introducida en el campo anterior. Si la secuencia informada en este campo es diferente de la anterior, se mostrará un pop-up con un mensaje de error en pantalla.

.. figure:: /figuras/uCloud_menu_usuario_018.png
   :alt: Menu de Usuário
   :align: center

----

.. attention:: *Es importante tener en cuenta que la Plataforma uCloud **no realiza** ninguna validación previa respecto a la existencia del correo electrónico informado o su efectivo funcionamiento. En caso de que no haya correo electrónico de destino, o error al escribir, el usuario no podrá realizar el restablecimiento de su contraseña de acceso. En este caso, deberá ponerse en contacto con el administrador de su cuenta*.

* **Correo Electrónico**: Este campo es obligatorio, en él se debe informar una dirección de correo electrónico válida. Esta dirección de correo electrónico será crítica durante el proceso de restablecimiento de contraseña del usuario, ya que la plataforma uCloud utiliza este correo electrónico para enviar un mensaje que permite al usuario crear una contraseña para él automáticamente.

* **Teléfono**: Este campo es obligatorio, y debe llenarse con un número de teléfono de servicio celular móvil, use el siguiente formato:

  * **Dos (02)** números que identifican el código de área del número de teléfono del servicio móvil (XX). No es necesario introducir el número *'cero (0)'* que precede al código de área en la norma brasileña.
  * **ocho (08) o nueve (09)** números que identifican el número de teléfono del servicio móvil del usuario. No es necesario informar a ningún otro carácter para la separación de grupos de números de teléfono del servicio celular móvil.
  * Ejemplo de relleno: `(11)999991234`

* **Posición**: Este campo es obligatorio, pero es meramente informativo para identificar la posición del usuario que desea aprovisionar.

* **Empresa**: Este campo es obligatorio, pero es meramente informativo para identificar la organización a la que está asociado este usuario.

* **Tipo de cuota**: Este campo es obligatorio, es un campo del tipo *"drop down list"*, cuando el usuario haga clic en este se presentará ala lista de opciones del tipo de cuota disponibles para aprovisionar a un usuario, consulte las opciones a continuación:

.. figure:: /figuras/uCloud_menu_usuario_019.png
   :alt: Tipo de Cota de Usuário
   :align: center

----

* **Cuota de Grupo**: Cuando se selecciona en esta opción, el usuario comparte los límites de recursos financieros o computacionales (cuotas) que se definen en la configuración del grupo. Los usuarios con una cuota de grupo deben conocer la información presentada en la pantalla de inicio (*dashboard* - consulte el elemento **Dashboard**), ya que la Plataforma uCloud niega la creación de recursos informáticos o el consumo de valores financieros que excedan los límites disponibles en el grupo al que está vinculado el usuario.

* **Cuota de Usuario**: Cuando el usuario la selecciona, la Plataforma uCloud solicita que se informen los límites de recursos computacionales (cuotas) financieros o individuales, como se muestra en la pantalla a continuación:

----

Grupos
-----------------------

----

Visualizando Grupo
------------------------

----

Creando un Nuevo Grupo
-------------------------

----

Contrato
-------------------------

----

Gobernanza Financiera vía Contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Aislamiento Financiero de los Recursos Computacionales
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Aislamiento Lógico de Recursos Computacionales
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Relacionar *Budget* al Contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Budget*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Accediendo al *Budget*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creando *Budget* y *Sub-Budget*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Intervalo Trimestral
""""""""""""""""""""

----

Intervalo Semestral
""""""""""""""""""""

----

Intervalo Anual
""""""""""""""""""""

----

Intervalo Mensual
""""""""""""""""""""

----

Editando Budget 
~~~~~~~~~~~~~~~~~

----

Visualizando el Informe de Costos de `Budgets`
~~~~~~~~~~~~~~~~~

----

Visualizando Contrato
~~~~~~~~~~~~~~~~~

----

Sección: General
""""""""""""""""""

----

Sección: Reglas de Facturación
""""""""""""""""""""""""""""""""""""

----

Sección: Categorías de Precio
""""""""""""""""""""""""""""""""""""

----

Sección: Políticas de Alertas
""""""""""""""""""""""""""""""""""""

----

Sección: Precio de los Recursos - Contrato
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Cuota del Contrato
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Contacto Primario
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Administradores
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Datos de la Empresa
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Virtual Datacenters Concedidos
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Usuarios
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Grupos
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Datos de Facturación
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Perfiles de Permisos
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Productos
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Permisos Concedidos
""""""""""""""""""""""""""""""""""""""""""

----

Sección: Perfil de Facturación de Container
""""""""""""""""""""""""""""""""""""""""""

----

Aprovisionamiento de Contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Menú Configuración
=====================

----

General
--------

----

Sección: General
~~~~~~~~~~~~~~~~~~~

----

*Card*: Sincronizar *Active Directory*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Aplicar perfiles
"""""""""""""""""

----

Sección: Precio de los Recursos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear un costo estándar del sistema
"""""""""""""""""""""""""""""""""""""

----

Sección: Configuraciones de Usuario *LDAP Server*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Seção: *Upload* de Termo de Responsabilidade
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Consola
-------

----

*Card*: Controladores de consola
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear controlador de consola
"""""""""""""""""""""""""""""

----

Red
-----

----

Sección: Configuraciones de Red
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Card*: Controladores SDN
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creando SDN controlador
"""""""""""""""""""""""

----

Subredes públicas
-------------------

----

*Card*: Subredes públicas
~~~~~~~~~~~~~~~~~~~~~~~~

----

Actualizar
""""""""""

----

Añadir Subred
""""""""""

----

Suscripciones
---------------

----

*Card*: Suscripciones
~~~~~~~~~~~~~~~~~~~~~~

----

Creando Suscripción
""""""""""""""""""""

----

Flavor Billing Profile
-----------------------

----

Creando Flavor Billing Profile
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Perfiles de Permiso
---------------------

----

Visualizar y Editar Perfil de Permisos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creando Perfil de Permiso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Perfiles de Visualización
-----------------------------

----

Creando Perfil de Visualización
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Editando Perfil de Visualización
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Billing Admin
---------------

----

Administración de Billetaje
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Lanzar Accountant
"""""""""""""""""

----

Gestionar cachés
"""""""""""""""""

----

Etiquetado de Recursos USN
---------------------------

----

Creación de un Etiquetado de Recursos USN
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Gestión de Cuentas
------------------------------

----

*Card*: Lista de *Tiers*
~~~~~~~~~~~~~~~~~~~~~~

----

Crear *Tier*
""""""""""

----

Sección: Lista de Paquetes
~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Paquete
""""""""""""

----

*Card*: Lista de Cuentas
~~~~~~~~~~~~~~~~~~~~~~~

----

Editar Paquete
"""""""""""""

----

Añadir y eliminar *Tiers*
"""""""""""""""""""""""""

----

Configuración de Ambiente
------------------------------

----

*Card*: Configuración de ambiente
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Añadir configuración
""""""""""""""""""""""

----

Sección: Elementos ocultos
~~~~~~~~~~~~~~~~~~~~~~~~

----

Añadir configuración
""""""""""""""""""""""

----

*Card*: Elementos de exhibición
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Añadir configuración
""""""""""""""""""""""

====

Menú Seguridad
==============

----

Tickets (nuevo)
----------------

----

Llamadas de procesos
~~~~~~~~~~~~~~~~~~~~~

----

Botón: Abrir llamada
""""""""""""""""""""

----

Botón: Calendario
""""""""""""""""""""

----

Botón: Búsqueda
""""""""""""""""""""

----

*Card*: Llamadas abiertas - urgente
""""""""""""""""""""

----

*Card*: Llamadas abiertas
""""""""""""""""""""

----

*Card*: Llamadas cerradas
""""""""""""""""""""

----

Informe de llamadas
~~~~~~~~~~~~~~~~~~~~~~~~

----

Dashboard de Servicios
""""""""""""""""""""""""

----

Botón: Calendario
""""""""""""""""""""""""

----

Botón: Búsqueda
""""""""""""""""""""""""

----

Assessments (nuevo)
----------------------

----

Auto assessment
~~~~~~~~~~~~~~~

----

*Card*: Modelos
"""""""""""""""""

----

Modelos de Auto assessment
"""""""""""""""""

----

Crear nuevo Modelo
"""""""""""""""""

----

*Card*: Clientes
"""""""""""""""""

----

Crear nuevo Cliente
"""""""""""""""""

----

Listando Cliente
"""""""""""""""""

----

Asociando modelo al Cliente
"""""""""""""""""

----

Status de los formularios de Auto assessment
""""""""""""""""""""""""""""""""""""""""""""

----

Generando gráficos de visualización
""""""""""""""""""""""""""""""""""""""""""""

----

CIS Control (nuevo)
~~~~~~~~~~~~~~~~~~

----

*Card*: Assessment
"""""""""""""""""""

----

Nuevo Assessment
"""""""""""""""""""

----

*Ethical Phishing*
----------------------

----

Acceso del usuario: Gestor Admin
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

**Dashboard del Gestor Admin**
""""""""""""""""""""""""""""""

----

**Mi Dashboard** 
""""""""""""""""""""""""""""""

----

**Dashboard Global de Contratos**
""""""""""""""""""""""""""""""

----

**Dashboard del Contrato**  
""""""""""""""""""""""""""""""

----

**Contratos**
""""""""""""""""""""""""""""""

----

**Usuarios**
""""""""""""""""""""""""""""""

----

**Campañas**
""""""""""""""""""""""""""""""

----

**Contactos**
""""""""""""""""""""""""""""""

----

**Modelos**
""""""""""""""""""""""""""""""

----

**Perfiles de envío**
""""""""""""""""""""""""""""""

----

**Landing Pages**
""""""""""""""""""""""""""""""

----

Acceso del usuario: *User*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

**Accediendo**
"""""""""""""""

----

**Dashboard del usuario User**
"""""""""""""""

----

**Mi Dashboard**
"""""""""""""""

----

**Dashboard del Contrato**
"""""""""""""""

----

**Campañas**
"""""""""""""""

----

**Contactos**
"""""""""""""""

----

**Modelos**
"""""""""""""""

----

**Landing Pages**
"""""""""""""""

----

Menú Máquinas Virtuales
======================

----

Introducción
--------------

----

Accediendo a una Máquina Virtual
--------------

----

Gestionando una Máquina Virtual
--------------

----

Sección General: Máquinas Virtuales
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Sección: Rendimiento Instantáneo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Sección: Metrics (exclusivo **AWS**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Sección: Interfaces de Red
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Sección: Disco
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Sección: Snapshots
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Sección: Signatures (**Exclusivo Azure y Google Cloud Platform**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Sección: Historial de Rendimiento (**Exclusivo Azure y GCP**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creando una Máquina Virtual
--------------------------------

----

*Wizard* Etapa 1 (Selección de la Nube)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Wizard* Etapa 2 (Informaciones básicas de la máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Wizard* Etapa 3 (Informaciones básicas de la máquina virtual - continuación)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Wizard* Etapa 4a (Informaciones de seguridad de la máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Wizard* Etapa 4b (Informaciones de seguridad - Exclusivo Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Wizard* Etapa 5a (User data)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Wizard* Etapa 5b (**User data VMware**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Wizard* Etapa 6 (Visualizar las configuraciones de la máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Menú Orquestador
=================

----

Cluster
------------------

----

Cluster Service
~~~~~~~~~~~~~~~~

----

Menú Scaling Groups
===================

----

Creando un Scaling Group
----------------------------

----

Creando un Scaling Group AWS
----------------------------

----

Problemas conocidos con el Grupo de Escalabilidad de AWS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creando un Scaling Group Azure
--------------------------------

----

Creando un Scaling Openstack
--------------------------------

----

Creando un Scaling vCloud
--------------------------------

----

Menú Base de Datos
===================

----

Gestionando una Base de Datos
-----------------------------

----

Sección General: Grupo de Seguridad
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Sección: Grupos de Seguridad
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Aprovisionando una Base de Datos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creación de Base de Datos (MySQL y AWS)
---------------------------------------

----

Etapa 1 - Selección del proveedor de Servicios de Nube (AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 2 - Selección de la Base de Datos (MySQL y AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 3 - Especificaciones de la Base de Datos (MySQL y AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 4 - Configuraciones de acceso a la Base de Datos (MySQL y AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 5 - Especificaciones de Red y Seguridad (MySQL y AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 6 - Parámetro de Copia de Seguridad (MySQL y AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creación de Base de Datos (MySQL y Azure)
-----------------------------------------

----

Etapa 1 - Selección del Proveedor de Servicios de Nube (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 2 - Selección de la Base de Datos (MySQL y Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 3 - Especificaciones de la Base de Datos (MySQL y Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 4 - Configuraciones de acceso a la Base de Datos (MySQL y Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 5 - Especificaciones de Red y Seguridad (MySQL y Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 6 - Parámetro de Copia de Seguridad (MySQL y Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creación de Base de Datos (MySQL y GCP)
---------------------------------------

----

Etapa 1 - Selección del proveedor de Servicios de nube (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 2 - Selección de la Base de Datos (MySQL y GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 3 - Especificaciones de la Base de Datos (MySQL y GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 4 - Configuraciones de acceso a la Base de Datos (MySQL y GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 5 - Especificaciones de Red y Seguridad (MySQL y GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Etapa 6 - Parámetro de Copia de Seguridad (MySQL y GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Menú Virtual Datacenters
========================

----

Gestionando Virtual Datacenters
---------------------------------

----

**Sección: General**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Regiones**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Redes**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Par de Claves**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Grupo de Seguridad**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Modelos**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Flavors**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Storages**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Catálogo**
~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Balanceadores**
~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Bases de datos**
~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

**Sección: Máquinas virtuales**
~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Editando un Virtual Datacenter
------------------------------

----

Creando un Virtual Datacenter
------------------------------

----

Menú Financiero
===============

----

Empresas Privadas
-----------------

----

Empresas Públicas (USN)
------------------------

----

Ambiente Corporativo
-----------------------

----


**Reglas Financieras**
------------------------

----

Regla de Facturación
~~~~~~~~~~~~~~~~~~~~



----

**Informes**
----------------

----

Paneles Basados en el Consumo
-------------------------------

----

Informe de Historial de Servicio
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este informe permite al administrador de costos seguir la evolución (mensual, semanal o diaria) de los costos de cada ``Product Name`` registrado en el proveedor de servicios de nube pública. Estos costos son separados en costos con y sin etiquetas (*tags*).

El recurso de etiquetas (*tag*) es la forma más usual y la indicada por el proveedor de servicios de nube pública para que las empresas apliquen alguna identificación a los costos recurrentes de su infraestructura de nube pública. Cada proveedor posee sus características específicas sobre qué servicios o productos **no se permite** aplicar etiquetas (*tags*), es decir, no es posible etiquetar (*tag*) todos sus servicios y productos.

La característica de *no permitir vincular etiquetas (tags)* en todos sus productos puede llevar las empresas a un error conceptual para la aplicación y distribución de costos por departamentos, centros de costos, proyectos o cualquier otra aplicación para las etiquetas (*tags*).

Así, la plataforma uCloud presenta, especifica y segrega la suma de los valores de cada ``Product Name`` de los proveedores de servicios de nube pública, de forma que el administrador de costos de las empresas pueda identificar correctamente los totales con y sin etiquetas (*tags*).

En un enfoque de trabajo de FinOps, todo empieza por identificar cuáles son los recursos que más consumen. En este caso, desde el menú del historial de servicios, el cliente puede visualizar el listado de los recursos que más se consumen en su factura. Están agrupados por ``ProductName`` y por ``Product Family``.

Al seleccionar la opción del menú HISTORIAL DE SERVICIO, se solicita elegir un Contrato, en la secuencia el tipo de ``Intervalo`` y el ``Periodo``, a través de este informe es posible analizar los costos de forma detallada, como se muestra en las imágenes a continuación.

Cuando se selecciona este informe, la plataforma uCloud presenta la pantalla siguiente, en la que el usuario debe introducir o seleccionar un único contrato:

.. image:: /figuras/fig_his_spa/001_historial_servicio_listato_contratos.png
   :alt: Menu Financeiro - Histórico de Serviço
   :align: center

----

* **Contrato**: La plataforma uCloud muestra una lista únicamente de los contratos a los que el usuario está vinculado, y el usuario debe introducir o seleccionar un único contrato a la vez. Al seleccionar el contrato deseado, la plataforma uCloud presenta la pantalla siguiente:

.. image:: /figuras/fig_his_spa/002_historial_facturación_pantalla_inicial.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

A continuación se describen los campos para la presentación de este informe:

* **Intervalo**: Este campo es del tipo "dropdown" y el usuario puede seleccionar el periodo ideal para evaluar los datos de consumo de su ambiente. Al realizar un análisis comparativo mensual, el cliente puede comprender cómo evoluciona su factura a lo largo del tiempo, de acuerdo con la facturación del proveedor. Al hacer clic con el cursor del ratón en ``Intervalo``, la plataforma uCloud presenta las opciones:
  
  * **MENSUAL**: Cuando se selecciona el análisis mensual, el cliente puede comprender cómo evoluciona su factura a lo largo del tiempo, según la facturación del proveedor. Esta vista permite comprender el consumo de productos según la factura del cliente. 
  
     En el ejemplo siguiente, al seleccionar el campo ``Período`` y, a continuación, ``Mensual``, el calendario con los meses pasa a estar disponible para selección. Es posible seleccionar un mínimo de 1 mes y un máximo de todos los meses del año. Para ejemplificar, hemos seleccionado los 3 últimos meses, como se muestra en la siguiente imagen.

.. image:: /figuras/fig_his_spa/003_historial_servicio_calendario_mensual.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

* **SEMANAL**: Este filtro permite obtener una visión más granular del consumo, permitiendo comprender e identificar picos de consumo en semanas a lo largo de los meses. En este caso, puede generar indicaciones de aplicaciones o comportamientos que generan picos de consumo en una semana determinada y no en otra. 
     
     Es importante tener en cuenta que por el momento la plataforma uCloud sólo trabaja con el concepto de semanas cerradas del mes (de domingo a sábado). Estas semanas se numeran secuencialmente del 1 al 52 y se presentan en la parte izquierda del calendario. El campo ``Período`` muestra el calendario ``Semanal``. Como se muestra en la siguiente imagen:

.. image:: /figuras/fig_his_spa/004_historial_servicio_calendario_semanal.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

* **DIARIO**: Este filtro permite obtener una visión con la menor granularidad de periodo posible. Esto permite comprender e identificar los picos de consumo a lo largo de los días. En este caso, puede generar indicaciones de aplicaciones o comportamientos que muestran picos de consumo en un día determinado y no en otro. El campo ``Periodo`` muestra el calendario ``Diario``. Como se muestra en la siguiente imagen:


.. image:: /figuras/fig_his_spa/005_historial_servicio_calendario_diario.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

* **Periodo**: Este es un campo obligatorio, la plataforma uCloud cambia este campo después de que el usuario seleccione el periodo en el campo anterior.

* **Container**: Este es un campo obligatorio del tipo "dropdown”, cuando el usuario hace clic con el cursor del ratón, la plataforma uCloud muestra una lista de todos los containers aprovisionados a los que el usuario está vinculado para uso.

* **Linked Account**: El término Containers en la plataforma uCloud se utiliza para representar un ambiente de nube, ya sea público y/o privado. Un container es una abstracción lógica para agrupar todos los recursos (máquinas virtuales, servidores, discos, storages) de un determinado tipo de hypervisor. Todos los proveedores adoptan una estructura organizacional **lógica** para crear su ambiente de totalización de costos. 
    
    Para la plataforma uCloud, se aprovisiona un **Container**, que puede ser la cuenta "**RAÍZ**" de la empresa. La plataforma uCloud denomina "**Sub Account**" a las subdivisiones de esta cuenta principal (Unidades Organizacionales o Cuentas Hijas, entre otras), ésta permite que las empresas puedan crear para asignar los costos de computación de nube para diferentes unidades o centros de costos. Este campo es del tipo "dropdown" y lista todas las *Sub Accounts* que han sido aprovisionadas para la cuenta raíz, como se muestra en la siguiente imagen:

.. image:: /figuras/fig_his_spa/006_historial_servicio_linked.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

* **Botón Filtrar**: El usuario debe pulsar con el cursor del ratón sobre este botón ``Filtrar`` una vez rellenados todos los filtros deseados, en ese momento la plataforma uCloud procesa las informaciones almacenadas en sus bases de datos y presenta el informe en pantalla. A continuación se muestra una pantalla para ilustrar **como simple ejemplo** el resultado tras el procesamiento para la visualización del informe:

.. image:: /figuras/fig_his_spa/007_historial_servicio_filtro.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

Dentro del HISTORIAL DE SERVICIO se encuentra el cuadrante "Valor Total" que muestra el consumo de la nube para el mes seleccionado en los campos de filtro.

Con esta información es posible tener una visión de cómo se comporta el ambiente, de modo que el usuario puede empezar a elaborar una estrategia para encontrar formas de optimización. 

A continuación se analiza en profundidad cómo se distribuyen estos costos entre los productos de la nubes.

* **Sección Gráficos Históricos de Costos por Categoría**:

En el cuadrante "Historial de costos por categoría", el panel presenta un gráfico para cada mes seleccionado y la relación de todos los servicios de la nube, referido también como ``Product Name`` respectivo de cada proveedor de servicios de nube pública.

Siguiendo el patrón de nomenclatura de cada una de las nubes, las barras muestran cuánto se gastó y cuánto el servicio representa en el consumo total de la factura. Al pasar el ratón por encima de las barras, el panel presenta el nombre del producto y sus respectivos gastos, como se muestra en la imagen siguiente:

.. image:: /figuras/fig_his_spa/008_historial_servicio_costos_categoria.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

La presentación estos gráficos por parte de la plataforma uCloud es un gráfico de barras superpuestas (*Stacked Columns*).

* **Configuraciones del Gráfico**: es una pestaña ubicada en la parte inferior de la pantalla en la que el usuario puede personalizar la forma de presentación de estos gráficos. Basta con hacer clic con el cursor del ratón en la *pestaña* y la plataforma uCloud muestra las opciones de configuración:

.. image:: /figuras/fig_his_spa/009_historial_servicio_configuración_gráfico.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

* **Sección Visualización de Datos por Costos**:

En el cuadrante de visualización de datos por costo, el panel muestra los artículos de servicio (PRODUCT NAME) y junto a ellos los meses elegidos con sus respectivos gastos totales separados en dos categorías, COBROS DIRECTOS y COBROS INDIRECTOS, como se muestra en la pantalla de ejemplo a continuación:

.. image:: /figuras/fig_his_spa/010_historial_servicio_cobros.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

* **Cobros Directos**: La categoría ``Directos`` es la suma de los valores de todos los productos y/o servicios a los que el proveedor de servicios de nube pública **permite SÍ vincular** alguna forma de identificación, o etiqueta (*tag*), que vinculada a los recursos computacionales por el propietario de los recursos es la forma más usual para la identificación y asignación de los valores recurrentes entre departamentos, centros de costos, proyectos, iniciativas.

* **Cobros Indirectos**: La categoría ``Indirectos`` es la suma de los valores de todos los productos y servicios que los proveedores de servicios de la nube pública **NO PERMITEN/ACEPTAN** que sean marcados con cualquier tipo de etiqueta (*tag*) para ser vinculados a los recursos computacionales por el propietario del recurso (s). Cada proveedor de servicios en la nube pública tiene su especificación sobre qué productos y servicios no se pueden marcar.

La información explícitamente segmentada y presentada en forma de este informe puede apoyar la toma de decisiones (*insights*) para alinear la distribución de costos internamente en la empresa (*charge back*). Esta presentación se apoya en las mejores prácticas de *FinOps* para identificar correctamente los costos recurrentes de los recursos de computación en nube pública.

.. note:: |nota| El objetivo de este informe no es presentar las respectivas etiquetas (*tags*) en el cuerpo del informe, sino presentar al administrador de costos el total de los valores identificables por departamento, centro de costos y proyecto asignados mediante etiquetas (*tag*). La plataforma uCloud permite al administrador de costos consultar los valores por etiqueta (*tag*) en diversos otros informes financieros.

----

Informe de Costos Cadenciados
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este informe presenta la variación del valor de los recursos computacionales de cada servicio ``Product Name`` y muestra la variación de sus valores en el mes en curso comparado únicamente con los valores del mes anterior. La plataforma uCloud no permite cambiar la visualización a otros meses.

Además, la plataforma uCloud muestra la variación de los valores de los recursos computacionales en dos cuadros diferentes:

A. *Un primer cuadro* donde se muestra la variación de valores con el periodo que va desde el primer día del calendario (día 01) del mes en curso hasta el día en que el usuario está consultando este informe en la plataforma uCloud (en los ejemplos ilustrativos en las pantallas mostradas = día 26).

B. *Un segundo cuadro* que muestra la suma del valor total del consumo de todo el mes anterior y la **previsión** para el cierre del mes en curso (aunque aún no haya valores en *billing o bucket* de este proveedor de servicios en la nube pública.

  La información relativa a la variación de los valores del mes anterior *en comparación* con el mes en curso permite identificar y visualizar la variación de los valores financieros en comparación con el mes anterior y la **previsión** de los valores de cierre de las facturas para el mes en curso.

  Es importante destacar que, aunque no existan datos de *billing o bucket* por parte del proveedor de servicios de nube pública, la plataforma uCloud utiliza un algoritmo que proyecta los valores (aunque estos no existan), basándose en el consumo medio de los últimos seis (06) meses almacenado en las bases de datos internas de la plataforma uCloud.

La visualización de este informe permite identificar y visualizar los distintos tipos de costos -tanto los normalmente previstos así como los estacionales o imprevistos- para el cierre del mes. Este informe permite identificar y proyectar una mejor asignación del flujo de caja contable de la empresa.

Es importante mencionar que en todas las pantallas de los informes presentados en este documento, los valores están siendo convertidos en moneda Real Brasileño (R$) - a pesar de que el proveedor almacene los valores en Dólares Americanos. El valor de la Tasa de Conversión Dólar <> Real está indicado en el Contrato en la sección *Reglas de Facturación*.

* **Contrato**: La plataforma uCloud muestra una lista únicamente de los contratos a los que el usuario está vinculado; el usuario debe introducir o seleccionar un solo contrato a la vez. Cuando selecciona el contrato que desea, la plataforma uCloud muestra la pantalla siguiente:

.. image:: /figuras/fig_costos_cadenciados_spa/001_costos_cadenciados_listado.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

En el momento en que se selecciona el contrato, la plataforma uCloud inicia el procesamiento y el cálculo de los valores almacenados en su base de datos interna y presenta la pantalla del informe. La figura siguiente es meramente ilustrativa y sirve solo como ejemplo:

.. image:: /figuras/fig_costos_cadenciados_spa/002_costos_cadenciados_pantalla_inicial.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

A continuación se describen las secciones de este informe.

* **Cuadros de Periodos**: En esta sección se muestran los dos cuadros con las cifras correspondientes al periodo y al mes:

.. image:: /figuras/fig_costos_cadenciados_spa/003_costos_cadenciados_cuadro_general.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

  * **Cuadro Naranja**: Este *primer cuadro* muestra la suma de los costos de todos los recursos computacionales para el período que comienza el primer día de calendario del mes en curso (día 01) hasta el día actual en que el usuario está consultando este informe en la plataforma uCloud (en los ejemplos ilustrativos de las pantallas mostradas = día 26).
     
     En la parte superior de este cuadro, la plataforma uCloud muestra el valor total de los costos del periodo actual. En él se destaca un valor que se refiere al valor del mes en curso descontado (sustraído) de los valores del periodo del mes anterior. En la parte inferior de este cuadro, la plataforma uCloud muestra la suma de los costos de todos los recursos computacionales correspondientes al período del mes anterior.

  * **Cuadro Blanco**: Este *segundo cuadro* muestra la *previsión* del valor para el cierre del mes de los costos de todos los recursos computacionales para el mes en curso (aunque aún no existan valores en *billing o bucket* de este proveedor de servicios de nube pública). Esta *previsión* se obtiene calculando la variación aritmética de los valores de los últimos seis (06) meses almacenados en la base de datos interna de la plataforma uCloud.
  
    Si el usuario está en "Visualizando este informe" en una fecha anterior a la fecha de cierre de la factura, éste se convierte en una previsión. Esta *previsión* puede ser muy concreta si el usuario visualiza este informe en una fecha cercana a la fecha de cierre de la factura (por ejemplo, el 29 del mes en curso). También en este cuadro, la plataforma uCloud destaca un valor que se refiere a los importes del mes en curso descontados (sustraídos) de los valores del mes anterior. En la parte inferior de este cuadro, la plataforma uCloud muestra la suma de los costos de todos los recursos computacionales del mes anterior.

La plataforma uCloud utiliza un icono para indicar la tendencia de estos resultados:

* **Icono de Flecha Arriba** |icone_seta_acima|: Este icono representa un resultado superior (tendencia ascendente) al del mes anterior.
* **Icono de flecha abajo** |icone_seta_abaixo|: Este icono representa un resultado inferior (tendencia descendente) al del mes anterior.
* **Icono Neutro** |icone_neutro|: Este icono representa un resultado igual (tendencia estable) al del mes anterior.

En los casos en que una empresa utilice la plataforma uCloud por un período inferior a seis (06) meses, es posible que no haya suficientes datos de facturación almacenados para calcular estas variaciones - datos insuficientes ya sea en *billing/bucket* del proveedor o en las bases de datos internas. En estas situaciones, la plataforma uCloud puede presentar estos cuadros con valores cero (en blanco), como se muestra en el ejemplo siguiente:

.. image:: /figuras/fig_costos_cadenciados_spa/004_costos_cadenciados_datos_cero.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

.. attention:: |atencao| Esto **no es un error**, significa que: puede no existir valores y/o datos almacenados en las bases de datos internas; o la configuración de acceso al archivo de billing/bucket no está correctamente aprovisionada; o el proceso de cálculo de billing no ha sido realizado/iniciado hasta el momento. En este caso, póngase en contacto con el equipo de soporte de su contrato. Para ayudarle a monitorizar la correcta configuración de sus credenciales en el ambiente del proveedor de la nube pública.

----

* **Sección Top 15 Costo por Grupo**: 


En esta sección, la plataforma uCloud presenta una lista de los quince (15) primeros Grupos que acumulan los mayores valores de costos de recursos computacionales. El número de Grupos presentados está directamente relacionado con la organización de los Grupos aprovisionados en el Contrato de su ambiente en la plataforma uCloud. Es importante tener en cuenta que aunque existan varios Grupos, sólo los quince (15) Grupos que acumulen los valores más altos serán listados en esta sección. La siguiente figura es meramente ilustrativa y sirve sólo como ejemplo:

.. image:: /figuras/fig_costos_cadenciados_spa/005_costos_cadenciados_top15_grupo.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

A continuación se describen las columnas de esta sección:

  * **Grupos**: Esta columna presenta el nombre del (de los) Grupo (s) tal y como ha(n) sido(s) aprovisionado(s) en la plataforma uCloud.
  * **Mes Actual**: Esta columna muestra la suma de los valores de todos los recursos computacionales del proveedor de la nube pública para el mes en curso (actual), que están vinculados a todos los usuarios que forman parte de este Grupo - aunque este informe se consulte en una fecha anterior a la fecha de cierre de la factura.
  * **Último mes**: Esta columna presenta la suma de los valores de todos los recursos computacionales del proveedor de nube pública, del mes inmediatamente anterior al mes en curso (último mes), que están vinculados a todos los usuarios que forman parte de este Grupo - valores del cierre del mes anterior almacenados en las bases de datos internas.
  * **Proyección**: Esta columna presenta la proyección del valor para el mes en curso de todos los recursos computacionales que están vinculados a todos los usuarios que forman parte de este Grupo - aunque este informe sea consultado en una fecha anterior a la fecha de cierre de la factura.
  * **Proyección Δ**: Esta columna muestra la diferencia numérica en el valor financiero para el mes en curso, en comparación con el mes anterior, de todos los recursos computacionales que están vinculados a todos los usuarios que forman parte de este Grupo - aunque este informe se consulte en una fecha anterior a la fecha de cierre de la factura.
  * **Δ%**: Esta columna presenta la diferencia porcentual del valor financiero del mes en curso, con respecto al mes anterior, de todos los recursos computacionales que están vinculados a todos los usuarios que forman parte de este Grupo - aunque este informe se consulte en una fecha anterior a la fecha de cierre de la factura.
  * **Icono de Indicador de Tendencia**: Esta columna presenta un icono que representa la tendencia de la variación de los valores del mes en curso en comparación con el mes anterior.

    * **Icono de Flecha Arriba** |icone_seta_acima|: Este icono representa un resultado superior (tendencia ascendente) al del mes anterior.
    * **Icono de flecha Abajo** |icone_seta_abaixo|: Este icono representa un resultado inferior (tendencia descendente) al del mes anterior.
    * **Icono Neutro** |icone_neutro|: Este icono representa un resultado igual (tendencia estable) al del mes anterior.

----


* **Sección Top 15 Costo por Servicio**: 


En esta sección, la plataforma uCloud presenta la lista de los quince (15) mejores Servicios (*PRODUCT NAME*) del proveedor de servicios de nube pública que han acumulado los valores más altos en el mes en curso.

La cantidad de servicios (*product name*) mostrada está directamente relacionada con la suma total de sus valores acumulados en el archivo *billing* y almacenados en las bases de datos internas de la plataforma uCloud.

.. important:: Es importante mencionar que, aunque exista una amplia diversidad de otros servicios (*product name*), en este apartado sólo se enumeran los quince (15) con los valores más altos.
   
La figura siguiente es meramente ilustrativa y sirve sólo como ejemplo:

.. image:: /figuras/fig_costos_cadenciados_spa/006_costos_cadenciados_top15_servicios.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

  * **Servicios**: Esta columna presenta el nombre de los Servicios (*product name*) tal y como se expresan en el archivo de *billing* del proveedor de servicios de nube pública.
  * **Mes Actual**: Esta columna presenta la proyección de todas las incidencias de este Servicio (*product name*) del proveedor de la nube pública, para el mes en curso (actual) - aunque este informe se consulte en una fecha anterior a la fecha de cierre de la factura.
  * **Último mes**: Esta columna presenta la suma de los valores de Servicios (*product name*) en el proveedor de la nube pública, del mes inmediatamente anterior al mes en curso (último mes) - valores del cierre del mes anterior almacenados en las bases de datos internas.
  * **Proyección**: Esta columna muestra la proyección del valor para el Servicio (*product name*) para el mes en curso - aunque este informe se consulte en una fecha anterior a la fecha de cierre de la factura.
  * **Proyección Δ**: Esta columna muestra la diferencia numérica (*delta*) del valor financiero del mes en curso con respecto al mes anterior, aunque este informe se consulte en una fecha anterior a la fecha de cierre de la factura.
  * **Δ%**: Esta columna presenta la diferencia porcentual (*delta*) del valor financiero del mes en curso con respecto al mes anterior, aunque este informe se consulte en una fecha anterior a la fecha de cierre de la factura.
  * **Icono de Indicador de Tendencia**: Esta columna muestra un icono que representa la tendencia en la variación de los valores del mes actual en comparación con el mes anterior.


    * **Icono de Flecha Arriba** |icone_seta_acima|: Este icono representa un resultado superior (tendencia ascendente) al del mes anterior.
    * **Icono de flecha Abajo** |icone_seta_abaixo|: Este icono representa un resultado inferior (tendencia descendente) al del mes anterior.
    * **Icono Neutro** |icone_neutro|: Este icono representa un resultado igual (tendencia estable) al del mes anterior.

----

* **Sección Exportar Informes**: 

Esta sección, en la parte inferior de la pantalla, permite exportar informes en formato CSV de todos los servicios, consumos y gastos de forma detallada, permitiendo seleccionar intervalos ``Mensual``, ``Semanal`` y ``Diario``, a criterio del usuario.

.. image:: /figuras/fig_costos_cadenciados_spa/007_costos_cadenciados_exportación.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

  * **Botón**  ``Exportación Detallada``: En esta opción, la plataforma uCloud crea un archivo CSV con el nombre CADENCE-DETAILED-NOME_DO_CONTRATO-MES-ANO.CSV compuesto por 8 columnas.

  * **Botón** ``Exportar Servicios``: En esta opción, la plataforma uCloud crea un archivo CSV con el nombre CADENCE-SERVICES-NOME_DO_CONTRATO-MES-ANO.CSV compuesto por 5 columnas. 

.. image:: /figuras/fig_costos_cadenciados_spa/008_costos_cadenciados_informe_delta.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

  * **Botón** ``Exportar Informe Δ``: En esta opción, la plataforma uCloud crea un archivo CSV que muestra la diferencia de consumo de los ``Product Name`` y ``Family Name`` de los provedores con los datos del mes en curso, en comparación con el mes anterior. Con esta información, es posible visualizar cómo se está comportando cada uno de los servicios, pudiendo así tomar acciones de control y cálculo más efectivas y dirigidas al *PRODUCT NAME* de la nube.

  En el archivo CSV, la columna VARIACIÓN MES ANTERIOR % muestra el porcentaje de la variación y la columna VARIACIÓN MES ANTERIOR $ muestra la variación en dólares. Como se muestra en las siguientes imágenes, Financiero/Costo Cadenciado/Intervalo/Periodo/Exportar Informe Detallado.

  La exportación del informe delta se envía por correo electrónico. Si el usuario prefiere ver el informe en pantalla, puede encontrarlo en el cuadrante situado encima de la exportación de informes, que se muestra más arriba.

  Para recibir el informe por correo electrónico, basta introducir una dirección de correo electrónico válida y hacer clic en enviar, como se muestra a continuación:

.. image:: /figuras/fig_costos_cadenciados_spa/009_costos_cadenciados_modal_delta.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :align: center
----

  La plataforma uCloud puede tardar algún tiempo para seleccionar, calcular y enviar este archivo. Pero al final del procesamiento, envía el archivo CSV y confirma el envío con un mensaje pop-up al usuario.

.. note:: En los casos en que el usuario no reciba ningún mensaje de correo electrónico, consulte la carpeta SPAM/Basura con la dirección de correo electrónico de origen *noreply@dominio.com.br*. Algunos sistemas de correo electrónico bloquean los mensajes con "noreply@...", o los reenvían automáticamente a la carpeta SPAM/Basura.


Informe de Costo Relacional de Producto
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Informe de Visualización de Recursos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Informe de Costos de *Budgets*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Informe de Monitoreo de Consumo (IMC)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Accediendo al IMC.v1
""""""""""""""""""

----

Creando el IMC.v1
""""""""""""""""""

----

Siguiendo el *status* en el menú de Tareas
"""""""""""""""""""""""""""""""""""""""""""

----

Habilitación del *download* del IMC.v1
"""""""""""""""""""""""""""""""""""""""""""

----

Visualizando el IMC.v1
"""""""""""""""""""""""""""""""""""""""""""

----


Informes Basados en Límites de Costos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Los informes de límite de costos son aquellos basados en el consumo, implementados con el objetivo de establecer un límite de costo como punto de referencia, para que el usuario pueda monitorear los gastos y, a través de proyecciones, predecir cuándo el consumo total del mes supera este valor de referencia. 

Para acceder a estas nuevas implementaciones de la plataforma uCloud, el usuario de la aplicación debe hacer clic en el menú **“Financiero”** y luego en el submenú **“Informes”**. A continuación se muestran dos clases de paneles, basados en: Consumo y Facturas.


.. figure:: /figuras/fig_lc_spa/001_límite_costos_pantalla_inicial.png
   :alt: Financeiro relatórios acesso painéis
   :align: center

----


El acceso permite consultar los informes correspondientes al mes en curso mediante la introducción del periodo deseado en el campo de búsqueda. Esta visualización permite al usuario mantenerse informado de las previsiones de costo en forma detallada.


El primer tópico **"Paneles Basados en el Consumo"** agrupa los tipos de informes:

 
.. figure:: /figuras/fig_lc_spa/002_límite_costos_paneles_consumo.png
   :alt: Painéis Baseados em Consumo 
   :align: center

----


1. Historial de Servicio;
2. Costo Cadenciado;
3. Costo Relacional de Producto;
4. Costos de Budgets;
5. **Informes Basados en Límites de Costos.**


.. attention:: |atencao| El número de informes mostrados en el menú Financiero, submenú Informes, tópicos "Paneles basados en consumo y factura" puede variar su cantidad de botones de acuerdo al contrato del cliente.


Este registro trata del acceso al botón de opción: **Informes basados en límites de costos**, al hacer clic sobre el mismo se muestran tres nuevos informes para esta modalidad:


  *  A. Límite de Costo por contrato
  *  B. Límite de Costos para Administradores y  
  *  C. Análisis de Riesgos.


.. figure:: /figuras/fig_lc_spa/003_límites_costos_opciones.png
   :alt: Relatórios baseados em limite de custos e análise de risco
   :align: center

----


Definiendo los Informes
"""""""""""""""""""""""""""""""""""""""""""

A continuación se describe cada informe basado en el límite de costo, junto con una breve explicación de cómo utilizarlos:


----

A. Límite de Costos para Administradores
"""""""""""""""""""""""""""""""""""""""""""

El informe de límite de costos para administradores permite que el usuario observe el consumo realizado mes a mes, lo que hace posible ejecutar el monitoreo sobre qué meses se ha excedido el límite de costo definido y representado en la pantalla por una línea punteada.


En la siguiente imagen se puede ver la visualización de este informe con un gráfico de columnas:


.. figure:: /figuras/fig_lc_spa/004_límite_costos_datos.png
   :alt: Gráfico colunas do RLC
   :align: center

----


**Nuevas características:**

La pantalla del "Informe de límites de costos para administradores" se diferencia de los demás informes, ya que es posible realizar todas las operaciones: crear, editar, eliminar y ejecutar. Esto facilita al usuario la realización de las acciones disponibles.

----

**Paso a paso:**

En este punto es informado el paso a paso para la realización de estas acciones en la pantalla de límites de costos.

----

**1. Ejecutando sin guardar**


Para ejecutar el informe sin un límite de costos previamente guardado, presione el botón "Configurar límite de costos" situado en la esquina inferior derecha del *card*, como se muestra en la siguiente imagen:


  
.. figure:: /figuras/fig_lc_spa/005_límite_costos_configurar.png 
   :alt: Configurar limite de custo  
   :align: center

----


En este flujo se abre el modal "Límite de costo dinámico" donde el usuario puede realizar la configuración que desea para **generar** el **Informe de Límites de Costos**.  


La siguiente imagen muestra los espacios que se deben completar.


.. figure:: /figuras/fig_lc_spa/006_límite_costos_pantalla_dinámico.png
   :alt: Limite de custo dinâmico
   :align: center

----
  

A continuación se detalla cada espacio del modal anterior para el relleno:


**Etapas para la Configuración:**


1. El usuario debe indicar un nombre para el límite de costo;
2. Indicar el intervalo, puede ser: mensual, trimestral, semestral o anual;
3. Indicar el valor de referencia;
4. Elegir la moneda deseada, debe ser BRL (Real), USD (Dólar), MXN (Peso Mexicano), EUR (Euro) o COP (Peso Colombiano);
5. Añadir los filtros necesarios: Contrato, Nube, Cuentas vinculadas y Dimensión.



.. figure:: /figuras/fig_lc_spa/007_límite_costos_etapas.png
   :alt: Limite de custo dinâmico
   :align: center

----  


.. important:: |nota| Los filtros de contrato, nube y cuentas vinculadas pueden funcionar juntos, sin embargo, Dimensión debe utilizarse únicamente con otros filtros de Dimensión.


.. figure:: /figuras/fig_lc_spa/008_límite_costos_nube_filtros.png 
   :alt: Selecionar Nuvem
   :align: center

----


El usuario también puede añadir varios filtros al mismo tiempo mediante el *checkbox* situado en el menú desplegable. 


**Detalles de los Intervalos:**


Cada intervalo configura automáticamente su mes inicial y final. La tabla siguiente describe el mes de inicio y fin para cada tipo:


.. figure:: /figuras/fig_lc_spa/009_límite_costos_detalle_intervalos.png 
   :alt: Detalhes dos intervalos 
   :align: center

----


**Procedimientos posteriores a la configuración:**


Tras realizar la configuración, el usuario debe pulsar el botón "Ejecutar", situado en la esquina inferior derecha del modal. Esto inicia el proceso de carga de los datos en la pantalla.


Una vez finalizada la carga, el usuario dispone de un gráfico en el centro de la pantalla con la línea de límite de costo y el costo total del mes, separados por nombre del producto (cuando se utiliza el filtro Contrato y/o Nube) o por nombre de la Dimensión (cuando se utiliza el filtro Dimensión).
  

.. figure:: /figuras/fig_lc_spa/010_límite_costos_procedimientos_posteriores.png
   :alt: Filtrar Dados em tela
   :align: center

----


A continuación se muestran otras tres informaciones:


   1. Costo total por mes y moneda;
   2. Costo por nombre del producto, separado por mes;
   3. Resumen de las configuraciones aplicadas para generar el informe.


El usuario puede observar la siguiente imagen para refinar la visualización del gráfico de arriba:
  

.. figure:: /figuras/fig_lc_spa/011_límite_costos_configuraciones_aplicadas.png
   :alt: Informações extras
   :align: center

----


En la imagen de arriba, el *card* "Configuraciones Aplicadas", permite al usuario hacer clic en "Editar", botón de color naranja situado en la esquina superior derecha. 


Al hacer clic en "Configuraciones aplicadas", se permite al usuario modificar una o varias informaciones para volver a ejecutar el informe.


**Casos en que los datos se presentan de formas diferentes:**


* En el caso de que el filtro sea introducido por Dimensión, la agrupación no se realiza por nombre de producto, sino por cuáles Dimensiones el costo atiende.



.. figure:: /figuras/fig_lc_spa/012_límite_costos_filtro_dimensión.png
   :alt: Filtro por Dimensão 
   :align: center

----
  

* En el caso de que se añaden dos Dimensiones, y haya un costo que abarca ambas. En la sección "Costo por Dimensión", este registro se ingresa como "Consumo de Dimensión por grupo".


.. figure:: /figuras/fig_lc_spa/013_límite_costos_dos_dimensiones.png
   :alt: Consumo de Dimensões por grupo 
   :align: center

----


Para que este conocimiento sea accesible al usuario, se ha introducido un *tooltip* (icono de sugerencia contextual) en cada tipo, que explica el funcionamiento.


.. figure:: /figuras/fig_lc_spa/014_límite_costos_dimensiones_mensaje.png
   :alt: Tootip em Consumo de Dimensões  
   :align: center

----


**2. Guardando una configuración de límite de costo (Creación)**


Para guardar una configuración, es necesario realizar el "Paso a Paso 1", mostrado arriba.


A continuación, el usuario debe buscar el tercer *card* "Configuraciones Aplicadas" y pulsar "Guardar".


De este modo, esa configuración queda guardada para la ejecución del informe.

----


**3. Ejecutando partiendo de una configuración guardada**


Después de realizar el "Paso a Paso 1 y 2", el usuario debe hacer clic en la acción ``Actualizar`` para recargar el listado de configuraciones existentes. El icono para actualización de la pantalla se muestra en la siguiente imagen:


.. figure:: /figuras/fig_lc_spa/015_límite_costos_botón_actualizar.png
   :alt: Atualização da tela botão refresh
   :align: center

----


A continuación, el usuario debe hacer clic en ``Seleccionar un límite de costo`` y aparece una pantalla para seleccionar una configuración guardada a partir de su nombre.

En este escenario, se ofrecen al usuario otras cuatro opciones de "Acciones", que se enumeran a continuación:


   1. Ejecutar;
   2. Editar;
   3. Filtrar por periodo;
   4. Eliminar.
  

.. figure:: /figuras/fig_lc_spa/016_límite_costos_botones.png
   :alt: Botões de ações limite de custo
   :align: center

----


**4. Editando un límite de costo**


Para realizar una edición, el usuario debe seleccionar un límite de costo y pulsar "Editar", el tercer botón de la sección "Acciones".
  

.. figure:: /figuras/fig_lc_spa/017_límite_costos_editar.png
   :alt: Editando limite de custo 
   :align: center

----

En este flujo, se muestra el modal "Edición de límite de costos":


.. figure:: /figuras/fig_lc_spa/018_límite_costos_pantalla_edición.png 
   :alt: Modal Edição
   :align: center

---- 
  

En él, el usuario puede cambiar las configuraciones del límite de costo y guardarlas pulsando el botón "Editar" de la esquina inferior derecha.

----

**5. Eliminando un límite de costo**


Una vez que haya seleccionado un límite de costo, el usuario debe hacer clic en "Eliminar", el cuarto botón de la sección "Acciones":


.. figure:: /figuras/fig_lc_spa/019_límite_costos_botón_eliminar.png 
   :alt: Botão Remover
   :align: center

----

Para finalizar, es necesario actualizar el listado de límites de costos para comprobar si la información ha desaparecido.

----


**6. Filtrando por período**


El usuario debe seleccionar un límite de costo y, a continuación, hacer clic en ``Filtrar por intervalo de tiempo``, el segundo botón de la sección "Acciones", representado por una lupa.

  
.. figure:: /figuras/fig_lc_spa/020_límite_costos_filtrar_intervalo.png 
   :alt: Botão Filtrar Intervalo
   :align: center

----


A continuación se muestra el modal "Búsqueda personalizada por periodo":

.. figure:: /figuras/fig_lc_spa/021_límite_costos_busqueda_personalizada.png 
   :alt: Busca personalizada por período 
   :align: center

----  

En este modal, el usuario puede observar el nombre y el intervalo del límite de costo seleccionado, pudiendo cambiar el mes de inicio del período.


.. figure:: /figuras/fig_lc_spa/022_límites_costos_selecionar_fechas.png
   :alt: Selecionar o período
   :align: center

----  

Después de hacer esta modificación, el usuario puede pulsar ``Ejecutar`` y procesar el límite de costo seleccionado, con los filtros que se encuentren presentes dentro del límite de costo. Sin embargo, ahora en un período de tiempo diferente.


*Reglas:*


   * El usuario sólo puede retroceder hasta el mes en que el límite de costo ha sido creado.
   * No es posible seleccionar el mes inicial como superior al mes actual.

----


**7. Generando proyecciones para los meses siguientes**


En caso de que el usuario seleccione el intervalo trimestral, semestral o anual, se utilizan los meses por delante de este periodo, de forma que se realiza una proyección basada en los últimos 6 (seis) meses de registros.


La figura siguiente muestra este periodo de proyección en el modal "Límite de Costo Dinámico":


.. figure:: /figuras/fig_lc_spa/023_límites_costos_proyecciones.png
   :alt: Cost Threshold dinâmico
   :align: center  

----

Después de cargar las informaciones, es posible observar que, al generar el informe, algunos meses tienen un asterisco **(*)** al lado.
 

.. attention:: |atencao| Este asterisco al lado del mes significa: "Proyección". Se basa en las informaciones de los últimos 6 meses. Por lo tanto, el periodo que aún ocurre puede delinearse mediante la utilización de la base pasada.

   
.. note:: La base de los últimos 6 meses proyecta los meses futuros, que se muestran con un asterisco. 


Además, hay un subtítulo en el gráfico, que informa del periodo de consumo utilizado para generar la proyección.


.. figure:: /figuras/fig_lc_spa/024_límites_costos_proyeccion_mensaje.png
   :alt: Relatório legenda
   :align: center
  
----

Y en las informaciones de costos por nombre de producto o por dimensión, el nombre "proyección" aparece al lado de los meses que fueron generados a través de esta. 

.. figure:: /figuras/fig_lc_spa/025_límites_costo_proyeccion_costo.png
   :alt: Custo por nome do produto
   :align: center

----


.. centered:: Posibles mensajes de error:

----

A continuación se enumeran algunos de los mensajes de error que el usuario puede recibir al ejecutar el informe de límite de costos:


1. **No hay datos que correspondan a este filtro**
  
.. figure:: /figuras/fig_lc_spa/026_límites_costos_no_hay_datos.png 
   :alt: Erro filtro
   :align: center

----


Esto sucede cuando el usuario construye un filtro que no contiene ningún registro que corresponda a estas configuraciones.


2. **Aún no es posible realizar este procesamiento**


.. figure:: /figuras/fig_lc_spa/027_límites_costos_no_es_posible.png
   :alt: Filtrar dados na tela  
   :align: center
  
----


Esto ocurre cuando el usuario utiliza la opción "Filtrar por periodo" e indica un mes posterior al mes actual.

*Sugerencia para evitar este problema*: basta establecer el mes inicial como el mes actual o anterior.


3. **Límite de costo no válido**


.. figure:: /figuras/fig_lc_spa/028_límites_costos_no_válidos.png
   :alt: Limite de custo inválido 
   :align: center

----
  

Ocurre cuando el usuario pulsa ``Eliminar`` y luego pulsa ``Ejecutar`` en el mismo límite de costo que ha eliminado. El usuario no tiene que preocuparse, en 5 segundos el listado se recarga y elimina el límite de costo que fue elegido.

Para evitar este problema, basta pulsar el botón ``Actualizar`` después de la eliminación.


4. **No es posible generar la proyección de costos** 


.. note:: |nota| Se requiere un mínimo de 6 meses de historial de datos.


Ocurre cuando la fecha de finalización del límite de costo es superior al mes en curso y es necesario generar la proyección de costos para el mes futuro y en el momento del procesamiento se constata que no existen 6 meses de datos anteriores para lograr generar esta proyección.


5. **La fecha inicial no puede ser anterior a la fecha de creación**
  

Esto ocurre cuando el usuario hace clic en "Filtrar por periodo" e introduce un mes inicial anterior a la fecha de creación del límite de costo.

.. figure:: /figuras/fig_lc_spa/029_límites_costos_fecha_inicial.png
   :alt: Erro data criação
   :align: center

----


B. Análisis de Riesgos
"""""""""""""""""""""""

El informe de análisis de riesgos permite que a través de un límite de costo guardado se pueda realizar un análisis y exhibir en la pantalla el consumo actual, el consumo previsto para el mes en curso y el riesgo de que el consumo exceda el límite de costo previamente definido.


.. figure:: /figuras/fig_lc_spa/030_límites_costos_riesgos_pantalla_inicial.png
   :alt: Análise de risco
   :align: center

----


**Paso a paso:**


En este punto, es informado el paso a paso para la realización de estas acciones dentro de la pantalla de límite de costo.

----

**1. Ejecutando un análisis de riesgos**


Para realizar el procesamiento, el usuario debe crear un límite de costos en la pantalla "Informe de límites de costos", y a continuación acceder a la pantalla "Análisis de riesgos", donde se enumeran todos los límites de costos guardados.
 

A partir de este punto, es posible seleccionar una o más opciones para procesar el análisis de riesgos en función de la configuración del límite de costo, como se muestra en la imagen siguiente:
  

.. figure:: /figuras/fig_lc_spa/031_límites_costos_riesgos_listado.png 
   :alt: Selecionar limite
   :align: center

----
 
Una vez realizado el procesamiento, el usuario puede visualizar:

* 1. Consumo actual;
* 2. Previsión del consumo actual;
* 3. Límite de costo;
* 4. Riesgo de que el consumo actual supere el límite de costo.


Además, también se muestra el alcance de cada límite de costo, indicando el nombre del contrato al que pertenece, la nube y/o si existen cuentas vinculadas.


Una vez seleccionadas las opciones deseadas, el botón ``Ejecutar`` situado junto al menú desplegable queda disponible para ser pulsado. En este ejemplo, el usuario ha seleccionado las siguientes opciones de límite de costos: anual, mensual, InformeAnual y Semestral/Contrato.


Consulte la imagen de abajo para obtener una mejor visualización:
  
.. figure:: /figuras/fig_lc_spa/032_límites_costos_pantallas_riesgos.png
   :alt: Resultado análise de risco 
   :align: center

----
 

En la imagen anterior es posible observar una escala que contiene el nivel de riesgo. Para comprender mejor los riesgos, el usuario debe hacer clic en el botón situado en la esquina inferior derecha de la pantalla, representado por una flecha blanca que apunta hacia la derecha.

Al pulsarlo, se abre una tabla donde el usuario puede visualizar la descripción de cada tipo de riesgo que puede ser presentado en pantalla. Los riesgos pueden presentarse como:


* No disponible;
* Muy bajo;
* Bajo;
* Moderado;
* Alto;
* Muy alto y
* Extremo.


A continuación se muestran las imágenes para una mejor visualización:

.. figure:: /figuras/fig_lc_spa/033_límites_costos_descripciones.png
   :alt: Legenda de risco
   :align: center


.. figure:: /figuras/fig_lc_spa/034_límites_costos_descripciones_detalles.png
   :alt: Legenda de risco expandida
   :align: center

----
 
A medida que se pasa de un nivel a otro, los colores cambian. El riesgo no disponible no presenta ningún color, mientras que los riesgos bajo y muy bajo se muestran en verde. 

Los riesgos moderado y alto se muestran en amarillo, mientras que los riesgos muy alto y extremo se muestran en rojo.

----

**2. Generar informe de límite de costo partiendo del análisis de riesgos**

Una vez realizado el procesamiento del análisis de riesgos, el usuario puede hacer clic en el icono del gráfico situado en la esquina superior derecha del *card* generado mediante el resultado. 
  
.. figure:: /figuras/fig_lc_spa/035_límites_costos_detalles.png
   :alt: Visualizar limite
   :align: center

----

De este modo, pasa a la pantalla de informe de límites de costos, donde se procesa automáticamente el límite de costos seleccionado.

----

**3. Generar análisis de riesgos partiendo del informe de límites de costo**


Después de que el usuario haya ejecutado un límite de costo ya guardado, aparece una nueva opción en la sección "Configuraciones aplicadas", donde el usuario es redirigido a la pantalla de análisis de riesgos, procesando automáticamente a partir del límite de costo procesado.

  
.. figure:: /figuras/fig_lc_spa/036_límites_costos_generar_analisis.png
   :alt: Visualizar como análise de risco
   :align: center

----

Paneles Basados en Facturas
-----------------------------

----

Mi Factura
~~~~~~~~~~~~

----

Financiero
~~~~~~~~~~~~

----

Informe Consolidado de Facturación (ICF)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta opción de submenú permite al usuario consultar informes de consumo, que posibilitan el gobierno de costos de los recursos computacionales de nube, de forma muy granular y con presentación de valores en Unidad de Servicio de Nube (USN).

.. attention::  |atencao| Unidad de Servicio de Nube (USN) es un modelo de fijación de precios para servicios de nube, asignado a las entidades y agencias que integran la esfera gubernamental brasileña. Pretende establecerse como un método previsible, lineal y flexible para la obtención de un importe específico cobrado por los servicios de computación en nube.

----

Accediendo al ICF
""""""""""""""""""

Para acceder al informe, el usuario debe hacer clic en “Financiero”, situado en el menú de funcionalidades de la parte izquierda de la pantalla, y después hacer clic en “Informes”.

Cuando el usuario selecciona esta opción, la plataforma uCloud muestra la siguiente pantalla:

.. image:: /figuras/fig_icf_spa/001_informes_consolidado.png
   :alt: seleccionar menú financiero
   :align: center
----

Como en el ejemplo anterior, observamos que el menú financiero está dividido en dos grupos: "Paneles Basados en el Consumo" y "Paneles Basados en Facturas", el Informe Consolidado de Facturación se encuentra en el segundo grupo.

.. image:: /figuras/fig_icf_spa/002_icf_pantalla_inicial.png
   :alt: pantalla inicial menú financiero
   :align: center
---- 

.. image:: /figuras/fig_icf_spa/003_icf_pantalla_selección.png
   :alt: pantalla selección
   :align: center
----  

Al hacer clic en el botón correspondiente, la plataforma uCloud presenta la siguiente pantalla:

.. image:: /figuras/fig_icf_spa/004_icf_historial_facturación.png
   :alt: pantalla inicial
   :align: center
----

----

Seleccionando el ICF
""""""""""""""""""""

El usuario puede seleccionar un periodo y un contrato para buscar el historial de facturas, al hacer clic en el campo de **inserción de fecha**, la plataforma uCloud entrega una pantalla con un calendario, para que se pueda seleccionar el periodo deseado (en este, es posible desplazarse por meses y años pasados), después de seleccionada la fecha, los botones disponibles para el usuario son: ``Cancelar`` y ``Aplicar``:


* Botón ``Cancelar``: Puede ser utilizado por el usuario, si quiere desistir de la selección.
* Botón ``Aplicar``: Debe ser pulsado después de seleccionar el periodo de búsqueda.

.. image:: /figuras/fig_icf_spa/005_icf_historial_fecha.png
   :alt: seleccionar fecha
   :align: center
----

En el campo para buscar el contrato deseado, se muestran todos los contratos registrados en la plataforma. Según la demanda, se puede realizar una búsqueda completa pulsando la opción ``Seleccionar todos`` o una búsqueda dirigida, donde el usuario simplemente elige los contratos de su interés.

.. image:: /figuras/fig_icf_spa/006_icf_historial_listado.png
   :alt: seleccionar contrato
   :align: center
----

El Informe Consolidado de Facturación dispone de 5 tipos de filtros, que pueden ser utilizados por el usuario, estos son:

  1. ID de la Propuesta
  2. CR
  3. Número de contrato
  4. Número OC 
  5. Producto

.. image:: /figuras/fig_icf_spa/007_icf_historial_filtros.png
   :alt: filtros 
   :align: center
----

Los filtros elegidos por el usuario permanecen rellenos en “naranja”, si no se selecciona ningún filtro, las opciones aparecen sin marcas. En el ejemplo siguiente, el usuario ha seleccionado los filtros *ID de la Propuesta* y *Número de contrato*.

.. image:: /figuras/fig_icf_spa/008_icf_historial_filtros_selecionados.png
   :alt: filtros seleccionados
   :align: center
----

Una vez finalizada la selección de los datos para el Informe Consolidado de Facturación, se debe pulsar el botón ``Buscar``. 

.. image:: /figuras/fig_icf_spa/009_icf_historial_selección_contratos.png
   :alt: botón buscar
   :align: center
----

Si el usuario desea rehacer la búsqueda, sólo tiene que hacer clic en el botón ``Volver`` y reiniciar todo el proceso.

.. attention:: |atencao| En la esquina superior derecha están los iconos de las opciones de abrir y cerrar facturas.

En el recorte de la esquina superior derecha de la pantalla, la siguiente imagen muestra el icono accionado «Abrir todas las facturas».

.. image:: /figuras/fig_icf_spa/010_icf_historial_generar_facturas.png
   :alt: abrir todas las facturas
   :align: center
----

Estas opciones permiten al usuario determinar ambas acciones en el periodo deseado sobre todos los contratos existentes que pueden ser investigados, individualmente o en conjuntos específicos.

Al habilitar la apertura de la factura, el modal es exhibido:

.. image:: /figuras/fig_icf_spa/011_icf_historial_abrir_factura.png
   :alt: abrir factura
   :align: center
----

Después que el usuario selecciona los campos de acuerdo con lo deseado, el contrato y el mes, el botón ``Abrir Facturas`` se habilita para ser pulsado, así la operación es realizada.

Al habilitar el cierre de la factura, el modal es presentado:

.. image:: /figuras/fig_icf_spa/012_icf_historial_cerrar_factura.png
   :alt: cerrar factura
   :align: center
----

Una vez que el usuario selecciona los campos según el contrato y mes deseados, el botón ``Cerrar Facturas`` se habilita para ser pulsado, así se realiza la operación.

En cualquier momento se puede pulsar el botón ``Cancelar``, en los dos casos detallados anteriormente.

----

Siguiendo la consulta del ICF
""""""""""""""""""""""""""""""""""""

Al hacer clic en buscar, el usuario debe esperar que la plataforma uCloud obtenga las informaciones solicitadas, esta acción puede tomar algunos minutos conforme el ejemplo siguiente.

.. image:: /figuras/fig_icf_spa/013_icf_historial_busqueda.png
   :alt: esperando la búsqueda
   :align: center
---- 

Una vez finalizada la búsqueda, si no hay informaciones relacionadas con las selecciones de los filtros, la plataforma uCloud informa que no hay historial de facturación para el contrato en el período informado.

.. image:: /figuras/fig_icf_spa/014_icf_nohaydatos.png
   :alt: no hay datos
   :align: center
---- 

En la existencia de informaciones, la plataforma uCloud evoluciona hacia dos tipos de escenario:

1. En la evolución del filtrado y la búsqueda de datos, el número y el nombre de los contratos existentes que presentan un fallo en la búsqueda de los valores se muestran en la parte izquierda de la pantalla y aparecen en rojo, como en el ejemplo:

.. image:: /figuras/fig_icf_spa/015_icf_contratos_fallados.png
   :alt: contratos fallados
   :align: center
----  

.. attention:: |atencao| Usuario, si esto ocurre en tu búsqueda, por favor, póngase en contacto con el soporte de la plataforma uCloud.

2. Siguiendo el flujo de búsqueda de datos, se listan los contratos encontrados.

.. image:: /figuras/fig_icf_spa/016_icf_listado_contratos.png
   :alt: listado de contratos
   :align: center
---- 

----


Listado de contratos en el ICF
""""""""""""""""""""""""""""""""""""

Tras cargar las informaciones, la plataforma muestra la lista de los contratos encontrados según la búsqueda realizada por el usuario, la pantalla exhibe ocho columnas:

  * el nombre de dichos contratos;
  * sus periodos de consumo;
  * el mes de facturación;
  * la fecha de cierre;
  * su *status* (Cerrado o Abierto); 
  * precio; 
  * Precio en dolar 
  * Acciones.

Esta última columna: "Acciones", incluye los 6 botones listados a continuación, según la siguiente imagen:

   * Ver detalles
   * Bajar Velocloud
   * Abrir Factura 
   * Cerrar Factura
   * En la pantalla
   * Bajar

.. image:: /figuras/fig_icf_spa/017_icf_botones.png
   :alt: botones de acción
   :align: center
----

Si la lista de contratos es demasiado larga, la funcionalidad de la barra de desplazamiento permite al usuario navegar hacia arriba y hacia abajo a lo largo de toda la pantalla.

.. image:: /figuras/fig_icf_spa/018_icf_pantalla_detalles.png
   :alt: listando contratos
   :align: center
----  

A continuación se muestra las informaciones detalladas de esta pantalla:

* **Total**: Valor total de la facturación de los contratos investigados. La plataforma uCloud convierte automáticamente los valores de USN a Real (R$), lo que permite al usuario evaluar el valor en moneda local.
* **Botón** ``Exportar``: Este botón permite al usuario exportar las informaciones de todos los contratos filtrados, en formato de tabla MS-Excel (.xlsx). La plataforma uCloud descarga el archivo en la máquina del usuario y exporta las informaciones con el nombre “*invoices.xlsx*” en el directorio/*folder* configurado en las opciones del navegador que el usuario está utilizando.

.. image:: /figuras/fig_icf_spa/019_icf_exportar.png
   :alt: botón exportar
   :align: center
----  

En este flujo se detallan las columnas de la pantalla "Listado de contratos":

* **Contrato**: Presenta el(los) nombre(s) del(de los) contrato(s) filtrado(s) en la búsqueda.
* **Período de Consumo**: Presenta la fecha de inicio y fin del mes para el que se contabiliza el valor financiero del contrato. También muestra la hora de inicio y fin de cada uno de los datos enumerados. El periodo de consumo es siempre anterior al mes de facturación. 
* **Mes de Facturación**: Informa el mes en el que vence y debe pagarse la factura. Siempre es el mes siguiente al mes del periodo de consumo.
* **Fecha de Cierre**: Esta columna indica al usuario si la factura está abierta o cerrada. Para los contratos que presentan el *status* "Abierto", se muestra el icono "tooltip", que llama la atención del lector sobre el mensaje: *“No se informó la fecha de cierre de su factura porque aún está abierta”*, (que se muestra en el siguiente ejemplo). Los contratos que presentan el *status* “Cerrado”, en cambio, muestran la fecha y hora de cierre de la factura.

.. image:: /figuras/fig_icf_spa/020_icf_alerta.png
   :alt: mensaje alerta
   :align: center
----

* **Status**: Presenta el estado de la factura, hay dos tipos: Abierto o Cerrado.
* **Precio**: Presenta el valor total de la factura del mes, según la política del contrato. En este ejemplo, el valor se expresa en moneda brasileña (Real - R$).
* **Precio en dolar**: Presenta el importe total de la factura del mes, expresado en dolares.

.. note:: |nota| Las cuatro columnas: contrato, mes de facturación, precio y precio en dolar posibilitan la alternancia de los datos presentados.

----

Detallando las acciones del ICF
"""""""""""""""""""""""""""""""""

La última columna de los contratos listados es la columna de acciones, tiene 6 botones: ``Ver Detalles``, ``Bajar Velocloud``, ``Abrir Factura`` y ``Cerrar Factura``, ``En la pantalla``, ``Bajar``, la función de cada uno se detalla a continuación.


* **Botón** ``Ver detalles``: Al hacer clic en esta opción, el usuario puede ver los detalles de la factura del contrato. Para las facturas con *status* “Cerrado”, la plataforma uCloud muestra la pantalla siguiente:

.. image:: /figuras/fig_icf_spa/021_icf_detalles_contrato.png
   :alt: detalhes factura
   :align: center
----

En el primer *card* “Factura del contrato” es posible visualizar la cotización del dólar en la fecha que marca el inicio de la factura del contrato en cuestión, junto con el valor total del consumo en el mes anterior al de la factura seleccionada.

Por ejemplo:

Si la factura seleccionada corresponde al mes de noviembre, los valores de consumo mostrados corresponden al mes anterior, en este caso octubre.

Siguiendo el flujo del análisis, el segundo *card* “Consumo de recursos durante el mes” exhibe un gráfico de barras.  Al lado, el “Gráfico de consumo por grupo” indica el consumo de recursos por grupo, mostrado en un gráfico circular, ambos gráficos representan un recurso visual que ayuda al usuario a comprender los datos del contrato seleccionado.

El último card “Grupos” exhibe informaciones más específicas sobre los grupos que utilizan el contrato, el usuario puede hacer clic en “Detalles” y la plataforma entrega el nombre de los grupos y los costos que cada uno representa sobre el valor total del contrato.

.. image:: /figuras/fig_icf_spa/022_icf_grupo_contrato.png
   :alt: detalhes grupos
   :align: center
----

El botón ``Exportar``, situado en la parte superior derecha de esta pantalla, ofrece al usuario la posibilidad de realizar el *download* de los archivos en formato CSV y PDF.

.. image:: /figuras/fig_icf_spa/023_icf_boton_exportar.png
   :alt: botón exportar pdf y csv
   :align: center
----

En formato PDF, el archivo se descarga inmediatamente. Este fichero contiene las informaciones resumidas de los contratos, que son las mismas que se presentan en la opción “Detalles” explicada anteriormente.

Veamos el ejemplo:

.. image:: /figuras/fig_icf_spa/024_icf_detalles_pdf.png
   :alt: datos pdf
   :align: center
----

En el caso de que el usuario necesite un archivo con la totalidad de la lista de ítems de la factura, debe hacer clic en CSV para descargar un archivo tipo hoja de cálculo (MS-Excel). Una vez realizado esto, la plataforma uCloud presenta un modal llamado “Generando Nuevo Informe”.

En él, se solicita un correo electrónico para que el usuario sea informado sobre la finalización de la producción del archivo y su disponibilidad para visualización, la adición del correo electrónico es opcional, si el usuario no desea ser informado basta dejar el campo sin rellenar.

En la pantalla se puede aún programar la producción del informe para una fecha específica o si la producción sigue una fecha recurrente.

----

Caso de uso:
""""""""""""""""""""""""""""""

**Obtener el informe en formato CSV**


Para obtener el informe en formato CSV pueden darse dos tipos de situaciones: 

1- Si aún no hay ningún informe generado por el sistema, la opción de *descargar el último archivo generado* no aparece habilitada. La creación del informe debe ser solicitada, haciendo clic en la opción ``Generar Informe``, conforme el ejemplo:

.. image:: /figuras/fig_icf_spa/025_icf_generar_informe.png
   :alt: generar informe  
   :align: center
----

Una vez realizada la última acción, en el icono del menú Tareas, situado en la parte superior derecha, la plataforma uCloud muestra una alerta informando que se está generando un nuevo informe.

.. note:: En esta etapa, el usuario puede seguir el progreso en el menú Tareas.

.. image:: /figuras/fig_icf_spa/026_icf_alerta_informe.png
   :alt: alerta creación informe 
   :align: center
----

Al pulsar sobre el icono de tareas, la plataforma presenta una nueva pantalla según la imagen de abajo, informando sobre el estado de la acción, en este ejemplo, el archivo de facturación del contrato ha sido generado correctamente.

.. image:: /figuras/fig_icf_spa/027_icf_tareas.png
   :alt: pantalla menú tareas 
   :align: center 
----

Para obtener el informe, el usuario debe hacer clic de nuevo en el botón ``Exportar``, y al seleccionar la opción CSV, la pantalla muestra el botón habilitado en color naranja. En este ejemplo, el mensaje que aparece para descargar el archivo generado es “Último archivo generado el 2024/02/26 17:25:42”.

.. image:: /figuras/fig_icf_spa/028_icf_ultimo_informe.png
   :alt: generando informe
   :align: center
----

Al hacer clic en el botón, se realiza el *download* del archivo CSV y queda a disposición del usuario, conforme se muestra en el siguiente ejemplo.

.. image:: /figuras/fig_icf_spa/029_icf_datos_csv.png
   :alt: datos csv
   :align: center
----

2 - Si ya existe un informe generado, al pulsar sobre la opción de descargar el archivo en formato CSV, el botón aparece habilitado en color naranja, con la fecha y hora del momento de su creación. Corresponde al usuario decidir si los datos obtenidos en esa fecha son los más adecuados para su búsqueda o si son necesarios los datos actualizados.

Para actualizar y producir un nuevo informe el usuario debe hacer clic en el botón ``Generar Informe`` y repetir el proceso del caso de uso, anteriormente presentado. Observe el siguiente ejemplo:

.. image:: /figuras/fig_icf_spa/030_icf_ultimo_informe_generado.png
   :alt: datos actualizados
   :align: center
----

Para las facturas con *status* “Abierta”, la plataforma presenta la siguiente pantalla:

.. image:: /figuras/fig_icf_spa/031_icf_pantalla_factura_abierta.png
   :alt: detalhes status factura abierta
   :align: center
----

En la pantalla aparecen las mismas informaciones exhibidas en la pantalla de *status* “Cerrado”, pero como la factura todavía está abierta el mensaje *“Los montos mostrados incluyen facturas que aún no se han cerrado y no pueden considerarse válidas hasta que se cierren”* se visualiza destacado.

.. note:: |nota| Todos los procedimientos descritos en el *status* “Cerrado” sobre la obtención de los archivos en formato PDF y CSV también se pueden realizar cuando el *status* de la factura está “Abierto”.

* **Botón** ``Bajar`` |ícone_baixar| :  Si el usuario ya conoce las informaciones relacionadas con el contrato listado y desea descargar toda la lista de ítems de la factura en un archivo tipo hoja de cálculo (MS-Excel), basta hacer clic en el botón ``Bajar``, y se presenta el modal “Generando Nuevo Informe”. Para obtener el fichero CSV el usuario debe seguir el mismo procedimiento presentado en el Caso de Uso.

.. _aqui: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/usr-manual.html#caso-de-uso

.. image:: /figuras/fig_icf_spa/032_icf_pantalla_bajar.png
   :alt: descargar informe
   :align: center
----

* **Botón** ``Abrir Factura`` |ícone_abrir_fatura| : Este botón sólo está disponible para las facturas en las que su *status* se encuentra con la información “Cerrado”; abrir una factura cerrada significa que la empresa necesita alguna acción de corrección en los valores de la factura, que debe ser proporcionado antes del pago del valor presentado.

Al pulsar el botón se muestra la siguiente pantalla, y corresponde al usuario confirmar o cancelar la acción.

.. image:: /figuras/fig_icf_spa/033_icf_reabrir_factura.png
   :alt: acción abrir factura
   :align: center
----

* **Botón** ``Cerrar Factura`` |ícone_fechar_fatura| : Este botón sólo está disponible para las facturas en las que su *status* se encuentra con la información “Abierto”; en la columna “Fecha de Cierre” en caso de que el usuario pase el cursor del ratón sobre el símbolo de atención, se muestra el mensaje: “No se informó la fecha de cierre de su factura porque aún está abierta”, tal y como se muestra en el siguiente ejemplo.

.. image:: /figuras/fig_icf_spa/034_icf_status_abierta.png
   :alt: mensaje cerrar factura 
   :align: center
----

Al hacer clic en el botón se muestra una pantalla de confirmación, y corresponde al usuario confirmar o cancelar la acción.

.. image:: /figuras/fig_icf_spa/035_icf_cerrar_factura.png
   :alt: acción cerrar factura
   :align: center
----

----


Informe Tendencia de Facturación (ITF)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

El Informe Tendencia de Facturación, denominado abreviadamente ITF, se basa en facturas que hacen referencia a las informaciones de valores financieros sobre un periodo ya cerrado. Permite al usuario consultar informaciones relacionadas a la facturación de un contrato, y detalla la visualización a partir de un filtro mensual. 

Este informe posibilita la detección de cualquier anomalía en el gasto, partiendo de determinados contratos analizados. Proporcionando una visión analítica y completa en dos formatos: - Nombre del producto y - *Tag*.

A partir de los informes de facturación debe ser posible ejecutar las reglas de tendencia de facturación, pudiendo proyectar los gastos hasta con 6 meses de antelación.

En la secuencia se detalla el flujo de consultas a las informaciones basadas en factura, que demuestran la aplicación de los filtros disponibles y la presentación de gráficos online, así como la posibilidad del *download* del archivo en formato .xlsx (Excel) para su uso posterior.    

----

Accediendo el ITF
""""""""""""""""""

Para acceder al ITF, basta hacer clic en el menú Financiero y, a continuación, en el submenú Informes, como se muestra en la figura siguiente:


.. image:: /figuras/fig_rtf_spa/01_submenu_informes.png
   :alt: Informes de paneles basados en el consumo y la facturación 
   :align: center
----

Esta pantalla se divide en dos grupos: "Paneles Basados en el Consumo" y "Paneles Basados en Facturas", el ITF se encuentra en el segundo tópico, destacado en la figura siguiente.

.. image:: /figuras/fig_rtf_spa/02_paneles_consumo_base.png
   :alt: Paneles basados en facturación 
   :align: center
----

----

Creando un ITF
""""""""""""""""""

Al pulsar sobre el botón ``Tendencia de facturación``, la plataforma muestra la siguiente pantalla:

.. image:: /figuras/fig_rtf_spa/03_financiero_contrato.png
   :alt: Seleccionar contrato 
   :align: center
----

En esta imagen se puede observar los contratos vinculados al usuario que está logueado. Este modal permite la búsqueda por el nombre del contrato con la ayuda de la barra de búsqueda, una vez encontrado el contrato deseado basta seleccionarlo y se presenta una nueva pantalla para continuar la consulta.  

.. image:: /figuras/fig_rtf_spa/04_financeiro_pantalla_inicial_linked_accounts.png
   :alt: Pantalla inicial
   :align: center
----

En la imagen de arriba se puede observar las siguientes funcionalidades:


* ``Volver`` 
* ``Exportar informe`` 
* ``Intervalo`` 
* ``Agrupar por``
* ``Buscar``
* ``Seleccionar Linked Accounts``.

.. important:: La funcionalidad Seleccionar Linked Accounts sólo estará disponible si el usuario tiene *Linked Accounts* en el contrato seleccionado.


.. image:: /figuras/fig_rtf_spa/05_datos_financieros.png
   :alt: Seleccionar fecha
   :align: center
----

Para crear un ITF en esta pantalla, el usuario debe iniciar el procedimiento seleccionando el intervalo, donde es necesario elegir los meses en el calendario presentado, y hacer clic en el período inicial y final para obtener el informe deseado.

.. image:: /figuras/fig_rtf_spa/06_datos_financieros_detallados.png
   :alt: Seleccionar fecha
   :align: center
----

Si el usuario desea seleccionar algún mes del año anterior o posterior, basta pulsar las flechas derecha o izquierda. En el ejemplo mostrado arriba, el intervalo seleccionado está comprendido entre NOV/2022 y ENE/2023.

A continuación, en el menú desplegable situado al lado del campo referente al Intervalo, el usuario debe seleccionar el tipo de agrupación del informe: por **nombre del producto** o por **TAG**, y hacer clic en el botón ``Buscar``.

.. image:: /figuras/fig_rtf_spa/07_financiero_agrupación.png
   :alt: Tipo de agrupación
   :align: center
----

El siguiente ejemplo trata de una consulta por *TAG* y la plataforma uCloud presenta una pantalla de alerta con el mensaje de atención, que se muestra a continuación. Para continuar la búsqueda el usuario debe hacer clic en el botón ``Ok``.

.. image:: /figuras/fig_rtf_spa/08_financiero_alerta_tag.png
   :alt: Mensaje de atención
   :align: center
----

Para descargar los datos obtenidos, basta hacer clic en el botón ``Exportar informe``, de color verde, situado en la parte superior derecha de la pantalla.

.. image:: /figuras/fig_rtf_spa/09_financiero_botón_exportar.png
   :alt: Botón Exportar
   :align: center
----

Un nuevo modal se presenta, y para que la exportación sea completada, es necesario rellenar todos los campos, como se muestra en la imagen de abajo.

.. image:: /figuras/fig_rtf_spa/10_financiero_modal_exportar.png
   :alt: Modal Exportar
   :align: center
----

* **Intervalo**: Se divide en mensual, semanal y diario.
* **Periodo**: Para seleccionar el periodo basta pulsar sobre el mes inicial y final. En caso del usuario necesitar un mes del año anterior o posterior, debe hacer clic en las flechas al lado del año mostrado para retroceder o avanzar, como se ha mencionado anteriormente.
* **Tipo**: Presenta las opciones de *Recursos* y *Tags*.

El último paso en este modal es hacer clic en el botón ``Exportar informe`` para que la pantalla ``Generando nuevo Informe`` sea presentada.

.. image:: /figuras/fig_rtf_spa/11_financiero_modal_generando_nuevo_informe.png
   :alt: Modal Exportar
   :align: center
----

En este modal, si el usuario quiere ser notificado, debe rellenar el campo con el correo electrónico.

Si el usuario desea programar el informe, sólo tiene que seleccionar la fecha y hacer clic en la opción: ``Programar informe``, que estará disponible para activación en el momento en que el campo de la fecha se haya rellenado. 

En la condición de programación recurrente, sólo es necesario activar el botón situado debajo del campo de fecha.

Si desea generar el informe por primera vez, basta hacer clic en ``Generar informe``. 

Si el usuario tiene interés en descargar del último archivo generado, debe continuar el flujo descrito a continuación.

----

Como descargar el archivo
""""""""""""""""""""""""""

Después de confirmar el éxito de la tarea, el usuario debe rehacer los pasos para volver a la página de Informes, así como el proceso para exportar los datos, hasta que aparezca el modal **Generando Nuevo Informe**.

.. image:: /figuras/fig_rtf_spa/12_accion_descargar_nuevo_informe.png
   :alt: acción descargar informe
   :align: center
---- 

Para descargar el ITF en archivo formato .xlsx (Excel), el usuario debe hacer clic en el botón situado en la parte inferior del modal ``Último informe generado el`` acompañado de la fecha y hora en que la tarea se mostró como *successful* en el menú Tareas.


.. note:: El botón para *download* queda disponible para activación sólo después de que la tarea presente el *status* de *successful*.

----

Siguiendo el *download* en el Menú Tareas
""""""""""""""""""""""""""""""""""""""""""

Al solicitar la generación de un nuevo informe, es posible seguir la evolución de la *task* en el Menú Tareas, según la imagen de abajo.


.. image:: /figuras/fig_rtf_spa/13_seguiendo_menú_tareas.png
   :alt: Éxito
   :align: center
----


El archivo se descarga en formato .xlsx (Excel), como se muestra a continuación. 


.. image:: /figuras/fig_rtf_spa/14_archivo_descargar.png
   :alt: Planilla 
   :align: center
----


Visualizando el ITF
"""""""""""""""""""""

Como ya se ha mencionado, existen dos tipos de visualización en la exportación para obtener un análisis más completo del informe:

1. Nombre del producto
2. *Tag* (son los campos del archivo .csv detallado)


El ITF tiene la posibilidad de filtrar tanto por producto como por *tag*. 

A partir de este primer filtrado, deben aparecer todos los recursos del contrato elegido (sea dividido por nombre del producto o por *tag*), presentando informaciones específicas sobre cada uno de ellos, teniendo en cuenta cuatro métricas:

1. Gasto promedio
2. Tolerancia de los gastos
3. Media móvil
4. Costo

----

Agrupación por nombre del producto
"""""""""""""""""""""""""""""""""""

La primera pantalla del informe que se presenta son las informaciones generales sobre el contrato, donde a la izquierda se muestra un gráfico sobre el gasto total por mes. 

.. image:: /figuras/fig_rtf_spa/15_costo_total_mes.png
   :alt: Gráfico de contratos
   :align: center
----

Para proyectar el costo, el usuario debe seleccionar el mes de proyección en la parte superior de la pantalla y hacer clic en el botón ``Proyectar Costo``. A continuación, se añade una nueva columna a los gráficos presentes en todo el informe.  

.. image:: /figuras/fig_rtf_spa/16_costo_total_mes_proyectar_costo.png
   :alt: Proyección de costos
   :align: center
----

Si deseas eliminar la nueva barra, basta hacer clic en el botón ``Borrar`` que aparece al lado de ``Proyectar Costo``.


Justo debajo, en el área de recursos del informe, se presenta la cantidad total de recursos presentes en el contrato elegido, y se muestran cuatro valores:

1. Gasto Promedio Más Elevado
2. Gasto Promedio Más Bajo
3. Gasto Promedio General
4. Valor Total


En la parte derecha, el gráfico se presenta con la proyección de gastos para cada mes dentro del periodo seleccionado.


.. image:: /figuras/fig_rtf_spa/17_recursos_del_informe.png
   :alt: Informe por recurso
   :align: center
----

Al abrir el informe, es posible observar un botón de color naranja en la esquina derecha de la pantalla, representado por una flecha blanca que apunta hacia el lado izquierdo.  

.. image:: /figuras/fig_rtf_spa/18_recursos_del_informe_flecha.png
   :alt: Pestaña lateral
   :align: center
----

Al pulsar este botón, una pestaña se expande con los nombres de los productos de este contrato. Con la ayuda de la barra de búsqueda, es posible rastrear un recurso específico, y al hacer clic el usuario es llevado directamente hasta su gráfico.

.. image:: /figuras/fig_rtf_spa/19_pestanã_lateral.png
   :alt: Pestaña lateral en Detalle
   :align: center
----


Si el usuario ha seguido el flujo para la exportación del informe para visualización offline, el archivo se presenta de la siguiente manera:

.. image:: /figuras/fig_rtf_spa/20_producto_offline.png
   :alt: Planilla
   :align: center
----

En este ejemplo de informe *offline*, hay nueve columnas:

* *Created by*
* *Product name*
* *Product family*
* *Usage type*
* *Cloud identifier*
* *Linked*
* *2022-11*
* *2022-12*
* *2023-01*


Las tres últimas columnas hacen referencia al año y mes del periodo seleccionado, en este ejemplo de Nov/2022 a Ene/2023.

----

Agrupación por *Tag*
"""""""""""""""""""""""

Cuando se agrupa por *tag*, un menú desplegable se presenta en el área del contrato con las siguientes opciones de filtrado:


* Todos los *Tags*
* Métrica
* Nombre


.. image:: /figuras/fig_rtf_spa/21_agrupación_por_tag.png
   :alt: Agrupación por Tag
   :align: center
----

Si el usuario ha seguido el flujo para la exportación del informe y visualización *offline*, el archivo se presenta de la siguiente manera:

.. image:: /figuras/fig_rtf_spa/22_agrupación_por_tag_offline.png
   :alt: Agrupación por Tag
   :align: center
----
  
Este ejemplo de informe *offline* presenta diez columnas de informaciones, que son:

* *Created by*
* *Product name*
* *Product family*
* *Usage type*
* *Cloud identifier*
* *Linked*
* *Tag*
* *2022-12*
* *2023-01*
* *2023-02*


Las tres últimas columnas hacen referencia al año y mes del periodo seleccionado, en este ejemplo de Dic/2022 a Feb/2023.

----

Filtrado por anomalía
"""""""""""""""""""""""

Permite al usuario realizar el filtrado por anomalía dentro del contrato, analizando todos los recursos. Para esto, dispone de una *flag* "Mostrar únicamente anomalías" con la opción de activarla o no. Al activarla, los recursos mostrados en pantalla son reducidos, mostrando exclusivamente aquellos que realmente tienen anomalías de gastos.


.. image:: /figuras/fig_rtf_spa/23_unicamente_anomalias.png
   :alt: Flag anomalia
   :align: center
----

La representación de una anomalía se realiza mediante la superación del límite de gastos calculados en función de la regla de cálculo de los 3 cuartiles. Al hacer clic en el *tooltip* situado junto a la *flag* "Mostrar únicamente anomalías", aparece el siguiente mensaje:

.. image:: /figuras/fig_rtf_spa/24_ecuaciones_utilizadas.png
   :alt: Mensaje ecuaciones
   :align: center
----

Si las anomalías son inexistentes, se muestra una advertencia en la pantalla de detalles del contrato del informe, como se presenta en la imagen siguiente.

.. image:: /figuras/fig_rtf_spa/25_no_hay_anomalias_de_costos.png
   :alt: Mensaje de anomalía
   :align: center
----

Además de esta advertencia, ningún gráfico es presentado.

Sin embargo, si hay anomalías de gastos, una columna de color distinto aparece junto a los gráficos, como se muestra en la imagen siguiente. 

.. image:: /figuras/fig_rtf_spa/26_anomalias_grafico.png
   :alt: Gráfico de anomalías
   :align: center
----

----

Linked Accounts
"""""""""""""""""""""""

Si el usuario no tiene cuentas asociadas al contrato, un mensaje aparece debajo de la fecha: "Este contrato no tiene *Linked Accounts*".


.. image:: /figuras/fig_rtf_spa/27_contrato_no_tiene_linked_accounts.png
   :alt: Linked Accounts
   :align: center
----


Sin embargo, si el usuario tiene cuentas asociadas al contrato, puede visualizarlas al activar la *flag* "Seleccionar *Linked Accounts*" según el ejemplo presentado.


.. image:: /figuras/fig_rtf_spa/28_seleccionar_linked_accounts.png
   :alt: Botón Linked Accounts
   :align: center
----

Al activarlo, las cuentas asociadas al contrato son mostradas justo debajo de la *flag* que se mantiene de color naranja. Y las cuentas son liberadas para selección, como se muestra en la siguiente imagen.


.. image:: /figuras/fig_rtf_spa/29_cuentas_seleccionadas.png
   :alt: Linked account seleccionada
   :align: center
----


Una vez seleccionada la cuenta deseada, los gráficos referidos a ésta se presentan de la misma forma que los mostrados anteriormente (Visualizando el ITF). También es posible optar por todas las cuentas presentadas, en este ejemplo hay dos *Linked Accounts*. 


Si deseas olvidar la cuenta seleccionada, debes hacer clic en el botón ``Borrar`` que aparece al lado de las cuentas de la lista.

Si el usuario está interesado en exportar los datos de las *Linked Accounts* para su máquina, sólo es necesario seguir los pasos descritos anteriormente en el tópico: "Como descargar el archivo".

====

**Utilidades**
---------------

----

**Dimensión**
~~~~~~~~~~~~~~

----

Creando una Dimensión
""""""""""""""""""""""""

----

Creando una Agrupación de *Tags*
""""""""""""""""""""""""""""""""

----

Creando *Tag*
""""""""""""""""

----

Utilizando el operador lógico
""""""""""""""""""""""""""""""""

----

Listado de Dimensión
""""""""""""""""""""""""

----

Editando una Dimensión
""""""""""""""""""""""""

----

Donde se utiliza la “Dimensión”
""""""""""""""""""""""""""""""""""

----

**Tags Virtuales**
~~~~~~~~~~~~~~~~~~~

----

*Tags* Virtuales de la plataforma uCloud
""""""""""""""""""""""""""""""""""""""""""

----

Normalizando *Tags* Virtuales
""""""""""""""""""""""""""""""""""""""""""

----

¿Cuándo utilizar?
""""""""""""""""""""""""""""""""""""""""""

----

Restricciones de los *Tags*
""""""""""""""""""""""""""""""""""""""""""

----

¿Cómo se utiliza?
""""""""""""""""""""""""""""""""""""""""""

----

Menú Orden de Servicio
=======================

----

Utilizando la Orden de Servicio
---------------------------------

----

Creando la Orden de Servicio
---------------------------------

----

Añadir Estimación de Costos en USN y UST
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Gestionando la Orden de Servicio
----------------------------------

----

*Card* : General
~~~~~~~~~~~~~~~~~~

----

*Card* : Estimación de Costos (USN)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Card* : Configuración de Estimación de Costos (UST)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

*Card* : De acuerdo
~~~~~~~~~~~~~~~~~~~~~~~~

----

Menú Recomendaciones (nuevo)
=============================

----

Menú Account Providers 
=======================

----

Menú Containers
===============

----

Gestionando un Container
------------------------

----

Creando un Nuevo Container
---------------------------

----

Menú Hosts
==========

----

Crear Hosts
--------------

----

Visualizando un Host
-----------------------

----

Menú Redes
============

----

Redes
----------

----

Gestionar Red
----------------

----

Añadir “Subred” al ambiente AWS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Añadir “Subred” al ambiente Azure
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Añadir “Subred” al ambiente GCP
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Añadir “Subred” en el ambiente Privado (VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Nueva Red
--------------------

----

Crear Red en los Proveedores de Servicios de Nube Pública
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Red en Ambiente Privado (On-Premises)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Red en Proveedores de Servicios de Nube Pública (AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Red en Proveedores de Servicios de Nube Pública (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Red en Proveedores de Servicios de Nube Pública (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Red en Ambiente Privado (VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

IPs públicas
----------------

----

Solicitando una IP Pública (**AWS y GCP**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Solicitando una IP Pública (**Azure**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Solicitando una IP Pública (ambiente privado: **VMware vCenter**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Grupos de Seguridad y ACLs
--------------------------

----

Gestionar Grupo de Seguridad
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Grupo de Seguridad
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Par de Claves
-----------------

----

Gestionar un Par de Claves
~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creando un Par de Claves
~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Importando un Par de Claves
~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Balanceadores
---------------------

----

Gestionando Balanceador
~~~~~~~~~~~~~~~~~~~~~~~

----

Creando Balanceador (Ambientes AWS y GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creando Balanceador (Ambiente Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Grupos de Recursos vCloud
-----------------------------

----

Crear Grupo de Recursos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

VPN
------------------------

----

Crear VPN en 3 pasos
~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Customer Gateway
~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Private Gateway
~~~~~~~~~~~~~~~~~~~~~~~~

----

Crear Túnel VPN
~~~~~~~~~~~~~~~~~~~~~~~~

----

Menú Storage
=============

----

Crear Storage
---------------

----

Visualizando un Storage
--------------------------

----

Menú Modelos
==============

----

Menú Flavors
============

----

Crear Flavor
------------

----

Visualizando un Flavor
-------------------------

----

Menú Workflows
==============

----

Direct Execution
----------------

----

Editando Workflow
----------------

----

Creando Workflow
----------------

----

Definición del Flujo de Trabajo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Inclusión de Tareas Asociadas
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Creando Tareas Asociadas
--------------------------

----

Tarea de Cierre/Activación Programada de la Máquina Virtual
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Tarea de Crear Imagen de Disco (Snapshot)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


----

Tarea de Script
~~~~~~~~~~~~~~~~~~~~


----

Client Server (Puppet)
----------------------

----

Aprovisionar un Puppet Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

----

Catálogo de Servicios
--------------------

----

Recursos: Nuevo Servicio
~~~~~~~~~~~~~~~~~~~~~~

----

Recursos: Enviar
~~~~~~~~~~~~~~~~

----

Mis servicios anteriores
~~~~~~~~~~~~~~~~~~~~~~~~

----

Marketplace: Historial de servicios contratados
""""""""""""""""""""""""""""""""""""""""""""""

----

Mis ofertas contratadas
""""""""""""""""""""""""""

----

Mis ofertas registradas
""""""""""""""""""""""""""

----

Menú Tareas
============

----

Pestaña de Tareas
---------------------

----

Pestaña de Aprobaciones Pendientes
-------------------------------------

----

Pestaña de Tareas Programadas
---------------------------------

----

Menú Inventario de Recursos
=============================

----

Crear grupo de recursos dinámicos
------------------------------------

----

Editor de Etiquetados (tags) Nativo
-------------------------------------

----

Tag
~~~~~~~~~~~~~~~~~~~~~~~~

----

Sin Tag
~~~~~~~~~~~~~~~~~~~~~~~~

----

Menú Colores y Personalización
===============================

----

Personalización de la Interfaz Gráfica
-----------------------------------------

----

Informaciones del tema
~~~~~~~~~~~~~~~~~~~

----

Identidad
~~~~~~~~~~

----

Colores: Modo claro
~~~~~~~~~~~~~~~~~~~~

----

Colores: Modo oscuro
~~~~~~~~~~~~~~~~~~~~

----

Temas registrados
~~~~~~~~~~~~~~~~~~

====

**Equipe Ustore**


uCloud Manual de uso.
Actualización 05/12/2023.
 



.. |atencao| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/hand-stop-o.png?raw=true

.. |nota| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/hand-pointer-o.png?raw=true

.. |importante| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/warning.png?raw=true

.. |dica| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/asterisk.png?raw=true

.. |botao_adiciona| image:: /figuras/uCloud_botao_adicionar.png

.. |botao_adiciona_user| image:: /figuras/uCloud_botao_adicionar_usuario_exist.png

.. |botao_adiciona_grp| image:: /figuras/uCloud_botao_criar_grupo.png

.. |botao_cria_user| image:: /figuras/uCloud_botao_criar_usuario.png

.. |botao_editar| image:: /figuras/uCloud_botao_editar.png

.. |botao_exclui_grp| image:: /figuras/uCloud_botao_excluir_grupo.png

.. |botao_adiciona_aogrupo| image:: /figuras/uCloud_botao_adicionar_aogrupo.png

.. |botao_adiciona_verde| image:: /figuras/uCloud_botao_adiciona_verde.png

.. |botao_conecta_container| image:: /figuras/uCloud_botao_conecta_container.png

.. |botao_criar_VM| image:: /figuras/uCloud_botao_criar_VM.png

.. |botao_desabilita| image:: /figuras/uCloud_botao_disable.png

.. |botao_download| image:: /figuras/uCloud_botao_download.png

.. |botao_enable| image:: /figuras/uCloud_botao_enable.png

.. |botao_excluir| image:: /figuras/uCloud_botao_excluir.png

.. |botao_exclui_VDC| image:: /figuras/uCloud_botao_excluir_VDC.png

.. |botao_exclui_user| image:: /figuras/uCloud_botao_exclui_usuario.png

.. |botao_exportar| image:: /figuras/uCloud_botao_exportar.png

.. |botao_filtrar| image:: /figuras/uCloud_botao_filtrar.png

.. |botao_lanca_acct| image:: /figuras/uCloud_botao_lancar_acct.png

.. |botao_limpa_acct| image:: /figuras/uCloud_botao_limpar_acct.png

.. |botao_pesquisar| image:: /figuras/uCloud_botao_pesquisar.png

.. |botao_refresh| image:: /figuras/uCloud_botao_refresh.png

.. |botao_proximo| image:: /figuras/ucloud_botao_proximo.png

.. |botao_voltar| image:: /figuras/ucloud_botao_voltar.png

.. |botao_criar_off| image:: /figuras/ucloud_botao_criar_cinza.png

.. |botao_criar_on| image:: /figuras/ucloud_botao_criar_verde.png

.. |botao_cencela_verm| image:: /figuras/ucloud_botao_cancela_verm.png

.. |botao_seleciona_azul| image:: /figuras/uCloud_botao_seleciona_azul.png

.. |icone_conf_verde| image:: /figuras/uCloud_icone_confirma_verde.png

.. |icone_cancela_vermelho| image:: /figuras/uCloud_icone_cancela_vermelho.png

.. |icone_cota_grp| image:: /figuras/ucloud_icone_cota_grupo.png

.. |icone_cota_indv| image:: /figuras/ucloud_icone_cota_individual.png

.. |icone_desb_verm| image:: /figuras/uCloud_icone_desabilita_vermelho.png

.. |icone_edita_on| image:: /figuras/uCloud_icone_editar_on.png

.. |icone_habil_verde| image:: /figuras/uCloud_icone_habilita_verde.png

.. |icone_lixo| image:: /figuras/uCloud_icone_lixo.png

.. |icone_abre_fatura| image:: /figuras/uCloud_icone_abrir_fatura.png

.. |icone_agenda| image:: /figuras/uCloud_icone_agendar.png

.. |icone_amplia_vdc| image:: /figuras/ucloud_icone_amplia_vdc.png

.. |icone_anexa_branco| image:: /figuras/uCloud_icone_anexar_branco.png

.. |icone_conecta_rede| image:: /figuras/uCloud_icone_conecta_rede.png

.. |icone_desconecta| image:: /figuras/uCloud_icone_desconectar.png

.. |icone_download| image:: /figuras/uCloud_icone_download.png

.. |icone_edita_user| image:: /figuras/uCloud_icone_edita_user.png

.. |icone_private_net| image:: /figuras/uCloud_icone_private_template.png

.. |icone_remove_user| image:: /figuras/uCloud_icone_remove_user.png

.. |icone_visualiza| image:: /figuras/uCloud_icone_visualiza.png

.. |icone_vm_start| image:: /figuras/ucloud_icone_vm_start.png

.. |icone_vm_stop| image:: /figuras/ucloud_icone_vm_stop.png

.. |icone_vm_reboot| image:: /figuras/ucloud_icone_vm_reboot.png

.. |icone_vm_suspend| image:: /figuras/ucloud_icone_vm_suspend.png

.. |icone_vm_desconecta| image:: /figuras/ucloud_icone_vm_desconecta.png

.. |icone_vm_ssh| image:: /figuras/ucloud_icone_vm_ssh.png

.. |icone_vm_rdp| image:: /figuras/ucloud_icone_vm_rdp.png

.. |icone_vm_clone| image:: /figuras/ucloud_icone_vm_clone.png

.. |icone_vm_resume| image:: /figuras/ucloud_icone_vm_resume.png

.. |icone_edita_vdc| image:: /figuras/ucloud_icone_edita_vdc.png

.. |icone_revert_snap| image:: /figuras/ucloud_icone_revert_snap.png

.. |icone_wf_ativo| image:: /figuras/ucloud_icone_wf_ativo.png

.. |icone_wf_parado| image:: /figuras/ucloud_icone_wf_parado.png

.. |icone_lapis_workflow| image:: /figuras/ucloud_icone_edita_workflow.png

.. |botao_adicionacarrinho| image:: /figuras/ucloud_botao_colocacarrinho.png

.. |botao_finalizapedido| image:: /figuras/ucloud_botao_finalizapedido.png

.. |icone_log_wf| image:: /figuras/ucloud_icone_info_workflow.png

.. |icone_refresh| image:: /figuras/ucloud_icone_refresh.png

.. |icone_sino| image:: /figuras/ucloud_icone_sino.png

.. |icone_grafico_barra01| image:: /figuras/ucloud_icone_grafico01.png

.. |icone_grafico_barra02| image:: /figuras/ucloud_icone_grafico02.png

.. |icone_graph_large| image:: /figuras/ucloud_icone_big_graph.png

.. |icone_troca_mes| image:: /figuras/ucloud_icone_mes.png

.. |icone_seta_acima| image:: /figuras/ucloud_icone_fatur_acima.png

.. |icone_seta_abaixo| image:: /figuras/ucloud_icone_fatur_abaixo.png

.. |icone_neutro| image:: /figuras/ucloud_icone_fatur_estavel.png

.. |icone_next_ativo| image:: /figuras/ucloud_icone_next_activo.png

.. |icone_next_off| image:: /figuras/ucloud_icone_next_off.png

.. |icone_lupa| image:: /figuras/ucloud_icone_lupa.png

.. |ícone_baixar| image:: /figuras/fig_rcf/ícone_baixar.png

.. |ícone_abrir_fatura| image:: /figuras/fig_rcf/ícone_abrir_fatura.png

.. |ícone_fechar_fatura| image:: /figuras/fig_rcf/ícone_fechar_fatura.png


