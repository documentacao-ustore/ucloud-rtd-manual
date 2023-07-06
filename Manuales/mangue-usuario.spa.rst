Mangue.io - Manual de uso
+++++++++++++++++++++++++++++

.. image:: /figuras/mangue-logo-peq.png
    :alt: Logo Mangue
    :scale: 50 %
    :align: center
=====

Solucciones de tecnología de la información que permitem implementar una arquitectura computacional escalable, sólida y confiable en la nube distribuida. 

====

Presentación
============

Este documento tiene como objetivo explicar el uso de la plataforma “Mangue.io”, una plataforma de gestión de ambientes de múltiples orquestadores de *container*. En este manual se presentan los conceptos, las pantallas, las funcionalidades y los comandos de uso de este producto.

Apreciamos el *feedback* con su informe de experiencia de uso de nuestra aplicación, si tiene algo que sugerir, por favor enviar correo electrónico, la dirección se encuentra en la página anterior. 


====

Introducción
============

Mangue.io es una plataforma de gestión de ambientes de múltiples orquestadores de *containers*, que permite la orquestación, el despliegue (localización y programación) y la operacionalización (ejecución) de *containers* de aplicaciones dentro de uno o más *clusters* computacionales (públicos o privados) o entre ellos.

La plataforma opera en un modelo *multicloud* híbrido y, de esta forma, permite a las organizaciones un control total, soporte para la sustentación de copias de seguridad (*backup*), replicación y migración de ambientes. Centrado en un enfoque ágil, seguro y productivo de entrega continua de aplicaciones orientadas a la implementación, pruebas y actualizaciones con *downtime* cero y *rollback* de *deployments*.

La plataforma Mangue.io soporta la implantación y operacionalización de aplicaciones basadas en imágenes a partir de un servicio de registro. Además, también permite la creación de servicios para aplicaciones (internas o externas al *cluster* al que pertenece la aplicación).


====

Acceso a la plataforma
======================


El acceso a la plataforma se realiza a través de una página web, el usuario debe utilizar un navegador de Internet, tras introducir la dirección URL/enlace se visualizará la pantalla de presentación inicial.

Después de iniciar una sesión en el navegador elegido, la dirección/ruta de acceso a la aplicación debe rellenarse de la siguiente manera:

https://<mangueserver_IP_Address>:80
https://mangue_Server_Name.com/

Tras introducir la dirección correctamente, la pantalla de inicio de sesión del usuario es similar a la figura de abajo:

.. image:: /figuras/fig_mangue/001_mangue_login.png
    :alt: Tela de login 
    :scale: 80 %
    :align: center
=====

Las credenciales de inicio de sesión y contraseña son las mismas que las de la plataforma uCloud, con la que está integrada la plataforma Mangue.io. Todo usuario aprovisionado en uCloud puede utilizar automáticamente sus credenciales para acceder al Mangue.io.

Tras introducir sus credenciales de acceso (usuario y contraseña) y realizar el procedimiento de inicio de sesión, una imagen similar puede ser presentada al usuario, en caso de que exista un *cluster* asociado al contrato del usuario en el Mangue.io.

.. image:: /figuras/fig_mangue/002_mangue_tela_inicial.png
    :alt: Tela inicial
    :align: center
=====

La pantalla de arriba, representa un ejemplo de la pantalla de inicio que el usuario visualiza después de ingresar las credenciales válidas para el acceso a la plataforma Mangue.io.

====

Configuraciones de navegación
=============================

En la esquina superior derecha de la plataforma hay un menú de configuración que se identifica por un engranaje |icone_engrenagem|, donde el usuario tiene la opción de seleccionar a qué contrato, *cluster* y/o *namespace* (áreas de trabajo) quiere tener acceso.

Al hacer clic en cualquiera de los campos, la información de la pantalla cambia automáticamente.

.. image:: /figuras/fig_mangue/003_mangue_aba_selecao.png
    :alt: Aba de Seleção da Configuração 
    :scale: 80 %
    :align: center
=====

Al seleccionar un contrato, las opciones para selección de *clusters* son actualizadas, listando sólo aquellos que están asociados al contrato seleccionado, así como el permiso que el usuario conectado tiene en estos *clusters* - corresponde al nivel de permiso que tiene en el contrato del uCloud. 

Los contratos que aparecen en esta parte son sólo los que ya tienen algún *cluster* integrado a Mangue.io, a continuación de este documento la descripción de cómo integrar y/o crear un *cluster* en la aplicación. En el momento de la selección, se cambia el *cluster* a través del cual se comunica la plataforma y se actualiza las informaciones de la pantalla para este nuevo contexto.

En el momento en que el usuario selecciona el *cluster* y el *namespace*, los valores de la pantalla de *Overview* se cambian con los datos específicos de la selección del usuario.

====

Pantalla de início
==================

La pantalla de inicio de *Overview* presenta algunos gráficos referentes a los valores de consumo de recursos computacionales específicos de la selección del usuario, el detalle de los gráficos sigue abajo:

====

Gráfico del precio mensual del *cluster*
----------------------------------------

Este gráfico de barras, presenta la evolución del costo referente al uso de la infraestructura computacional que soporta y ejecuta las aplicaciones.

En el eje vertical se puede observar el valor y en el eje horizontal se muestra el valor referido al consumo diario de la infraestructura. Es posible seleccionar el intervalo de tiempo para ver el consumo de la infraestructura, pudiendo visualizar los últimos 7 días, los últimos 30 días, el mes actual, el mes anterior, así como personalizar un intervalo de tiempo deseado.

Se puede observar que los valores fluctúan en función del consumo de recursos de la infraestructura computacional para soportar todas las aplicaciones (*deployments*) que están activas en el *cluster* seleccionado.

.. image:: /figuras/fig_mangue/004_mangue_preco_mensal_cluster.png
    :alt: Preço Mensal do Cluster 
    :scale: 80 %
    :align: center
=====

Este gráfico permite seguir la variación del **costo real de la infraestructura** necesaria para mantener y soportar la ejecución de un *cluster*, día a día. En el área: "Título del gráfico" es posible conocer el valor total acumulado, hasta el día presente.

Estos valores se almacenan en una base de datos interna de la plataforma Mangue.io, de forma que el usuario puede seguir la evolución del valor correspondiente al consumo de los recursos computacionales para soportar un *cluster* activo y funcional.

Si el usuario lo desea, esta base de datos ('Taquillero') se puede limpiar, eliminando toda la información almacenada, de forma a "poner a cero" todos los valores acumulados. 

Para este propósito, el usuario debe hacer clic en el icono "Papelera" |icone_lixo|. La plataforma Mangue.io solicita la confirmación del usuario para esta acción presentando la pantalla abajo:

.. image:: /figuras/fig_mangue/005_mangue_deletar_bilhetador.png
    :alt: Deletar Dados Financeiros do Cluster_Bilhetador
    :align: center
=====


Para que el usuario confirme la acción de eliminar todos los datos financieros (valores) de consumo referidos al *cluster* seleccionado en la pestaña "Configuración de Navegación", basta hacer clic en el botón de color verde ``Eliminar``. 

Con esta acción se eliminan todos los valores de consumo del *cluster* y se inicia un nuevo periodo de recogida de informaciones, perdiendo toda la información acumulada (la serie histórica) del *cluster* seleccionado.

====

Cálculo del valor de consumo del *cluster*
------------------------------------------

Los valores aquí mostrados se calculan en base al valor/hora de vCPU y Memoria RAM que está almacenado en la base de datos de Mangue.io.

La plataforma Mangue.io almacena el consumo de recursos (CPU y Memoria) de las aplicaciones a cada minuto; al término de una hora (60 min), almacena el valor total del consumo en estos 60 minutos. Al final de cada día (24 horas) la plataforma Mangue.io almacena el valor referente al consumo de recursos computacionales, para mantener todas las aplicaciones activas en cada *container*.

El precio de CPU y Memoria utilizado es el mismo precio de los recursos del contrato, el valor se establece a través de uCloud, el precio del contrato se puede ver en el mangue a través de la pantalla **Permisos / Contrato**:

.. image:: /figuras/fig_mangue/005.1_mangue_formula.png
    :alt: Fórmula mangue.io
    :scale: 80 %
    :align: center
=====

Al final de cada ciclo de 24 horas, el valor total de consumo de los recursos computacionales se almacena en la base de datos de la plataforma Mangue.io y presentada anteriormente en el gráfico: Precio Mensual del *Cluster*.

====

Gráfico de uso total de la CPU
------------------------------

En esta pantalla, también es posible ver el uso de la CPU, en MiliCores, de cada recurso de kubernetes, para eso, el usuario tiene que especificar el *namespace* y los recursos de los que desea visualizar el consumo de CPU, y hacer clic en el icono lupa |icone_lupa_vermelha|, para realizar la búsqueda, retornando los últimos treinta minutos de consumo de CPU y Memoria.

.. image:: /figuras/fig_mangue/006_mangue_uso_total_cpu.png
    :alt: Uso Total de CPU
    :align: center
=====

Gráfico de uso total de Memoria
-------------------------------

Al realizar la búsqueda del ítem *Gráfico de Uso Total de CPU*, la plataforma recupera las informaciones del valor del consumo de memoria, en MegaBytes, de los últimos treinta minutos de consumo de memoria correspondiente al *namespace* y recurso seleccionado.

.. image:: /figuras/fig_mangue/007_mangue_uso_total_memoria.png
    :alt: Uso Total de Memória
    :align: center
=====

Menú del usuario
================

La barra de Menú del usuario se encuentra a la izquierda de la pantalla y se muestra inicialmente en modo expandido, como en la figura a continuación.

.. image:: /figuras/fig_mangue/008_mangue_menu_usuario_expandido.png
    :alt: Menu Usuário (Modo Expandido) 
    :align: center
=====

Algunas opciones de menú tienen un submenú, que se presentan cuando el usuario sitúa el ratón sobre la indicación (el signo: más pequeño que "<"). Al hacer clic en este icono |icone_sinal_menor|, la interfaz presenta al usuario el submenú de esta opción, detallado en la secuencia.

=====

Workloads
=========

En esta opción del Menú de Usuario *Workloads* su *dashboard* presenta las informaciones sobre *Deployments*, *Daemonsets*, *Horizontal Autoscaler*, *StatefulSets* y los *Updates*.

.. image:: /figuras/fig_mangue/009_mangue_submenu_workload.png
    :alt: Exemplo de submenu  
    :scale: 80 %
    :align: center
=====

Un **Deployment** es un objeto del Kubernetes, orquestador utilizado por el Mangue.io, que no es más que un controlador de implantación que proporciona actualizaciones declarativas para otros dos objetos Kubernetes: *Pods* y *ReplicaSets*.

Los **Pods** son las unidades lógicas más pequeñas (computacionales) implantables que se pueden crear y administrar desde Mangue.io. *ReplicaSet* tiene por objetivo mantener un conjunto estable de réplicas de *Pods* en ejecución en cualquier momento.

El **StatefulSet** es el objeto de la API de carga de trabajo que se utiliza para gestionar las aplicaciones en el estado. Es el responsable de gestionar la implantación y el dimensionamiento de un conjunto de *Pods* y proporciona garantías sobre su orden y exclusividad.

Los **Daemonsets** gestionan grupos de *pods* replicados. Sin embargo, *DaemonSets* intenta adherirse a un modelo de un *pod* por nodo, ya sea en todo el *cluster* o en un subconjunto de nodos. A medida que se añaden "nodos" a un *cluster*, los *DaemonSets* añaden automáticamente *pods* a los nuevos nodos según sea necesario.

El **Auto Escalador Horizontal** escala automáticamente el número de *pods* en un controlador de replicación, un conjunto de réplicas o un conjunto con estado, basándose en la utilización observada de la CPU (o con soporte para métricas personalizadas, en algunas otras métricas proporcionadas por la aplicación). Tenga en cuenta que el escalamiento automático horizontal del *pod* no se aplica a los objetos que no pueden ser escalados, por ejemplo, *DaemonSets*.

====

Deployments
-----------

El menú *Workload/Deployments* muestra todos los *deployments* de un cluster en un determinado *namespace*.

Un **Deployment** es un objeto del Kubernetes, orquestador utilizado por el Mangue.io, que no es más que un controlador de implantación que proporciona actualizaciones declarativas para otros dos objetos Kubernetes: *Pods* y *ReplicaSets*.

.. image:: /figuras/fig_mangue/014_mangue_workloads_deployments.png
    :alt: Workloads_Deployments
    :align: center
=====

En la tabla tenemos las siguientes columnas con sus respectivas informaciones: 

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

   Cuando el usuario selecciona una fila o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, estos representan acciones al usuario para ser ejecutadas de una sola vez en todas las filas seleccionadas. 

   En este caso se presentan tres iconos con acciones muy distintas:

      * **Reversión** |icone_reversao|:** Esta opción permite al usuario realizar la acción de revertir la versión actual de el (los) *deployment(s)* seleccionado(s) para su versión inmediatamente anterior a la existente en la plataforma de Mangue.io. 

      * **Escalar** |icone_escalar|: La función de esta acción permite al usuario informar el número (entero) deseado para incrementar el número de réplicas de la aplicación (*deployment*). 

      * **Papelera** |icone_lixo_vermelho|: Acción que permite al usuario eliminar todos los elementos seleccionados con una sola orden. 

      * **Cambiar versión** |icone_alterar_versao|: Esta opción permite actualizar múltiples *deployments* a la vez, al que el usuario puede informar la próxima versión de cada uno de ellos. 

* **Deploys:** Es la representación del nombre del *deployment.d*
* **Labels:** Son los identificadores de los *deployments*, utilizados para ser el enlace a un servicio. 
* **Instancias:**  Muestra la cantidad de réplicas que están operativas de un *Deployment*, y la cantidad total de réplicas operativas deseadas para este *Deployment*. Están divididas por una barra ("/") donde los valores encontrados antes de la barra son las réplicas operacionales, y los valores después de la barra representan la cantidad esperada de réplicas operacionales.
* **Status:** El *status* de un *deployment* identifica su estado actual. Pueden ser presentados como *Running*, *Pending* o *“!”* (signo de exclamación).

      * El *status* **Running** identifica que ningún error está sucediendo con el *Deployment*.

      * El *status* **Pending** identifica algún estado de transición en el *Deployment*. Ya sea por actualización, inicio del proceso del *container* o cualquier actividad que identifique un estado de transición.

      * El *status* **“!”** (signo de exclamación) identifica una alarma, en otras palabras, que un error sucedió con el *Deployment* y sus réplicas. Por ejemplo: la imagen de un *container* se pasa con una versión inexistente, por lo tanto, el *download* de este container no se produce;

* **IP de acceso:** Si el *Deployment* tiene un servicio asociado, es en este campo donde la IP del equilibrador de carga puede ser un servicio de tipo *Load Balancer*; puerto para acceso al servicio si es un servicio externo (tipo *nodePort*) o la *string* “IP interna” si se trata de un servicio interno del *cluster* (tipo *ClusterIP*);
* **Imagen y Versión:** En caso de que tenga más de una imagen o versión de un *container* se enumeran uno debajo del otro, como en el ejemplo del 6º *Deployment* listado en la imagen de la tabla *Deployment.*
* **Acciones:** La última columna presenta un *Dropdown* para el menú de acciones que se pueden realizar en los *deployments:* 

.. image:: /figuras/fig_mangue/015_mangue_dropdown_menu_acoes.png
    :alt: Dropdown Menu_Ações
    :align: center
=====

A. Añadir Persistent Volume Claim
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Las aplicaciones que se ejecutan en *containers* almacenan sus datos en memoria, y los *containers* y *pods* que se ejecutan por Kubernetes pueden morir, lo que impacta en la pérdida de los datos almacenados en memoria. 

En caso de que un usuario tenga informaciones sensibles que persistir, tales como volúmenes de base de datos, se debe crear un *Persistent Volume Claim*.

.. image:: /figuras/fig_mangue/016_mangue_add_pvc.png
    :alt: Adicionar_PersistentVolumeClaim
    :align: center
====

En esta pantalla el usuario debe rellenar los campos con las siguientes informaciones: 

* **Nombre:** Introducir el nombre del volumen que se desea crear.
* **Tamaño:** El usuario debe llenar un número entero que representa el tamaño del archivo de volumen que se desea crear.
* **Unidad de Tamaño:** El usuario debe seleccionar la unidad de tamaño que es utilizada para crear el volumen. Las opciones son:

      * **Kilo:** Kilobytes cuando el usuario desea crear un archivo con el valor anterior multiplicado por 1.000;

      * **Mega:** Megabytes cuando el usuario desea crear un archivo con el valor anterior multiplicado por 1.000.000;

      * **Giga:** Gigabytes cuando el usuario desea crear un archivo con el valor anterior multiplicado por 1.000.000.000;

      * **Tera:** Terabytes cuando el usuario desea crear un archivo con el valor anterior multiplicado por 1.000.000.000.000;

      * **Peta:** Petabytes cuando el usuario desea crear un archivo con el valor anterior multiplicado por 1.000.000.000.000.000;

.. attention:: La plataforma Mangue.io no valida, previamente, si hay espacio en disco disponible, en el tamaño informado. Al usuario no es presentado ningún aviso si el ambiente computacional no tiene el espacio necesario, ni se presenta ningún mensaje de error al momento de crear este volumen persistente con las características informadas.


.. note:: El usuario puede verificar una indicación de error en la columna **Status** en la pantalla del menú *Workloads/Deployments* y consultar el *deployment* específico, al que se ha asociado el *PersistentVolume*, ver la **Figura 14 Workloads – Deployments**, según la imagen anterior mostrada en el tópico **Deployments**.

** **Storage Class:** El usuario debe seleccionar cuál es el volumen de *NFS Storage* disponibles en la lista presentada. 
* **Modo de acceso:** Esta columna presenta la configuración de acceso a este volumen, estos modos de acceso pueden ser tres:

      * **ReadWriteOnce:** El volumen es montado y puede recibir instrucciones de lectura y escritura sólo desde un único *node*;

      * **ReadOnlyMany:** El volumen es montado y tiene permiso de sólo lectura, pero desde diferentes *nodes* simultáneamente, no se permite la escritura;

      * **ReadWriteMany:** El volumen es montado y puede recibir instrucciones de lectura y escritura simultáneamente, pero desde diferentes *nodes;*

* **Container:** Cuando el usuario haga clic en esta ubicación, se presenta el nombre del *container* de la aplicación con un símbolo similar a éste |uCloud_icone_coluna_acionavel|.
* **Mounth Path:** Es la ruta donde se monta el volumen en el *container*. Si la base del ambiente de aplicación es un ambiente Linux la ruta de montaje del volumen, debe utilizar la notación del sistema operativo correspondiente al ambiente; si la base del ambiente de aplicación es un ambiente MS-Windows, debe utilizar la notación de montaje del volumen con las carpetas del sistema operativo correspondiente.

Para confirmar todos los valores y opciones informados, basta con que el usuario haga clic en el botón ``Finalizar`` para crear el *Persistent Volume* y esperar el *feedback* de creación, en la esquina superior derecha de la pantalla de la plataforma Mangue.io.

=====

B. Añadir Servicio
~~~~~~~~~~~~~~~~~~

La segunda opción de este submenú permite que el usuario pueda añadir un servicio, al hacer clic se abre la siguiente pantalla de interfaz modal:

.. image:: /figuras/fig_mangue/017_mangue_add_servico.png
    :alt: Adicionar Serviço_Deployment
    :align: center
=====

En este modal, el usuario debe rellenar los siguientes campos:

* **Nombre del Servicio:** El usuario debe rellenar con el nombre del servicio que desea crear;
* **Labels de Deployment:** El usuario debe informar las que son asociadas a este servicio;
* **Tipos de acceso al servicio:**  Interno, Externo o *LoadBalancer*:

      * **Interno:** Son los servicios que sólo pueden ser accedidos desde el interior del *cluster*;

      * **Externo:** Corresponde a los servicios que permiten el acceso desde fuera del *cluster*. Se proporciona un puerto TCP-IP entre 30.000 -- 32.767;

      * **LoadBalancer:** Se integran directamente con los *Cloud Providers (AWS, AZURE, GOOGLE)* creando un *loadbalancer* LAYER 7 para la app correspondiente.

* **Puerto de entrada:** Introduzca el número de puerto TCP-IP del *container* asignado para la entrada al servicio.
* **Puerto de destino para el servicio:** Informar el puerto TCP-IP de entrada en el *container*, el servicio recibirá la solicitud en el puerto de entrada y la pasará al puerto de destino.
* **Seleccionar el protocolo**: TCP o UDP;
* **Botón** ``Añadir``:   Si el servicio necesita exponer más de un puerto, el usuario debe volver al Puerto de Entrada/Puerto de Destino, y añadir tantos puertos de entrada/salida como sean necesarios.

Para confirmar todas las opciones arriba indicadas, el usuario debe hacer clic con el ratón en el botón **Crear Servicio** y esperar el *feedback* de creación.

====

C. Eliminar Deployment
~~~~~~~~~~~~~~~~~~~~~~

La tercera opción de este submenú permite al usuario eliminar definitivamente un *Deployment* del *cluster* y del *namespace* que fue seleccionado en la pestaña **Configuraciones**; al hacer clic, se abre la siguiente pantalla de interfaz modal solicitando confirmación por parte del usuario:

.. image:: /figuras/fig_mangue/018_mangue_deletar_deployment.png
    :alt: Deletar Deployment 
    :scale: 80 %
    :align: center
=====


Esta acción es inmediata e irreversible, la plataforma Mangue.io elimina el *deployment* seleccionado por el usuario del *contrato/cluster/namespace.*

Basta con que el usuario haga clic en el botón ``Eliminar`` para confirmar su acción y la plataforma Mangue.io elimina el *deployment* del ambiente seleccionado.

.. note:: Esta acción **no** elimina cualquier componente adicional externo a este *deployment* - por ejemplo, un *PersistentVolume* asociado, por lo que si un archivo externo existe, sigue existiendo en el volumen de destino. Esta acción sólo elimina el *deployment* del ambiente, pero no elimina ningún archivo adicional del ambiente computacional.

====

D. Editar Deployment
~~~~~~~~~~~~~~~~~~~~~

Algunas informaciones no pueden ser editadas a través de los formularios de Mangue.io. Elementos como: 

* Puerto del *container*;
* Añadir una variable de ambiente;
* Eliminar una variable de ambiente.

En el cumplimiento de todas las demandas de edición para un Deployment, se puede editar directamente el YAML del Deployment en la plataforma Mangue.io.

Esta opción presenta como ejemplo la imagen: Editar *Deployment*. Su contenido representa el archivo.JSON con todas las configuraciones del *deployment* en Kubernetes, el usuario puede editar lo que sea necesario, confirmar presionando el botón  ``Editar`` y esperar el *feedback* de la acción por la plataforma Mangue.io.

Esta funcionalidad está dirigida a los usuarios que conocen el formato de los archivos de Kubernetes.

.. image:: /figuras/fig_mangue/019_mangue_editar_deployment.png
    :alt: Editar Deployment
    :align: center
=====

E. Cambiar *Tags*
~~~~~~~~~~~~~~~~~

La función de esta pantalla permite al usuario cambiar los *Tags* asociados a la aplicación seleccionada. A partir de esta pantalla se puede crear un *Tag* pulsando sobre el icono |icone_adicionar| para asociarlo a la aplicación.

.. image:: /figuras/fig_mangue/019.1_mangue_alterar_tag.png
    :alt: Alterar Tags
    :align: center
=====

.. important:: Para crear un *Tag* hay que especificar su clave y valor.

.. image:: /figuras/fig_mangue/019.2_mangue_criar_tag.png
    :alt: Criar Tag
    :align: center
=====

F. Escalar Deployment
~~~~~~~~~~~~~~~~~~~~~

La función de esta pantalla permite al usuario informar el número (entero) deseado para incrementar el número de réplicas de la aplicación (*deployment*), las cuales son iniciadas automáticamente después de la confirmación con el clic del ratón sobre el botón ``Escalar``.

.. image:: /figuras/fig_mangue/020_mangue_escalar_deployment.png
    :alt: Escalar Deployment
    :align: center
=====

Cabe destacar que se produce un aumento del consumo en el uso de la CPU y la memoria del *Cluster* para soportar la ejecución simultánea de las réplicas de esta aplicación en la infraestructura del *Cluster*.

====

G. Migrar Deployment
~~~~~~~~~~~~~~~~~~~~

En la sexta opción del menú de acciones de *Deployment*, tenemos la opción de migrar *deployment* entre diferentes *clusters* configurados en la plataforma Mangue.io.

El usuario debe seleccionar a qué *cluster* integrado en Mangue.io desea migrar el *deployment* elegido.

El campo de *cluster* destinatario es un campo de tipo *"dropdown list"*, cuando el usuario haga clic en éste, se presenta la lista de los *clusters* disponibles asociados al contrato elegido en el menú de configuración.

Para realizar la migración, el usuario sólo tiene que hacer clic en el botón ``Migrar`` y esperar el *feedback* de la acción por parte de la plataforma Mangue.io. Como resultado de esta acción, se presenta una alerta de éxito en el menú superior derecho de la pantalla.

.. image:: /figuras/fig_mangue/021_mangue_migrar_deployment.png
    :alt: Migrar Deployment
    :align: center
=====

H. Cambiar Versión
~~~~~~~~~~~~~~~~~~

Después de hacer clic en “Actualizar Versión de la Aplicación” la plataforma presenta la imagen “Actualizar Versión de *Deployment*”. A través de este control, el usuario puede generar una “nueva versión” para cualquier *deployment* existente en la plataforma Mangue.io. 

.. image:: /figuras/fig_mangue/022_mangue_atualizar_deployment.png
    :alt: Atualizar versão de Deployment
    :align: center
=====

Este campo es alfanumérico y el usuario puede ingresar con la información deseada para identificar la nueva versión del *deployment* seleccionado. Las nuevas versiones son de control exclusivo del usuario, ya que se refieren a las ofertas creadas por este usuario.

Tras rellenar con la información deseada, el usuario debe pulsar el botón ``Enviar`` para confirmar la acción de crear la versión para el *deployment*.

.. attention:: Estas nuevas versiones no están necesariamente relacionadas con cualquier versión del software que las compone, o cualquier software que se utilizó para componer la oferta, diferentes versiones se pueden encontrar fuera de la plataforma Mangue.io.

====

J. Rollback
~~~~~~~~~~~

Esta opción permite al usuario realizar la acción de revertir la versión de *deployment* a su versión inmediatamente anterior a la existente en la plataforma Mangue.io.

Esta acción en particular no activa ninguna pantalla adicional de confirmación, su acción es inmediata.


.. important:: Al seleccionar esta opción, la plataforma Mangue.io realiza la acción de reversión de la versión de forma inmediata, sin solicitar ningún tipo de confirmación por parte del usuario. 

.. nota:: Es recomendable tener precaución y prestar atención, ya que esta acción crea algún tipo de bajo rendimiento al *deployment* en el que se está realizando la acción de *rollback*.

====

Informaciones de Deployment
---------------------------

Si el usuario hace clic en el nombre de un *deployment*, la plataforma de Mangue.io muestra la pantalla de detalles del *deployment*, como se puede observar en la siguiente imagen.

El usuario puede observar que esta pantalla tiene varias secciones, cada una de las cuales se describe a continuación respectivamente.

.. image:: /figuras/fig_mangue/023_mangue_overview_deployment.png
    :alt: Overview do Deployment
    :align: center
=====

A. Sección: Deployment Overview
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta sección muestra tres gráficos, dos de rendimiento y uno de valor:

* CPU;
* Memoria;
* Precio en los últimos 30 días.

En ellos se muestra el rendimiento de la CPU (en milicores), la Memoria (en megabytes) y el Precio en los últimos 30 días, todo referido al *deployment* seleccionado por el usuario. La línea roja en el gráfico de precios indica la tendencia del gráfico.

También es posible visualizar botones de interacción para el usuario, con los que se puede especificar el periodo de los gráficos de CPU y Memoria.

.. image:: /figuras/fig_mangue/024_mangue_consumo_deployment.png
    :alt: Overview do consumo do deployment
    :align: center
=====

B. Sección: Replicaset
~~~~~~~~~~~~~~~~~~~~~~

La sección **ReplicaSet** muestra una tabla que lista todos los *replicasets* presentes para un *deployment*, en esta lista se muestran informaciones como:

* Nombre;
* Número de *pods* disponibles;
* Cantidad de *pods* totales en un momento determinado;
* Imagen junto con su versión especificada;
* Tiempo (en días) desde el momento de creación de este *replicaset*;
* Un botón con la opción de borrarlo, como se muestra en la siguiente figura.

.. image:: /figuras/fig_mangue/025_mangue_replicaset.png
    :alt: ReplicaSet
    :align: center
=====

En esta parte, la plataforma la plataforma Mangue.io presenta las siguientes informaciones: 

* **#**: Número secuencial de *replicaset* en esta lista.
* **Nombre:** Esta columna muestra el nombre del *replicaset*, el usuario puede comprobar que el ambiente de Kubernetes, genera nombres únicos para cada *replicaset.*
* **Pods Disponibles:** Esta columna muestra la cantidad de *pods* para este *replicaset*.
* **Pods Totales:** Esta columna muestra la cantidad total de *pods*, configurados para este *replicaset*.
* **Imagen:** Esta columna muestra la información del archivo de imagen utilizada para crear este *deployment*.
* **Duración:** Esta columna muestra el total de días que este *replicaset* existe desde el momento de su creación hasta el presente día en que el usuario visualiza esta lista.

====

C. Sección: PODs
~~~~~~~~~~~~~~~~

En la sección **Pods** hay una tabla con la lista de todos los *pods* presentes para el *deployment*, cada uno detalla su información como:

* Nombre;
* “Nodo” en el que se está siendo ejecutado; 
* *Status* actual de *pod*, 
* Imagen junto con su versión y tiempo de vida.

.. image:: /figuras/fig_mangue/026_mangue_pods.png
    :alt: PODs
    :align: center
=====

En esta sección, la plataforma de Mangue.io presenta las siguientes informaciones:

* **Nombre:** Nombre del *deployment* que se establece en el momento de la creación.
* **Nodo:** Muestra el nombre del node Kubernetes que ejecuta este *deployment.*
* **Status:** Presenta el *status* del *deployment* en su respectivo *node*. El *status* de un *deployment* identifica el estado actual. Pueden ser representados por:

      * **Running** identifica que ningún error está sucediendo con el *deployment*;

      * **Pending** identifica algún estado de transición en el *deployment.* Ya sea por actualización, inicio del proceso del *container* o cualquier actividad que identifique un estado de transición.

      * **“!”** (signo de exclamación) identifica una alarma, es decir, que algo malo ha ocurrido con el *deployment* y sus réplicas. Por ejemplo: la imagen de un container es pasada con una versión inexistente de modo que el *download* no ocurre.

* **Imagem:** Esta columna presenta la información de la imagen pública que fue utilizada para la creación de este *deployment.* Esta imagen se puede encontrar en sitios públicos que contienen información técnica relacionada con la aplicación en sí, un ejemplo es el *Docker Hub* (https://hub.docker.com/). 
* **Duración:** Muestra el tiempo (en días) transcurrido desde la creación de este *deployment*.
* **Acciones:** Esta columna presenta el botón ``Acciones`` |icone_acao| al ser pulsado, muestra las acciones que pueden ser realizadas sobre cada *pod* listado, como muestra la siguiente figura: 
 
.. image:: /figuras/fig_mangue/027_mangue_submenu_pods.png
    :alt: submenu PODs 
    :scale: 80 %
    :align: center
=====

Cada una de las opciones de este submenú se detalla y se describe a continuación:

      * **Eliminar Pod:** Al hacer clic en la opción de eliminar, sólo hay que esperar el *feedback* de la acción. Eso genera una alerta de “Éxito” o “Error” en el menú superior derecho. Como primera opción existe la deleción del *pod* en cuestión, al seleccionar esta opción aparece el siguiente modal:

.. image:: /figuras/fig_mangue/028_mangue_deletar_pod.png
    :alt: submenu Ações_Deletar_POD
    :align: center
=====

      * **Gráfico de Performance:** La segunda opción posibilita al usuario observar los gráficos de performance de CPU y Memoria para cada *pod*, una vez que se hace click en esta opción, se presenta al usuario la pantalla de abajo con los gráficos de consumo de CPU y memoria del *pod* seleccionado.

.. image:: /figuras/fig_mangue/029_mangue_performance_pod.png
    :alt: submenu Performance de um POD
    :align: center
=====

      * **Log:**  Esta tercera opción permite al usuario ver los *logs* de un determinado *pod* de forma similar a lo que se consigue con una sesión de emulación de consola de terminal SSH. 

        El usuario puede filtrar el número de registros (filas) que desea observar (las opciones son: 10, 20, 50, 100, 300, 500, 1000, todos). 

        Si el *Pod* tiene más de un *container* en ejecución, hay un *dropdown* donde se puede seleccionar qué *container* el usuario quiere ver los *logs*, como se muestra en la siguiente imagen:

.. image:: /figuras/fig_mangue/030_mangue_log_pods.png
    :alt: submenu Ações_LOG diversos PODs
    :align: center
=====

      * **Línea de Comando**: La cuarta opción ofrece al usuario ejecutar las líneas de comando en el *prompt* del sistema operativo del *pod*, de una forma similar a la que se obtiene con una sesión de emulación de consola de terminal SSH. Esta funcionalidad se extiende a uno o más *containers* que existan dentro del *pod* en cuestión. 

.. note:: Para habilitar esta función es necesario acceder al menú Integraciones y seguir los pasos correspondientes al *Container Execution*.

En caso de que el *Pod* tenga más de un *container* en ejecución hay un *dropdown* donde es posible seleccionar qué *container* el usuario desea ejecutar los comandos, como se muestra en la siguiente imagen:

.. image:: /figuras/fig_mangue/031_mangue_comando_pod.png
    :alt: submenu Ações_Linha de Comando Outro POD
    :align: center
=====

D. Sección: Volúmenes y Secretos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta sección enumera todos los **Volúmenes** (archivos que almacenan datos) o **Secretos** (archivos, o configuraciones de autenticación cuando se requieren), asociados con el *deployment* seleccionado.

.. image:: /figuras/fig_mangue/032_mangue_volumes_segredos.png
    :alt: Volumes e Segredos
    :align: center
=====

La plataforma Mangue.io presenta las siguientes informaciones en esta sección:

* **#:** Esta columna muestra el número secuencial del volumen o secreto que se presenta en esta lista.
* **Nombre:** Esta columna presenta el nombre del volumen o secreto (archivo del sistema operativo) que se muestra en esta lista.
* **Tipo:** Esta columna presenta el tipo de item que se muestra en esta lista, que puede ser un **volumen** o un **secreto**.

====

E. Sección: Eventos
~~~~~~~~~~~~~~~~~~~

En esta sección se enumeran todos los eventos vinculados a un *deployment*. Estos eventos pueden ser: por cambio en la cantidad de *Pods*/Réplicas, cambio en la versión de los *containers* del *deployment* o cualquier otro cambio en su estado.

.. image:: /figuras/fig_mangue/033_mangue_eventos.png
    :alt: Eventos de Deployment
    :align: center
=====

La plataforma  Mangue.io presenta la siguiente información en esta sección:

* **#:** Número secuencial del evento en la lista presentada.
* * ***Tipo:** Describe el tipo de evento ocurrido, y se pueden enumerar los siguientes tipos de eventos:

      * **Normal**;

      * **Warning**;

* **Objeto:** Describe qué objeto configurado en la plataforma Mangue.io fue el origen del evento listado. La identificación del tipo de objeto, permite al usuario identificar este origen para poder acceder a él y actuar en la resolución del evento, redefiniéndolo, u optando por su eliminación. Sus tipos pueden ser algunos de los enumerados a continuación:

      * *Deployments*,

      * *Daemonsets*,

      * *Horizontal Autoscaler*,

      * *Pods*;

      * *Statefulsets*;

      * *Updates*;

      * *Servicios*;

      * *Ingress*;

      * *Storage Class*;

      * *PersistentVolumes*;

      * *PersistentVolumesClaim*.

**Mensaje:** En esta columna la plataforma del Mangue.io presenta una lista de mensajes que pueden ayudar a identificar el éxito del evento o la causa raíz de un potencial problema, de esta manera permite al usuario tomar alguna acción para eliminar la causa raíz del problema o estar seguro del éxito de este evento.

      * *Pulled*;

      * *Created*;

      * *Started*;

      * *NoPods*;

      * *FailedGetScale*;

      * *ProvisioningFailed*;

      * *FailedBinding*.

====

F. Sección: Autoescalador Horizontal de Pods
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

La plataforma Mangue.io permite al usuario definir las reglas para que la performance del *deployment* sea siempre la mejor posible, y la plataforma Mangue.io puede aumentar el procesamiento en paralelo del *deployment*, ejecutar diversas instancias (réplicas) para asegurar que los usuarios tengan siempre la mejor experiencia de uso posible.

Cabe destacar que es necesario que exista una instancia activa del *Kubernetes Metrics Server* operando en el *cluster* para que se produzca la ejecución del *Horizontal Pod Auto Scaler*. Por defecto, la instalación del Mangue.io contempla la instalación del servicio de métricas.

Si el *deployment* no tiene Auto Escalador Horizontal, la pantalla se muestra como el ejemplo siguiente:

.. image:: /figuras/fig_mangue/034_mangue_autoescalador_inexistente.png
    :alt: Nenhum auto escalador horizontal encontrado
    :align: center
=====

Para que el usuario pueda crear una regla de **Escalador**, basta hacer clic en el icono de suma |icone_adicionar| como en la imagen de arriba, para que se presente la interfaz donde el usuario configura la(s) regla(s) de cómo la plataforma debe medir el consumo de infraestructura del *deployment*, para iniciar nuevas réplicas dentro de la infraestructura computacional de modo que la performance sea atendida.

.. image:: /figuras/fig_mangue/035_mangue_criacao_autoescalador.png
    :alt: Auto Escalador Horizontal_Criação
    :align: center
=====

* **Mínimo de Réplicas:** Indicar el valor mínimo de réplicas del *deployment* (obligatorio un número entero - por ejemplo: 1, 2) que la plataforma Mangue.io debe mantener activas para que la aplicación tenga el rendimiento mínimo necesario para garantizar la optimización de la experiencia del usuario. El valor mínimo para este campo es “um' (1).

* **Máximo de Réplicas:** Informar el valor máximo de réplicas del *deployment* (obligatorio un número entero - por ejemplo: 1, 2) que la plataforma Mangue.io debe iniciar para que la aplicación soporte el crecimiento de la demanda de acceso de los usuarios, y garantizar la optimización de la experiencia del usuario. El valor máximo para este campo es “quince” (15).

* **% máximo de uso de la CPU:**  El usuario debe hacer clic en el botón verde con el signo '+', para que la plataforma muestre el campo donde el usuario informa el valor porcentual máximo (obligatorio un número entero - por ejemplo, 20, 22, 30) que será utilizado por la plataforma Mangue.io como límite máximo de asignación de **CPU** para ejecutar las réplicas de un *deployment*. Este número es el límite máximo que la plataforma considera para iniciar la creación y ejecución de una nueva réplica del *deployment*. El valor máximo de este campo es “cien por ciento” (100%).

* **% máximo de uso de memoria:** El usuario debe hacer clic en el botón verde con el signo '+' para que la plataforma presente el campo donde el usuario informa el valor porcentual máximo (obligatorio un número entero - por ejemplo, 20, 22, 30) a ser utilizado por la plataforma Mangue.io como límite máximo de asignación de recursos de **memoria** para ejecutar las réplicas de un *deployment*. Este número es el límite máximo que la plataforma considera para iniciar la creación y ejecución de una nueva réplica del *deployment*. El valor máximo de este campo es “cien por ciento” (100%).

Es importante destacar que al confirmar el evento de creación de un Auto Escalador Horizontal, hay un tiempo de espera para que éste aparezca en la pantalla. Este tiempo se debe a la necesidad de que el escalador recopile métricas para convertirse en un objeto activo en *Kubernetes*.

La definición de "Reglas de Escalabilidad" controla el aumento/disminución del número de réplicas de la aplicación, y en consecuencia hay un aumento/disminución del consumo de recursos computacionales para ejecutar el mayor/menor número de réplicas activas. Por lo tanto, hay un aumento/disminución del valor del coste de infraestructura durante el tiempo en que las varias réplicas son ejecutadas.

Después de la definición, o en el caso de una regla existente, el usuario ve la pantalla de abajo:

.. image:: /figuras/fig_mangue/036_mangue_autoescalador_existente.png
    :alt: Auto Escalador Horizontal - Existente
    :align: center
=====

* **#:** Número secuencial de Auto Escalador Horizontal en la lista presentada.
* **Nombre:** Identifica el nombre del Auto Escalador creado, y normalmente debe ser el mismo nombre del *deployment*;
* **Min. Réplicas:** Identifica el parámetro colocado en la definición del Auto Escalador y correspondiente al número mínimo de réplicas que este escalador mantiene activo para garantizar el rendimiento al *deployment*.
* **Máx. Réplicas:** Indica el parámetro colocado en la definición del escalador, corresponde al número máximo de réplicas que se mantienen activas para garantizar la performance del *deployment;*
* **Número de Réplicas:** Identifica la cantidad de réplicas activas del *deployment* en el momento actual.
* **Uso de CPU:** Presenta la regla definida al auto escalador para los límites máximo y mínimo de uso de la CPU. Esta norma debe ser interpretada de la siguiente manera:

      * El primer número es el consumo actual del recurso de CPU.

      * El segundo número es el límite máximo de ocupación de la CPU, límite en el que la plataforma Mangue.io **pone en marcha** (activa) una nueva réplica del *deployment*. 

* **Utilización de Memória:** Muestra la regla definida al auto escalador, para los límites mínimos y máximos de asignación de memoria. Esta norma debe ser interpretada de la siguiente manera:

      * El primer número es el consumo actual de asignación del recurso Memoria.

      * El segundo número es el límite máximo de asignación de memoria, el límite en el que la plataforma Mangue.io **pone en marcha** (activa) una nueva réplica del *deployment*.

* **Acciones:** Esta columna presenta el botón ``Acciones`` |icone_acao| al ser pulsado, presenta las acciones que se pueden realizar sobre el Auto Escalador Horizontal, hay dos opciones: 

      * Eliminar autoescalador horizontal de pods;

      * Editar autoescalador horizontal de pods.

.. image:: /figuras/fig_mangue/037_mangue_acoes_autoescalador.png
    :alt: submenu Ações_Auto escalador horizontal 
    :scale: 80 %
    :align: center
=====

Al hacer clic en la opción "Eliminar", el usuario confirma la eliminación de las reglas de escalabilidad creadas y éstas dejan de aplicarse para el *deployment*. 
	
.. attention:: Un *feedback* de alerta es creado en la esquina superior derecha de la pantalla, informando del éxito o error.

La opción "Eliminar" del menú de acciones del Horizontal *Autoscalers* presenta la siguiente pantalla:

.. image:: /figuras/fig_mangue/038_mangue_deletar_autoescalador.png
    :alt: submenu Ações_Deletar auto escalador horizontal
    :align: center
=====

Al hacer clic en la opción ``Editar``, la plataforma Mangue.io presenta la pantalla de abajo, donde es posible al usuario cambiar los valores existentes del Auto Escalador Horizontal. La siguiente imagen "Auto Escalator Horizontal - Creación" muestra opciones sobre cómo cambiar los valores.

.. image:: /figuras/fig_mangue/039_mangue_criar_autoescalador.png
    :alt: Regras de Auto Escalador Horizontal_Criação
    :align: center
=====

Es importante destacar que las reglas de Auto Escalador Horizontal descritas anteriormente sólo están asociadas al *deployment* seleccionado por el usuario.

A través del menú *Workloads*/Autoescalador Horizontal el usuario puede ver todas las reglas de Auto Escalador Horizontal, configuradas en la plataforma del Mangue.io, asociadas a sus respectivos *deployments*.

====

G. Precio de la Aplicación en el último mes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta sección muestra la pantalla "Precio de la aplicación en el último mes", donde se listan las columnas de moneda, precio por memoria, precio por CPU y precio total de la aplicación, a continuación se detalla cada una de las columnas:

.. image:: /figuras/fig_mangue/040_mangue_preço_deployment.png
    :alt: Preço da Aplicação (deployment)
    :align: center
=====

* **Moneda**: Presenta el nombre de la moneda que se refiere a los valores mostrados en las columnas de esta tabla.
* **Precio por memoria**: Presenta el valor total, para el mes en curso, del consumo del recurso de memoria RAM para mantener el *deployment* en funcionamiento (ver fórmula de cálculo);
* **Precio por CPU**: Presenta el valor total, para el mes actual, de consumo de recursos de CPU para mantener el *deployment* en funcionamiento (ver fórmula de cálculo);
* **Precio total del APP**: Esta columna muestra la suma de las dos columnas anteriores (Precio por memoria y Precio por CPU). Con esta información, el usuario puede evaluar el **costo real de la infraestructura** necesaria para mantener y soportar la ejecución de un *deployment* activo y funcional 24x7. 

=====

Daemonsets
----------

Esta sección presenta todos los *Daemonsets* de un *cluster* en un determinado *namespace*, en la siguiente tabla tenemos informaciones como:

.. image:: /figuras/fig_mangue/041_mangue_daemonsets.png
    :alt: Listagem de Daemonsets
    :align: center
=====

* **#**: Número secuencial del *Daemonset* en la lista presentada.
* **Nombre**: Es la representación del nombre del *Daemonsets*.
* **Labels**: Son los identificadores de los *Daemonsets*, utilizados para ser el enlace a un servicio;
* **Instancias**: Está representada por la cantidad de réplicas operacionales de un *Daemonsets*, y por la cantidad total de réplicas operacionales deseadas para este *Daemonsets*. Están divididos por una barra ("/") donde los valores encontrados antes de la barra son las réplicas operacionales, y los valores después de la barra representan la cantidad esperada de réplicas operacionales.
* **Status:** El *status* de un *Daemonsets* identifica su estado actual. Puede ser representados por *Running*, *Pending* o *"!"* (signo de exclamación):

      * El *status* *Running* identifica que ningún error está sucediendo con el *Daemonsets*.

      * El *status* *Pending* identifica algún estado de transición en el *Daemonsets*. Ya sea por actualización, inicio del proceso del *container* o cualquier actividad que identifique un estado de transición.

      * El status “!” (signo de exclamación) identifica una alarma, en otras palabras, que algo incorrecto ha sucedido con el *Daemonsets* y sus réplicas. Por ejemplo: la imagen de un *container* es pasada con una versión inexistente, de modo que el *download* no ocurre.

* **IP de acceso**: Si el *Daemonsets* tiene un servicio asociado, es en este campo donde la IP del balanceador de carga puede ser un servicio de tipo *loadbalancer*, puerto para acceder al servicio si es un servicio externo (tipo nodePort) o la *string* "IP interna" si es un servicio interno del *cluster* (tipo *clusterIP*).
* **Imagen y versión**: En caso de que tenga más de una imagen o versión de un *container* se enumeran uno debajo del otro, como en el ejemplo del 6º *Daemonsets* listado en la imagen de la tabla de *Daemonsets*.
* **Duración**: Presenta el tiempo de duración del *Daemonsets*.
* **Acciones**: Esta columna muestra el botón ``Acción`` |icone_acao| al ser pulsado, muestra las siguientes opciones:

  .. image:: /figuras/fig_mangue/041.1_mangue_acoes_daemonsets.png
    :alt: Editar e deletar Daemonsets 
    :scale: 80 %
    :align: center
=====

      * **Editar DaemonSets**: Esta opción presenta el *Daemonset* en formato JSON, el usuario puede editar lo necesario y seleccionar la opción de editar y esperar el *feedback* de la acción por parte de la plataforma Mangue.io.

      * **Eliminar DaemonSets**: Al seleccionar esta acción, la plataforma Mangue.io pide la confirmación del usuario, como se muestra en la siguiente figura:

.. image:: /figuras/fig_mangue/042_mangue_deletar_daemonsets.png
    :alt: Confirmação para deletar Daemonsets
    :align: center
=====

Informaciones del Daemonset
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Si el usuario hace clic en el nombre de algún *Daemonset* presente en la lista, la plataforma Mangue.io muestra la pantalla con las informaciones de un *Daemonset*, como se muestra en el ejemplo siguiente:

.. image:: /figuras/fig_mangue/042.1_mangue_overview_daemonsets.png
    :alt: Overview Daemonsets
    :align: center
=====

Autoescalador Horizontal de Pods
--------------------------------

La plataforma Mangue.io permite al usuario establecer reglas para que el desempeño de la aplicación sea siempre el mejor posible y que el *deployment* pueda aumentar el procesamiento paralelo, varias instancias del *deployment* (réplicas) para garantizar que los usuarios tengan siempre la mejor experiencia de uso posible.

La definición de "Reglas de Escabilidad" controla el aumento de la cantidad de réplicas de un *deployment*, y en consecuencia hay un aumento en el valor del costo de la infraestructura, durante el tiempo que se ejecutan las varias réplicas. En la tabla tenemos informaciones como: 

.. image:: /figuras/fig_mangue/043_mangue_lista_autoescalador.png
    :alt: Horizontal Autoscaler
    :align: center
=====

* **# Columna Accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso se mostra el icono de “Papelera” |icone_lixo_vermelho| que permite eliminar todos los elementos por indicados por el usuario con un solo comando.

* **Nombre**: Identifica el nombre del Autoescalador creado, y normalmente debe ser el mismo nombre del *Deployment*;
* **Min. Réplicas**: Identifica el parámetro colocado al crear el escalador correspondiente al número mínimo de réplicas que este escalador garantiza para el *Deployment* al que está asociado;
* **Máx. Réplicas**: Indica el parámetro colocado al crear el escalador, corresponde al número máximo de réplicas que se mantienen activas para garantizar que el *Deployment* está asociado; 
* **Número Actual de Réplicas**: Identifica el estado actual de la cantidad de réplicas de *Deployment* a las que está asociado el escalador.
* **Acciones**: Esta columna presenta el botón ``Acción``  |icone_acao| al ser pulsado, muestra las acciones que se pueden realizar sobre el Autoescalador Horizontal, hay dos opciones:

.. image:: /figuras/fig_mangue/044_mangue_acoes_autoescalador.png
    :alt: submenu Ações_Auto escalador horizontal 
    :scale: 80 %
    :align: center
=====

En el menú de "Acciones" del Autoescalador Horizontal existe la opción de eliminar, al seleccionarla se muestra el siguiente modal:

.. image:: /figuras/fig_mangue/045_mangue_deletar_autoescalador.png
    :alt: Deletar Auto Escalador Horizontal
    :align: center
=====

Al hacer clic en el botón ``Eliminar``, el Autoescalador Horizontal es eliminado, y las reglas de escabilidad creadas dejan de ser obedecidas por el *Deployment*;

.. attention:: Un *feedback* de alerta es creado en la esquina superior derecha de la pantalla informando del "éxito" o "error".

====

Pods
----

Un **Pod** del *Kubernetes* es un grupo de *containers*, implantados juntos, en el mismo *host*.

Los *pods* operan a un nivel más alto que los *containers* individuales, porque es muy común tener un grupo de *containers* trabajando juntos para producir un artefacto o procesar un conjunto de trabajo.

Por ejemplo:

Para ilustrar lo que es un *pod*, por analogía, se puede utilizar la frase *a pod of whales* que significa "un grupo de ballenas" en este caso específico, el término *pods* se refiere al grupo de ballenas.

.. note:: Un *Pod* es un grupo de uno o más *containers*, con almacenamiento/recursos de red compartidos y una especificación de cómo ejecutar los *containers*.

El contenido de un *pod* es siempre colocado y programado conjuntamente, y luego ejecutado en un contexto compartido.

.. important:: Un *pod* modela un "*host lógico*" específico de la aplicación. Contiene uno o varios *containers* de la aplicación que se encuentran acoplados de forma relativamente fuerte.

La plataforma Mangue.io puede ayudarle a crear tantos *pods* sean necesarios para su ambiente de Kubernetes, la asociación de *Deployment* a un *Pod* se describe en otra sección de este manual, junto con la descripción del proceso de creación de un *Pod*.

.. image:: /figuras/fig_mangue/046_mangue_listagem_pods.png
    :alt: Listagem de PODs
    :align: center
=====

La imagen de arriba muestra el listado de pods creados y, a continuación, la descripción con el significado de cada una de las siete columnas de esta pantalla:

* **# columna accionable**: Esta columna presenta una forma alternativa de borrar (eliminar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable  |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es presentado el icono “Papelera” |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando.

* **Nombre**: Nombre del *Deployment* que se establece en el momento de su creación;
* **Nodo:** Presenta el nombre del nodo Kubernetes que está ejecutando este *Deployment*;
* **Status**: Presenta el *status* del *Deployment* en su respectivo *node*. El *status* de un *Deployment* identifica el estado actual. Pueden ser representados por:

      * **Running** identifica que ningún error está sucediendo con el *Deployment*.

      * **Pending** identifica algún estado de transición en el *Deployment*. Ya sea por actualización, inicio del proceso del *container* o cualquier actividad que identifique un estado de transición.

      * **“!”** (signo de exclamación) identifica una alarma, es decir, que algo incorrecto ha ocurrido con el *Deployment* y sus réplicas. Por ejemplo: la imagen de un *container* es pasada con una versión inexistente, así el download de este *container* no ocurre;

* **Imagen:** Esta columna muestra la información de la imagen pública utilizada para la creación de este *Deployment*. Esta imagen se puede encontrar en sitios públicos que contienen informaciones técnicas relacionadas con la aplicación en sí, un ejemplo es el Docker Hub (https://hub.docker.com/).
* **Duración:** Muestra el tiempo (en días) transcurrido desde la creación de este Deployment.
* **Acciones:** Esta columna muestra el botón de ``Acciónes`` |icone_acao|, al ser pulsado, muestra las acciones que se pueden realizar sobre cada *Pod* listado, como muestra la figura abajo.

.. image:: /figuras/fig_mangue/027_mangue_submenu_pods.png
    :alt: submenu PODs 
    :scale: 80 %
    :align: center
=====

Cada una de las opciones de este submenú se describe a continuación:

      * **Eliminar Pod:** Al hacer clic en la opción **Eliminar** sólo hay que esperar el *feedback* de la acción. Se genera una alerta de “éxito” o de “error” en el menú superior derecho. Como primera opción tenemos la deleción del *Pod* en cuestión, al seleccionar esta opción aparece el siguiente modal:

.. image:: /figuras/fig_mangue/028_mangue_deletar_pod.png
    :alt: submenu Ações_deletar POD 
    :scale: 80 %
    :align: center
=====

      * **Gráfico de Performance:** En la segunda opción, el usuario puede observar los gráficos de performance de CPU y Memoria para cada *Pod*, una vez que se hace click en esta opción, se le presenta al usuario la pantalla de abajo con los gráficos de consumo de CPU y de memoria para el *Pod* seleccionado.

.. image:: /figuras/fig_mangue/029_mangue_performance_pod.png
    :alt: submenu Performance de um POD
    :align: center
=====

      * **Log**: En la tercera opción, el usuario puede ver los *logs* de un determinado *Pod* de forma similar a lo que se consigue con una sesión de emulación de consola de terminal SSH. 
  
        El usuario también puede filtrar el número de registros (líneas) que desea observar (las opciones son: 10, 20, 50, 100, 300, 500, 1000, all). Si el *Pod* tiene más de un *container* en ejecución existe un *dropdown* donde es posible seleccionar cual *container* el usuario desea visualizar los *logs*, como se muestra en la siguiente imagen:

.. image:: /figuras/fig_mangue/030_mangue_log_pods.png
    :alt: submenu Ações_log diversos pods
    :align: center
=====

      * **Línea de Comando:** En la cuarta opción, el usuario puede ejecutar líneas de comando en el *prompt* del sistema operativo del *Pod*, de forma similar a lo que se obtiene con una sesión de emulación de consola de terminal SSH. Esta funcionalidad se extiende a uno o más *containers* que existen dentro del *Pod* en cuestión. 

.. important:: Para habilitar esta función es necesario acceder al **Menú Integraciones** y seguir los pasos correspondientes al *Container Execution*.

En caso de que el *Pod* tenga más de un *container* en ejecución existe un *dropdown* donde es posible seleccionar qué *container* el usuario desea ejecutar los comandos, como se muestra en la siguiente imagen:

.. image:: /figuras/fig_mangue/031_mangue_comando_pod.png
    :alt: submenu Ações_linha de comando outro pod
    :align: center
=====

Statefulsets
------------

En esta funcionalidad la plataforma del Mangue presenta todos los *statefulsets* de un *cluster* en un determinado namespace, en la siguiente imagen se muestra informaciones como:

.. image:: /figuras/fig_mangue/048_mangue_statefulsets.png
    :alt: Listagem de Statefulsets
    :align: center
=====

* **# columna accionable:** Esta columna presenta una forma alternativa de borrar (eliminar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso se mostra el icono “Papelera” |icone_lixo_vermelho| que permite eliminar todos los elementos seleccionados con un solo comando.

* **Nombre:** Es la representación del nombre del *Statefulsetss*.
* **Labels:** Son los identificadores de los *Statefulsetss*, usados para ser el acoplamiento a un servicio. 
* **Instancias:** Los valores mostrados aquí indican que la cantidad de réplicas de un *Statefulsets* están divididos por una barra ("/") donde los valores que se encuentran en el lado izquierdo de la barra es el valor de las réplicas activas y operativas, y los valores en el lado derecho de la barra representa la cantidad máxima de réplicas que pueden ser activadas para mantener el rendimiento deseado del *Statefulsets*;
* **Status:** El status de un *Statefulsets* identifica el estado de cada *Statefulsets* listados. Puede ser presentado por **Running**, **Pending** o **"!"** (signo de exclamación).

      * El status **Running** identifica que ningún error está sucediendo con el *Statefulsets*.

      * El status **Pending** identifica algún estado de transición en el *Statefulsets*. Ya sea por actualización, inicio del proceso del *container* o cualquier actividad que identifique un estado de transición.		

      * El status **"!"** (signo de exclamación) identifica una alarma, es decir, que algo incorrecto ha ocurrido con el *Statefulsets* y sus réplicas. Por ejemplo: la imagen de un *container* es pasada con una versión inexistente, de modo que el download de este *container* no ocurre;

*  **IP:** En el caso de que el *Statefulsets* tenga un servicio asociado, es en este campo donde la IP del balanceador de carga puede ser un servicio de tipo *Loadbalancer*, puerto de acceso al servicio si es un servicio externo (tipo *nodePort*), o el *string* "IP interna" si es un servicio interno del *cluster* (tipo *ClusterIp*).
* **Imagen y versión:** Si hay más de una imagen o versión de un *container*, se listan uno debajo del otro, como en el ejemplo del 6º *Statefulsets* listado en la imagen de la tabla *Statefulsets*.
* **Duración:** Esta columna presenta el tiempo transcurrido desde el momento de creación del *Statefulsets*.
* **Acciones:** Esta columna presenta el botón de ``Acción`` |icone_acao| al ser pulsado, presenta dos opciones así como la siguiente figura:

.. image:: /figuras/fig_mangue/048.1_mangue_acoes_statefulsets.png
    :alt: Ações editar e deletar statefulsets
    :scale: 80 %
    :align: center
=====

      * **Editar Statefulsets**: Esta opción presenta una pantalla con un archivo JSON con toda la configuración del *Statefulsets* en Kubernetes, el usuario puede editar lo que sea necesario y seleccionar la opción de editar y esperar el *feedback* de la acción por la plataforma Mangue.io. Esta función atiende a los usuarios que tengan conocimiento sobre el formato de los archivos de Kubernetes.

.. image:: /figuras/fig_mangue/049_mangue_editar_statefulsets.png
    :alt: Editar
    :align: center
=====

      * **Eliminar Statefulsets:** En el menú de acciones del *Statefulsets* hay la opción de eliminar, basta el usuario hacer clic en el botón para confirmar la acción, según la pantalla que se muestra a continuación:

.. image:: /figuras/fig_mangue/050_mangue_deletar_statefulsets.png
    :alt: mensagem confirmação
    :align: center
=====

Updates
-------

Un *Update* es considerado como un evento de actualización en un *Cluster* Kubernetes, su funcionalidad está destinada a facilitar el control y la comunicación directa, entre el ambiente Kubernetes y la interfaz del Mangue.io.

.. image:: /figuras/fig_mangue/051_mangue_update.png
    :alt: Update
    :align: center
====
 
La imagen anterior muestra la lista de *updates* creados y, a continuación, la definición de cada una de las ocho columnas:

* **#:** Número secuencial del evento en la lista presentada;
* **Deployment Name:** Indica el nombre del *Deployment*. 
* **Tipo:** Determina el tipo del *update* a ser realizado, hay dos tipos de actualización, son:

      * **Actualización:** Ocurre cuando el usuario determina cuál es la próxima versión y el *container* del *Deployment*;

      * **Rollback:** es una operación que revierte el evento  para una versión anterior.

* **Status:** Hay dos estados posibles, son:

      * **UPDATED** Este estado corresponde a una actualización realizada;

      * **OUTDATED** Se refiere a un estado anterior o antiguo, que está esperando el evento de actualización a través de la plataforma Mangue;

* **Namespace:** Corresponde al *Namespace* de la aplicación que se va a actualizar y está en ejecución;
* **Nuevas imágenes:** Se refiere a las nuevas imágenes y versiones de los *containers* que son actualizados;
* **Duración:** Equivale al tiempo que la actualización ha sido registrada/ejecutada;
* **Acciones:** Esta columna presenta el botón de ``Acción``  |icone_acao| al ser pulsado, muestra una única opción:

.. image:: /figuras/fig_mangue/052_mangue_botao_atualizar.png
    :alt: ação atualizar 
    :scale: 80 %
    :align: center
=====

      * **Actualizar:** Al seleccionar la opción de actualizar en el botón de Acciones de la tabla, la plataforma Mangue.io presenta una pantalla de confirmación para la operación:

.. image:: /figuras/fig_mangue/053_mangue_mensagem_atualizar.png
    :alt: mensagem atualizar 
    :scale: 80 %
    :align: center
=====

Al hacer clic en el botón ``Actualizar``, se dispara el evento de actualización para el *Deployment* correspondiente. 

Se utilizan las imágenes y versiones de los *containers* que aparecen en el campo "Nuevas imágenes". Se crea un *feedback* de alerta en la esquina superior derecha de la pantalla informando del “Éxito” o del “Error”.

Justo encima de la tabla, hay tres elementos con los que el usuario podrá actuar:

.. image:: /figuras/fig_mangue/053.1_mangue_pesquisar_atualização.png
    :alt: Pesquisar atualização
    :align: center
=====

* **Acción de búsqueda:** Si la lista presentada en esta pantalla es muy larga (ocupa más de una página), hay un campo donde el usuario puede buscar por el nombre del *Update* deseado. Sólo tiene que introducir parte del nombre y pulsar “Enter” o hacer clic en el icono de la lupa |icone_lupa_verde|. Como resultado de esta búsqueda sólo aparecerán los *Updates* que contengan la palabra clave de la búsqueda;
* **Acción de actualizar:** Basta hacer click en el icono |icone_update| para actualizar la interfaz de la plataforma Mangue.io con los valores más recientes de esta tabla de *Updates*.
* **Crear integración de Updates:** Basta hacer clic en el signo |icone_adicionar| para el usuario registrar una nueva actualización para un *Deployment* en un determinado *Namespace*. La plataforma Mangue.io presenta al usuario la siguiente pantalla:

.. image:: /figuras/fig_mangue/054_mangue_criar_integracao.png
    :alt: Criar integração
    :align: center
=====

Sigue la descripción de los campos de esta pantalla:

** **Token:** Este campo se rellena con un *string* de caracteres, después de que el usuario haga clic en el botón ``Generar Token``, en este momento el campo se rellena con el *string* de token que se informa para comunicación con la API del Mangue.io. Este token debe ser guardado y debe ser informado para autenticar las versiones del CI. Cuando se genera un token, éste debe ser enviado vía API al servidor del Mangue.io, ya que él es el responsable de garantizar la integridad de la solicitud enviada.
* **Namespace:** Al hacer clic en este campo se muestra una lista (dropdown) con todos los *Namespaces* existentes en el *cluster* seleccionado en la pestaña “Selección de Configuración”.
* **Deployment:** Al hacer clic en el campo se muestra una lista (dropdown) con todos los *Deployments* asociados al *namespace* seleccionado del espacio anterior.
* **Crear:** Una vez que el usuario ha configurado todos los campos de esta pantalla, con los criterios correctos para añadir un evento de actualización (*update*), debe hacer clic en el botón ``Crear`` para añadir el evento de actualización en la plataforma Mangue.io. 
  
  Este nuevo evento se añade a la lista con el status *pending*. 
  
  Al hacer clic en el botón "Crear", se genera el permiso para el usuario registrar las actualizaciones en la plataforma a través de llamadas a la API del Mangue. 
  
  Se crea un *feedback* de alerta en la esquina superior derecha de la pantalla informando del “Éxito” o del “Error”. 

.. note:: Si el evento no aparece listado, inmediatamente, el usuario debe hacer clic en el icono |icone_update| (*update*) para actualizar las informaciones en la pantalla.

A continuación se enumeran dos ejemplos de los beneficios para la funcionalidad de *Updates*:

        **Ejemplo 1**:

    Un usuario tiene un *pipeline* de CI/CD que se ejecuta y genera algunas versiones estables por día. Dado que el usuario tiene su *cluster* Kubernetes gestionado por Mangue.io y sus aplicaciones instaladas es posible registrar actualizaciones en la plataforma a través del *pipeline* de CI/CD, y esperar que el evento de actualización sea disparado por la interfaz del Mangue.io.


        **Ejemplo 2**:

    Un usuario tiene *pipeline* de CI/CD que se ejecuta y genera algunas versiones estables por día. Dado que el usuario tiene su *cluster* Kubernetes gestionado por Mangue.io y sus aplicaciones instaladas es posible actualizar la aplicación directamente a través del *pipeline* de CI/CD.

====

Catálogo
========






Nueva Aplicación
----------------




====

A. Primer paso: Nueva Aplicación
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

B.Validar Nueva Aplicación
~~~~~~~~~~~~~~~~~~~~~~~~~~




====

C. Segundo paso: Deploy en los Clusters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

D. Tercer paso: Habilitar Cero Dow-time
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

Deploy via Yaml
---------------




====

A. Clusters disponibles
~~~~~~~~~~~~~~~~~~~~~~~




====

B. Template
~~~~~~~~~~~




====

C. Browse
~~~~~~~~~




====

D. Submit
~~~~~~~~~




====

E. Server VsCode
~~~~~~~~~~~~~~~~




====

ConfigMap
=========




====

Cluster Events
==============




====

Cron Jobs, Jobs
===============




====

A. Cron Jobs
------------






B. Jobs
-------






Facturación
===========




====

Informe Consolidado
-------------------




====

Historial
---------






A. Historial de facturación mensual del Cluster
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

B. Historial de facturación del Cluster 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

C. Por Tags
~~~~~~~~~~~




====

D. Alertas
~~~~~~~~~~




====

Recomendaciones
===============




====

Permisos
========




====

Contrato
--------






A. Informaciones del contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

B. Informaciones de usuarios
~~~~~~~~~~~~~~~~~~~~~~~~~~~~







Roles
-----




====

A. Sección: Roles
~~~~~~~~~~~~~~~~~




====

B. Sección: Role Bindings
~~~~~~~~~~~~~~~~~~~~~~~~~




====

Service Accounts
----------------




====

Cluster Role
------------




====

A. Sección: Cluster Roles
~~~~~~~~~~~~~~~~~~~~~~~~~




====

B. Sección: Cluster Role Binding
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

C. Sección: Pod Security Policy
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~






Integraciones
=============




====

Clusters
--------




====

Integrar Cluster
----------------




====

Integrar Múltiplos Clusters
---------------------------




====

Crear Cluster on Premise
------------------------






Proceso simplificado de integración de cluster mediante formulario
------------------------------------------------------------------




====

A. Google Kubernetes Engine - GKE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

B. Elastic Kubernetes Service - Amazon EKS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

C. Azure Kubernetes Service - AKS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

D. IBM Cloud
~~~~~~~~~~~~




====

Container Execution
-------------------




====

Performance
-----------




====

A. Sección: Añadir la Supervisión
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

B. Sección: Monitoreo Disponible
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




====

Helm
----




====

Server VS Code
--------------



====

Services, Load Balancing and Networking
=======================================




====

Servicios
---------




====

Ingress
-------




====

Namespaces
==========




====

Nodes
=====




====

Migración de cluster
====================




====

Proceso de Migración de Workloads
---------------------------------




====

Migración de Namespace
----------------------




====

Registry
========




====

Secrets
=======




====

Schedule Task
=============




====

Storage
=======




====

Storage Class
-------------




====

PersistentVolume
----------------




====

PersistentVolumeClaims
----------------------




====

Tareas
======




====

Clusters Workloads
==================




====

Conclusión
==========





====
