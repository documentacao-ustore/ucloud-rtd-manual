

.. image:: /figuras/ucloud.png
   :alt: logo ucloud
   :align: center

----

uCloud - Manual del Usuário
+++++++++++++++++++++++++++


Soluciones de tecnologías de la información que permiten implementar una arquitectura de cómputo escalable, sólida y confiable en una nube distribuida.

====


Presentación
============

Este documento tiene como objetivo explicar el uso de la Plataforma *uCloud*, una plataforma de *Cloud Service Broker* (broker de servicios en nube) que permite administrar múltiples proveedores de servicios de nube, tanto privados como proveedores de nube pública. 

En este manual se presentan los conceptos, las pantallas, las funcionalidades y los comandos de uso de este producto.

====

Introducción
============

Las organizaciones empresariales han incorporado la nube como solución para administrar sus entornos y adoptan una combinación de nubes privadas y públicas, el gran desafío actual es la gestión de estos entornos híbridos de múltiples nubes *(hybrid multi-cloud)* con el fin de lograr una visión unificada, así como obtener un control centralizado de los costos financieros, ya que cada organización empresarial tiene una necesidad y se enfrenta a diferentes desafíos.

La Plataforma de uCloud ha sido desarrollada para estos escenarios, independientemente de cuantos proveedores (públicos y/o privados) existan, el usuario podrá interactuar con sus plataformas:

   * Infraestructura como Servicio *(Infrastructure as a Service - IaaS)*;
   * Plataforma como Servicio *(Platform as a Service - PaaS)*.

Como se mencionó anteriormente, uCloud está posicionado como una plataforma de *Cloud Service Broker - CSB* *(Broker de servicios en la nube)* que permite administrar múltiples proveedores de servicios en la nube, tanto privados como proveedores de nube pública.

Una plataforma *CSB* como la Plataforma uCloud permite a las organizaciones actuar en cinco puntos fundamentales para la gestión de entornos híbridos multi-nube, son:


Gobernanza Financiera
---------------------

Además del control de la infraestructura, la Plataforma de uCloud permite a las empresas usuarias de esta plataforma establecer límites, tanto financieros como cuantitativos de recursos (cuotas). Estos límites financieros o de infraestructura pueden aplicarse en tres niveles:

  * Para un proveedor público en general (ver el elemento Contratos, en el Menú Administración);
  * Para un grupo de usuarios (ver el elemento Grupos en el menú Administración);
  * Para un usuario/individuo (ver el elemento Usuarios, en el Menú Administración).

De esta forma, la organización aplicará criterios de gobernanza financiera y control de gastos, como también podrá acompañar los costos de su entorno híbrido de multi-nube a través de una única interfaz.  

La adopción de la aplicación de límites (cuotas) financieros y/o recursos computacionales en diversos niveles alcanza el nivel de usuario, Así el control de costos será efectivo y permitirá evitar que el presupuesto de la organización sorprenda en situaciones que el costo de la infraestructura computacional sea exorbitante o por encima de los valores preestablecidos.

Otro aspecto de la Plataforma de uCloud es la reducción de costos de certificación y capacitación de los especialistas, en cada una de las interfaces de cada proveedor (público y/o privado), ya que el empleo de una interfaz de uso y gestión única y sencilla permite extraer más productividad del entorno del proveedor de la nube. Incluso si el usuario no cuenta con capacitación o certificación en la consola específica del proveedor (pública y/o privada), la plataforma uCloud permitirá al usuario aprovisionar un recurso informático en el entorno deseado de manera sencilla y fácil.

Billing (Facturación de los Servicios)
--------------------------------------

La Plataforma de uCloud proporciona a las organizaciones empresariales información sobre los costes recurrentes relacionados con el uso de los recursos computacionales en la(s) operación(es) en un entorno multinube híbrido. Este es solo uno de los puntos que forma parte de la práctica de *Cloud Financial Management - FinOps* (Gestión financiera de la nube).

Es importante resaltar que, individualmente, la Plataforma de uCloud no atiende a los tres pilares de la práctica de *FinOps* por *default*. Ustore posee otros productos que pueden ser complementarios y el conjunto de productos tiene potencial para actuar como un entorno capaz de englobar y atender la práctica de *FinOps*.

El requisito soportado por uCloud es el punto de *Información* *(Inform)*, los otros puntos de esta mejor práctica de *FinOps*: la *Optimización* y la *Operación* pertenecen a los otros productos de la cartera de Ustore que complementa la Plataforma de uCloud.

Se debe aclarar que la Plataforma de uCloud no crea ni genera valores de recursos computacionales, estos montos se generan en los proveedores de nube pública de los que la aplicación uCloud *extrae* *(descargar)* el archivo de *Billing* *(facturación)* de estos proveedores. Despues añade esta información en sus bases de datos internas para que, posteriormente, de acuerdo con los criterios comerciales del contrato puedan ser aplicados y estos costos calculados y convertidos para la moneda corriente en Brasil.

De esta forma, el usuario permanece *informado* de la evolución de los costos y podrá seguir si estos costos se encuentran dentro de los criterios de la gobernanza financiera de la organización.

Generalmente estos costos se presentan en archivos de texto no estructurados *(Comma-separated Values - CSV)* generados cada período (promedio de 8 horas) y la Plataforma de uCloud agrega la información de este archivo *CSV* a su base de datos interna para agilizar y simplificar la presentación de estos valores en la pantalla del usuario.

Exclusivamente, los usuarios con un perfil específico pueden `visualizar costos` y permanecer *informados* de los valores de consumo de sus recursos computacionales totales en cada proveedor de la nube (pública y/o privada). Esto permite que el usuario pueda realizar un seguimiento de los costos acumulados de los recursos informáticos activos en los proveedores de servicios en la nube.

Monitoreo de la Infraestructura
-------------------------------

Una funcionalidad importante de la Plataforma de uCloud es la reciente implementación del módulo de gestión de eventos (monitoreo) que permite recopilar acontecimientos y alarmas que se han generado en los entornos de nube (público y/o privado), activar notificaciones y crear informes personalizados.

Todas estas facilidades reducen los costos para las organizaciones, una vez que elimina la necesidad de contratación de servicios de monitoreo de los proveedores, pues tal servicio puede representar altos costos los cuales pueden impactar de forma negativa en el presupuesto (sobrepasar el límite) destinado a infraestructura de nube pública.

Esta funcionalidad permite integrar a un entorno de gestión de Service Desk para control *IT Service Management* (gestión de servicios de TI).

Inventario (*Assessment*)
-------------------------

La plataforma de uCloud se conecta a los proveedores de la nube mediante el registro de credenciales de acceso específicas de cada fornecedor de servicios en la nube (público y/o privado). Para ello, las empresas deben proporcionar credenciales de modo *operativo*.

Esta credencial operativa es proporcionada por el administrador del servicio en la nube y son autorizaciones que se generan en las cuentas de los proveedores que solo tienen permiso para interactuar con la consola del proveedor público en la nube a través de una API, no son calificaciones normales con información estándar de inicio de sesión y contraseña. De esta forma, la seguridad y las normas de regulación de seguridad de la información están previstas y atendidas en su totalidad.

Como las credenciales *operativas* se configuran en la Plataforma de uCloud, la primera actividad es sincronizar la configuración y el inventario de recursos informáticos existentes en el proveedor (máquinas virtuales - cargas de trabajo). Esta lista de máquinas virtuales se extrae y se agrega a las bases de datos de uCloud para que la presentación en la pantalla del usuario sea rápida.

Con este inventario disponible directamente dentro de la Plataforma de uCloud, el usuario podrá operar cada una de las máquinas virtuales, independientemente de cuál sea el proveedor de la nube que esta función está aprovisionada. Vea a continuación las posibles operaciones a aplicar a los recursos computacionales existentes en los proveedores de nube (público y/o privado).

Es importante mencionar que el uCloud no tiene recursos computacionales, estos recursos existen en las nubes de los proveedores de servicios de nube pública o en los entornos de virtualización *(hypervisors)* instalados en su DataCenter privado. A través de la API Rest, la Plataforma de uCloud, envía acciones (tareas) al administrador de entorno de nube específico (público y/o privado) para que realicen la acción deseada.

El usuario podrá seguir el resultado de cualquiera de las acciones de operación en los recursos computacionales de forma casi inmediata, vale recordar que no es la Plataforma de uCloud la que *ejecuta* las acciones, sino el entorno donde la máquina virtual existe (ya sea público y/o privado). Este es el encargado de ejecutar la tarea enviada a través de la API Rest.

Si el resultado no se refleja en la interfaz de la pantalla del usuario, la consola de destino puede tardar un cierto tiempo en realizar esta tarea y solo después de que finalice la ejecución de ella, se mostra el resultado en la interfaz de uCloud.

Existe una opción de menú donde el usuario podrá seguir el porcentaje de progreso de estas tareas, su resultado de éxito o el mensaje de error referente a alguna restricción del entorno destino.

Es importante resaltar que pueden existir restricciones aplicadas al usuario aprovisionado en la Plataforma de uCloud, porque ello puede haber agotado el límite de su cuota financiera o de recursos computacionales, de esta forma la Plataforma de uCloud generar un aviso de 
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

  * Amazon Web Services *(AWS)*
  * Google Cloud Plataform *(GCP)*
  * Microsoft *Azure*
  * IBM Cloud
  * Huawei Cloud
  * Oracle Cloud Infrastructure *(OCI)*

Actualmente, la plataforma uCloud está lista para conectarse con las siguientes plataformas *(hypervisors)* de administración de entornos de nube privada:

  * `VMware` *(vCenter Versões 5.0, 5.1, 5.5, 6.0, 6.5, 6.7, 7.x ou superior)*
  * `vCloud`
  * `Hyper-v` *(Windows 2008R2, Windows 2012, Windows 2012R2 e Windows 2016 ou superior)*
  * `Openstack`
  * `Xen Server`
  * `XCP-NG`
  * `KVM`

La plataforma uCloud, además de las funciones CSB *(Cloud Service Broker)*, también es un agregador 
de funcionalidades que permite a los usuarios, de forma sencilla y centralizada, controlar varias consolas de administrador de entornos virtualizados *(hypervisors)* desde el entorno local privado *on-premises* o desde el entorno del proveedor de nube pública. Agrega monitoreo, flujo de trabajo en la nube *(Cloud Workflow)* y le permite implementar un repositorio ‘biblioteca’ centralizado de archivos de referencia *(playbooks)* para el uso de herramientas de infraestructura como código
*(Infrastructure as a Code)*.


Integración e Interoperabilidad Multiplataforma *(API uCloud)*
=============================================================

La interoperabilidad es la capacidad de dos o más sistemas (ordenadores, medios de comunicación, redes, programas informáticos y otros componentes de la tecnología de la información) para interactuar e intercambiar datos según un método definido, con el fin de obtener los resultados esperados. La interoperabilidad define si dos componentes de un sistema, desarrollados con diferentes herramientas, de diferentes proveedores, pueden o no actuar juntos.

La comunicación entre estos "sistemas" se basa en el consumo de una interfaz de programación de aplicaciones *(API)* que permite enviar y recibir llamadas para la ejecución de alguna actividad o la extracción de algún tipo de información almacenada. Las siglas API provienen de la expresión inglesa *Application Programming Interface* que, traducida al portugués, puede entenderse como interfaz de programación de aplicaciones. En otras palabras, la API es un conjunto de reglas que permite la comunicación entre plataformas a través de una serie de normas y protocolos.

A través de las API, los desarrolladores pueden establecer comunicación (interoperabilidad) entre programas y aplicaciones capaces de comunicarse con otras plataformas.

El principal ejemplo es la integración nativa y directa de la Plataforma uCloud con la consola de los proveedores de nubes públicas, todo ello mediante la interoperabilidad a través de la API de las consolas de los proveedores.

Otro ejemplo muy común de uso de la Plataforma uCloud es la emisión de facturas para los sistemas de showback y chargeback, así como el envío de información y alertas sobre los recursos gestionados.

Nuestros clientes (y/o integradores) pueden utilizar la documentación de la API de la Plataforma uCloud con sus plataformas internas para complementar o automatizar ciertas actividades o acciones que están más allá de las capacidades nativas de la Plataforma uCloud. Por ejemplo: *consultar y extraer de la Plataforma uCloud el coste de la factura de los objetos de valor de un proveedor de la nube pública a través de una aplicación financiera/contable para la emisión de facturas*.

La Plataforma uCloud dispone de documentación de su API, pero el acceso a la documentación completa debe solicitarse al Equipo de Atención al Cliente *(contato@usto.re)* para que se cree y envíe una credencial de acceso a la documentación de la Plataforma uCloud.

El Equipo de Ustore está preparado para ayudar y evaluar las demandas de interoperabilidad e integración entre la Plataforma uCloud y las aplicaciones que tienen y permiten el uso de APIs para la interoperabilidad.



Arquitectura de Referencia de la Plataforma uCloud
==================================================

A continuación presentamos una arquitectura de referencia para la Plataforma uCloud con sus componentes, proveedores e integraciones nativos.

.. figure:: /figuras/ucloud_future_vision_small_2.png
   :alt: Arquitectura de Referencia de la Plataforma uCloud
   :align: center

----

La Plataforma uCloud se comunica con la consola de los proveedores a través de la API Rest, por lo que cada acción realizada o configurada en las pantallas de uCloud envía acciones (tareas) al administrador (público y/o privado) del entorno de nube (consola) específico para que puedan realizar la acción deseada.

Ustore se compromete a mantener el constante desarrollo de sus Plataformas de Software y aplicar las mejores prácticas *(best practices)* de *DevOps* vigentes en el mercado de TI en la actualidad.

Nuestro compromiso es mantener la compatibilidad de integración, para que los últimos cambios e implementaciones en la consola de proveedores y todo el software que mantenemos mantengan la interoperabilidad, para que la nueva funcionalidad esté siempre disponible a través de la interfaz de la Plataforma uCloud.

Se utiliza un conjunto de prácticas y herramientas diseñadas para aumentar la capacidad de una organización para entregar aplicaciones y servicios más rápido que los procesos tradicionales de desarrollo de software.

.. Consulte la documentación específica acerca de *roadmap* de evolución de la plataforma uCloud o en el sitio web de Ustore (www.ustore.com.br).


Acceso a la Plataforma uCloud
=============================

El acceso a la plataforma se realiza a través de una dirección de Internet, el usuario debe utilizar un navegador de Internet *(Internet browser)* e introducir la dirección URL/enlace, para que el usuario vea la pantalla de presentación inicial. Los navegadores de Internet 
compatibles con la Plataforma uCloud son: Microsoft Edge versión 86.x, Google Chrome versión 85.x, Firefox verano 80.x u Opera versión 71.x.

La Plataforma uCloud está adaptada para que su interfaz se presente en **Portugués (nativo), Español e Inglés**. Esta configuración la realiza el usuario. En su perfil es posible seleccionar el idioma de presentación de la interfaz, sin tener que cambiar la configuración de idioma de su sesión de navegador de Internet.

.. figure:: /figuras/ucloud_idioma_plataforma_001.png
   :alt: Idioma de la Plataforma uCloud
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
   :alt: Pantalla de inicio de sesión de la Plataforma uCloud
   :align: center

----

Las credenciales de inicio de sesión y la contraseña deben haber sido aprovisionadas previamente en la Plataforma uCloud por un usuario con un perfil de administrador (u otro usuario con este permiso).

El usuario debe informar sus datos de inicio de sesión y contraseña en los campos y hacer clic en el cursor del mouse en el botón **Entrar**.

Si las credenciales de acceso no han sido aprovisionadas, no existen o en el último caso, el usuario no recuerda la información correcta de sus credenciales, no tendrá acceso a la plataforma. Ver el Item **Solicitud de Nueva Contraseña**, en caso de que el usuario oscurezca algún tipo de información para proceder con el inicio de sesión de acceso a la Plataforma uCloud.

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
---------

Después de informar al usuario y la contraseña, puede ver la pantalla principal del portal de uCloud, como se muestra en la pantalla a continuación, tiene un menú en el lado izquierdo con una lista de opciones, y cada opción representa una pantalla de administración de uCloud, algunas pantallas solo estarán disponibles de acuerdo con el nivel de acceso del usuario.

El usuario puede notar que la pantalla del panel de control está dividida en secciones, que se describen a continuación:


Sección Contenedores
--------------------

En esta sección se presentan todos los proveedores de la nube (públicos y /o privados) donde cada contenedor está representado con un "botón" en la interfaz, como se muestra a continuación:

.. figure:: /figuras/uCloud_acesso_platafform_003.png
   :alt: sección contenedores dashboard
   :align: center

----

Con cada necesidad de buscar información del contenedor el usuario interesado, debe seleccionar con el mouse el "botón" que representa el contenedor. 

Por lo tanto, para que el usuario pueda verificar sus cuotas y asignación de recursos, simplemente seleccione el contenedor elegido en la sección Gráficos de Uso de Recursos. Luego, al final de la selección, se cambiará la imagen de la pantalla y mostrará como resultado la representación de la asignación respectiva que se refiere al contenedor seleccionado.

Debido a que la Plataforma uCloud es un entorno híbrido de múltiples nubes, se mostrarán tantos botones como sea necesario para representar todas las nubes (públicas y/o privadas) que se hayan configurado en el entorno de uCloud.

En el caso de que solo haya un botón, esto significa que el cliente tiene un único proveedor de servicios en la nube configurado en su entorno.

Consulte el elemento **Contenedores** para comprender los procesos de cómo configurar un proveedor de servicios en la nube (público y/o privado) en la plataforma uCloud.

Sección de Gráficos de uso de recursos
--------------------------------------

En esta sección el usuario puede comprobar la cantidad de recursos computacionales disponibles (cuota límite) y los valores totales que ya han sido utilizados/consumidos por ella:

.. figure:: /figuras/uCloud_acesso_platafform_004.png
   :alt: sección graficos de uso de recursos
   :align: center

----

Estos límites (cuotas) han sido definidos y/o asignados al usuario, siguen los estándares y reglas de negocio de la organización, que estaban asociados con este usuario en el momento del aprovisionamiento de sus credenciales en la Plataforma uCloud.

Consulte los elementos Grupos y Usuarios para configurar o cambiar los límites (cuotas) de recursos computacionales o financieros, tanto para grupos como para un límite individual para un usuario específico.


Sección Últimas Tareas
----------------------

La plataforma uCloud es un entorno que se comunica con las consolas de los proveedores de la nube o con el hipervisor utilizado internamente en Datacenter en su organización a través de la API Rest. De esta forma, todas las acciones -actividades- funciones solicitadas a través de la Plataforma uCloud se 'encapsulan' como si fueran un `mensaje` y se envían a la consola de destino para que la consola realice las ´tareas´ enviadas.

.. figure:: /figuras/uCloud_acesso_platafform_005.png
   :alt: sección últimas tareas
   :align: center

----

En consecuencia, la sección Tareas presenta la última lista de acciones - actividades - roles solicitados por el usuario que está registrado y activo (login) en la Plataforma uCloud.

En esta sección, se presentará una lista de algunas tareas, que demuestran el porcentaje realizado y lo(s) resultado(s) respectivo(s) de esta(s) acción(es), ya sea para acciones completas exitosas o incompletas, debido a algún error recibido como respuesta de la consola de destino (pública y/o privada).

Consulte otros detalles en el elemento **Tareas**.

Sección Máquinas Virtuales
--------------------------

En esta sección, se enumerarán las máquinas virtuales que han experimentado interacciones o cambios recientes a través de la interfaz de la plataforma uCloud.

.. figure:: /figuras/uCloud_acesso_platafform_006.png
   :alt: sección últimas tareas
   :align: center

----

Importante destacar un punto: Máquina virtual que ha sido cambiada en cualquiera de sus características, a través de la consola del proveedor de servicios en la nube (pública y/o privada), esta máquina virtual no formará parte de esta lista. La plataforma uCloud enumera solo las máquinas virtuales que han sido cambiadas por usuarios registrados y activos (inicio de sesión) en la plataforma uCloud.

Consulte el elemento **Menú de Usuario** para comprender las funcionalidades de cada opción de menú hacer.


Accesos directos de la sección a los menús principales
------------------------------------------------------

En esta sección se presentan accesos directos a las características más frecuentes de la Plataforma uCloud, de una forma más accesible y directa.

.. figure:: /figuras/uCloud_acesso_platafform_007.png
   :alt: sección últimas tareas
   :align: center

----

Se puede acceder a todos los accesos directos presentados hasta ahora a través de sus respectivas funciones en el Menú de Usuario, que se coloca en la barra lateral izquierda en la interfaz de la plataforma uCloud.

Es importante tener en cuenta que el usuario activo (login) puede tener restricciones en ciertas opciones de menú, dependiendo del perfil asociado a ese usuario, determinado por la organización a la que está asociado el usuario. 

De esta forma, se enumerarán los accesos directos correspondientes al perfil del usuario al que se permitirá el acceso.

Solicitud de Nueva Contraseña
-----------------------------

Si el usuario no recuerda sus datos para iniciar sesión en la Plataforma uCloud, la aplicación le permite recuperar la contraseña de acceso durante el proceso de inicio de sesión o si el usuario recibe el mensaje en la esquina superior de la pantalla con una advertencia emergente **"Usuario o contraseña incorrectos"** como se muestra en la figura a continuación:

.. figure:: /figuras/uCloud_nova_senha_001.png
   :alt: solicitud de nueva contraseña
   :align: center

----

El usuario debe hacer clic en el cursor del mouse en la opción **"¿Olvidó su contraseña?"** como se detalla en la siguiente figura:

.. figure:: /figuras/uCloud_nova_senha_002.png
   :alt: solicitud de nueva contraseña
   :align: center

----

Si la información de inicio de sesión del usuario existe, pero si necesita ingresar una nueva contraseña, la Plataforma uCloud presentará al usuario el formulario para el cambio.

.. figure:: /figuras/uCloud_nova_senha_003.png
   :alt: solicitud de nueva contraseña
   :align: center

----

En el primer campo, el usuario informa la dirección de correo electrónico que está registrada y en el segundo campo debe rellenar con la información de inicio de sesión del usuario que se aprovisionó en la Plataforma uCloud.

Después de informar un correo electrónico válido y una cuenta de usuario para el acceso, el usuario debe hacer clic en el cursor del mouse en el botón verde `Edición`, la interfaz mostrará el siguiente mensaje:

.. figure:: /figuras/uCloud_nova_senha_004.png
   :alt: solicitud de cambiar contraseña
   :align: center

----

El usuario debe comprobar el recibimiento de un mensaje en su buzón de correo electrónico con las instrucciones para restablecer la contraseña. El usuario debe proceder como se describe en el correo electrónico y restablecer su contraseña de acceso.

.. figure:: /figuras/uCloud_nova_senha_005.png
   :alt: solicitud de cambiar contraseña
   :align: center

----

Debe verificar que el dominio "@ucloud.usto.re" esté bloqueado en su lista de mensajes no deseados (spam) para permitirle recibirlo.

Cuando el usuario hace clic en el cursor del mouse sobre el enlace/url presente en su correo electrónico, el usuario será llevado a una sesión de su navegador *(browser)* de Internet conectado a la plataforma uCloud, se mostrará la pantalla a continuación:

.. figure:: /figuras/uCloud_nova_senha_006.png
   :alt: solicitud de cambiar contraseña
   :align: center

----

Después de que el usuario informe de la nueva cadena en el campo **Nueva Contraseña**, el usuario debe volver a introducirla en el siguiente campo **Confirmar Contraseña** igual a la notificada en el campo anterior.

Después de confirmar la nueva contraseña, el usuario debe hacer clic en el cursor del mouse en el botón **Guardar**, la interfaz mostrará el siguiente mensaje:

.. figure:: /figuras/uCloud_nova_senha_007.png
   :alt: cambiar contraseña
   :align: center

----

Después de este procedimiento, el usuario puede realizar el proceso de inicio de sesión utilizando la información del usuario y la nueva contraseña. La nueva contraseña estará disponible de inmediato, y no tiene que esperar ningún período para la vigencia de la misma.


Usuario no aprovisionado
------------------------

Si la información de inicio de sesión del usuario no se ha registrado previamente o la combinación de datos de correo electrónico e inicio de sesión, la Plataforma uCloud mostrará un mensaje *pop-up*, en la esquina superior derecha de la pantalla, con la información de que los datos informados para cambiar la contraseña no existen en la Plataforma uCloud.

.. figure:: /figuras/uCloud_user_nao_provisionado_001.png
   :alt: usuario no aprovisionado
   :align: center

----

En este caso, simplemente póngase en contacto con el administrador de la plataforma uCloud de su organización para que puedan aprovisionar sus datos para el inicio de sesión. Solo un usuario correctamente aprovisionado tendrá su acceso efectivo.


Menú de Usuario
===============

La barra de menú del usuario se encuentra a la izquierda de la pantalla y se muestra inicialmente en modo expandido, como en la figura a continuación:

.. figure:: /figuras/uCloud_menu_usuario_001.png
   :alt: menú de usuario modo expandido
   :align: center

----

Algunas opciones de menú tienen un submenú, que se presenta cuando el usuario coloca el mouse sobre la indicación (signo inferior "<"). Al hacer clic en este icono, la interfaz presenta el submenú de esta opción al usuario, vea el ejemplo en la figura a continuación:

.. figure:: /figuras/uCloud_menu_usuario_002.png
   :alt: ejemplo de un submenú
   :align: center

----

Es posible que el usuario elija reducir la presentación de la barra de Menú de Usuario al modo Solo icono, para tener un área de presentación más grande. Para cambiar entre el Modo Expandido del Menú de Usuario y los Iconos del Modo de Menú de Usuario, hay un gráfico verde con tres barras , fácil de identificar para el usuario. Este elemento estará presente en cualquier pantalla de la Plataforma uCloud.

Cuando el usuario hace clic en este elemento, la barra de Menú de Usuario se cambiará a los Iconos de Modo, como se muestra en la figura a continuación:

.. figure:: /figuras/uCloud_menu_usuario_003.png
   :alt: menú de usuario modo iconos
   :align: center

----

Cuando la barra de Menú de Usuario está en modo de icono, los submenús se mostrarán como se muestra a continuación:

.. figure:: /figuras/uCloud_menu_usuario_004.png
   :alt: abrir un submenú en modo icono 
   :align: center

----

Las siguientes páginas detallan cada una de las opciones del menú de usuario y su funcionalidad.



Menú de Administración
======================

Al presentar algunos conceptos sobre el entorno de administración de uCloud, es importante aclarar algunos puntos sobre la Plataforma uCloud, en los conceptos existen tres términos que serán ampliamente utilizados en el entorno de uCloud:

  * **Contrato:** Es la forma en la que se define la relación *'comercial'* entre el prestador y la empresa que te contrató. En el contrato se definen los costos, el margen financiero, la tasa de conversión de moneda, los costos de recursos (opcional) y la cuota general (límite) que puede ser una cuota financiera o una cuota de recursos computacionales.

  * **Grupo:** Es una forma lógica definida únicamente dentro de la Plataforma uCloud que puede definir un grupo de usuarios (por ejemplo, DevOps), un departamento (por ejemplo, ventas), una iniciativa (por ejemplo, VDI), a la que se asocian múltiples usuarios como parte integral de este grupo. Estos "grupos" no existen en los proveedores de nube (públicos y/o privados) existen solo dentro de la Plataforma uCloud.

  * **Usuario:** Un usuario es la entidad que ha identificado el acceso a la Plataforma uCloud para tomar medidas sobre los recursos informáticos de los proveedores (públicos y/o privados).

La siguiente figura ejemplifica, en una imagen, la relación entre estos tres términos y es fundamental que el usuario utilice esta figura como referencia para entender los enlaces.

.. figure:: /figuras/ucloud_arquitetura_conceitual001.png
   :align: center

----

Es importante entender que un **Contrato** puede tener múltiples usuarios y varios grupos; cada **Grupo** puede contener estos usuarios. Sin embargo, la Plataforma uCloud permite que un Usuario forme parte de un solo contrato y un grupo, y un solo Grupo está vinculado a un solo contrato.

En el siguiente documento se describe que al configurar las cuotas (límites financieros o de recursos) del contrato, estos límites serán compartidos/divididos por cada uno de los grupos existentes, y por lo tanto los usuarios se limitan a las cuotas del grupo al que están incluidos.

Es posible señalar, en la figura anterior, que el término *Virtual DataCenter (VDC)* este término es una asignación lógica de máquinas virtuales que permite a las organizaciones definir uno (o más) grupos de servidores que forman parte de una nube. Un VDC puede representar un departamento, una subsidiaria o un grupo de usuarios, y otra información en el elemento **Virtual DataCenter**.

El término 'Administración' varía en función del perfil del usuario que está accediendo al sistema en ese momento. uCloud tiene cinco perfiles diferentes, que generalmente podemos describir a continuación:

  #. **Usuarios del sistema:** son usuarios habituales los que acceden al sistema para consumir recursos. Existe la posibilidad de *Usuarios con perfil de solo lectura*, quienes pueden designar usuarios regulares o habituales que solo pueden acceder a la Plataforma uCloud para ver la información.

  #. **Usuarios Administradores de Contrato:** son los usuarios que están asociados a un contrato y en este contrato pueden definir reglas de boletería, provisión y cambio de otros usuarios en la plataforma.

  #. **Usuarios Administradores de Grupo:** son usuarios que están asociados a un grupo de usuarios, pueden aprovisionar y cambiar a otros usuarios en la plataforma.

  #. **Usuario Administrador Financiero:** son usuarios con un perfil para acceder a la información financiera de uCloud.

  #. **Usuario Administrador:** son usuarios con perfil de acceso completo y pueden realizar intervenciones globales en la configuración de la plataforma. Este perfil de usuario es exclusivo de Ustore o de un perfil de usuario único de la organización que compró las licencias de la plataforma uCloud. Este usuario administrador tiene permiso para administrar todas las funciones y recursos globales que ofrece la plataforma. 


.. note::
  |atencao| *El perfil de administrador no se tratará en este documento. Por favor, póngase en contacto con su punto focal en Ustore para obtener el documento específico: Manual del Administrador de la Plataforma uCloud. Por seguridad, las mejores prácticas indican que  solo debe haber un usuario aprovisionado con este tipo de perfil.*




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




Switch Roles - Escenario de Ejemplo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

En la figura anterior podemos ver que los usuarios Maria, João y Carlos pertenecen a un solo contrato y este contrato tiene un solo proveedor (por ejemplo, *AWS*).

El usuario **Josué** está asociado con dos acuerdos diferentes, y para evitar que este usuario tenga que cambiar entre diferentes sesiones de inscripción (terminando una sesión e iniciando otra con otra credencial), Ustore ha desarrollado e implementado la funcionalidad **Switch Roles**.

De esta manera, **solo** el usuario Josué, a través de la funcionalidad de *Switch Roles* puede cambiar entre los contratos a los que está vinculado, simplemente cambiando entre los contratos vinculados.

El usuario **Josué** es responsable de administrar completamente la infraestructura del entorno de Azure, pero en el entorno de AWS, solo puede ver los recursos computacionales porque no tiene permiso para operar estos recursos informáticos (por ejemplo, *Read Only*).

A través de la funcionalidad *Switch Roles* será posible aplicar este cambio de rol, sin necesidad de intercambio de usuarios, esto se hará a través de la selección de contrato y/o contenedor al que este usuario quiera acceder.

También para ilustrar este ejemplo, con la nueva implementación de Perfil de Permisos, puede crear diferentes conjuntos de permisos y vincular cada conjunto (Perfil de Permisos) a cada usuario y aprovisionar un nivel muy específico de granularidad.


Escenario de Ejemplo (*AWS*):
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


Escenario de Ejemplo (*AZURE y AWS*):
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


Switch Roles - Utilizando :
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


Menú Administración / Usuarios
------------------------------


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
Manual del Entorno VDI Ustore*



Visualización de un Usuario
---------------------------

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




Creación de Usuario
-------------------

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

 .. *1. **Gobernanza Financiera**

 .. *2. **Billing (Facturación de los Servicios)**

 .. *3. **Supervisión de la Infraestructura**

 .. *4. **Inventario (*Assessment*)**

.. La plataforma de uCloud se conecta ...

..  *5. **Operación de la Infraestructura**

.. Con el inventario disponible ...

Submenú Máquinas Virtuales
--------------------------

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

Editando Workflows xxxx
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

Menú Tareas
===========

Pestana Tareas
--------------

Pestana Aprobaciones Pendientes
-------------------------------

Pestana Tareas Programados
--------------------------

Menú Inventário de Recursos
===========================

Editor de Etiquetas *(tags)* Nativo
-----------------------------------

Conclusión
----------

====

**Equipo Ustore**


uCloud Manual de uso
Revisión 22/11/2022


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





































 

