uCloud - Notas Mayo - 2022 
==========================

.. figure:: /figuras/ucloud_logo_peq.png
   :alt: Logo uCLoud
   :scale: 50 %
   :align: center
   
----

Plataforma uCloud versão: *update tag 5.2-b35*

Presentación
=============

En general, el profesional de la infraestructura de TI utiliza diversas consolas para aprovisionar recursos computacionales, sea dentro de la organización (*datacenter* privado) o en algún proveedor de la nube. La computación en nube es una evolución de los servicios y productos de tecnología de la información bajo demanda, denominada por Brantner et al., 2008 de *Utility Computing*, que tiene como objetivo ofrecer componentes básicos como: almacenamiento, procesamiento y ancho de banda de una red a través de proveedores especializados con un bajo coste por unidad utilizada. En la  contemporaneidad, mantenerse actualizado y preparado en todas las «consoles» es un desafío para este profesional.

En el intento de aumentar la productividad y reducir el grado de dependencia de estas consolas, el mercado ha desarrollado el concepto de infraestructura como código (*IaaC - Infrastructure as a Code*). Este concepto aborda solo el momento del aprovisionamiento inicial (hasta con la utilización de scripts para la instalación de estándares y softwares), pueden existir demandas en las que el profesional de TI deberá conectarse a la consola del ambiente, para efectuar alguna intervención en la infraestructura que no sea posible a través del concepto de IaaC. Estar conectado y quedarse cambiando entre las distintas consolas de la nube, requiere una gran experiencia y conocimiento del profesional de TI.

Las plataformas CSB (*Cloud Service Broker*) se han desarrollado para ocupar este nicho y concentrar el inventario de los recursos computacionales de las nubes públicas y privadas en una única interfaz y que transfiere al usuario el control y la operación de estos recursos multi-nube.

Como se ha mencionado, el propio mercado desarrolló las metodologías de aprovisionamiento de recursos computacionales a través de *scripts* automatizados (también llamados *playbooks*). Entre estos formatos hay algunos que el mercado mundial ha adoptado más ampliamente, se puede mencionar a Ansible, Terraform y Puppet.

El mercado también ha creado la demanda de programar la ejecución de una secuencia de diversos *scripts* dentro de un flujo controlado y encadenado, de modo que un error en uno de estos *scripts* puede interrumpir todo el flujo para evitar el aprovisionamiento de una infraestructura computacional sin la adecuada calidad.

Atenta a la constante evolución del mercado brasileño y a las demandas de nuestros usuarios, la **Ustore** presenta las nuevas implementaciones, las correcciones, las integraciones, las actualizaciones en el menú de funcionalidades y su descripción detallada.

Además de la ampliación del concepto existente, este *Release Notes detalla el update* ocurrido en la plataforma uCloud, contenida en la (tag.5.2-b35) atendiendo a las diversas demandas mercadológicas de nuestros clientes, capaces de transformar la forma de gestionar las nubes públicas y privadas con la plataforma uCloud.

Nuevas Implementaciones
=======================

Las novedades presentadas a continuación han sido categorizadas en:

* Acciones correctivas para la adecuación a los cambios ocurridos en los proveedores de la nube;
  
* Integraciones realizadas en el portal;

* Actualizaciones globales en algunos menús de funcionalidad del portal.

Además de las innovaciones más sólidas, enumeradas en tres temas. Estas nuevas implementaciones se describirán en detalle en el transcurso de este documento.

#. Account
#. TAGs Virtuales
#. Oracle OPS

Acciones Correctivas
====================

En este *Release Notes* se enumeran todas las acciones correctivas implementadas, motivadas por determinadas situaciones comunicadas a nuestro equipo de desarrolladores.

Amazon Web Services (AWS)
-------------------------

En relación con la interacción con el proveedor de servicios de nube pública AWS, no hubo ninguna modificación, corrección, nueva implementación o nueva funcionalidad.

Microsoft Azure (Azure)
-----------------------

En cuanto a la interacción con el proveedor de servicios de nube pública Microsoft AZURE, podemos enumerar las siguientes alteraciones:

#. Adaptación del *Scaling Group* para adaptarse a la actualización del modelo de respuesta enviado por la nube.  Después de esta implementación, al crear un *Scaling Group* el proceso crea automáticamente un Grupo de Instancias, para ser gestionadas por este *Scaling Group*.

#. Ajuste al modelo de tratamiento de la eliminación de discos asociados a Máquinas Virtuales. Esta mejora ha sido necesaria debido a un cambio en la forma en que se realiza la eliminación en la nube. Adaptación en el PMC para acompañar esta mejora.

Google Cloud Plataform (GCP)
----------------------------

En cuanto a la interacción con el proveedor de servicios de nube pública Google *Cloud Platform* (GCP), podemos enumerar los siguientes cambios:

* Nueva ejecución en el funcionamiento de los *Listeners* y Miembros de un Balanceador.

* Adición de soporte al crear el Balanceador utilizando el protocolo HTTP.

* Aplicación de reglas UDP (*User Datagram Protocol*) para Grupos de seguridad.
 
* Inclusión de las nuevas regiones, son:

  * Columbus, Ohio, América del Norte: us-east-5

  * Dallas, Texas, América del Norte: us-south1

  * Madrid, España, Europa: europe-southwest1

  * Milán, Italia, Europa: europe-west8

  * París, Francia, Europa: europe-west-9

Huawei Cloud (Huawei)
---------------------

En cuanto a la interacción con el proveedor de servicios de nube pública Huawei Cloud, no hubo ninguna alteración, corrección, nueva implementación o nueva funcionalidad.

IBM Cloud
---------

En cuanto a la interacción con el proveedor de servicios de nube pública IBM Cloud, podemos enumerar la siguiente modificación:

#. Implementación de la regla de negocio para deshabilitar la edición de la única NIC (*Network Interface Card*) de la Máquina Virtual.

VMware 6.5 o superior (vCenter/vSphere)
---------------------------------------

En cuanto a la interacción con el hipervisor de nube privada VMware 6.5 (o superior), podemos enumerar los siguientes cambios:

#. Actualización en la forma de crear subredes para adecuarse a la nueva versión de uSDN.

#. Comportamiento anómalo corregido, varias conexiones se abrían al mismo tiempo.

VMware vCloud
-------------

En cuanto a la interacción con el hipervisor de nube privada VMware 6.5 (o superior), podemos citar los siguientes cambios:

* Corrección de la importación de *container*.

* Actualización de la API a la versión 35.0.

Integraciones
-------------

* Hubo una implementación y mejora de la comunicación con el agente de monitoreo (*Mangue/uCloud*).

Actualizaciones
---------------

A continuación enumeramos la lista de actualizaciones que se han implementado en la Plataforma uCloud:

#. Ampliación de la cobertura de las traducciones de los elementos o ítems del portal, tanto al español como al inglés.

#. Actualización de la tabla de precios de los *flavors*.

#. Revisión de la comunicación en los mensajes de excepción del portal, enfoque en la interacción del usuario con el contenido y la experiencia de uso.

Menu Virtual Datacenter (VDC)
-----------------------------

#. Reducción del tiempo de carga en la pantalla de edición de VDC de un *container*.

Menú Perfiles de Visualización
------------------------------

#. Adición de los módulos uLog y uMonitor como opción de selección en los Perfiles de Visualización.

Descripción de las nuevas implementaciones
==========================================

A continuación describiremos las características técnicas y operativas de tres de las nuevas implementaciones que se aplicaron para esta nueva versión/*release* de la Plataforma uCloud. En este capítulo se enumeran las nuevas implementaciones, que serán aclaradas a lo largo de este documento.

#. Account

#. TAGs Virtuales

#. Oracle Cloud Infrastructure (OCI) - *solo las funcionalidades de operación*

Descripción del Account
=======================

La Plataforma uCloud puede implantarse de dos maneras diferentes:

\ A. \ Instalación dedicada (*on-premises*)

Para el escenario de la instalación dedicada (*on-premises*) la funcionalidad de *Account* puede no ser aplicada, probablemente esta instalación pertenece a una sola empresa, y esta empresa no compartirá la Plataforma uCloud entre otras organizaciones. También en este escenario, vamos a suponer que la instalación de la Plataforma uCloud se utilizará solo en la(s) propia(s) nube(s) (pública y/o privada).

\ B. \ Instalación compartida como servicio (*SaaS - Software as a Service*)

La funcionalidad *Account* está pensada para el escenario de instalación compartida (*SaaS*), donde la empresa (la denominaremos **organización**) tiene como objetivo prestar servicios de *Cloud Service Broker* con la Plataforma uCloud entre sus diversas operaciones (regionales o internacionales) y para sus diversos clientes finales.

El escenario arriba mencionado de la Plataforma uCloud SaaS es ideal para un proveedor de servicios de conectividad/comunicación (*organización*) que puede compartir la Plataforma uCloud entre sus operaciones regionales y también entre sus clientes finales que desean los beneficios de una operación, gobernanza financiera y *billing*.

Esta funcionalidad ayuda la gestión y el control del ambiente de la organización, de manera centralizada, a través de su regla de negocio, permite la creación de "Cuentas" y la asignación de los Contratos, Grupos y sus Usuarios (elementos pertenecientes al universo "*Switch Roles*").

Posibilita organizar y compartir los recursos entre las "Cuentas" creadas, así como aplicar políticas de control de servicios a los **contratos**, **grupos** y **usuarios**, optimizando la mejora de la gobernanza. Este nuevo modelado inserta la capa "Cuenta" en el menú de **Administración**, que representa un nuevo proceso para promover la alineación en torno a la funcionalidad "Cuentas" y así llevar a las organizaciones a lograr un mayor control.

Esta funcionalidad "Cuentas" tiene como objetivo dar a la organización la posibilidad de segmentar los clientes por tamaño (máquinas virtuales), por volumen de ingresos (costes financieros), permite entender el rendimiento por "Cuenta" y filtrar su historial por línea de negocio.

Para ejemplificar una forma de cobrar por la "oferta de servicio" de Gestión Centralizada de la Nube por parte de la Plataforma uCloud, utilizaremos el ejemplo de los *niveles de consumo* de la infraestructura computacional basado en el número de Máquinas Virtuales Gestionadas por la Plataforma uCloud, llamado "Tier". Los *Tiers* representan el modelo de tarificación existente en la funcionalidad "Cuentas", la regla de negocio creada establece la contabilización de los recursos obtenidos y generados por una determinada cuenta.

En el portal, los *Tiers* se clasifican en los niveles A - J (1 a 10) y se calculan en función de las reglas establecidas mediante dos parámetros: - Un determinado número de máquinas virtuales genera un determinado coste máximo *(número de máquinas frente a coste/valor)*. En el caso de una cuenta creada, al alcanzar uno de los parámetros, inmediatamente, la aplicación escala al siguiente nivel. A continuación, se describen los niveles de los *Tiers*:

+---------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+
| **Tier**            |  **A** |  **B** |  **C** |  **D** | **E**  |  **F**  |  **G**  |  **H**  |  **I**  |  **J**  |
+=====================+========+========+========+========+========+=========+=========+=========+=========+=========+
|| **Cantidad de**    ||       ||       ||       ||       ||       ||        ||        ||        ||        ||        |
|| **Máqs.Virtuales** || ≤ 20  || ≤ 30  || ≤ 50  || ≤ 75  || ≤ 100 || ≤ 150  || ≤ 200  || ≤ 250  || ≤ 300  || ≤ 500  |
+---------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+
| **Valor Mensual**   | $1.500 | $3.000 | $4.000 | $6.000 | $8.000 | $16.000 | $24.000 | $32.000 | $40.000 | $64.000 |
+---------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+

.. important:: Todas las cantidades y valores mostrados arriba son meramente ilustrativos, sirven solo como ejemplos.

Ejemplo de casos de uso
-----------------------

* *Contrato Empresa Galáxia (cant. VMs 20)*:

Solo con el fin de ejemplificar un escenario, vamos a describir la oferta de servicios utilizando la Plataforma uCloud en la modalidad SaaS (Software como Servicio) para la empresa Galáxia, y en su "*Conta*" hay 20 máquinas virtuales (activas y gestionadas por la Plataforma uCloud), se ajusta al nivel *Tier* "A" - siendo el valor mensual a invertir por la empresa Galáxia de R$ 1.500 reales o dólares (dependiendo del país en el que esté establecida la empresa). Una observación importante, si la cuenta utiliza solo 18 máquinas, seguirá siendo clasificada como *Tier* "A".

Segmentación por Cuentas
------------------------

Existen dos clases de "*Contas*" que se clasifican en dos tipos, las cuentas de tipo **Integrator** y las cuentas de tipo **Producer**, que se detallan a continuación:

* \ A. \ **Cuenta Integrator** Esta cuenta es la responsable de crear los perfiles de las cuentas *Integrator* y *Producer*, al crear estos perfiles alimenta los *tiers* y paquetes, además de establecer, la cuenta *Producer* su regla de uso. Para ejemplificar: funciona como una especie de *cluster*, aglomerando o categorizando otras corporaciones.

  * Por ejemplo: 

  Para el caso de una **corporación** multinacional que utiliza una cuenta *Integrator*, se puede considerar una "Cuenta Integrator" para los países que la componen: México, Brasil, Chile y Colombia.
  La corporación es responsable de crear otras cuentas y escalar los permisos de otros usuarios. Tiene como particularidad la lista de todas las cuentas Producer, la lista de todos los contratos asociados y puede aplicar las reglas de negocio.

* \ B. \ **Cuenta Producer** Esta cuenta *Producer* pertenece a la organización que consume el recurso, representa una unidad de agrupación menor y puede operar todo el portal.

  * Por ejemplo: 
  
  En la continuación del ejemplo anterior, esta corporación multinacional crea las "cuentas Producer" para las organizaciones que pertenecen a ella dentro de un determinado país que se ha mencionado anteriormente, en Brasil, la organización posee las empresas A y B que gestionan los contratos a1 y b1.

A continuación se muestra una ilustración que presenta el concepto completo del alcance de la funcionalidad **Account** implementada en la Plataforma uCloud. Los nombres y denominaciones utilizados son meramente ilustrativos.

.. figure:: /figuras/ucloud_arquitetura_conceitual003.png
   :align: center
   
----

Las cuentas *Producer* pueden tener un administrador o más (en este nivel el perfil de este usuario es de un Administrador del Sistema - por ejemplo, *root*), los contratos dejan de ser creados cuando el recurso de la cuenta corporativa termina, los perfiles de visualización y permisos obedecen a la regla de negocio aplicada por la cuenta *Integrator*.

La estrategia de utilización de la funcionalidad "*Contas*" ofrece una mejor percepción del valor en el nivel jerárquico en el que se quieren organizar los datos en el contexto de la organización, facilitando su tránsito por los niveles operativo, directivo y ejecutivo.

Con la creación de esta funcionalidad, el administrador de la cuenta puede gestionar los permisos de visualización y los permisos de cada **usuario** dentro de cada **grupo**, contenidos en un determinado **contrato**. Así, el acceso se niega por defecto, siendo concedido solo cuando los permisos especifican "permitir".

Adicionalmente, la funcionalidad "*Contas*" posibilita utilizar las políticas de control que establecen las barreras de protección de permisos y visualización de los usuarios, dependiendo de las características de tipo de usuario, grupo y contrato al que pertenezcan.

Al establecer estos patrones de permisos, accesos y visualizaciones de los recursos, organiza y califica el privilegio que tendrá cada usuario dentro de los ambientes de los proveedores de la nube pública a los que pertenece cada contrato/grupo/usuario, creando así permisos diferentes y necesarios para crear controles minuciosos en cada cuenta.

Descripción de TAGs Virtuales
=============================

En un contexto amplio, un *TAG* (un rótulo o etiqueta) es una palabra clave que señala o identifica un determinado recurso computacional (o servicio derivado de su existencia) almacenado en un proveedor de la nube, un repositorio o una base de datos. Los *TAGs* son un tipo de metadatos, capaces de proporcionar información que describe los datos, esto facilita la búsqueda automatizada para la recuperación de informaciones. Un *TAG* es una etiqueta en la que el usuario asigna una **Clave** y un **Valor** a un recurso computacional de la nube pública.

En el escenario de cualquier tipo de nube, los datos contenidos en los *TAGs* se utilizan junto con otras formas de etiquetaje que los proveedores de la nube aplican para clasificar la información acerca de sus recursos. Así, los *TAGs* ayudan la búsqueda, organización, identificación, gestión y finalmente el filtrado de los recursos utilizados de cualquier proveedor de la nube, por ejemplo: AWS, Azure, Google, entre otros.

Estos *TAGs* (etiquetas), una vez vinculados a un recurso, se utilizan para categorizar dichos recursos de manera que puedan ser clasificados por: propósito, propiedad, criterio o ubicación. Por ejemplo, el usuario, o la organización, pueden definir un conjunto de *TAGs* para las instancias de Amazon EC2, de su cuenta, para ayudar a rastrear el propietario y/o el nivel de agrupación (apilamiento de valores - *stack*) de cada recurso computacional de la nube pública consumido.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual001.png
   :align: center

----

.. note:: La figura de arriba es un ejemplo y las informaciones son meramente ilustrativas.

En la imagen de arriba utilizamos dos máquinas virtuales como ejemplo para ilustrar la vinculación de *TAGs* a los recursos. Un detalle que se menciona muy poco es que los proveedores de servicios en la nube pública *no permiten vincular TAGs a todos sus productos y/o servicios* (consulte la documentación del proveedor para saber cuáles son los recursos susceptibles de tener un *TAG* vinculado al recurso).

En el ejemplo de arriba vinculamos "**dos** *TAGs* diferentes" al mismo recurso (máquina virtual) de esta manera inducimos que los informes financieros por *TAG* totalicen el valor del costo del *TAG* dos veces (el mismo valor en cada *TAGs*) y para este ejemplo en esta situación duplicar el costo dentro del mismo período.

Pero debemos señalar que para el ambiente del proveedor de servicios en la nube pública, una vez que se crea un *TAG* este no estará automáticamente vinculado a cualquier recurso (o servicios derivados de la existencia del recurso). El usuario debe crear primero el/los *TAG(s)* y después vincular manualmente el/los *TAG(s)* al/los recurso(s) deseado(s). Como se trata de un proceso manual y realizado por un usuario en la consola del proveedor de servicios en la nube, el recurso de los *TAGs* puede consumir mucho tiempo del administrador de costes de la nube pública. Puede existir una cantidad muy grande de líneas en el archivo de *billing/bucket* para el Administrador de Costos verificar. Este proceso de verificación y vinculación de *TAGs* es continuo y manual.

.. important:: Debido a que los *TAGs* son accesibles a muchos servicios en los proveedores de la nube, es relevante evitar añadir datos privados o confidenciales a los *TAGs* virtuales, como por ejemplo: identificación personal, información confidencial o sensible.

La Plataforma uCloud sincroniza y recibe el contenido del archivo de *billing* (CSV) del proveedor de servicios en la nube pública y, en consecuencia, recibe todos los *TAGs* existentes en el proveedor.

TAGs Virtuales de la Plataforma uCloud
--------------------------------------

Mencionamos anteriormente que el proceso de vinculación de un *TAGs* a un recurso es manual, requiere mucho tiempo y, principalmente, no se repite de forma automática para nuevos servicios de un recurso que ya tenga un *TAG* vinculado.

La nueva función de *TAGs* virtuales de la plataforma uCloud crea una automatización para el proceso de vinculación de los *TAGs* a los recursos existentes en el ambiente del proveedor de servicios de la nube pública.

El procesamiento de *TAGs virtuales* de la Plataforma uCloud, puede vincular automáticamente un *TAG* específico a un recurso a ser seleccionado basado en el *Nombre del Producto y/o Familia del Producto y/o Identificador del Recurso*. Es importante destacar que la conjunción "**y/o**" demuestra el alto grado de granularidad que el usuario puede seleccionar para atender al uso específico de su necesidad. 

Veamos a continuación cómo la nueva implementación de *TAGs* Virtuales permite automatizar la vinculación de *TAGs* en los recursos.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual002.png
   :align: center

----

.. note:: La figura de arriba es un ejemplo y las informaciones son meramente ilustrativas.

En el ejemplo anterior, siempre que la Plataforma uCloud efectúe la sincronización del archivo CSV de *billing/bucket*, **automáticamente** los *TAGs* serán vinculados para todos los registros (filas) de recursos en el archivo de *billing* para los que la correlación de *Product Name* o *Product Family* o *Identificador de Recurso* sea encontrada.

Los "Tags Virtuales" son aplicados a los recursos de la nube (por ejemplo: máquinas virtuales, bases de datos) para que sea posible crear clasificaciones por proyectos, divisiones por centros de costos, entre otros tipos de agrupaciones. Estas claves y valores *TAGs* pueden o no reflejarse en los informes de *billing* disponibles para consulta solo a través de la consola del proveedor de la nube pública. Así, los recursos importados desde el archivo de *bucket/billing* que existe en los proveedores de la nube pública que por cualquier política de estos proveedores dejan de indexar la etiqueta al recurso del servicio en la nube, pueden recibir un "TAG virtual". Pero es muy importante destacar que estos "TAGs virtuales" existen solo en la base de datos de la Plataforma uCloud, no siendo escritos (o sincronizados) en el *bucket/billing* que existe en el ambiente del proveedor de servicios de la nube pública.

Este es un servicio único y está disponible con la nueva implementación de la Plataforma uCloud para facilitar la clasificación de los recursos utilizados en las **distintas nubes** a través del "*TAG Virtual*". El *TAG Virtual* debe ser creado por la organización cliente, puede basarse en el perfil de categorización, según el recurso utilizado y la necesidad de identificación en el informe financiero, ya sea por finalidad, propiedad, criterio o ubicación, entre otros.

El "*TAG Virtual*" debe ser aplicado por el cliente usuario dentro del portal uCloud, con el fin de permitir la identificación automatizada del recurso que dejó de ser etiquetado por los diversos proveedores de la nube por las diferentes reglas y políticas internas de cada uno de ellos. Después de la aplicación de la "*TAG Virtual*" como un recurso de la plataforma uCloud y luego aplicar a través del *Accountant virtual-tag-applier*, y la normalización de ellos, utilizando el *Accountant virtual-tag-normalizer*. De este modo, se facilitará la visualización de las informaciones para la toma de decisiones, registradas en los informes financieros, en relación con el uso de los recursos proporcionados por las distintas nubes que no han sido previamente etiquetados por la propia nube.

Las organizaciones que utilizan procesos automatizados para gestionar la infraestructura incluyen los *TAGS* adicionales específicos para la automatización, en general, crean agrupaciones relevantes para organizar los recursos en las dimensiones técnicas, comerciales y de seguridad.

Normalización de TAGs Virtuales
-------------------------------

Es importante mencionar que la existencia continua de un recurso en el proveedor de servicio en la nube, genera nuevos servicios o productos que surgen de la existencia/mantenimiento del recurso en la nube del proveedor de servicio en la nube pública (por ejemplo, *snapshots*).

Cuando un cliente solicita la creación de una copia de seguridad de la imagen de disco (*snapshot*), un nuevo *snapshot* puede, no necesariamente, recibir la vinculación de un *TAG* en el proceso de *TAGs* Virtuales.

Para cubrir este vacío existe la nueva funcionalidad de **Normalización de TAGs**.

Este proceso realiza una comparación de cada línea del archivo de *billing* y cuando encuentra un recurso "sin TAG Virtual" pero esta línea es un nuevo servicio/producto de un recurso con *TAG* Virtual, este proceso **HACE UNA COPIA** del *TAG* Virtual del recurso principal aunque su combinación de *ProductName*, *ProductFamily*, *Identificador del Recurso* no haya podido vincular el *TAG* Virtual.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual003.png
   :align: center

----

.. note:: La tabla de arriba es un ejemplo y las informaciones son meramente ilustrativas

Este proceso puede llevar algún tiempo, ya que se realiza con la comparación de *string* de caracteres de cada línea de **billing** de forma individual. 

Con este proceso la Plataforma uCloud complementa la nueva funcionalidad de los *TAGs* Virtuales, pero solo debe ejecutarse cuando el usuario Administrador de Costes identifique que hay recursos sin *TAGs* Virtuales.

¿Cuándo utilizar?
-----------------

A partir de esta nueva implementación, orientada a la clasificación, normalización y visualización de las informaciones obtenidas de diversos proveedores de nube pública, la nueva funcionalidad " TAGs Virtuales" permite "*etiquetar/marcar*", es decir, señalar los recursos que por alguna regla o definición, no ha sido posible encontrar registrados en el *billing* de un determinado proveedor de nube utilizado por la organización o cliente usuario. 

Dado que cada nube presenta diferentes informes de los recursos utilizados, la dificultad para el profesional de TI conseguir normalizar y comprender la clasificación presentada por las diversas nubes, o incluso la información suprimida por la ausencia de *TAGs* que agrupan en un formato relevante, informaciones preciosas, sean cuantitativas, cualitativas o financieras, facilitando a la organización y/o a su cliente usuario la posibilidad de tomar decisiones asertivas, mediante el uso de esta nueva implementación, denominada "TAGs Virtuales". Desarrollado por Ustore como una solución para satisfacer esta ausencia, demandada en los "*reports*" que tienen un comportamiento similar en los distintos proveedores de la nube, como AWS, Azure, Google entre otros.

El portal uCloud genera el report financiero, este informe recupera informaciones por nombre de producto o por TAG. Es el portal ucloud el que ofrece este servicio único de "TAGs virtuales" que permite y/o facilita la gestión y clasificación de determinados recursos que ya no reciben TAGs en la nube, como se ha dicho anteriormente, por reglas o políticas internas establecidas por los propios proveedores.

Es necesario utilizar esta nueva implementación, cuando la organización y el cliente usuario necesitan recuperar informaciones por *TAG* o nombre de producto de forma diferente, en las diversas nubes, ya que cada proveedor de nube, como Google, AWS y Azure trata el informe de registro de *billing* de forma diferenciada. Y cada una de ellas utiliza nomenclaturas propias para cada tipo de recurso ofrecido.

Al aplicar "TAGs virtuales" a los recursos de la nube (por ejemplo, bases de datos y máquinas virtuales) es posible crear clasificación por divisiones de centros de costes, proyectos y otros tipos de agrupaciones.

La nueva implementación del portal uCloud permite presentar informes en el reporte financiero generado de acuerdo a lo clasificado o "etiquetado" por el usuario para agrupar o identificar informaciones, sea por nombre de producto, propósito, propiedad, criterio o ubicación, entre otros.

.. note:: Las claves y los valores de los *TAGs* pueden o no reflejarse en el informe (*report*) de facturación (*billing*) de las distintas nubes. Los *TAGs* no tienen significado semántico en Amazon EC2, se interpretan como una cadena de caracteres.

Así, los recursos importados del archivo de *billing* de las nubes públicas que por alguna política de estos proveedores no indexen la etiqueta al recurso del servicio en la nube, pueden recibir un "*TAG virtual*" dentro del portal.

Restricciones de los TAGs
-------------------------

En el caso de la aplicación de "TAGs virtuales", hay algunos consejos básicos y restricciones que deben aplicarse:

* Número máximo de *TAGs* por recurso: 50

* Tamaño máximo de la clave: 128 caracteres

* Tamaño máximo del valor: 256 caracteres

* Caracteres permitidos:

  * Los caracteres permitidos en los servicios son: letras (a-z, A-Z), números (0-9) y espacios representables, así como los siguientes caracteres: + - = . _ : / @.
   
  * Para habilitar las etiquetas de instancia en los metadatos, las claves de las etiquetas de instancia permiten utilizar letras (a-z, A-Z), números (0-9) y los siguientes caracteres:+ - = . , _ : @. Evite los espacios o /, y no puede formar solo . (un punto), .. (dos puntos) o _index.
  
.. note:: En todos los recursos, cada clave de la etiqueta debe ser exclusiva y solo puede tener un valor.
 
.. important:: Las claves y los valores de los *TAGs* distinguen entre mayúsculas y minúsculas.

.. warning:: El prefijo aws: se reserva para el uso de AWS. No se puede editar o eliminar la clave o el valor de un *TAG* cuando tiene una clave *TAG* con este prefijo. Los *TAGs* con el prefijo aws: no cuentan para los *TAGs* de límite de recursos.

¿Cómo se utiliza?
-----------------

Esta nueva implementación permite etiquetar los recursos ausentes de etiqueta en el billetaje de las nubes, sea por regla o por definición. Lo que resulta en la obtención de información relevante de aquellos recursos que ya no serían categorizados y recuperados. 

Hay algunas estrategias comunes de etiquetaje que ayudan en la identificación y gestión de los recursos en la nube, para organizar los recursos y para asignar los costes, así como varias categorías de etiquetaje en la nube, por ejemplo en AWS:

* Técnicas

* Automatización

* Comerciales

* Seguridad

Los *TAGs* adicionales son más eficientes para crear agrupaciones, *TAGs* técnicos, *TAGs* de automatización, *TAGs* comerciales y *TAGs* de seguridad. Entre ellas se encuentran: Nombre, ID de la aplicación, Rol de la aplicación, *Cluster*, Ambiente, Versión, Fecha/Hora, Aceptación/Rechazo, Seguridad, Proyecto. Propietario, centro de Costes/Unidad de negocio, Cliente, Confidencialidad y Conformidad.

.. note:: Comportamiento del *TAG* en la nube de AWS - Los *TAGs* creados por el sistema que comienzan con **aws**: están reservados para el uso de AWS, no se puede editar o eliminar un *TAG* que comience con el prefijo aws. En cuanto al límite de creación de *TAGs*, cada recurso puede tener un máximo de 50 *TAGs* creados por el usuario.

Podemos resumir que el proceso de utilización de la funcionalidad de los *TAGs* virtuales se aplica en dos momentos distintos:

1. **Creación y automatización del uso de TAGs Virtuales**

   \ a. \ Aprovisionar un nombre de identificación para **un único** perfil de *TAGs* virtuales con todas las vinculaciones de *TAGs* basadas en la combinación de *Product Name* y/o *ProductFamily* y/o *Identificador del Recurso*.

   \ b. \ Vincular Perfil de *TAGs* Virtuales al identificador de la nube (*container*)

   \ c. \ Realizar el procesamiento y la sincronización de los archivos de *Billing/Bucket*

   \ d. \ Visualización de los informes financieros en la plataforma uCloud usando la totalización por **TAGs**.

   \ e. \ Si se identifica que todavía hay recursos *SIN TAGs* (recordemos la existencia de algunos recursos que el proveedor de servicios en la nube pública no vincula a ningún *TAG*; o que la combinación de *ProductName*, *ProductFamily*, *Identificador del Recurso*, no fue suficiente para asociar la totalidad de las líneas del archivo de *billing*), la Plataforma uCloud permite abordar esta ausencia de *TAGs* con el proceso siguiente.

2. **Normalización de TAGs Virtuales**

   \ a. \ Este proceso solo debe aplicarse cuando la combinación existente en el perfil de *TAGs* virtuales no puede aplicar *TAGs* a todos los recursos.

   \ b. \ Este proceso debe ejecutarse SOLO UNA VEZ al mes, ya que lleva un cierto tiempo para completar la normalización de todas las líneas de *billing* en el período del mes en curso. Este proceso debe *iniciarse manualmente y normaliza los TAGS virtuales solo para un único periodo, no es recurrente ni automático*.

A continuación se muestra la pantalla con la nueva implementación en el portal uCloud:

.. figure:: /figuras/fig_release_note_maio_spa/ucloud_menu_configuração_tag_virtual_spa001.png
   :align: center

----

Con la incorporación de la nueva funcionalidad en el portal y la posibilidad de emplear los "TAGs Virtuales" para recuperar la información previamente etiquetada del recurso utilizado en cualquier proveedor de la nube, de forma única, donde la utilización puede darse en dos flujos, detallados a continuación:

#. Etiquetaje de recursos en la nube a través de la especificación de un [**ProductName**], [**ProductFamily**] y el [**Identificador de la Nube**].

   \ a. \ Para este flujo el usuario puede especificar, por ejemplo, que el recurso perteneciente al *ProductName Amazon Elastic Compute Cloud*, en [*ProductFamily*] **Data Transfer**, vinculado al identificador de la nube i-0e85640d78d096974 tenga los *TAGs* especificados en el formulario, aunque estos *TAGs* no sean proporcionados por la nube.


.. figure:: /figuras/fig_release_note_maio_spa/ucloud_menu_configuração_tag_virtual_spa002.png
   :align: center

----

.. figure:: /figuras/fig_release_note_maio_spa/ucloud_menu_configuração_tag_virtual_spa003.png
   :align: center

----

   \ b. \ Vincular el perfil de *TAGs* Virtuales creado, a la nube (*container*) aprovisionada en la plataforma uCloud.

.. figure:: /figuras/fig_release_note_maio_spa/ucloud_menu_configuração_tag_virtual_spa004.png
   :align: center

----

2. Normalización de *TAGs* para los recursos de nube no recuperados en *TAG* categorizada.

   \ a. \ Para este flujo, será posible habilitar que en el momento de la recolección de los datos de facturación de la nube, los recursos obtenidos que no vengan por defecto con el *TAG* del proveedor de la nube, sean normalizados con los *TAGs* que estén asociados a este recurso.

   * Si ya existe un *TAG* con la misma clave en el otro lado, el *TAG* no será sobrescrito.
  
   * Todos los *Hyper Identifiers* que pertenecen al mismo [*productName*].

En el momento de exportar el informe de facturación los "TAGs Virtuales" vuelven normalizados, según los recursos utilizados en los *TAGs*.

.. figure:: /figuras/fig_release_note_maio_spa/ucloud_menu_configuração_tag_virtual_spa005.png
   :align: center

----

La figura de arriba presenta la aplicación de **TAGs Virtuales**, mediante Accountant *virtual-tag-applier*, y su normalización, utilizando Accountant *virtual-tag-normalizer*.

Oracle Cloud Infrastructure (OCI)
=================================

Ante la necesidad de las organizaciones de mantener un rendimiento consistente, ellas tienden a adoptar la estrategia de utilizar múltiples proveedores de nubes públicas. Para satisfacer esta demanda, Ustore lanza la nueva implementación "Oracle Cloud Infrastructure (OCI)", que integra la nube pública Oracle OCI al portal uCloud.

Este nuevo *release* de la Plataforma uCloud, ofrece solamente las funcionalidades de operación de infraestructura OCI, de acuerdo a la lista que se presenta a continuación.

A partir de este *release notes*, nuestro portal da soporte a la nube, proporciona los recursos y funcionalidades de **Operación de embitne** OCI que se enumeran a continuación:

.. figure:: /figuras/ucloud_oracleoci0002.png
   :align: center

----

Cabe señalar que la lista actual presentada anteriormente está directamente relacionada con la disponibilidad de las funcionalidades presentes en el actual kit de desarrollo de software (*SDK - Software Development Kit*) publicado por Oracle, utilizado por el equipo de DevOps de Ustore (mayo/2022) para la integración con *Oracle Cloud Infrastructure*.

El desarrollo continuo promovido por el equipo de DevOps de Ustore, como la ampliación de nuevas funcionalidades presentes en otras evoluciones del SDK Oracle, proporciona la evolución de los *releases* y/o versiones de la Plataforma uCloud, que serán relacionadas en futuros *Release Notes* de la Plataforma uCloud.

.. note:: En el momento presente en este *Release Notes* (mayo, 2022) la API y el SDK para OCI aún no permiten un soporte completo para la implementación del cobro y el cálculo de *billing* de la infraestructura presente en el ambiente OCI. Esperamos la evolución del SDK y API *Oracle Cloud Infrastructure* para implementar la funcionalidad de *billing* para OCI.

Este conjunto de nuevas funcionalidades implementadas y descritas, contenidas en este documento, generaron el desarrollo de esta nueva versión (*update tag 5.2-b35*).  Así, Ustore reafirma su compromiso constante con la evolución de la plataforma y el alineamiento a las necesidades del mercado y de sus clientes.
