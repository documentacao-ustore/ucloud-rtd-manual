
.. image:: /figuras/mangue-logo-peq.png
    :alt: Logo Mangue
    :scale: 50 %
    :align: center
=====

.. centered:: Português_     -     Español     -     English_

.. _Português: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/mangue-usuario.html 

.. _English: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/MEnglish/mangue-usuario.eng.html

====

Manual del usuario
++++++++++++++++++

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

      * **Reversión** |icone_reversao|: Esta opción permite al usuario realizar la acción de revertir la versión actual de el (los) *deployment(s)* seleccionado(s) para su versión inmediatamente anterior a la existente en la plataforma de Mangue.io. 

      * **Escalar** |icone_escalar|: La función de esta acción permite al usuario informar el número (entero) deseado para incrementar el número de réplicas de la aplicación (*deployment*). 

      * **Papelera** |icone_lixo_vermelho|: Acción que permite al usuario eliminar todos los elementos seleccionados con una sola orden. 

      * **Cambiar versión** |icone_alterar_versao|: Esta opción permite actualizar múltiples *deployments* a la vez, al que el usuario puede informar la próxima versión de cada uno de ellos. 

* **Deploys:** Es la representación del nombre del *deployment.d*
* **Labels:** Son los identificadores de los *deployments*, utilizados para ser el enlace a un servicio. 
* **Instancias:**  Muestra la cantidad de réplicas que están operativas de un *Deployment*, y la cantidad total de réplicas operativas deseadas para este *Deployment*. Están divididas por una barra (“/”) donde los valores encontrados antes de la barra son las réplicas operacionales, y los valores después de la barra representan la cantidad esperada de réplicas operacionales.
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


.. note:: El usuario puede verificar una indicación de error en la columna **Status** en la pantalla del menú *Workloads/Deployments* y consultar el *deployment* específico, al que se ha asociado el *PersistentVolume*, según la imagen anterior mostrada en el tópico *Deployments*.

* **Storage Class:** El usuario debe seleccionar cuál es el volumen de *NFS Storage* disponibles en la lista presentada. 
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

Para confirmar todas las opciones arriba indicadas, el usuario debe hacer clic con el ratón en el botón ``Crear Servicio`` y esperar el *feedback* de creación.

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

Después de hacer clic en “Actualizar Versión de la Aplicación” la plataforma presenta la imagen "Actualizar Versión de *Deployment*". A través de este control, el usuario puede generar una “nueva versión” para cualquier *deployment* existente en la plataforma Mangue.io. 

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

* **Imagem:** Esta columna presenta la información de la imagen pública que fue utilizada para la creación de este *deployment.* Esta imagen se puede encontrar en sitios públicos que contienen información técnica relacionada con la aplicación en sí, un ejemplo es el Docker Hub_ 

.. _Hub: https://hub.docker.com/

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
* **Tipo:** Describe el tipo de evento ocurrido, y se pueden enumerar los siguientes tipos de eventos:

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

* **Mensaje:** En esta columna la plataforma del Mangue.io presenta una lista de mensajes que pueden ayudar a identificar el éxito del evento o la causa raíz de un potencial problema, de esta manera permite al usuario tomar alguna acción para eliminar la causa raíz del problema o estar seguro del éxito de este evento.

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
* **Instancias**: Está representada por la cantidad de réplicas operacionales de un *Daemonsets*, y por la cantidad total de réplicas operacionales deseadas para este *Daemonsets*. Están divididos por una barra (“/”) donde los valores encontrados antes de la barra son las réplicas operacionales, y los valores después de la barra representan la cantidad esperada de réplicas operacionales.
* **Status:** El *status* de un *Daemonsets* identifica su estado actual. Puede ser representados por *Running*, *Pending* o *“!”* (signo de exclamación):

      * El *status* **Running** identifica que ningún error está sucediendo con el *Daemonsets*.

      * El *status* **Pending** identifica algún estado de transición en el *Daemonsets*. Ya sea por actualización, inicio del proceso del *container* o cualquier actividad que identifique un estado de transición.

      * El status **“!”** (signo de exclamación) identifica una alarma, en otras palabras, que algo incorrecto ha sucedido con el *Daemonsets* y sus réplicas. Por ejemplo: la imagen de un *container* es pasada con una versión inexistente, de modo que el *download* no ocurre.

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

    En este caso se mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos por indicados por el usuario con un solo comando.

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

    En este caso es presentado el icono "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando.

* **Nombre**: Nombre del *Deployment* que se establece en el momento de su creación;
* **Nodo:** Presenta el nombre del nodo Kubernetes que está ejecutando este *Deployment*;
* **Status**: Presenta el *status* del *Deployment* en su respectivo *node*. El *status* de un *Deployment* identifica el estado actual. Pueden ser representados por:

      * **Running** identifica que ningún error está sucediendo con el *Deployment*.

      * **Pending** identifica algún estado de transición en el *Deployment*. Ya sea por actualización, inicio del proceso del *container* o cualquier actividad que identifique un estado de transición.

      * **“!”** (signo de exclamación) identifica una alarma, es decir, que algo incorrecto ha ocurrido con el *Deployment* y sus réplicas. Por ejemplo: la imagen de un *container* es pasada con una versión inexistente, así el download de este *container* no ocurre;

* **Imagen:** Esta columna muestra la información de la imagen pública utilizada para la creación de este *Deployment*. Esta imagen se puede encontrar en sitios públicos que contienen informaciones técnicas relacionadas con la aplicación en sí, un ejemplo es el Docker Hub_.
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

    En este caso se mostra el icono "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos seleccionados con un solo comando.

* **Nombre:** Es la representación del nombre del *Statefulsetss*.
* **Labels:** Son los identificadores de los *Statefulsetss*, usados para ser el acoplamiento a un servicio. 
* **Instancias:** Los valores mostrados aquí indican que la cantidad de réplicas de un *Statefulsets* están divididos por una barra ("/") donde los valores que se encuentran en el lado izquierdo de la barra es el valor de las réplicas activas y operativas, y los valores en el lado derecho de la barra representa la cantidad máxima de réplicas que pueden ser activadas para mantener el rendimiento deseado del *Statefulsets*;
* **Status:** El status de un *Statefulsets* identifica el estado de cada *Statefulsets* listados. Puede ser presentado por **Running**, **Pending** o **“!”** (signo de exclamación).

      * El status **Running** identifica que ningún error está sucediendo con el *Statefulsets*.

      * El status **Pending** identifica algún estado de transición en el *Statefulsets*. Ya sea por actualización, inicio del proceso del *container* o cualquier actividad que identifique un estado de transición.		

      * El status **“!”** (signo de exclamación) identifica una alarma, es decir, que algo incorrecto ha ocurrido con el *Statefulsets* y sus réplicas. Por ejemplo: la imagen de un *container* es pasada con una versión inexistente, de modo que el download de este *container* no ocurre;

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

* **Acción de búsqueda:** Si la lista presentada en esta pantalla es muy larga (ocupa más de una página), hay un campo donde el usuario puede buscar por el nombre del *Update* deseado. Sólo tiene que introducir parte del nombre y pulsar “Enter” o hacer clic en el icono de "La lupa" |icone_lupa_verde|. Como resultado de esta búsqueda sólo aparecerán los *Updates* que contengan la palabra clave de la búsqueda;
* **Acción de actualizar:** Basta hacer click en el icono |icone_update| para actualizar la interfaz de la plataforma Mangue.io con los valores más recientes de esta tabla de *Updates*.
* **Crear integración de Updates:** Basta hacer clic en el signo |icone_adicionar| para el usuario registrar una nueva actualización para un *Deployment* en un determinado *Namespace*. La plataforma Mangue.io presenta al usuario la siguiente pantalla:

.. image:: /figuras/fig_mangue/054_mangue_criar_integracao.png
    :alt: Criar integração
    :align: center
=====

Sigue la descripción de los campos de esta pantalla:

* **Token:** Este campo se rellena con un *string* de caracteres, después de que el usuario haga clic en el botón ``Generar Token``, en este momento el campo se rellena con el *string* de token que se informa para comunicación con la API del Mangue.io. Este token debe ser guardado y debe ser informado para autenticar las versiones del CI. Cuando se genera un token, éste debe ser enviado vía API al servidor del Mangue.io, ya que él es el responsable de garantizar la integridad de la solicitud enviada.

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


La plataforma Mangue.io permite al usuario crear aplicaciones (*Deployments*) de dos formas diferentes: la forma simplificada que guía el usuario a través de la secuencia de pantallas y la forma elaborada que permite al usuario el *upload* de un archivo de texto.

A continuación se describen los dos formatos de creación de aplicaciones (*deployments*): 

La primera es la forma simplificada, ocurre al guiar el usuario por las pantallas, que después de todo el llenado y confirmación del usuario, los datos informados son convertidos en un archivo con "sintaxis *YAML*", esta construcción (prácticamente sin errores) es utilizada para generar la aplicación.

El objetivo de este primer enfoque es minimizar los posibles errores de sintaxis *YAML* en el ambiente Kubernetes, demanda un alto grado de especialización y conocimiento del desarrollador. La sintaxis correcta para el ambiente, debe tener todas las dependencias necesarias para la generación del resultado deseado de la manera correcta y lista para el uso en el ambiente Kubernetes (por ejemplo: una aplicación / *Deployment*).

La otra forma es permitir al usuario hacer *upload* de un archivo de texto, cuyo contenido es la codificación de la aplicación en sintaxis *YAML*, ya adaptada y preparada para un ambiente Kubernetes. Si el desarrollador (usuario) tiene suficiente práctica para crear sus propios *scripts* en sintaxis *YAML*, puede utilizarlos y traer estos para la plataforma Mangue.io con la finalidad de conducir en que *Cluster, Pod, Node*, este código / *script* es ejecutado y gestionado.

Cuando el usuario acceder al menú Catálogo, la plataforma Mangue.io presenta la pantalla a continuación, en la secuencia, la descripción de cada una de las opciones del flujo de este menú.

.. image:: /figuras/fig_mangue/055_mangue_catalogo.png
    :alt: Catálogo
    :align: center
=====

Nueva Aplicación
----------------

Esta modalidad es la forma en que la plataforma Mangue.io conduce al usuario a través de pantallas, solicitando las informaciones en secuencia para que, posteriormente, la plataforma Mangue.io compile las informaciones generando la aplicación dentro del *Cluster* y Namespace seleccionados en la pestaña |icone_engrenagem| “Selección de Configuración”.

A continuación se describen los pasos que se deben seguir para rellenar los formularios de las pantallas que guían al usuario. 

====

A. Primer paso: Nueva Aplicación
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para la creación de una nueva aplicación (*Deployment*) la plataforma Mangue.io segmenta el proceso en dos etapas, el usuario debe rellenar los siguientes campos:

.. image:: /figuras/fig_mangue/056_mangue_criar_deployment.png
    :alt: Criar deployment
    :align: center
=====

* **Nombre:** Este campo es obligatorio, el usuario debe informar el nombre de la aplicación (*Deployment*) con el que se identifica en la plataforma Mangue.io;
* **Réplicas:** Este campo es obligatorio, el usuario debe informar un número (entero) que desea asignar para ejecutar la aplicación (*Deployment*) desde su creación. 

    Este número se asigna desde la infraestructura computacional para que el usuario obtenga la mejor experiencia de performance, y la plataforma Mangue.io se encarga de asignar estos recursos computacionales;

* **Buscar imagen**: Este campo es obligatorio, una búsqueda de imagen de una aplicación se realiza en el servidor de registro de imágenes http://hub.docker.com. El usuario puede introducir una secuencia de caracteres (aunque sea parcial) de cualquier imagen catalogada en el *Hub Docker*, y la plataforma Mangue.io realiza la búsqueda y presenta una lista que contiene la secuencia de caracteres. Vea el ejemplo siguiente, con la búsqueda de la secuencia “wordp”, para buscar la imagen de la aplicación *Wordpress*:

.. image:: /figuras/fig_mangue/057_mangue_pesquisar_imagem.png
    :alt: Pesquisar imagem
    :align: center
=====

Basta con que el usuario haga clic con el cursor del ratón en la línea de la imagen deseada para seleccionar la mejor imagen disponible.

* **Nombre del Container:** Este campo es obligatorio, en él debe ser informado el nombre del *container* a ser utilizado en la plataforma Mangue.io;
* **Bloquear la ejecución de usuario privilegiado:** En este campo el usuario puede bloquear los *containers* del *Deployment* para que sean ejecutados de forma privilegiada, con acceso a los recursos y las capacidades *Kernel* de la máquina *Host*;
* **Especificar ID de usuario, grupo o archivo de sistema:** En este campo es posible indicar el ID de usuario, grupo o archivo de sistema en el que se ejecuta el *container*.
* **Tags de Aplicación:** En este campo el usuario puede informar los *Tags*. También es posible crear un *Tag* para asociarlo a la aplicación.
* **Botón** ``Añadir``: Para crear una nueva aplicación (*Deployment*) la plataforma Mangue.io segmenta el proceso en dos etapas; después de confirmar la acción sobre el botón ``Añadir`` el usuario visualiza la siguiente pantalla:

.. image:: /figuras/fig_mangue/058_mangue_modal_imagem.png
    :alt: Modal imagem
    :align: center
=====

* **Versión de la Imagen:** Este campo es obligatorio, el usuario debe informar como la aplicación (*Deployment*) es identificada en el ambiente. Este campo se puede llenar con números o caracteres, para satisfacer la demanda del usuario (Ex.: latest, última, 1.xx, 1.20).

* **ContainerPort:** Este campo es obligatorio, el usuario debe informar cuál puerto TCP-IP del *container* puede ser utilizado para que la aplicación (*Deployment*) quede disponible al acceso de otros usuarios;

      * **Máximo Recurso a ser utilizado [CPU en milicores]:** En este campo el usuario es capaz de informar el máximo de recursos de CPU que pueden ser asignados, en la infraestructura computacional del *Cluster* para ofrecer el máximo rendimiento para esta aplicación (*Deployment*). Esta cantidad debe ser informada con un número entero, para soportar y ejecutar la aplicación (*Deployment*).

      * **Mínimo Recurso a ser utilizado [CPU en milicores]:** En este campo el usuario es capaz de informar el mínimo de recursos de CPU que pueden ser asignados, en la infraestructura computacional del *Cluster* para ofrecer el desempeño mínimo aceptable para esta aplicación (*Deployment*). Esta cantidad debe ser informada con un número entero, para soportar y ejecutar la aplicación (*Deployment*).

      * **Máximo recurso a ser utilizado [Memoria en milicores]:** En este campo el usuario debe informar el máximo de recursos de memoria RAM que pueden ser asignados, en la infraestructura computacional del *Cluster* para proporcionar el máximo rendimiento a esta aplicación (*Deployment*). Esta cantidad debe ser introducida como un número entero para apoyar y ejecutar el (*Deployment*);

      * **Mínimo Recurso a ser utilizado** [Memoria en milicolores]: En este campo el usuario debe informar el mínimo de recursos de memoria RAM que pueden ser asignados, en la infraestructura computacional del *Cluster* para ofrecer el desempeño mínimo aceptable para esta aplicación (*Deployment*). Esta cantidad debe ser informada con un número entero, para soportar y ejecutar la aplicación (*Deployment*).

* **Permitir ejecución privilegiada:** En este campo el usuario debe informar si el *container* tiene acceso a los recursos y capacidades *Kernel* de la máquina *Host*;

* **Especificar ID de usuario, grupo o archivo de sistema:** En este campo es posible indicar el ID de usuario, grupo o archivo de sistema que el *container* es ejecutado.

* **Registry Secret:** En este campo el usuario debe introducir el nombre del *Secret* del servidor de imágenes asociado a esta imagen. Al hacer clic con el ratón sobre este campo, la plataforma Mangue.io presenta una lista de archivos de *Secrets* disponibles en el servidor de imagen privado. 

* **Botón** ``Próximo``: Cuando el usuario hace clic en el botón ``Próximo`` la plataforma Mangue.io muestra la pantalla con campos respectivos de *Secrets* y Variables de ambiente del *container*. Vea la siguiente pantalla:

.. image:: /figuras/fig_mangue/059_mangue_secrets_e_variaveis.png
    :alt: Secrets e variáveis do ambiente container
    :align: center
=====

* Variables de Ambiente:

      * Nombre de la variable de ambiente:

      * Contenido de la variable de ambiente:

      * Botón ``Añadir``: 

* *Secrets*

      * Nombre del Secreto:

      * Variable de Ambiente:

      * Llave del Secreto:

      * Valor del Secreto:

      * Botón ``Añadir``: 

      * Botón ``Crear Secret``: 

      * Botón ``Volver``: 

      * Botón ``Crear Finalizar``: 

Tras pulsar el botón ``Finalizar``, la plataforma Mangue.io cierra las subpantallas y vuelve a la primera etapa del proceso de la nueva aplicación, presenta la configuración listada, como en el ejemplo de abajo:

.. image:: /figuras/fig_mangue/061_mangue_lista_aplicacao.png
    :alt: Lista aplicação
    :align: center
=====

A continuación describimos el contenido de las columnas que se muestran en esta lista:

* **#:** Presenta el número secuencial del *container* en la lista presentada.
* **Container:** Presenta el nombre del *container* informado en los pasos anteriores, el inicio del proceso de creación de una nueva aplicación (*Deployment*).
* **Imagen:** Muestra el nombre de la imagen de la aplicación seleccionada del servidor de registro de imágenes (ej.: http://hub.docker.com).
* **Versión:** Presenta la información de la versión de la aplicación (*Deployment*) informada en las etapas anteriores.
* **Acciones:** Esta columna presenta el botón ``Acción`` |icone_acao| al ser pulsado, presenta un submenú con las siguientes opciones:

.. image:: /figuras/fig_mangue/062_mangue_acoes_submenu.png
    :alt: Ações submenu 
    :scale: 80 %
    :align: center
=====


      * **Añadir PersistentVolumeClaim**: A través de esta pantalla el usuario puede configurar las características del archivo referente al *PersistentVolumeClaim* (PVC). 

La plataforma Mangue.io simplifica el proceso de configuración del PVC, ofreciendo al usuario opciones en la interfaz gráfica que dirigen las decisiones relativas al PVC, del siguiente modo:

.. image:: /figuras/fig_mangue/063_mangue_add_pvc.png
    :alt: Adicionar persistentvolume claim
    :align: center
====

          * **Tamaño / 1Gi, 5Gi, 10Gi:** El usuario puede seleccionar el tamaño del volumen simplemente haciendo clic con el cursor del ratón sobre el número deseado, seleccionando la mejor opción de tamaño para este PVC. Las opciones están expresadas en Gigabytes (1, 5, ou 10).

          * **Tamaño / Personalizado:** Otra forma de crear un PVC con un volumen con un tamaño diferente de las opciones anteriores, la plataforma Mangue.io presenta una barra deslizante (*slide bar*) que permite al usuario seleccionar el tamaño deseado del PVC. Usando el cursor del ratón sobre el indicador naranja, el usuario puede mover este indicador (para izquierda o derecha) para establecer el tamaño final deseado. El tamaño mínimo es de 1 gigabyte y el máximo de 100 gigabytes.

          * **Storage Class:** Este campo es una lista (*dropdown list*) compuesta solo por *NFS Servers* configurados en la plataforma Mangue.io. El usuario debe seleccionar el servidor *NFS* más adecuado para recibir el archivo de PVC.

          * **Modo de Acceso:** Esta columna presenta la configuración de acceso a este volumen, estos modos de acceso pueden ser tres, son: *ReadWriteOnce*, *ReadOnlyMany*, *ReadWriteMany*.

          * **Mouth Path:** En este campo el usuario debe informar la ruta donde el volumen es montado en el *container*. Si la base de la aplicación es un ambiente Linux, la ruta de montaje del volumen debe utilizar la notación del ambiente del sistema operativo Linux.

          * **Nombre del Volumen:** En este campo el usuario debe informar el nombre del archivo de volumen creado en el ambiente del sistema operativo del *Cluster*.

      * **Añadir ConfigMap:** Un *ConfigMap* es un objeto API utilizado para almacenar datos no confidenciales en pares clave-valor. En esta sub pantalla el usuario puede incluir y configurar el(los) archivo(s) de *ConfigMap(s)* deseado(s) para su ambiente.

.. image:: /figuras/fig_mangue/064_mangue_add_configmap.png
    :alt: Adicionar configmap
    :align: center
=====

          * **Nombre del ConfigMap:** Este campo es obligatorio el usuario debe informar el nombre deseado para registrar en la plataforma de Mangue.io y identificar este *ConfigMap*.

          * **Botón** ``Añadir`` |icone_adicionar|

          * **Mount Path:** Este campo es obligatorio el usuario debe informar la ruta donde se monta el volumen en el *container*. Si la base de la aplicación es un ambiente Linux, la ruta de montaje del volumen debe utilizar la notación del ambiente del sistema operativo Linux. 

          * **Nombre del archivo:** Este campo es obligatorio el usuario debe informar en el nombre del archivo que se crea en el sistema operativo de la máquina virtual que utiliza *ConfigMap*.

          * **Contenido del Archivo:** Este campo es obligatorio el usuario debe rellenar con el contenido específico del *ConfigMap*.

          * **Botón** ``Añadir ConfigMap``: Después de rellenar todos los campos anteriores, el usuario debe pulsar este botón con el cursor del ratón para que la plataforma Mangue.io pueda fomentar la creación, configuración y grabación del *ConfigMap* para esta nueva aplicación (*Deployment*).

      * **Editar Container:** Cuando se selecciona esta opción, la plataforma Mangue.io muestra la pantalla relacionada con el **Primer Paso: Nueva Aplicación**, para que el usuario pueda editar las configuraciones de este *container*.

      * **Eliminar Container:** Esta acción es definitiva y cuando se activa, la plataforma Mangue.io elimina toda la configuración inicial del *container*, **no es solicitada una confirmación de esta acción**.

====

B.Validar Nueva Aplicación
~~~~~~~~~~~~~~~~~~~~~~~~~~

Si el usuario hace clic con el ratón sobre el nombre del *container*, la plataforma Mangue.io presenta una pantalla con las informaciones de los recursos del *container*.

La plataforma Mangue.io identifica los recursos de *PersistentVolumeClaim*, *ConfigMap*, del *container* que el usuario ha configurado para la aplicación y enumera estas características según el ejemplo de la siguiente pantalla:

.. image:: /figuras/fig_mangue/065_mangue_recurso_container.png
    :alt: Recurso container
    :align: center
=====

* **#:** Esta columna muestra el número secuencial del *container* en la lista mostrada.
* **Nombre:** Esta columna muestra el nombre del recurso informado en los pasos anteriores.
* **Tipo:** Esta columna presenta el tipo de recurso que se ha creado en los pasos anteriores.
* **Mouth Path:** Esta columna muestra las informaciones del directorio del sistema operativo como se ha configurado en los pasos anteriores.
* **Acciones:** Esta columna presenta el botón de ``Acción`` |icone_acao| que al ser pulsado, presenta un submenú con las siguientes opciones:

.. image:: /figuras/fig_mangue/066_mangue_acoes_recursos.png
    :alt: Ações recursos 
    :scale: 80 %
    :align: center
=====

      * **Adjuntar a otro container:** Una facilidad de la plataforma Mangue.io permite que el usuario pueda adjuntar esta aplicación a un *container* diferente de lo que ha sido creado desde el inicio de este proceso. 

        Al hacer clic sobre esta opción la plataforma Mangue.io presenta la siguiente pantalla:

.. image:: /figuras/fig_mangue/067_mangue_criar_pcv.png
    :alt: Selecionar container
    :align: center
=====

Al hacer clic sobre el campo *containers* se presenta una lista (*dropdown list*) con los *containers* disponibles y configurados en la plataforma Mangue.io. Basta con que el usuario seleccione el *container* deseado y confirme la acción.

      * **Eliminar:** Esta acción es definitiva cuando activada la plataforma Mangue.io elimina toda la configuración inicial del *container*. 

.. attention:: No hay solicitud de una confirmación en la acción "Eliminar".

====

C. Segundo paso: Deploy en los Clusters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta sección posibilita al usuario entender cómo operar una facilidad de esta plataforma. Ella permite crear, lanzar y ejecutar esta nueva aplicación (*Deployment*) en más de un *Cluster* simultáneamente.

La plataforma posibilita operacionalizar la selección de uno o más *Cluster(es)*, actualmente configurados en el ambiente Mangue.io. Abajo la imagen y la descripción detallada de la sección:

.. image:: /figuras/fig_mangue/068_mangue_deploy_clusters.png
    :alt: Deploy clusters
    :align: center
=====

* **Clusters disponibles:** Este campo cuando se seleccionado presenta la lista (*dropdown list*) con todos los *Clusters* configurados en la plataforma y basta al usuario seleccionar cuales desea lanzar y ejecutar a la aplicación de *Deployment* que se está creando.
**Botón** ``Siguiente``: El usuario debe hacer clic en este botón para iniciar el tercer y último paso para crear una nueva aplicación (*Deployment*).

====

D. Tercer paso: Habilitar Cero Down-time
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Como se ha mencionado al principio de este tópico, el objetivo de este primer enfoque - Creación de nuevas aplicaciones a través de pantallas/formularios en Mangue.io - es minimizar los posibles errores de sintaxis *YAML* para un ambiente *Kubernetes*. 

La creación de código en sintaxis *YAML* en un ambiente *Kubernetes* exige un alto grado de experiencia y conocimiento del desarrollador. Así que la sintaxis correcta para el ambiente puede tener todas las dependencias necesarias para generar el resultado deseado e integrado en el uso del ambiente *Kubernetes* (por ejemplo, una aplicación / *Deployment*).

El desarrollo de un *script* de una aplicación (*Deployment*) con la sintaxis *YAML* en un ambiente de *Kubernetes* puede ser muy largo, y las dependencias entre secciones del *script* con elementos externos (PVCs, *ConfigMaps*, variables de ambiente, entre otros) puede inducir la creación del *script* con errores o fallos de ausencias de parámetros, derivados de la poca experiencia o intento de usar un *script* desarrollado por otra persona.

Por ejemplo:

Un *script* genérico encontrado en el ambiente virtual puede no dejar claras todas las dependencias de variables de ambiente y archivos externos. 

El proceso de adaptación de *scripts* (poco documentado en el año 2018) podría ser una gran frustración y dificultar la popularización del ambiente *Kubernetes*, por lo que la plataforma Mangue.io simplifica este proceso guiando al usuario a través de pantallas y formularios.

Después de rellenar por completo (esta segunda parte), de todos los campos de las pantallas y formularios relacionados con la creación de la aplicación (*Deployment*) la plataforma Mangue.io genera el *script YAML* completo y, en consecuencia, su compilación sin errores.

El lector de este documento puede ver a continuación la descripción de las próximas pantallas que forman parte del último paso antes de la finalización y creación de la aplicación (*Deployment*) que es ejecutada y gestionada por la plataforma Mangue.io.

.. image:: /figuras/fig_mangue/069_mangue_habilitar_downtime.png
    :alt: Habilitar zero downtime
    :align: center
=====

* **MaxSurge:** En este campo el usuario debe introducir el número máximo de réplicas que quiere mantener activas en la plataforma Mangue.io. Durante un proceso de actualización de la versión de la aplicación (*Deployment*), este número es responsable de mantener un mínimo de réplicas para asegurar la experiencia del usuario durante un proceso de actualización.

* **MaxUnavailable:** En este campo el usuario debe informar del número máximo de réplicas que desea mantener indisponibles en la plataforma Mangue.io, Durante un proceso de actualización de la versión de la aplicación (*Deployment*), este número indica al plataforma Mangue.io el número de réplicas que pueden ser actualizadas en paralelo.

* **Container:** Se trata de un encabezado de sección que indica el nombre del *container* que se está creando para esta nueva aplicación (*Deployment*).

* **Sección ReadinessProbe:** El ambiente *Kubernetes* usa sondeos de disponibilidad (*ReadinessProbe*) para saber cuando un *container* está listo para empezar a aceptar tráfico. Un *pod* se considera terminado cuando todos sus *containers* están listos. En los campos siguientes el usuario debe introducir los valores del ambiente de *ReadinessProbe*.

      * **SuccessThreshold:** En este campo el usuario debe introducir un número entero que define el número mínimo de *containers* que la plataforma Mangue.io debe mantener disponibles durante el proceso de actualización, para garantizar la experiencia del usuario que está utilizando la aplicación (*Deployment*).

      * **FailureThreshold:** En esta área el usuario debe registrar un número entero que define el número máximo de *containers* que no están disponibles durante un proceso de actualización de la versión de la aplicación (*Deployment*). Este número indica a la plataforma Mangue.io el número de réplicas que se pueden actualizar en paralelo.

      * **ReadinessPath:** En este espacio el usuario debe indicar la ruta del directorio donde se crea un archivo de registro (*log*) que almacena los eventos durante el proceso de actualización del *container*.

      * **RequestHeaders:** En esta subsección el usuario puede configurar el *layout* del contenido del archivo de registro de eventos de la actualización que debe ser creado, añadiendo columnas (*headers*) y el contenido de la columna;

      * **Nombre de Header:** En este campo el usuario debe informar el nombre de la columna que es creada dentro del archivo de registro (*log*) de las actividades de actualización.

      * **Valor de Header:** En este espacio el usuario debe indicar el valor inicial de la columna que es creada dentro del archivo de registro (*log*) de actividades de actualización.

      * **Botón** ``Añadir``: Este botón informa a la plataforma Mangue.io que el conjunto de *header/value* debe ser configurado en el archivo de registro de actividades (*log*) de actualización. El usuario puede añadir la cantidad de columnas que sean necesarias, sólo tiene que rellenar los valores de los campos anteriores y pulsar el botón ``Añadir``.

* **LivenessProbe:** El ambiente Kubernetes utiliza el sondeo de actividad (*LivenessProbe*) para saber cuándo reiniciar un *container*. Estos sondeos se realizan en intervalos de tiempo (segundos) definidos por el usuario y tras este periodo añade una línea en el archivo de *log*. En los espacios siguientes el usuario introduce los valores referidos al ambiente de *LivenessProbe*:

      * **PeriodSeconds:** En este campo el usuario debe informar un número entero que representa el período de segundos referente al intervalo de sondeo de actividad (*livenessprobe*).

      * **ReadinessPath:** En esta zona el usuario debe indicar la ruta del directorio donde se crea un archivo de registro (*log*) que almacena los eventos durante el proceso de actualización del *container*.

      * **Request Headers:** En esta subsección el usuario puede configurar el layout del contenido del archivo de registro de eventos de la actualización a ser creada, añadiendo las columnas (*headers*) y el contenido de la columna;

      * **Nombre del Header:** En este campo el usuario debe introducir el nombre de la columna que es creada dentro del archivo de registro (*log*) de las actividades de actualización.

      * **Valor de Header:** En este espacio el usuario debe indicar el valor inicial de la columna que se crea dentro del archivo de registro (*log*) de actividades de actualización.

      * **Botón** ``Añadir``: Este botón informa a la plataforma Mangue.io que el conjunto de *header/value* debe ser configurado en el archivo de registro de actividades (*log*) de actualización. El usuario puede añadir tantas columnas como sea necesario, sólo tiene que rellenar los valores de los campos anteriores y pulsar el botón ``Añadir``.

      * **Botón** ``Volver``: Si el usuario necesita volver a una etapa anterior, debe presionar este botón. Es importante destacar que en esta operación se pierde todas las informaciones que fueron rellenadas en esta pantalla por el usuario, la plataforma Mangue.io regresa a la pantalla anterior.

      * **Botón** ``Finalizar``: El usuario debe pulsar este botón cuando todos los campos de las pantallas anteriores hayan sido rellenados, y la solicitud se encuentre lista para comenzar la compilación de la aplicación (*Deployment*). La plataforma Mangue.io compila todas las informaciones de los campos y genera un *script YAML*. Al compilar este *script* y generar la aplicación (y todas sus dependencias: PVCs, *ConfigMaps*, Archivos de *Log*, entre otros) se ejecuta y gestiona dentro del ambiente de la plataforma Mangue.io.

En este punto, la plataforma Mangue.io cierra las pantallas de creación de aplicación (*Deployment*) y el usuario puede encontrar su nueva aplicación listada en la pantalla del menú *Workloads/Deployments*.

El usuario puede obtener más informaciones sobre su nueva aplicación en el menú “Informaciones de *Deployment*”.

====

Deploy via *YAML*
-----------------

Este es el segundo enfoque que la plataforma del Mangue.io permite al usuario, que es cargar un archivo de texto, cuyo contenido es la codificación de la aplicación en sintaxis *YAML*, ya adaptada y preparada para un ambiente Kubernetes.

*YAML* significa en inglés *“Ain’t Markup language”*, en español es lo mismo que "no es un lenguaje de marcado", según https://yaml.org/, es un estándar de serialización de datos amigables para cualquier lenguaje de programación. *YAML* fue creado con la convicción de que todos los datos pueden representarse adecuadamente como una combinación de listas, *hashes* (mapas) y datos escalares (valores simples). 

La sintaxis es relativamente simple y ha sido diseñada teniendo en cuenta que es muy legible, pero que también fue fácilmente mapeada a los tipos de datos más comunes en la mayoría de los lenguajes de alto nivel. Además, *YAML* utiliza una notación basada en endentación y un conjunto de caracteres distintos de los utilizados por el *XML*, haciendo que los dos lenguajes sean fácilmente compuestos uno en el otro.

Cualquier usuario con conocimiento de la sintaxis *YAML* puede utilizar la interfaz de Mangue.io para crear uno: *Deployment, Service, Statefulsets*, Volumen o *Ingress*.

La plataforma Mangue.io permite al usuario experimentado en *YAML* ingresar con su código de forma libre directamente a través de la interfaz (*data-entry*), o cargar un archivo (*upload*) en formato texto sin formato (ASCII) de un directorio/*Folder* de su ordenador para la plataforma Mangue.io.

Al hacer clic en la opción *Deploy* vía Código *YAML* la plataforma  Mangue.io muestra la siguiente pantalla:

.. image:: /figuras/fig_mangue/070_mangue_deploy_clusters.png
    :alt: Deploy em outros clusters
    :align: center
=====

A continuación se detallan cada uno de los objetos accionables de esta pantalla.

====

A. Clusters disponibles
~~~~~~~~~~~~~~~~~~~~~~~

El usuario debe hacer clic en el campo “*Clusters Disponibles*” para abrir una lista (*dropdown*) de todos los *Clusters* configurados en la plataforma Mangue.io, a continuación, seleccionar el *Cluster* destino en el que el *Deployment* es creado y ejecutado.

Hay un mensaje presente en la pantalla que es importante resaltar para el proceso de creación del *Deployment* vía *YAML*.

.. note:: Si no se selecciona ningún *Cluster*, es realizado el *deploy* en el *Cluster* utilizado actualmente.

====

B. Template
~~~~~~~~~~~

En la secuencia el usuario debe seleccionar una de las opciones de modelo (*template*) de código *YAML* que está previamente configurado en la plataforma Mangue.io, esta funcionalidad agrega productividad al usuario; cada tipo de modelo es una opción en la lista (*drop-down*):

      * **Default:** Permite al usuario configurar el código *YAML* de forma libre. En esta opción el usuario debe poseer un buen conocimiento de la sintaxis *YAML* para entrar con el código deseado. El usuario debe comenzar haciendo clic con el ratón en el área gris junto al número "1" antes de comenzar a escribir su código *YAML*. 

.. attention:: En cada nueva línea el usuario debe usar la tecla ``Enter`` para iniciar una nueva línea. 

El usuario debe utilizar su propia experiencia de desarrollo para estructurar la sintaxis de su código línea por línea. A través de esta opción, el usuario puede ingresar un código *YAML* para crear, para aprovisionar un nuevo *Pod* en la plataforma Mangue.io.

* **Deployment:** En esta opción, la plataforma Mangue.io presenta un modelo de código *YAML* con la sintaxis inicial para crear un *Deployment*. El usuario puede utilizar el ratón para hacer clic en la línea y la ubicación deseadas y, a continuación, comenzar a escribir sus parámetros específicos del *Deployment*. De esta forma, editar el modelo del código *YAML* que la plataforma presenta.

* **Servicio**: En esta opción, la plataforma Mangue.io presenta un modelo de código *YAML* con la sintaxis inicial para crear un Servicio. El usuario puede utilizar el ratón para hacer clic en la línea y la ubicación deseadas y, a continuación, empezar a escribir los parámetros específicos de su servicio. De esta forma, editar el modelo del código *YAML* que la plataforma presenta.

* **Statefulsets**: En esta opción la plataforma Mangue.io presenta un modelo de código *YAML* con la sintaxis inicial para crear un *Statefulsets*. El usuario puede hacer clic con el ratón en la línea y ubicación deseadas, a continuación se libera para comenzar a escribir sus parámetros específicos para el *Statefulsets*. De esta forma, editar el modelo del código *YAML* que la plataforma presenta.

* **Volumen**: En esta opción la plataforma Mangue.io presenta un modelo de código *YAML* con la sintaxis inicial para crear un Volumen. El usuario puede hacer clic con el ratón en la línea y ubicación deseadas y, a continuación, empezar a escribir sus parámetros específicos para el Volumen. De esta forma, editar el modelo del código *YAML* que la plataforma presenta.

* **Ingress**: En esta opción, la plataforma Mangue.io presenta un modelo de código *YAML* con la sintaxis inicial para crear una definición de *Ingress*. El usuario puede utilizar el ratón para hacer clic en la línea y la ubicación deseadas y, a continuación, empezar a escribir sus parámetros específicos. De esta forma, editar el modelo del código *YAML* que la plataforma presenta.

El usuario experimentado en *YAML* puede constatar que el uso de modelos aumenta la productividad y mantiene el código bien documentado y estructurado de acuerdo con las mejores prácticas.

====


C. Browse
~~~~~~~~~

Este botón permite al usuario cargar (*upload*) un archivo tipo texto no formateado (ASCII), con un código *YAML* previamente creado por el usuario. El usuario debe hacer clic sobre el botón ``Browse``, en esta acción la plataforma Mangue.io presenta la pantalla del “Explorador de Archivos” (*File Explorer*) de su ordenador, a continuación, debe seleccionar el *folder*/directorio donde se ubica el archivo de su código.

La plataforma Mangue.io está configurada para identificar y mostrar todos los archivos con extensión "*.yaml y *.yml" presentes en el *folder*/directorio seleccionado. En caso de que el usuario haya guardado su código fuente en un archivo con extensión diferente, éste debe introducir el nombre completo del archivo en el campo "Nombre" o seleccionar la opción "Todos los archivos (*.*) / *All files* (*.*)" para localizar y seleccionar el archivo deseado.

.. image:: /figuras/fig_mangue/071_mangue_arquivo_yaml.png
    :alt: Localizar e selecionar arquivo
    :align: center
=====

Cuando el usuario seleccionar el archivo deseado, haciendo clic en el botón ``Abrir /  Open`` la plataforma Mangue.io carga el contenido del archivo seleccionado para la interfaz, en este momento el usuario puede ver que la plataforma Mangue.io numera, secuencialmente, todas las líneas del código cargado.

En este punto el usuario puede editar el código directamente a través de la interfaz de la plataforma de Mangue.io, para personalizar o corregir cualquier línea del código *YAML* presente en la pantalla.

====


D. Submit
~~~~~~~~~

Cuando el usuario haya concluido la inserción de todo el contenido del código *YAML* y se encuentre seguro de que dicho código está correcto, debe pulsar sobre el botón verde ``Submit`` para que la plataforma Mangue.io cargue el código y su consecuente compilación al disponibilizar este código como un *Deployment*, Servicio, *Statefulsets*, Volumen o *Ingress*.

En este momento la plataforma Mangue.io cierra las pantallas de creación de aplicaciones (*Deployment*) entonces el usuario puede encontrar su nueva aplicación listada en el menú *Workloads/Deployments*.

El usuario puede visualizar más informaciones sobre su nueva aplicación en el menú de informaciones del *Deployment*.

====


E. Server VsCode
~~~~~~~~~~~~~~~~

.. image:: /figuras/fig_mangue/072_mangue_add_vscode.png
    :alt: Adicionar Server VS Code
    :align: center
=====

Para crear un Visual Studio Code es necesario hacer clic en el botón de |icone_adicionar| y rellenar los campos a continuación:

* **Nombre del Servidor VS Code**: Nombre del servidor Visual Studio Code a ser creado.
* **Tamaño del Servidor VS Code**: Tamaño del disco a la disposición del *Visual Studio Code*. La medida del tamaño se define en el campo “Tipo de tamaño”.
* **Tipo de Servicio**: El usuario puede seleccionar el tipo de servicio que se asignará al *Deployment* del *Visual Studio Code*. Las opciones disponibles son: *Cluster IP, NodePort, Load Balancer* y *Ingress*.
* **Puerto**: El usuario puede seleccionar el puerto que es utilizado en el servicio.
* **Tipo de Tamaño**: Especifica la unidad de tamaño. Las opciones disponibles son: Gi y Mi.
* **Ingress Class**:  Si el tipo de servicio seleccionado es el *Ingress*, es necesario seleccionar el *Ingress Class* a ser utilizado por el servicio.
* **URL del servidor VS Code**: Si el tipo de servicio seleccionado es el *Ingress*, es necesario especificar el camino de la ruta del *Ingress*. Ejemplo: */vscode*.
* **Activar autenticación**: El usuario puede asignar una contraseña que es necesaria para acceder al servidor *VS Code*.
* **Contraseña del Servidor VS Code**: Contraseña a ser utilizada para acceder al servidor *VS Code*.

====

ConfigMap
=========

En pocas palabras, se puede afirmar que *ConfigMap* es un conjunto de par de clave-valor destinado al almacenamiento de configuraciones, es almacenado dentro de los archivos que se pueden consumir a través de *pods*. Es muy similar con el *Secrets*, pero proporciona una manera de trabajar con *strings* que no tienen datos confidenciales, como contraseñas, claves, *tokens* y otros datos confidenciales.

Los archivos de *configMap*, pueden ser tanto archivos complejos que tienen pocas reglas, como archivos en formato *JSON* complejos y llenos de reglas.

Cabe destacar que un archivo de *configmap* puede contener, sí, el contenido complejo de un *JSON*, bastando al usuario llenar el contenido de este *configMap* obedeciendo la sintaxis correcta de un *JSON*.

Al seleccionar esta opción en la barra del menú, la plataforma Mangue.io presenta la siguiente pantalla, que contiene un listado de todos los *configmaps* registrados en la plataforma.

.. image:: /figuras/fig_mangue/073_mangue_configmaps.png
    :alt: Configmaps
    :align: center
=====

A continuación se describe cada columna de esta tabla:

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|.

    Cuando el usuario elige una línea o varias, la plataforma Mangue.io presenta el/los icono(s) encima de esta columna, estos representan acciones al usuario para ser ejecutadas de una vez para todas las líneas seleccionadas.

    En este caso se presenta un icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los ítems indicados por el usuario con un solo comando.

* **Nombre**: Esta columna es presentado el nombre del *configmap* añadido por el usuario. Al pulsar el ratón sobre el nombre, la plataforma Mangue.io muestra una pantalla con el (los) contenido(s) del (de los) archivos de *configmap*. 

Por defecto, sólo se visualiza una línea del contenido del archivo. Si el contenido es más grande que el campo, el usuario puede posicionar el ratón en la esquina inferior derecha, hasta que el cursor del ratón cambie a una doble flecha diagonal |icone_seta_diagonal|. De esta forma, permite al usuario redimensionar el espacio del contenido listado, y acomodar el tamaño que sea adecuado al usuario, para la mejor visualización del mismo.

.. image:: /figuras/fig_mangue/074_mangue_configmaps_arquivo.png
    :alt: Configmaps arquivo
    :align: center
=====

Importante resaltar que esta ventana no permite la edición del contenido listado.

* **Duración**: En esta columna se muestra el tiempo (en días) desde el momento de la creación del *configmap*.
* **Acciones**: Esta columna muestra el botón de ``Acción`` |icone_acao|, al ser pulsado, presenta dos opciones, como en la figura siguiente:

.. image:: /figuras/fig_mangue/075_mangue_acoes_configmap.png
    :alt: Ações configmap
    :align: center
=====

      * **Deletar Configmap**: Cuando el usuario seleccionar esta opción la plataforma Mangue.io presenta la pantalla abajo solicitando la confirmación de la opción de remoción del *configmap*.

.. image:: /figuras/fig_mangue/076_mangue_deletar_configmap.png
    :alt: Deletar configmap 
    :scale: 80 %
    :align: center
=====

.. note:: Es importante resaltar que esta acción es definitiva y elimina el archivo del sistema operativo, no siendo posible recuperarlo, ya que se borran todas las referencias de este *configmap* en la plataforma Mangue.io. Entonces es necesario recrear el archivo desde el principio.

----

      * **Editar Configmap**: Al seleccionar esta opción la plataforma Mangue.io presenta la siguiente pantalla ubicación en la que el usuario puede efectuar los cambios necesarios en el contenido del (los) archivo (s) de *configMap*:

.. image:: /figuras/fig_mangue/077_mangue_add_configmap.png
    :alt: Adicionar configMap
    :align: center
====

La siguiente imagen es un recorte de los elementos posicionados encima de la tabla, hay tres acciones diferentes y disponibles para el usuario:

.. image:: /figuras/fig_mangue/053.1_mangue_pesquisar_atualização.png
    :alt: Pesquisar atualização
    :align: center
====

* **Acción de búsqueda**: Si la lista que se muestra en esta pantalla es muy larga (ocupando más de una página), existe un campo donde es posible al usuario realizar una búsqueda por el nombre del *ConfigMap* deseado. Basta informar parte del nombre y pulsar ``Enter`` o hacer clic en el icono de "La lupa" |icone_lupa_verde|. Como resultado de esta búsqueda, sólo aparecen los *ConfigMap* que contienen la palabra clave de la búsqueda.

* **Acción de actualizar**: Basta hacer clic en el icono |icone_update| para que el Mangue.io actualice la interfaz con los valores más recientes de esta tabla de *ConfigMap*.

* **Acción de añadir un configMap**: Basta hacer clic en el signo de adición |icone_adicionar| para que el usuario pueda registrar un nuevo ConfigMap. La plataforma Mangue.io presenta la siguiente pantalla al usuario: 

.. image:: /figuras/fig_mangue/079_mangue_add_configmap.png
    :alt: Adicionar configmap 
    :scale: 100 %
    :align: center
=====

A continuación se describen los campos de la pantalla anterior:

* **Nombre del configmap**: En este campo el usuario debe escribir el nombre del *configmap* deseado, a continuación pulsar sobre el icono del signo de suma |icone_adicionar|, lo que hace que la plataforma Mangue.io añada los siguientes campos.

      * **Archivo “n”**: Cada vez que el usuario hace clic en el signo de adición |icone_adicionar| la plataforma Mangue.io inserta una línea gris con el número secuencial del archivo de *configMap*. Si el usuario necesita eliminar (borrar) el archivo configurado en el icono |icone_lixo_vermelho| sólo tiene que elegir eliminar el archivo "n" del *configMap*.

      * **Nombre del archivo**: En este espacio el usuario debe informar el nombre del archivo que se crea en el sistema operativo de destino que ofrece soporte a la ejecución del *deployment*. Es importante recordar que este nombre, y su extensión, deben seguir las reglas para nombrar archivos en el sistema operativo de destino, por lo que debe contener sólo caracteres ASCII estándar. 

.. attention:: No deben utilizarse letras acentuadas (á, é, í, ã, õ, ç y otras), ya que puede producirse un error en la creación del archivo en el sistema operativo.

----

      * **Contenido del archivo**: En este campo el usuario debe escribir el contenido del archivo nombrado, en el campo anterior; Contenido que debe ser informado según la necesidad técnica y el propósito de este *configmap*. 

      Por defecto se presenta sólo la visualización de algunas líneas del contenido del archivo, en caso de que el contenido sea más grande que el campo, el usuario puede posicionar el ratón en la esquina inferior derecha, hasta que el cursor del ratón cambie a una doble flecha diagonal |icone_seta_diagonal|. De esta forma, permite al usuario redimensionar el espacio del contenido listado y acomodar el tamaño que sea adecuado al usuario, para la mejor visualización del mismo.

* **Botón** ``Añadir Configmap``: Después de que el usuario informe (el/los) archivo(s) de *configmap* necesario(s), el usuario debe hacer clic con el ratón en el botón ``Añadir Configmap``, para que la plataforma Mangue.io pueda crear el/los referido(s) archivo(s) en el ambiente del sistema operativo de destino. Tras esta acción sobre este botón la plataforma cierra esta ventana y vuelve a la pantalla donde se presenta la lista de *Configmaps*.

====

Cluster Events
==============

A través de esta opción de menú, la plataforma Mangue.io presenta todos los eventos que ocurrieron en el *cluster* y *namespace* seleccionados en la pestaña engranajes |icone_engrenagem| "Selección de configuración". A cada selección de contrato/*cluster*/*namespace* la lista de eventos es atualizada automaticamente.

.. image:: /figuras/fig_mangue/080_mangue_cluster_events.png
    :alt: clusters Events
    :align: center
=====

Abajo la descripción del contenido de cada columna de la lista presentada:

* **#**: Número secuencial del evento en la lista presentada.
* **Nombre**: Nombre del evento que la plataforma Mangue.io generó para el *deployment*;
* **Tipo de Evento**: Describe el tipo de evento ocurrido, y se pueden listar los siguientes tipos de eventos:

      * Normal;

      * Warning.

* **Tipo de objeto**: Describe cual objeto configurado en la plataforma Mangue.io originó el evento listado. La identificación del tipo de objeto, permite al usuario identificar este origen, para que éste pueda tener acceso al objeto y actuar en la resolución del evento. Esto puede hacerse mediante la redefinición del objeto o optando por su eliminación. Los tipos de objeto pueden ser los enumerados a continuación:

      * *Deployments*;

      * *Daemonsets*;

      * *Horizontal Autoscaler*;

      * *Pods*;

      * *Statefulsets*;

      * *Updates*;

      * Servicios;

      * *Ingress*;

      * *StorageClass*;

      * *PersistentVolumes*;

      * *PersistentVolumesClaim*;

* **Nombre del Objeto**: Nombre del recurso del evento.

* **Mensaje**: 

      * *Pulled*;

      * *Created*;

      * *Started*;

      * *NoPods*;

      * *FailedGetScale*;

      * *ProvisioningFailed*;

      * *FailedBinding*;

* **Ejecutado hace**: Indica cuánto tiempo hace que se produjo el evento.

La siguiente imagen es un recorte de los elementos posicionados encima de la tabla, hay tres acciones diferentes disponibles para el usuario:

.. image:: /figuras/fig_mangue/081_mangue_pesquisar_evento.png
    :alt: Pesquisar evento
    :align: center
=====

* **Acción de búsqueda**: Si la lista que se muestra en esta pantalla es demasiado larga (ocupando más de una página), existe un campo donde el usuario puede realizar una búsqueda por el nombre del *Deployment* deseado. 

Basta introducir parte del nombre del evento y pulsar ``Enter`` o hacer clic en el icono de "La lupa" |icone_lupa_verde|. 

Como resultado de esta búsqueda, aparecen únicamente los eventos que contienen la palabra clave buscada.
 
* **Acción de actualizar**: Basta hacer clic en el icono |icone_update| para que Mangue.io actualice la interfaz con la lista más reciente de eventos de esta tabla.

====

Cron Jobs, Jobs
===============

En esta opción del menú, el usuario puede observar dos funciones distintas de la plataforma Mangue.io, que son los *Jobs* y los *cron Jobs*. El usuario visualiza la lista de todos los *Jobs* y *cron Jobs*, la lista presenta lo que está programado para el contrato, *cluster* y *namespace* seleccionados en la pestaña |icone_engrenagem| "Selección de Configuración". 

Con cada selección de contrato/*cluster*/*namespace*, la lista se actualiza automáticamente.

====

A. Cron Jobs
------------

Los *Cron Jobs* son útiles para crear tareas (*jobs*) periódicas y recurrentes, como realizar *backups* o enviar correos electrónicos. Los *Cron Jobs* pueden programar tareas individuales a una hora específica, como también, programar un trabajo para cuando el *cluster* probablemente esté inactivo.

La plataforma Mangue.io lista todos los *Cron Jobs* configurados en su ambiente:

.. image:: /figuras/fig_mangue/082_mangue_cronjobs.png
    :alt: Cron Jobs
    :align: center
=====

Abajo la descripción del contenido de cada columna de la lista presentada:

* **#**: Número secuencial del *Cron Job* en la lista presentada.
* **Nombre**: Nombre del *Cron Job* que la plataforma Mangue.io genera para el *deployment*.
* **Schedule**: Muestra la configuración de la programación (fecha y hora) prevista para ejecutar este *Cron Job*.
* **Duración**: Muestra el tiempo de duración del *Cron Job*.
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| cuando se pulsa, aparece la opción de eliminar el *CronJob*, como se muestra en la figura:

.. image:: /figuras/fig_mangue/083_mangue_deletar_cronjobs.png
    :alt: Deletar cron job 
    :scale: 100 %
    :align: center
=====

B. Jobs
-------

Un *Job* crea uno o más *pods* y asegura que un número específico de ellos sea cerrado con éxito. A medida que los *pods* son finalizados con éxito, el *Job* rastrea las conclusiones exitosas. Cuando se alcanza un número especificado de finalizaciones exitosas, la tarea (es decir, el *Job*) está completada. Eliminar un *Job* borra los *pods* creados.

El usuario también puede configurar un *Job* para que sea ejecutado, en paralelo en varios *pods*. 

.. image:: /figuras/fig_mangue/084_mangue_jobs.png
    :alt: Jobs
    :align: center
=====

A continuación se describe el contenido de cada columna de la lista presentada:

* **Nombre**: Nombre del *Job* que la plataforma Mangue.io genera para el *deployment*;
* **Status**: Esta columna presenta tres valores posibles, *"COMPLETED"*, *"IN PROGRESS"* y *"FAILED"*:

      * **COMPLETED**:  *Job* ejecutado con éxito;

      * **IN PROGRESS**: *Job* en ejecución;

      * **FAILED**: *Job* ha fallado en la ejecución.

* **Paralelismo**: Cantidad de *Pods* para la ejecución en paralelo.
* **Conclusiones**: Conclusiones exitosas.
* **Acciones**: Esta columna presenta el botón de ``Acción`` |icone_acao| al ser pulsado, presenta la opción de eliminar el *Job*, como se muestra en la figura:

.. image:: /figuras/fig_mangue/085_mangue_deletar_job.png
    :alt: Deletar Job 
    :scale: 80 %
    :align: center
=====

Facturación
===========

Esta opción de la plataforma Mangue.io es un gran aliada para el Gobierno Financiero de las empresas. Pocas herramientas disponibles actualmente en el mercado presentan los valores reales de consumo de infraestructura computacional para soportar un ambiente *serverless* basado en *containers* (*Kubernetes*).

El término *serverless* puede llevar a la falsa idea de que este ambiente no genera costos de infraestructura computacional, pero cualquier aplicación de *software* siempre necesita un recurso computacional (CPU, memoria, disco, sistema operativo - SO). 

Para que este *software* funcione, cada ítem conlleva sus propios costos de uso, almacenamiento y licencia (SO y *softwares*) y debe ser calculado diariamente para que cumpla con los criterios y políticas de Gobernanza de Costos y Gobernanza Financiera.

La plataforma Mangue.io dispone de una base de datos que acumula los valores de consumo de la infraestructura mes a mes, desde el momento de su instalación. Esta base de datos se calcula diariamente y acumula los valores de consumo, según la fórmula de cálculo presentada en el tópico “Cálculo del Valor de Consumo del Cluster”.

Al seleccionar esta opción del menú, la plataforma Mangue.io muestra la siguiente pantalla:

.. image:: /figuras/fig_mangue/086_mangue_faturamento_cluster.png
    :alt: Histórico faturamento cluster
    :align: center
=====

La plataforma Mangue.io presenta los valores del *cluster* y  *namespace* seleccionados en la pestaña engranajes |icone_engrenagem| “Selección de la configuración". En cada selección de un nuevo contrato/*cluster*/*namespace*, los valores y los gráficos son actualizados automáticamente.

Esta pantalla está dividida en dos secciones diferentes, a continuación se muestran los detalles de cada sección.

====

Informe Consolidado
-------------------

Esta pantalla presenta informaciones sobre el consumo mensual de los *clusters*, el usuario puede visualizar el precio de cada *cluster* en el gráfico circular de la imagen de abajo. Así como es posible ver el consumo por usuario, esto sólo ocurre cuando el *deployment* se crea a través de Mangue.io, ya que se guarda en el *deployment* la información del usuario responsable por su creación.

.. image:: /figuras/fig_mangue/087_mangue_overview_financeiro.png
    :alt: Overview financeiro 
    :scale: 80 %
    :align: center
=====

Al seleccionar un *cluster* las informaciones en la pantalla se recargan de acuerdo con el *cluster* seleccionado, esto incluye tanto los gráficos que informan el precio por *cluster* y el precio por usuario, como la tabla con detalles sobre costos de aplicaciones.

Por norma, la consulta se realiza considerando todos los *namespaces* del *cluster*, pero el usuario puede filtrar por un *namespace* específico haciendo clic en ``Seleccionar un namespace``, las informaciones de la pantalla se recarga como en el ítem anterior, diferenciándose por volver los valores solamente del *namespace* seleccionado.

También en esta pantalla se puede ver una lista de detalles sobre los costes de las aplicaciones, como se puede ver en la siguiente imagen:

.. image:: /figuras/fig_mangue/088_mangue_lista_aplicacoes.png
    :alt: Listando aplicação
    :align: center
=====  

* **Nombre**: Esta columna muestra el nombre del *deployment*, recordando que para que el *deployment* aparezca aquí debe estar en un *cluster* con la taquilla habilitada.

* **Usuario**: Esta columna muestra el usuario responsable por la creación de la aplicación.

* **Namespace**: Esta columna presenta el *namespace* al que pertenece la aplicación.

* **Precio de la CPU**: Esta columna muestra el coste por CPU de la aplicación correspondiente al mes seleccionado.

* **Precio de la memoria**: Esta columna muestra el coste por memoria de la aplicación correspondiente al mes seleccionado.

* **Precio total**: Esta columna presenta la suma del precio de la CPU y del precio de la memoria.

También existe la posibilidad de exportar las informaciones correspondientes a la tabla de arriba, en formato csv, a través de la funcionalidad “*export to csv*” representada por el botón |icone_exportar|, al pulsarlo el usuario puede descargar el archivo inmediatamente después.

====

Historial
---------

La evolución del consumo de los recursos de CPU y memoria del *cluster* se presenta en un formato de gráfico denominado "Histórico de facturación del *cluster*", tal y como se muestra en la siguiente imagen.

.. image:: /figuras/fig_mangue/089_mangue_historico_faturamento.png
    :alt: Histórico faturamento mensal cluster
    :align: center
=====

A. Historial de facturación mensual del Cluster
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta sección muestra un gráfico con la evolución del valor de consumo de recursos de CPU y Memoria del *cluster*, para soportar y ejecutar todos los contenidos del *Workloads* (*Deployments*, *Statefulsets*, *Horizontal Autoscaler*, *Pods*).

El usuario puede seleccionar el periodo para el que desea visualizar los valores seleccionando el mes y el año que aparecen encima del gráfico:

.. image:: /figuras/fig_mangue/090_mangue_mes_ano.png
    :alt: Selecione ano e mês 
    :scale: 80 %
    :align: center
=====

Al hacer clic en el icono del calendario, la plataforma Mangue.io muestra una pantalla de selección anual, en la que el usuario puede elegir el año que desea visualizar:

.. image:: /figuras/fig_mangue/091_mangue_ano.png
    :alt: calendário anual 
    :scale: 80 %
    :align: center
=====

Una vez que se hace clic en el icono del calendario, es posible seleccionar el año deseado en la plataforma Mangue.io, como se muestra en la imagen de la pantalla anterior. A continuación, el usuario puede seleccionar el mes que desea ver y sus valores acumulados:

.. image:: /figuras/fig_mangue/092_mangue_mes.png
    :alt: calendário mensal 
    :scale: 80 %
    :align: center
=====

Tan pronto el usuario selecciona el mes, la plataforma Mangue.io comienza el proceso de búsqueda y cálculo de los valores del mes y el año seleccionados. Este proceso puede llevar unos segundos y el usuario puede seguir la evolución de este procesamiento siguiendo una "línea negra" que aparece desde la izquierda hasta la derecha en la parte superior del navegador de Internet.

En el momento en que la línea rellene completamente la parte superior del área del navegador, la plataforma Mangue.io actualiza el gráfico de la pantalla con los valores diarios del mes y el año seleccionados.

Es importante mencionar que los valores diarios presentados reflejan hasta el día actual, es decir, si el usuario desea consultar los valores del mes, y el mes actual se encuentra (por ejemplo) en la primera quincena, el gráfico representa sólo del día 1 al día 15 del mes actual.

Este gráfico muestra una línea de la evolución del valor de consumo de la infraestructura computacional y puede entenderse como una progresión matemática. Es decir, es el valor de consumo del día anterior sumado al valor de consumo del día actual, y así sucesivamente.

Al principio de cada mes, el valor se "pone a cero" iniciando un nuevo ciclo de cálculo de consumo de la infraestructura computacional para el periodo del mes, hasta el día corriente. De esta manera, el valor del primer día del mes puede no presentarse inmediatamente, porque la plataforma Mangue.io necesita calcular el valor de este día después de las 24 horas del primer día - el valor del día corriente es presentado después de 24 horas. 

La línea del gráfico puede presentar "picos" y "valles" debido a varios factores, por lo que debe tener en cuenta el ambiente en su totalidad. El aumento del consumo puede deberse a la puesta en marcha de Autoescaladores Horizontales, Migraciones, *Updates*, *Cronjobs* creación de nuevas aplicaciones, *deployments*, entre otros.

Todas las situaciones enumeradas anteriormente son causas potenciales del aumento del consumo de infraestructura computacional y de la consiguiente evolución de los valores totales en este gráfico.

====

B. Historial de facturación del Cluster 
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este gráfico presenta el consumo acumulado mes a mes de los últimos cuatro (04) meses del periodo en el que se encuentra el usuario.

.. image:: /figuras/fig_mangue/093_mangue_historico_cluster.png
    :alt: Histórico faturamento cluster
    :align: center
=====

En la figura anterior, se puede ver el ejemplo de cómo la plataforma Mangue.io presenta los valores del consumo de infraestructura del *cluster*. Este gráfico muestra los últimos cuatro meses de consumo.

El valor acumulado del mes actual representa el consumo desde el primer día del mes hasta el día de la consulta; de este modo, si el día actual corresponde a la primera semana del mes, el valor acumulado representa el consumo de la semana. 

Es importante mencionar que la plataforma Mangue.io restablece todos los valores del mes en el primer día de cada mes. Y comienza la suma (progresión matemática) hasta el último día del mes (día 30 o 31 - excepto para el mes de febrero).

El eje vertical muestra los valores máximos redondeados al siguiente valor por encima del máximo en un periodo. Para que el usuario identifique el valor correcto, basta con situar el puntero del ratón sobre la barra del mes deseado, para que la plataforma Mangue.io presente el valor detallado del mes en el que se sitúa el cursor del ratón.

====

C. Por Tags
~~~~~~~~~~~

La plataforma Mangue.io permite que las aplicaciones *Kubernetes* tengan *tags*, compuestas por un conjunto de clave y valor, para agrupar aplicaciones similares, y visualizar su facturación. 

Los *tags* pueden ser creados o asociados a una aplicación durante el proceso de creación de una aplicación, como se demuestra en la sección **"Nueva Aplicación"** en el ítem **Catálogo**, o en una aplicación ya existente, como se demuestra en la sección **"Cambiar Tags"** en el ítem *Deployments*. 

La pantalla de facturación por *tags* está separada en dos secciones:

* Historial de Facturación Mensual por *tags*. 
* Detalles *tags*. 

.. image:: /figuras/fig_mangue/094_mangue_historico_tags.png
    :alt: Histórico de tags
    :align: center
----

En la sección Historial de Facturación Mensual por *tags*, el usuario debe seleccionar primero un *Cluster*, para que la plataforma pueda cargar los *tags* del *Cluster*. A continuación, el usuario puede seleccionar el periodo de facturación deseado y los *tags* que se mostrarán en el gráfico y en la sección Detalles de *tags*.

.. image:: /figuras/fig_mangue/095_mangue_detalhes_tag.png
    :alt: Detalhes tag
    :align: center
=====

En la sección Detalles de *tags*, se mostra una lista de todos los *tags* o de los *tags* seleccionados en la sección Historial de Facturación Mensual por *tags*. En el detallamiento del *tag* se mostra una lista de aplicaciones con el *tag* y un gráfico con la facturación del *tag* en los últimos 30 días.

El usuario puede eliminar un *tag* pulsando el botón de "Papelera" |icone_lixo|, en el Detallamiento del *tag*.

====

D. Alertas
~~~~~~~~~~

A través de las alertas, es posible al usuario ser notificado cuando se alcanza el presupuesto establecido para un *deployment* o conjunto de *deployments*, cuando se agrupan en *tags*. Además de poder configurar las acciones que deben ejecutarse cuando el presupuesto de estos recursos es alcanzado. Esto permite al usuario tener más control sobre el coste de cada servicio. 

Como se muestra en las siguientes imágenes, un card muestra "Alertas" y el otro "*Webhooks*", los detalles de cada un se describen a continuación: 

.. image:: /figuras/fig_mangue/096_mangue_alertas_webhooks.png
    :alt: Alertas e webhooks
    :align: center
=====

* **Alertas**: Presenta una lista de alertas, con las siguientes columnas:

      * **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

        Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

        En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

      * **Nombre**: Esta columna presenta el nombre de la alerta definida en el momento de su creación. Al seleccionar este campo, la pantalla muestra informaciones sobre la alerta, y el usuario puede ver una barra de progreso, *actions* y *webhooks* seleccionados en el momento de la creación. Como se puede ver en la imagen de abajo:

.. image:: /figuras/fig_mangue/097_mangue_alert.png
    :alt: Alerta 
    :scale: 100 %
    :align: center
=====

* **Barra de progreso**: Corresponde al valor actual de los *deployments* asociados a la alerta, teniendo como 100% el valor del presupuesto de la alerta.
* **Actions**: *Action* ejecutada en el momento en que los *deployments* asociados a una alerta alcanzan el precio del presupuesto.
* **Webhooks**: *Webhook* ejecutado en el momento en que los *deployments* asociados a una alerta alcanzan el precio del presupuesto.
* **Aplicación**: Esta columna presenta el *deployment* o conjunto de *deployments* seleccionados para la alerta correspondiente en el momento de la creación de la alerta.
* **Status**: Esta columna presenta dos valores posibles, "*DONE*" y "*PENDING*":

      * **DONE**: Indica que la alerta ha alcanzado el precio del presupuesto y se ha ejecutado, activando los *webhooks* y *actions* configurados.

      * **PENDING**: Indica que la alerta no ha sido ejecutada.

* **Fecha**: Esta columna presenta la fecha de creación de la alerta. 
* **Cuota de la alerta**: Esta columna presenta el precio del presupuesto establecido para la alerta.
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| que, al ser pulsado, presenta una única opción para eliminar la alerta:

.. image:: /figuras/fig_mangue/098_mangue_deletar_alerta.png
    :alt: Deletar alerta 
    :scale: 100 %
    :align: center
=====
	
      * **Eliminar la alerta**:  Cuando el usuario selecciona esta acción, la plataforma Mangue.io solicita la confirmación del usuario para eliminar (borrar) la alerta deseada de la base de datos de la plataforma:

.. image:: /figuras/fig_mangue/099_mangue_aviso_deletar.png
    :alt: Aviso deletar 
    :scale: 100 %
    :align: center
=====

En esta sección de alertas es posible ver el ícono de añadir alerta, como en el siguiente ejemplo |icone_adicionar|, al hacer clic en el botón es presentado un formulario para el usuario con campos que permiten la creación de una alerta, siguiendo un flujo de tres pasos, detalles, *webhook* y *actions*:

* **Detalles**: En esta etapa se solicitan informaciones destinadas específicamente a la alerta:

      * **Nombre**:  Campo correspondiente al nombre de la alerta; 

      * **Descripción**: Campo correspondiente a la descripción de la alerta; 

      * **Tipo**: Hay dos valores posibles para el tipo, por *Tag* para seleccionar un conjunto de *deployments*, y por *Deployment* para seleccionar sólo un *deployment*. Al seleccionar el *Tag* o el *deployment* se realiza una búsqueda del valor del coste total correspondiente al *deployment* o el *Tag* seleccionado, este valor se muestra en el campo "Coste Actual" de la pantalla.

* **Plazo**: En este campo se puede establecer un plazo para la ejecución de la alerta; las alertas con status *pending* no se ejecutan después del plazo establecido para la alerta.
* **Presupuesto**:  En este campo es posible indicar el precio del presupuesto de la alerta, cuando el coste total de la suma de los *deployments* seleccionados alcance el valor indicado la alerta es ejecutada. 

.. note:: El Valor del Presupuesto debe ser mayor que el valor del "Coste Actual".

.. image:: /figuras/fig_mangue/100_mangue_alerta_detalhes.png
    :alt: Alerta detalhes 
    :scale: 100 %
    :align: center
=====

* **Webhook**: En este paso hay una lista de *webhooks*, el usuario puede seleccionar ninguno o varios. Al seleccionar un *webhook* éste es listado abajo para que el usuario informe el tipo de retorno ejecutado, optando por HTTP o E-mail.

.. image:: /figuras/fig_mangue/101_mangue_alerta_webhook.png
    :alt: Alerta webhook 
    :scale: 100 %
    :align: center
=====  

* **Acciones**: En este paso es posible seleccionar una acción a realizar en el momento de la ejecución de la alerta, existen tres valores que el usuario puede seleccionar para la acción, como en el ejemplo de la imagen siguiente:

.. image:: /figuras/fig_mangue/102_mangue_alerta_acoes.png
    :alt: Alerta ações 
    :scale: 90 %
    :align: center
=====

* **Escalamiento de la aplicación**: Esta acción permite al usuario configurar el cambio de la cantidad de réplicas en ejecución de las aplicaciones seleccionadas. Una vez ejecutada la alerta, posibilita reducir/aumentar la cantidad de instancias de una aplicación, conforme al coste actual de la misma. Ejemplo en la siguiente imagen:

.. image:: /figuras/fig_mangue/103_mangue_escalonamento_aplicacao.png
    :alt: Escalonamento aplicação 
    :scale: 100 %
    :align: center
=====

* **Cambiar Request y Limits**: Esta acción permite al usuario cambiar el *Request* y el *Limit* de las aplicaciones seleccionadas, desde el momento en que se ejecuta la alerta. Ejemplo en la siguiente imagen:

.. image:: /figuras/fig_mangue/104_mangue_alterar_request_limit.png
    :alt: Alterar request limit 
    :scale: 100 %
    :align: center
=====

* **Parar la aplicación**: También es posible parar las aplicaciones seleccionadas desde el momento en que se ejecuta la alerta. Para tal, haga clic en ``Confirmar parada de la aplicación``.

.. image:: /figuras/fig_mangue/105_mangue_parar_aplicacao.png
    :alt: Parar aplicação 
    :scale: 100 %
    :align: center
=====

.. note:: Se debe indicar al menos un *webhook* o una acción para permitir la creación de la alerta.

* **Webhooks**: El *webhook* es una forma de envío de informaciones a algún destino cuando ocurre un evento, en este caso cuando los *deployments* relacionados con la alerta alcanzan el precio del presupuesto definido en la creación de la alerta, el *Webhook* dispara las informaciones. El Mangue.io ofrece dos formas de envío de las informaciones, a través del protocolo HTTP, y/o a través del Email.

.. image:: /figuras/fig_mangue/106_mangue_webhooks.png
    :alt: Webhoooks 
    :scale: 100 %
    :align: center
=====

* **# Columna accionable:** Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Esta columna presenta el nombre del webhook definido en el momento de su creación.
* **Método**: Esta columna presenta el método HTTP seleccionado al crear el *webhook*, con los siguientes valores: "*GET*", "*POST*", "*PUT*", "*DELETE*", "*PATCH*".
* **Url**: Esta columna presenta la url de destino para el envío del mensaje.
* **Body**: Esta columna muestra el cuerpo de la petición HTTP;
* **Email**: Esta columna muestra el email de destino para el envío de un mensaje por email.
* **Alertas**: Esta columna presenta una lista de alertas relacionadas con el *Webhook* correspondiente. 
* **Acciones**: Esta columna presenta el botón de ``Acción`` |icone_acao| al ser pulsado, presenta las opciones siguientes:

.. image:: /figuras/fig_mangue/107_mangue_acoes_webhook.png
    :alt: Ações webhook
    :scale: 100 %
    :align: center
=====

      * **Eliminar Webhook**: Cuando el usuario selecciona esta acción, la plataforma Mangue.io solicita la confirmación del usuario para eliminar (borrar) la alerta deseada de la base de datos:

.. image:: /figuras/fig_mangue/108_mangue_deletar_webhook.png
    :alt: Deletar webhook 
    :scale: 100 %
    :align: center
=====

      * **Editar Webhook**: Cuando el usuario selecciona esta acción la plataforma Mangue.io presenta el formulario presente en la imagen de abajo con las informaciones del webhook, para que el usuario pueda editarlas.

.. image:: /figuras/fig_mangue/109_mangue_editar_webhook.png
    :alt: Editar webhook 
    :scale: 100 %
    :align: center
=====

* **Nombre**: El nombre del *webhook* debe ser indicado;
* **Método**: Indica el método para la petición HTTP;
* **URL**: Informa la url para la petición HTTP;
* **Body**: Comunica el *body* para la petición HTTP;
* **Email**: Indica la dirección de correo electrónico para el envío de mensajes;
* **Mensaje**:  En este campo indicar el mensaje que es enviada al Email informado en el campo anterior.

En esta sección de *webhooks* es posible ver el ícono de añadir *webhook*, como en el siguiente ejemplo |icone_adicionar|. 

.. attention:: El formulario de adición del *webhook* es el mismo presentado para editar *webhook*.

====

Recomendaciones
===============

La plataforma Mangue.io puede realizar recomendaciones para optimizar el uso de la CPU y la memoria de las aplicaciones del *Cluster*, con el objetivo de evitar el desperdicio. En Kubernetes se realiza la asignación de recursos a una aplicación utilizando los siguientes conceptos:

* **Request**: Cantidad mínima de recursos asignados a la aplicación. 

    Ejemplo: una aplicación con *memory request* de 256 MB siempre tiene asignada esta cantidad de memoria, aunque la aplicación siempre utilice sólo 20 MB.

* **Limit**: Si la aplicación necesita utilizar más recursos de los especificados en *Request*, el Kubernetes intenta asignar más recursos en el caso de que la máquina no tenga ninguno disponible. 

    Es posible limitar la cantidad de recursos que el Kubernetes intenta asignar a la aplicación utilizando *Limit*. 

    Ejemplo: una aplicación con *request* de 256 MB y *limit* de 512 MB siempre tiene asignados 256 MB, si necesita más memoria se le pueden asignar hasta 512 MB y si no es suficiente la aplicación se queda sin memoria, lo que puede provocar lentitud o inestabilidad en la aplicación.

La plataforma realiza la optimización analizando las métricas históricas de uso de la CPU y la memoria, verificando así si una aplicación tiene asignados más recursos de los necesarios o con recursos no suficientes para mantener la estabilidad.

.. image:: /figuras/fig_mangue/110_mangue_recomendacoes.png
    :alt: Recomendações 
    :scale: 100 %
    :align: center
=====

En la página de recomendaciones se muestra una lista con las aplicaciones en el *Namespace* y *Cluster* actual, y, es posible buscar recomendaciones a través del nombre de la aplicación. 

A continuación describimos la información presente en la tabla de tareas programadas. 

* **#**: Número secuencial de la recomendación registrada en la plataforma Mangue.io.
* **App**: Nombre de la aplicación con la recomendación.
* **CPU Request Actual/Ideal**: Indica el valor actual y recomendado de *CPU Request*. Si no hay ninguna recomendación en esta columna, se muestra “- / -”.
* **CPU Limit Actual/Ideal**: Indica el valor actual y recomendado de *CPU Limit*. Si no hay ninguna recomendación en esta columna, aparece “- / -”.
* **Memory  Request Actual/Ideal**: Indica el valor actual y recomendado de *Memory Request*. Si no hay ninguna recomendación en esta columna, aparece “- / -”.
* **Memory Limit Actual/Ideal**: Indica el valor actual y recomendado del *Memory Limit*. Si no hay ninguna recomendación en esta columna, aparece “- / -”.
* **Acciones**: Esta columna tiene los siguientes elementos: 

      * Botón ``Aplicar``, al ser pulsado presenta los valores recomendados en la aplicación.

      * Botón ``Acción`` |icone_acao| al ser pulsado, presenta la siguiente opción:

.. image:: /figuras/fig_mangue/111_mangue_descartar_recomendacao.png
    :alt: Descartar recomendação 
    :scale: 100 %
    :align: center
=====

* **Descartar recomendación actual**: Al seleccionar la opción de descartar, la recomendación seleccionada es eliminada, y se mostra una recomendación anterior si la tiene.

* **Botón** ``Más sugerencias``: Redirecciona a una página donde se mostra una lista con las recomendaciones generadas anteriormente.

.. image:: /figuras/fig_mangue/112_mangue_historico_recomendacao.png
    :alt: Histórico sugestão recomendação 
    :scale: 100 %
    :align: center
=====

Permisos
========

Todos los puntos descritos en este segmento, se almacenan en la base de datos que soporta la instalación de la plataforma Mangue.io. Esta base de datos, y su contenido, debe ser gestionada y modificada en el prompt del sistema operativo Linux de los servidores (máquinas virtuales) que soportan la infraestructura de la plataforma Mangue.io.

Durante el proceso de implementación estándar de la plataforma Mangue.io, se instala un gestor de base de datos (MariaDB / MySQL) y el contenido de esta base de datos y sus registros relativos a *Clusters*, Permisos, *Billing*, Contratos, *ClusterRole*, *ClusterRoleBinding*, *Service* y *ServiceAccount*, se rellenan durante el proceso de post-instalación del software. 

No es objetivo de este documento describir el proceso de inclusión de nuevos registros en la base de datos de la plataforma Mangue.io, póngase en contacto con el área de soporte Ustore para que pueda acceder al documento “Manual de instalación de Mangue.io” (ver ítem: Contenido estándar de la base de datos).

En las siguientes pantallas se describen cómo la interfaz de la plataforma presenta el contenido de la base de datos a través de la interfaz HTML del Mangue.io.

====

Contrato
--------

A continuación se muestra la pantalla que presenta informaciones sobre el contrato seleccionado en el menú de configuración, se puede ver información sobre el contrato e informaciones sobre los usuarios del contrato.

.. image:: /figuras/fig_mangue/113_mangue_informacoes_contrato_user.png
    :alt: Informações contrato user 
    :scale: 100 %
    :align: center
=====

A. Informaciones del contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Se pueden visualizar los administradores del contrato, el precio por CPU y el precio por memoria definidos para el contrato.

====

B. Informaciones de usuarios
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta sección contiene informaciones sobre los usuarios del contrato y el nivel de permiso de cada uno de ellos. Los permisos por usuario reflejan el nivel de permiso asignado a un usuario en uCloud, siguiendo el ejemplo de la tabla siguiente:

.. image:: /figuras/fig_mangue/114.2_mangue_spa_table.png
    :alt: Tabela uCloud Mangue.io 
    :scale: 100 %
    :align: center
=====

En caso de que haya habido un cambio de permiso en alguno de los usuarios, sea un usuario retirado del contrato, un usuario añadido al contrato, o incluso un cambio de nivel de permiso, existe una rutina para sincronizar los permisos del usuario con uCloud, reflejando dichos cambios en Mangue.io. 

Sin embargo, si el usuario desea sincronizar los permisos de forma inmediata, hay un icone a la derecha  |icone_sync|, al ser pulsado, ejecuta la misma función de sincronización de permisos que sería realizada por la rutina.

A través de la lista de usuarios es posible extraer las siguientes informaciones:

* **Login**: Este campo presenta el login del usuario que fue aprovisionado en la base de datos de la plataforma Mangue.io.
* **Role**: Esta columna presenta el perfil de autorización (*role*) del usuario aprovisionado.
* **Service Account**: Esta columna presenta el *service account* asociado al usuario. 
* **Cluster Role**: Esta columna presenta el *cluster role* asociado al usuario. 
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| al ser pulsado, muestra la siguiente opción:
.. image:: /figuras/fig_mangue/115_mangue_deletar_permissoes.png
    :alt: Deletar permissões 
    :scale: 100 %
    :align: center
=====

* **Eliminar permisos**: Al seleccionar esta acción son eliminados los permisos del usuario correspondiente a la línea seleccionada. La plataforma solicita confirmación para eliminar el permiso del usuario en Mangue.io, según la imagen siguiente:
.. image:: /figuras/fig_mangue/116_mangue_aviso_permissao.png
    :alt: Aviso permissão 
    :scale: 100 %
    :align: center
=====

Roles
-----

El control de acceso basado en funciones/perfil (*Role Based Access Control - RBAC*) es un método para regular el acceso a los recursos informáticos o de red basado en las funciones de los usuarios individuales en su organización.

Un *RBAC role* (permiso/perfil) o *ClusterRole* contiene reglas que representan un conjunto de permisos.

.. note:: Un *role* siempre define permisos en un *namespace* específico; cuando se crea un *role*, se debe especificar el *namespace* al que pertenece.

====

A. Sección: Roles
~~~~~~~~~~~~~~~~~

En esta sección el usuario puede ver la lista de todos los *roles* existentes en el *cluster* que fue seleccionado en la pestaña de engranaje |icone_engrenagem| "Selección de configuración".

.. image:: /figuras/fig_mangue/117_mangue_roles.png
    :alt: Roles 
    :scale: 100 %
    :align: center
=====


* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|.

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: En esta columna es presentado el nombre del *role* añadido por el usuario.

* **Labels**: Labels se utilizan para especificar la identificación de los atributos de los objetos que son significativos, relevantes y que están presentes en la sintaxis *yaml* del *role*.

* **Duración**: Esta columna presenta el tiempo transcurrido en días desde la aplicación inicial de este *role*.

* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| al ser pulsado, presenta dos opciones:

.. image:: /figuras/fig_mangue/118_mangue_acoes_role.png
    :alt: Ações Role 
    :scale: 100 %
    :align: center
=====

      * **Eliminar Role**: Cuando el usuario selecciona esta acción, elimina el *role* del *cluster* que fue seleccionado en la pestaña de engranajes  |icone_engrenagem| “Selección de configuración”. Recuerda que esta acción es irreversible y definitiva. La plataforma Mangue.io solicita la confirmación del usuario para eliminar (borrar) el grupo deseado de la base de datos:

.. image:: /figuras/fig_mangue/119_mangue_deletar_role.png
    :alt: Deletar role 
    :scale: 100 %
    :align: center
=====


Si el usuario ha ejecutado esta acción por error, es necesario registrar el grupo en la base de datos de la plataforma Mangue.io a través de cualquier herramienta SSH; La acción de incluir configuraciones en la base de datos se realiza a través de la línea de comandos en el sistema operativo Linux de la máquina virtual que soporta la ejecución de la plataforma Mangue.io.

      * **Editar Role**: Recomendamos que sólo los usuarios con experiencia en la sintaxis *YAML* realicen cambios en un *role*, ya que codificar (o cambiar) la sintaxis de forma incorrecta puede llevar a la pérdida de acceso a todo el ambiente de *clusters* existentes.

Esta opción abre una pantalla para editar el *role* usando la sintaxis del código *YAML*, como la pantalla de ejemplo de abajo.

.. image:: /figuras/fig_mangue/120_mangue_editar_role.png
    :alt: Editar role 
    :scale: 100 %
    :align: center
=====

El usuario debe empezar haciendo clic con el ratón en la zona gris al lado del número de línea que desea editar, antes de empezar a digitar su código *YAML*. Para cada nueva línea deberá utilizar la tecla ``Enter`` para iniciar una nueva línea, utilizando su propia experiencia de desarrollo para estructurar la sintaxis de su código línea por línea. 

A través de esta opción el usuario puede ingresar (o editar) un código *YAML* para crear, editar el *role* en la plataforma Mangue.io.

Después de editar el *role*, el usuario debe hacer clic en el botón verde ``Enviar`` para que todo el código se envíe y se aplique al *cluster* que fue seleccionado en la pestaña engranajes |icone_engrenagem| "Selección de configuración". 

====

B. Sección: Role Bindings
~~~~~~~~~~~~~~~~~~~~~~~~~

Una vinculación de función/perfil (*rolebinding*) concede los permisos definidos en un *role* a un usuario o conjunto de usuarios. Éste contiene una lista de asuntos (usuarios, grupos o cuentas de servicio) y una referencia al *role* que está siendo concedido. Un *RoleBinding* concede permisos dentro de un *namespace* específico, mientras que un *ClusterRoleBinding* concede ese acceso a todo el *cluster*.

Un *RoleBinding* puede hacer referencia a cualquier papel en el mismo *namespace*. Como alternativa, un *RoleBinding* puede hacer referencia a un *ClusterRole* y vincular un *ClusterRole* al namespace del *RoleBinding*. Si quieres vincular un *ClusterRole* a todos los *namespaces* de su *cluster*, utiliza un *ClusterRoleBinding*.

.. image:: /figuras/fig_mangue/121_mangue_bindings.png
    :alt: Bindings 
    :scale: 100 %
    :align: center
=====

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Esta columna muestra el nombre del *rolebinding* añadido por el usuario. Al pulsar con el ratón sobre el nombre del *configmap* la plataforma Mangue.io muestra una pantalla con el contenido del archivo(s) *configmap*. Por norma se presenta sólo la visualización de una línea del contenido del archivo, si el contenido es más grande que el campo, el usuario puede posicionar el ratón en el rincón inferior derecho, hasta que el trazo del ratón cambie a una doble flecha diagonal |icone_seta_diagonal|, que permite al usuario redimensionar el tamaño del campo de contenido listado, para la mejor visualización de este campo.
* **Labels**: *Labels* se utilizan para especificar la identificación de los atributos del objeto que son significativos y relevantes y están presentes en la sintaxis *YAML* del *role*.
* **Duración**: Esta columna muestra el tiempo transcurrido en días desde el momento de la aplicación inicial de este *rolebinding*.
* **Acciones**: Esta columna presenta el botón ``Acción``  |icone_acao| al ser pulsado, ofrece dos opciones:
.. image:: /figuras/fig_mangue/122_mangue_acoes_bindings.png
    :alt: Ações Bindings 
    :scale: 100 %
    :align: center
=====

      * **Eliminar RoleBinding**: Cuando el usuario selecciona esta acción elimina el *rolebinding* del *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración". Recuerda que esta acción es irreversible y definitiva. La plataforma Mangue.io solicita la confirmación del usuario para eliminar (borrar) el *rolebinding* deseado de la base de datos de la plataforma: 

.. image:: /figuras/fig_mangue/123_mangue_aviso_bindings.png
    :alt: Aviso bindings
    :scale: 100 %
    :align: center
=====

En el caso de que el usuario haya ejecutado esta acción por error, es necesario registrar el *rolebinding* en la base de datos de la plataforma Mangue.io a través de cualquier herramienta SSH. 

La acción de incluir configuraciones en la base de datos se realiza a través de la línea de comandos en el sistema operativo Linux de la máquina virtual que soporta la ejecución de la plataforma Mangue.io.

      * **Editar Rolebinding**: Recomendamos que sólo los usuarios experimentados en la sintaxis *YAML* realicen cambios en un *rolebinding*, ya que codificar (o cambiar) la sintaxis de forma errónea puede provocar la pérdida de acceso a todo el ambiente de los *clusters* existentes.

Esta opción abre una pantalla para editar el *rolebinding* usando la sintaxis del código *YAML*, como el ejemplo de la pantalla de abajo:

.. image:: /figuras/fig_mangue/124_mangue_editar_binding.png
    :alt: Editar bindings 
    :scale: 100 %
    :align: center
=====

El usuario debe iniciar haciendo clic con el ratón en el área gris al lado del número de la línea que desea editar, antes de comenzar a escribir su código *YAML*. 

Para cada nueva línea el usuario debe utilizar la tecla ``Enter`` para iniciar una nueva línea. El usuario debe utilizar su propia experiencia de desarrollo para estructurar la sintaxis de su código línea por línea. 
A través de esta opción el usuario puede ingresar (o editar) con un código *YAML* para crear y editar el *rolebinding* en la plataforma Mangue.io.

Después de editar el *rolebinding*, el usuario debe hacer clic en el botón verde ``Enviar`` para que todo el código sea enviado y aplicado al *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración.

====

Service Accounts
----------------

Cuando un usuario accede al *cluster*, es autentificado por el *APIServer* como una cuenta de usuario específica (actualmente, generalmente es admin, a menos que el administrador del *cluster* haya personalizado su *cluster*). Los procesos en *container* dentro de los PODs también pueden ponerse en contacto con el *APIServer*. Cuando lo hacen, se autentifican como una cuenta de servicio específica (por ejemplo, *default*).

.. image:: /figuras/fig_mangue/125_mangue_service_account.png
    :alt: Service account 
    :scale: 100 %
    :align: center
=====

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Esta columna presenta el nombre del *serviceaccount* añadido por el usuario. 
* **Namespace**: Informa el *namespace* donde el *serviceaccount*  fue creado.
* **Duración**: Esta columna presenta el tiempo transcurrido en días desde el momento de la aplicación inicial de este *serviceaccount*.
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| al ser pulsado, presenta una única opción:

.. image:: /figuras/fig_mangue/125_mangue_deletar_serviceaccount.png
    :alt: Deletar service account 
    :scale: 100 %
    :align: center
=====

* **Eliminar ServiceAccount**: Cuando el usuario selecciona esta acción se elimina el *serviceaccount* del *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración". Cabe recordar que esta acción es irreversible y definitiva. La plataforma Mangue.io solicita la confirmación del usuario para eliminar (borrar) el *serviceaccount* deseado de la base de datos de la plataforma:

.. image:: /figuras/fig_mangue/126_mangue_aviso_service_account.png
    :alt: Aviso Service Account 
    :scale: 100 %
    :align: center
=====

Si el usuario ha ejecutado esta acción por error, es necesario registrar el *serviceaccount* en la base de datos de la plataforma Mangue.io a través de cualquier herramienta SSH. 

La acción de incluir configuraciones en la base de datos se realiza a través de la línea de comandos en el sistema operativo Linux de la máquina virtual que soporta la ejecución de la plataforma Mangue.io.

====

Cluster Role
------------

Un *RBAC role* o *ClusterRole* contiene reglas que representan un conjunto de permisos. 

*ClusterRole*, por otro lado, es un recurso sin espacio de nombres. Los recursos tienen nombres diferentes (*Role* y *ClusterRole*) porque un objeto de *Kubernetes* siempre necesita tener *namespace* o no; no puede ser ambos.

*ClusterRole* tiene varios usos, puedes utilizarlo para:

* Definir los permisos en recursos con *namespace* y ser concedidos dentro de *namespaces* individuales;

* Definir los permisos en recursos con *namespace* y ser concedido en todos los *namespaces*;

* Definir permisos en recursos con cobertura de *cluster*;

Si deseas definir una función en un *namespace*, utiliza un *role*; si quieres definir un *role* en todo el *cluster*, utiliza un *ClusterRole*.

El usuario puede notar que esta pantalla tiene varias secciones, cada una de las cuales se describe a continuación respectivamente.

====

A. Sección: Cluster Roles
~~~~~~~~~~~~~~~~~~~~~~~~~

En esta pantalla la plataforma Mangue.io presenta la lista de todos los *Cluster Roles* configurados y el tiempo transcurrido desde su creación.

.. image:: /figuras/fig_mangue/127_mangue_cluster_role.png
    :alt: Cluster role 
    :scale: 100 %
    :align: center
=====


* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Esta columna presenta el nombre del *Cluster Role* añadido por el usuario;
* **Labels**: *Labels* son utilizados para especificar la identificación de los atributos del objeto que son significativos, relevantes y que están presentes en la sintaxis *yaml* del *role*.
* **Duración**: Esta columna presenta el tiempo transcurrido en días desde la aplicación inicial de este *Cluster Role*.
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| al ser pulsado, muestra una única opción: 

.. image:: /figuras/fig_mangue/128_mangue_editar_clusterole.png
    :alt: Editar cluster role 
    :scale: 100 %
    :align: center
=====

* **Editar Cluster Role**: Recomendamos que sólo los usuarios con experiencia en sintaxis *YAML* realicen cambios en un *Cluster Role*, ya que codificar (o cambiar) la sintaxis de forma incorrecta puede llevar a la pérdida de acceso a todo el ambiente de *clusters* existentes.

Esta opción abre una pantalla de edición de *Cluster Role* utilizando la sintaxis del código *YAML*, como la pantalla de ejemplo que se muestra a continuación. 

El código de un *Cluster Role* puede ser largo, y esta pantalla puede ser muy larga, presentamos aquí sólo algunas líneas de la pantalla.

.. image:: /figuras/fig_mangue/129_mangue_editar_clusterrole.png
    :alt: Editar cluster role 
    :scale: 100 %
    :align: center
=====


Haciendo clic con el ratón en la zona gris junto al número de línea que el usuario desea editar, puede empezar a escribir su código *YAML*. 

En cada nueva línea, el usuario debe pulsar ``Enter`` para abrir otra línea. 

Se aconseja que el usuario utilice su propia experiencia de desarrollo para estructurar la sintaxis de su código línea por línea. 

En resumen, *Cluster Role* proporciona la opción de crear o editar el código *YAML* en la plataforma Mangue.io.

Después de editar el *Cluster Role* el usuario debe hacer clic en el botón verde ``Enviar`` para que todo el código sea enviado y aplicado al *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración". 

====

B. Sección: Cluster Role Binding
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

En esta pantalla la plataforma Mangue.io presenta la lista de todos los *Cluster Role Binding* configurados y el tiempo transcurrido desde su creación.

.. image:: /figuras/fig_mangue/130_mangue_cluster_role_binding.png
    :alt: Cluster role binding 
    :scale: 100 %
    :align: center
=====

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Esta columna presenta el nombre del *Cluster Role Binding* añadido por el usuario.
* **Labels**: *Labels* son utilizados para especificar la identificación de los atributos de los objetos que son significativos y relevantes y que están presentes en la sintaxis *YAML* del *role*.
* **Duración**:  Esta columna presenta el tiempo transcurrido en días desde el momento de la aplicación inicial de este *Cluster Role Binding*.
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| al ser pulsado, muestra una única opción: 

.. image:: /figuras/fig_mangue/131_mangue_editar_cluster_role_binding.png
    :alt: Editar cluster role binding 
    :scale: 100 %
    :align: center
=====

      * **Editar Cluster Role Binding**: Recomendamos que sólo los usuarios con experiencia en la sintaxis *YAML* realicen cambios en un *Cluster Role Binding*, ya que codificar (o cambiar) la sintaxis de forma incorrecta puede provocar la pérdida de acceso a todo el ambiente de *clusters* existentes.

Esta opción abre una pantalla de edición del *Cluster Role Binding* utilizando la sintaxis del código *YAML*, como el ejemplo de la pantalla de abajo.

.. image:: /figuras/fig_mangue/132_mangue_editar_clusterrolebinding.png
    :alt: Editar cluster rolebinding
    :scale: 100 %
    :align: center
=====


El usuario debe iniciar haciendo clic con el ratón en el área gris al lado del número de la línea que desea editar, antes de comenzar a escribir su código *YAML*. 

Para cada nueva línea el usuario debe utilizar la tecla ``Enter`` para iniciar una nueva línea. El usuario debe utilizar su propia experiencia de desarrollo para estructurar la sintaxis de su código línea por línea.

A través de esta opción el usuario puede ingresar (o editar) un código *YAML* para crear, editar el *Cluster Role Binding* en la plataforma Mangue.io.

Después de editar el *Cluster Role Binding* el usuario debe hacer clic en el botón verde ``Enviar`` para que todo el código sea enviado y aplicado al *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración".

====

C. Sección: Pod Security Policy
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

*Pod Security Policy* es un recurso *Kubernetes* que permite al usuario limitar las aplicaciones creadas por un *ServiceAccount* específico, o todos. Esto permite, por ejemplo, prohibir a un *ServiceAccount* crear una aplicación que utilice el usuário *root*.

La pantalla *Pod Security Policy* se divide en dos secciones: 

* *Pod Security Policy*.
* *Cluster Role* y *Role Binding* del *Pod Security Policy*.

.. image:: /figuras/fig_mangue/133_mangue_pod_clusterrole_binding.png
    :alt: Pod cluster role binding
    :scale: 100 %
    :align: center
=====

En la sección *Pod Security Policy* aparece una lista de los *Pod Security Policy* del *cluster* y se muestra una barra de búsqueda para buscar utilizando el nombre.

A continuación describimos las informaciones presentes en la tabla del *Pod Security Policy*.

* **#**: Número secuencial del *Pod Security Policy* registrado en la plataforma Mangue.io;
* **Nombre**: Nombre del *Pod Security Policy* especificado por el usuario durante la creación;
* **Privilegiado**: Permite que las aplicaciones creadas utilicen los recursos y capacidades *Kernel* de la máquina *Host*;
* **Permite escalada de privilegios**: Permite que la aplicación creada cambie su ID de usuario, permitiendo que los procesos hijos del *container* obtengan más privilegios que el proceso padre;
* **ID de usuario**: Rango de ID de usuario que las aplicaciones creadas pueden utilizar en la ejecución;
* **ID de grupo**: Rango de ID de grupo que las aplicaciones creadas utilizan en la ejecución;
* **ID de archivo del sistema**: Rango de ID de archivo del sistema que las aplicaciones creadas utilizan en la ejecución;
* **Acciones**: Esta columna presenta el botón de ``Acción`` |icone_acao| al ser pulsado, muestra dos opciones: 

.. image:: /figuras/fig_mangue/134_mangue_acoes_security.png
    :alt: Ações security
    :scale: 100 %
    :align: center
=====

      * **Crear Cluster Role**: Al seleccionar la opción de crear *cluster role*, se presenta la pantalla de abajo, a través de la cual el usuario puede crear un *Cluster Role* para *Pod Security Policy*.

      * **Eliminar Pod Security Policy**: Seleccionando la opción de eliminar, se elimina el *Pod Security Policy* del *Cluster*.

.. image:: /figuras/fig_mangue/135_mangue_adicionar_security.png
    :alt: Adicionar cluster role
    :scale: 100 %
    :align: center
=====

Para crear un *Pod Security Policy* es necesario hacer clic en el botón ``Añadir``  |icone_adicionar|, realizada la acción se mostra la pantalla siguiente:

.. image:: /figuras/fig_mangue/136_mangue_adicionar_pod_security.png
    :alt: Adicionar pod security 
    :scale: 100 %
    :align: center
=====

Los campos necesarios para la creación de *Pod Security Policy* son los siguientes:

* **Nombre del Pod Security Policy**: Nombre del *Pod Security Policy* a ser creado.

* **Permitir Containers Privilegiados**: Permite la creación de recursos que utilizan *containers* privilegiados, estos *containers* pueden tener acceso a los recursos y capacidades del *Kernel* de la máquina *Host*.

* **Permitir escalada de privilegios**: Permite que la aplicación creada cambie el ID de usuario, permitiendo que los procesos hijos del *container* obtengan más privilegios que el proceso padre.

* **Limitar usuario**: En caso de ser seleccionado, se muestra una lista (*drop-down list*), con las opciones de: 

      * **Prohibir Root**: Esta opción permite la creación de aplicación que utilice cualquier ID de usuario, con la excepción del ID de usuario *root*.

      * **Limitar por ID de usuario**: Esta opción limita la creación de la aplicación para que utilice un rango de ID de usuario especificado.

* **Limitar Grupo**: Permite sólo las aplicaciones que utilizan el rango de ID de grupo especificado.
* **Limitar archivo de sistema**: Permite sólo las aplicaciones que utilicen el rango de ID de archivo de sistema especificado.

Después de rellenar todos los campos obligatorios, el botón ``Añadir Pod Security Policy`` está disponible y cuando el usuario haga clic en él, la plataforma crea el *Pod Security Policy* y exhibe un mensaje de *status*.

En la sección de *Cluster Role* y *Role Binding* de *Pod Security Policy* se muestra una lista con los *Cluster Role* y *Role Bindings* del *Pod Security Policy* y se muestra una barra de búsqueda para buscar utilizando el nombre de los recursos.

A continuación se describe la información presente en la tabla de *Pod Security Policy*.

* **#**: Número secuencial del *Cluster Role* registrado en la plataforma Mangue.io.
* **Cluster Role**: Nombre del *Cluster Role* especificado por el usuario durante la creación.
* **Pod Security Policy**: Nombre del *Pod Security Policy* asociado al *Cluster Role*.
* **Permite escalada de privilegios**: Permite que la aplicación creada cambie el ID de usuario, permitiendo que los procesos hijos del *container* obtengan más privilegios que el proceso padre.
* **Role Binding**: Nombre del *Role Binding* asociado al *Cluster Role*.
* **Acciones**: Esta columna presenta el botón de ``Acción`` |icone_acao| al ser pulsado, presenta dos opciones: 

.. image:: /figuras/fig_mangue/137_mangue_acoes_role.png
    :alt: Ações role
    :scale: 100 %
    :align: center
=====

* **Crear Role Binding**: Al seleccionar la opción de crear *Cluster Role*, se presenta la pantalla de abajo, a través de la cual el usuario puede crear un *Role Binding* asociando el *Cluster Role* a *ServiceAccounts*;
* **Eliminar Role Binding**: En caso de tener un *Role Binding* asociado al *Cluster Role*, se muestra la opción de eliminar el *Role Binding*, al seleccionar la opción el *Role Binding* es eliminado.
* **Eliminar Cluster Role**: Al seleccionar la opción de eliminar, se borra el *Cluster Role* seleccionado.

.. image:: /figuras/fig_mangue/138_mangue_add_rolebinding.png
    :alt: Adicionar role binding
    :scale: 100 %
    :align: center
=====

Integraciones
=============

A través del menú **Integraciones**, el usuario puede conectar la plataforma Mangue.io con entidades, servicios y proveedores externos. 

Estas integraciones permiten al usuario ampliar el alcance de la plataforma Mangue.io mediante la conexión e integración de la infraestructura actual, que soporta y ejecuta la instalación de Mangue.io con gestores de *containers* en proveedores públicos. 

Este menú viene con el propósito de abordar otras cuestiones más allá de la simple gestión de *Kubernetes*, tales como:

* Integración a través de la línea de comandos en los *containers* que se ejecutan en el *cluster*;
* Creación de *Clusters Kubernetes* en las nubes públicas de AWS y Google; 
* Importar *Clusters Kubernetes* ya existentes;
* Importar credenciales para que los procedimientos de creación de *Clusters* en nubes públicas se realicen más fácilmente;
* Creación de *Clusters* *on premise*.

====

Clusters
--------

El menú Integraciones/*Clusters* permite al usuario integrar la plataforma Mangue.io a un *cluster* existente, que puede estar activo en otra infraestructura computacional, a la plataforma Mangue.io. Además esta pantalla presenta una lista con las informaciones de los *clusters* integrados al Mangue.io.

El menú Integraciones/*Clusters* permite realizar toda la gestión e integración de los *Clusters Kubernetes* gestionados por la plataforma desde un usuario. En este menú es posible aprovisionar *Clusters Kubernetes* en infraestructuras de Amazon y Google (EKS y GKE), recordando que para aprovisionar estos *clusters* es necesario añadir una credencial en el menú Integraciones/Credenciales.  

También es posible añadir un *Cluster Kubernetes* que no haya sido aprovisionado en la plataforma, ya sea en su ambiente *On Premise* o en la nube. Es importante destacar que los *clusters* que han modificado las APIs de *Kubernetes* pueden no responder positivamente a las llamadas APIS de *Kubernetes* realizadas por Mangue.io.

.. image:: /figuras/fig_mangue/139_mangue_integracao_clusters_kubernetes.png
    :alt: Integrações clusters kubernetes
    :scale: 100 %
    :align: center
=====

En la lista se puede encontrar la información de cada *Cluster* configurado e integrado a la plataforma Mangue.io:

* **Nombre**: Esta columna muestra el nombre utilizado para identificar el *Cluster* durante el proceso de configuración por parte del usuario.
* **IP pública**: Esta columna presenta la información de la dirección TCP-IP pública del *Cluster*. Esta es la dirección por la cual el *Cluster* puede ser utilizado para acceder a las aplicaciones (*deployments*) que se están ejecutando en este *Cluster*.
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| al ser pulsado, presenta una única opción:

.. image:: /figuras/fig_mangue/140_mangue_acoes_cluster.png
    :alt: Ações cluster
    :scale: 100 %
    :align: center
=====


      * **Editar Cluster**: En esta opción el usuario puede editar las características de un *Cluster* existente y cuando se selecciona la plataforma presenta la pantalla siguiente:

.. image:: /figuras/fig_mangue/141_mangue_editar_cluster.png
    :alt: Editar cluster
    :scale: 100 %
    :align: center
=====

* **Nombre del cluster**: En este campo el usuario puede cambiar el nombre de referencia con el cual el *cluster* está configurado.

* **IP para acceso a la API**: En este campo el usuario puede cambiar la dirección TCP-IP pública para poder acceder al *cluster*.

* **Puerto para el acceso a la API**: En este campo el usuario puede cambiar el PUERTO TCP-IP para poder acceder al *cluster*.

* **Cluster Admin Token**: En este campo el usuario puede cambiar la cadena de caracteres (*string*) que fue generado por el proveedor público con el fin de confirmar y autenticar la identidad (*token*) de la configuración con el *cluster*. En caso de que sea necesario cambiar esta cadena de caracteres, es importante consultar el proceso de generación de identificación (*token*) de cada proveedor, o de cada entorno de gestión de *container*, específicamente.

* **Confirmar**:  El usuario debe pulsar este botón después de confirmar todos los campos modificados.

* **Eliminar Cluster**: Cuando el usuario selecciona esta acción elimina el *cluster*. La plataforma Mangue.io solicita la confirmación del usuario para eliminar (borrar) el *cluster* de la plataforma:

.. image:: /figuras/fig_mangue/142_mangue_aviso_cluster.png
    :alt: Aviso cluster
    :scale: 100 %
    :align: center
=====

En el caso de que el usuario haya ejecutado esta acción por error, será necesario volver a incluir el *cluster* en la plataforma Mangue.io. Observe la secuencia de inclusión de un nuevo *cluster* que se describe en este documento a continuación.

La plataforma Mangue.io permite al usuario integrarse con la infraestructura del *cluster* existente, como también implementar o crear un nuevo *cluster*.

A continuación se describe el proceso de integración, que permite al usuario añadir un *cluster* existente o nuevo a la plataforma Mangue.io.

====

Integrar Cluster
----------------

Para iniciar el proceso de Integrar un *Cluster* el usuario debe hacer clic con el ratón en el botón de la izquierda para que la pantalla muestre los campos específicos.

.. image:: /figuras/fig_mangue/143_mangue_cluster_existente.png
    :alt: Integrar cluster existente
    :scale: 100 %
    :align: center
=====

* **Nombre del Cluster**: En este campo el usuario debe informar el nombre de referencia con el que es identificado el *cluster* en la plataforma Mangue.io.

* **Contrato**: Este campo es una lista (*dropdown list*) con los contratos del usuario, al seleccionarlo, el Cluster es asociado al contrato seleccionado.

* **Tipo de Cluster**: Este campo es una lista (*dropdown list*) con las cuatro opciones disponibles en la plataforma Mangue.io. Actualmente están disponibles los ambientes públicos: *Google Kubernetes Engine* (GKE), *Amazon Elastic Kubernetes System* (EKS), *Azure Kubernetes Service* (AKS) e *IBM Cloud* (IKS). Cuando seleccionada cada una de las opciones de destino, la plataforma Mangue.io se comporta de la manera adecuada para comunicarse y gestionar el *cluster* correctamente.

* **IP para el acceso a la API**: En este campo el usuario debe informar la dirección TCP-IP pública para que se pueda acceder al *cluster*.

* **Path de acceso a la API**: En este campo el usuario debe informar la ruta utilizada para acceder a la API de *Kubernetes*, en caso de existir.

* **Puerto de acceso a la API**: En este campo el usuario debe informar el número del PUERTO TCP-IP para poder acceder al *cluster*.

* **Cluster Admin Token**: En este campo el usuario debe informar la cadena de caracteres (*string*) que fue generada por el proveedor público del *cluster* con el objetivo de verificar y autenticar la identidad (*token*) de la configuración con el *cluster*. Es importante consultar el proceso de generación de identificación (*token*) de cada proveedor, o de cada ambiente de gestión de *container*, específicamente.

* **Botón** ``Integrar``: Al terminar de rellenar los campos de arriba, el usuario debe hacer clic con el ratón en el botón de ``Integrar`` para que la plataforma Mangue.io incluya este *cluster* en la lista presentada en esta pantalla.
      * **Acción de actualización**: Si la interfaz de Mangue.io no muestra el *cluster* recientemente configurado, el usuario debe hacer clic en el icono  |icone_update| para que la aplicación muestre la lista actualizada de esta tabla de *clusters*.

====

Integrar Múltiplos Clusters
---------------------------

.. image:: /figuras/fig_mangue/144_mangue_multiplos_clusters.png
    :alt: Multiplos clusters 
    :scale: 100 %
    :align: center
=====

Para iniciar el proceso de Integrar Múltiples *Clusters* el usuario debe hacer clic con el ratón en el botón de la derecha para que la pantalla muestre los campos específicos.

En esta pantalla el usuario puede integrar varios *Clusters* existentes en proveedores de nube pública. Debe seleccionar los que desea buscar, luego se mostrarán los campos: 

* **Contrato**: Este campo es una lista (*dropdown list*) con los contratos del usuario, cuando se selecciona, la plataforma carga las credenciales del contrato seleccionado.
* **Credencial**: El usuario debe seleccionar una de las credenciales de acceso registradas en la plataforma Mangue.io para confirmar la identidad del usuario con el ambiente contratado con la nube pública. Después de rellenar todos los campos, el usuario debe pulsar el botón ``Buscar`` y la plataforma mostra una lista (*dropdown list*) de los *Clusters* ya existentes en las plataformas seleccionadas. El usuario debe seleccionar los *Clusters* que desea integrar en la plataforma, después de haberlos seleccionado, el botón ``Integrar`` está disponible para ser pulsado.

====

Crear Cluster on Premise
------------------------

.. image:: /figuras/fig_mangue/145_mangue_cluster_premise.png
    :alt: Cluster on premise
    :scale: 100 %
    :align: center
=====

A través del botón ``Crear Cluster`` es posible crear un *cluster on premise*, donde el usuario puede informar el ip, usuario, contraseña y el tipo (*Master, worker*) de cada una de las máquinas que en conjunto forman el *cluster kubernetes*. El usuario debe rellenar informaciones como:

* **Nombre del cluster**: En este campo el usuario debe informar el nombre de referencia con el que se identifica el *cluster* en la plataforma Mangue.io.
* **Contrato**: Este campo es una lista (*dropdown list*) con los contratos del usuario, al seleccionarlo, el *Cluster* se asocia al contrato seleccionado.
* **IP de la máquina**: Dirección IP de la máquina que interesa incluir en el momento de crear el *cluster*.
* **Tipo da la máquina**: Determina el tipo de máquina, puede ser *worker* o *master*:

      * **Worker**: Son máquinas responsables por recibir las tareas asignadas por por el *node master*, ejecutarlas y reportar el *status* de vuelta al *node master*, por lo tanto, son las máquinas que ejecutan los *containers* *docker* que contienen las aplicaciones.

      * **Master**: El *node master* es considerado el cerebro del *cluster* *kubernetes*, ya que es el responsable de gestionar y controlar los *nodes workers*, tomando decisiones sobre dónde y cómo ejecutar las aplicaciones.

* **Usuario**: Usuario necesario para conectar a la máquina indicada en el campo IP.
* **Contraseña**: Contraseña necesaria para acceder con el usuario e ip informados en los campos anteriores.
* **ETCD**: Este es un campo *checkbox* que si habilitado, la máquina también funciona como ETCD. Si ninguna de las máquinas indicadas tiene ETCD habilitado, entonces por norma la máquina de node master también funciona como ETCD.

Es necesario disponer de al menos dos máquinas para crear un *cluster* con éxito. Las máquinas necesitan acceso a Internet. También se recomienda un mínimo de 2 CPU por nodo, 4 GB de memoria por nodo y 80 GB de almacenamiento por nodo.

Al pulsar en ``Crear``, se muestra una pantalla con la consola del proceso de creación del *cluster on premise*, como se muestra en la siguiente imagen:

.. image:: /figuras/fig_mangue/146_mangue_log_cluster.png
    :alt: Log cluster
    :scale: 100 %
    :align: center
====

Proceso simplificado de integración de cluster mediante formulario
------------------------------------------------------------------

La plataforma Mangue.io permite simplificar el proceso de integración con un *cluster* existente en proveedores de nube pública (*Amazon*, *Google*, *Azure* e *IBM*) a través de un formulario que direcciona al usuario a rellenar credenciales y configuraciones de forma muy clara y sencilla.

En la siguiente pantalla el usuario puede ver que debajo de cada logotipo de proveedor de servicios públicos hay un botón que muestra el formulario respectivo de cada proveedor:

.. image:: /figuras/fig_mangue/147_mangue_cirar_integrar.png
    :alt: Criar integrar cluster
    :scale: 100 %
    :align: center
=====

En las pantallas siguientes aclaramos las características del formulario específico para cada proveedor.

====

A. Google Kubernetes Engine - GKE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para realizar una integración (a través de un formulario) con un gestor de *container* existente en el proveedor Google, el usuario debe hacer clic con el cursor del ratón en la zona gris debajo del logo de **Google Kubernetes Engine** y la plataforma Mangue.io presenta la pantalla de abajo con el formulario GKE:

.. image:: /figuras/fig_mangue/148_mangue_google_info.png
    :alt: Google info
    :scale: 100 %
    :align: center
=====

* **Contrato**: El usuario selecciona el contrato para que la plataforma cargue las credenciales de este contrato.
* **Nombre del Cluster**: El usuario debe rellenar con el nombre de identificación del *cluster* para la plataforma Mangue.io.
* **Credenciales GKE**: El usuario debe seleccionar una de las credenciales de acceso registradas en la plataforma Mangue.io para confirmar su identidad con el ambiente contratado con *Google Cloud Platform*. Es importante tener en cuenta que se debe consultar la documentación específica de cada proveedor sobre cómo generar/crear estas credenciales con permiso del ambiente de gestión de *containers* del proveedor.
* **Número de nodes (por zona)**: En este campo el usuario debe informar un número entero, que definirá la cantidad de nodos (*nodes*) deseados para este *cluster*.
* **Región**: En este campo el usuario debe seleccionar de una lista (*dropdown*) las regiones disponibles en el proveedor específico. En este caso, sólo aparecerán las regiones globales específicas de *Google Cloud Platform*.
* **Tipo de Máquina**: En este campo el usuario debe seleccionar de una lista (*drop-down*) el tipo de configuración de máquina (CPU, Memoria, Disco o *Template*) disponibles en el proveedor. En este caso, sólo aparecerán los *templates* específicos de *Google Cloud Platform*.
* **Versión Principal**: En este campo el usuario selecciona la versión de *Kubernetes* disponible en el proveedor de la nube pública.
* **Crear Cluster**: Basta el usuario hacer clic en el botón ``Crear Cluster``, cuando todas las configuraciones referidas a todos los nodos (*nodes*) hayan finalizado. Para que la plataforma Mangue.io pueda añadir un nuevo *cluster* a la infraestructura interna hay que inicializar este nuevo *cluster* al ambiente computacional que es ejecutado como otro ambiente de gestión de *containers* (*cluster*).

      * **Acción de Actualizar**: La creación del *Cluster* depende del proveedor de la nube pública, el estado de la creación del *Cluster* puede ser seguido en Tareas.

====

B. Elastic Kubernetes Service - Amazon EKS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para realizar una integración (vía formulario) con un gestor de *containers* existente en el proveedor *Amazon AWS*, el usuario debe hacer clic con el cursor en la zona gris debajo del logo de *Elastic Kubernetes Service - Amazon EKS* y la plataforma Mangue.io presenta la pantalla de abajo con el formulario EKS:

.. image:: /figuras/fig_mangue/149_mangue_amazon_info.png
    :alt: Amazon info
    :scale: 100 %
    :align: center
=====

* **Contrato**: El usuario selecciona el contrato para que la plataforma cargue sus credenciales.
* **Nombre del Cluster**: El usuario debe rellenar este campo con el nombre de identificación del *cluster* para la plataforma Mangue.io.
* **Credencial**: El usuario debe seleccionar una de las credenciales de acceso registradas en la plataforma Mangue.io para confirmar su identidad con el ambiente contratado con *Amazon Web Services - AWS*. Es importante tener en cuenta que se debe consultar la documentación específica de cada proveedor sobre cómo generar/crear estas credenciales con permiso del ambiente de gestión de *containers* del proveedor;
* **Región**: En este campo el usuario debe seleccionar de una lista (*dropdown*) las regiones disponibles en el proveedor específico. En este caso, sólo apareceren las regiones globales específicas de *Amazon Web Services - AWS*.
* **Versión de Kubernetes**: En este campo el usuario selecciona la versión de *Kubernetes* disponible en el proveedor de la nube pública.
* **Template de la Máquina**: En este campo el usuario debe seleccionar de una lista (*dropdown*) el tipo de configuración de la máquina (CPU, Memoria, Disco o *Template*) disponibles en el proveedor. En este caso, sólo aparecen los *templates* específicos de *AWS*.
* **Cantidad de Nodos**: En este campo el usuario debe informar un número entero, necesario para la cantidad de nodos para la infraestructura del *cluster*.
* **Botón** ``Confirmar``: Basta el usuario hacer clic en el botón ``Confirmar``, cuando todas las configuraciones referidas a todos los nodos (*nodes*) estén terminadas, para que la plataforma Mangue.io añada un nuevo *cluster* a la infraestructura interna de la plataforma Mangue.io, inicializando este nuevo *cluster* al ambiente computacional que es ejecutado como otro ambiente de gestión de *containers* (*cluster*).

      * **Acción de actualizar**: La creación del *Cluster* depende del proveedor de la nube pública, el estado de la creación del *Cluster* puede ser acompañado en Tareas.

====

C. Azure Kubernetes Service - AKS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para efectuar una integración (a través de un formulario) con un gestor de *containers* existente en el proveedor *Azure*, el usuario debe hacer clic con el cursor en la zona gris debajo del logo *Azure Kubernetes Service - Azure AKS* y la plataforma Mangue.io presenta la pantalla de abajo con el formulario *AKS*:

.. image:: /figuras/fig_mangue/150_mangue_azure_info.png
    :alt: Azure info
    :scale: 100 %
    :align: center
=====

* **Contrato**: El usuario selecciona el contrato para que la plataforma cargue las credenciales de este contrato.
* **Nombre del Cluster**: En este campo el usuario debe rellenar con el nombre de identificación del *cluster* para la plataforma Mangue.io.
* **Credencial**: El usuario debe seleccionar una de las credenciales de acceso registradas en la plataforma Mangue.io para confirmar su identidad ante el ambiente contratado con *Azure*. Es importante tener en cuenta que se debe consultar la documentación específica de cada proveedor para generar/crear estas credenciales con permiso del ambiente de gestión de *containers* del proveedor.
* **Región**: En este campo el usuario debe seleccionar de una lista (*dropdown*) las regiones disponibles en el proveedor específico. En este caso, sólo aparecerán las regiones globales específicas de *Azure*.
* **Versión de Kubernetes**: En este campo el usuario selecciona la versión de *Kubernetes* disponible en el proveedor de la nube pública.
* **Template de la Máquina**: En este campo el usuario debe seleccionar de una lista (*dropdown*) el tipo de configuración de la máquina (CPU, Memoria, Disco o *Template*) disponibles en el proveedor. En este caso, sólo aparecen los templates específicos de *Azure*. 
* **Cantidad de Nodos**: En este campo el usuario debe informar un número entero, necesario para la cantidad de nodos para la infraestructura del *cluster*.
* **Botón** ``Confirmar``: El usuario debe pulsar el botón ``Confirmar`` cuando todas las configuraciones referidas a todos los nodos (*nodes*) estén finalizadas, así la aplicación añade un nuevo *cluster* a la infraestructura interna de la plataforma Mangue.io. Al inicializar este nuevo *cluster* al ambiente computacional que es ejecutado como otro ambiente gestor de *containers* (*cluster*).

      * **Acción de Actualizar**: La creación del *Cluster* depende del proveedor de la nube pública, el estado de la creación del *Cluster* puede ser acompañado en Tareas.

====

D. IBM Cloud
~~~~~~~~~~~~

Para realizar una integración (a través de un formulario) con un gestor de *containers* existente en el proveedor *IBM*, el usuario debe hacer clic con el cursor en la zona gris debajo del logo de *IBM Cloud Kubernetes Service - IBM IKS* y la plataforma Mangue.io presenta la pantalla de abajo con el formulario *IKS*:

.. image:: /figuras/fig_mangue/151_mangue_ibm_info.png
    :alt: IBM info
    :scale: 100 %
    :align: center
=====

* **Contrato**: El usuario selecciona el contrato para que la plataforma cargue las credenciales de este contrato.
* **Nombre del Cluster**: En este campo el usuario debe rellenar con el nombre de identificación del *cluster* para la plataforma Mangue.io.
* **Credencial**: El usuario debe seleccionar una de las credenciales de acceso registradas en la plataforma Mangue.io para confirmar su identidad con el ambiente contratado con *IBM Cloud*. Es importante tener en cuenta que se debe consultar la documentación específica de cada proveedor sobre como generar/crear estas credenciales con permiso al ambiente de gestión de *containers* del proveedor.
* **Región**: En este campo el usuario debe seleccionar de una lista (*dropdown*) las regiones disponibles en el proveedor específico. En este caso, sólo aparecen las regiones globales específicas de *IBM Cloud*.
* **Versión de Kubernetes**: En este campo el usuario selecciona la versión de *Kubernetes* disponible en el proveedor de la nube pública.
* **Template de la Máquina**: En este campo el usuario debe seleccionar de una lista (*dropdown*) el tipo de configuración de la máquina (CPU, Memoria, Disco o *Template*) disponibles en el proveedor. En este caso, sólo apareceren las plantillas específicas de *IBM Cloud*. 
* **Cantidad de Nodos**: En este campo el usuario debe informar un número entero, necesario para la cantidad de nodos para la infraestructura del *cluster*.
* **Botón** ``Confirmar``: El usuario debe pulsar el botón ``Confirmar`` cuando todas las configuraciones referidas a todos los nodos (*nodes*) estén finalizadas, así la aplicación añade un nuevo *cluster* a la infraestructura interna de la plataforma Mangue.io. Al inicializar este nuevo *cluster* al ambiente computacional que es ejecutado como otro ambiente gestor de *containers* (*cluster*).

* **Acción de Actualizar**: La creación del *Cluster* depende del proveedor de la nube pública, el estado de la creación del *Cluster* puede ser acompañado en Tareas.

====

Container Execution
-------------------

El menú Integraciones/*Container Execution* permite configurar una interfaz de comunicación con los *containers* que se están ejecutando en un *POD*. Para que esto sea posible, es necesario proporcionar una credencial para acceder al *cluster Kubernetes*. 

Esta credencial se llama * KubeConfig* - o archivo de configuración del *cluster Kubernetes*. En este archivo de configuración hay informaciones como: Certificados SSL para acceder a la API del *cluster*, la dirección de la API del *cluster*, y algunas otras informaciones descritas en KubeConfig_. 

.. _KubeConfig: https://kubernetes.io/docs/concepts/configuration/organize-cluster-access-kubeconfig/

.. image:: /figuras/fig_mangue/152_mangue_arquivo_config_kubernetes.png
    :alt: Container execution
    :scale: 100 %
    :align: center
=====

.. note:: Es importante tener en cuenta que la dirección TCP-IP informada desde la API del *cluster* debe ser una dirección alcanzable por la infraestructura computacional de la subred donde la plataforma Mangue.io ha sido implantada.

Si ya tiene registrado el *KubeConfig* el usuario puede visualizarlo pulsando sobre el icono |icone_exibir|. También es posible eliminar el *KubeConfig* registrado haciendo clic en el icono de "Papelera" |icone_lixo|.

====

Performance
-----------

La plataforma Mangue.io puede utilizar la API del *Metric Server* para recopilar métricas de *Kubernetes*, pero no solo métricas de rendimiento sobre sus *workloads*, *pods* y *containers*, sino también eventos y nuevos eventos generados por su *cluster*.

Esta pantalla está dividida en dos secciones, que se describen a continuación:

====

A. Sección: Añadir la Supervisión
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

En esta sección, en la parte superior de la pantalla, se presenta un formulario con los campos necesarios para que el usuario los rellene:

.. image:: /figuras/fig_mangue/153_mangue_add_monitoramento.png
    :alt: Add monitoramento
    :scale: 100 %
    :align: center
=====

* **IP de Supervisión**: Este campo es obligatorio, y debe rellenarse con el número de dirección TCP-IP del *Cluster* en el que está instalado el *Metric Server*.
* **Path del Metric Server**: Este campo es obligatorio, y debe ser rellenado con la ruta utilizada por el *Metric Server* en el *Cluster*.
* **Puerto de Supervisión**: Este campo es obligatorio, y debe rellenarse con el número de puerto TCP-IP del *Cluster* en el que está instalado el *Metric Server*.
* **Token**: En este campo el usuario debe utilizar un *Bearer Token* (mencionado en el tópico siguiente) de un *Service Account* con el permiso para realizar consultas en la API del *Metric Server*.
* **Confirmar**: El usuario debe pulsar este botón después de haber verificado todos los campos anteriores y así confirmar la configuración referida al servidor de monitoreo.

====

B. Sección: Monitoreo Disponible
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta sección de la pantalla presenta una lista de todos los servidores que están configurados en el ambiente de la plataforma Mangue.io.

A continuación se describe la información presente en esta lista.

* **#**: Número secuencial del servidor de supervisión registrado en la plataforma Mangue.io.
* **IP de Supervisión**: Esta columna muestra el número de dirección TCP-IP del servidor de supervisión.
* **Puerto de Supervisión**: Esta columna presenta el número de puerto TCP-IP del servidor de monitorización.
* **Bearer Token**: Esta columna muestra una parte del *Bearer Token* utilizado para realizar las consultas en el *Cluster*.
* **Billetaje**: Muestra si el billetaje está activado.
* **Acciones**: Esta columna muestra el botón de ``Acción`` |icone_acao| que al ser pulsado, presenta la figura siguiente:

.. image:: /figuras/fig_mangue/154_mangue_acoes_bilhetagem.png
    :alt: Ações desativar editar deletar
    :scale: 100 %
    :align: center
=====


      * **Activar/Desactivar Billetaje**: Al seleccionar esta opción se activa o desactiva el billetaje del monitoreo.

      * **Editar**: Al seleccionar la opción de editar se presenta la pantalla que aparece a continuación, a través de la cual el usuario puede modificar el contenido de los campos previamente descritos en el ítem “Sección: Añadir Supervisión”. 

.. image:: /figuras/fig_mangue/155_mangue_editar_monitoramento.png
    :alt: Editar monitoramento
    :scale: 100 %
    :align: center
=====

      * **Eliminar Supervisión**: Al seleccionar la opción de eliminar se solicita la confirmación de la acción por parte del usuario, y a continuación se crea un *feedback* de alerta en la esquina superior derecha de la pantalla informando del éxito o del error.

.. image:: /figuras/fig_mangue/156_mangue_aviso_deletar.png
    :alt: Aviso deletar
    :scale: 100 %
    :align: center
=====

Es importante tener en cuenta que esta acción es definitiva y elimina (borra) esta configuración de la plataforma Mangue.io, ya que se borran todas las referencias de este servidor de supervisión en la plataforma.

====

Helm
----

Helm es una herramienta que permite la instalación de aplicaciones *Kubernetes*, funcionando como un gestor de paquetes para el *Kubernetes*, las aplicaciones Helm se definen en los repositorios de aplicaciones Helm. Para utilizar la funcionalidad de es necesario haber registrado previamente el *KubeConfig* del *Cluster* en la plataforma Mangue.io.

.. image:: /figuras/fig_mangue/157_mangue_helm.png
    :alt: Helm
    :scale: 100 %
    :align: center
=====

En la pantalla inicial de la página de Helm, se mostra una tabla con los Helms instalados en la aplicación. Permitiendo al usuario buscar un Helm por su nombre. En la pantalla inicial, el usuario también puede ver los Helms que han sido borrados, lo que permite reinstalarlos de nuevo.

A continuación describimos las informaciones presentes en la tabla de Helms.

* **#**: Número secuencial del Helm registrado en la plataforma Mangue.io.
* **Nombre**: Nombre del Helm especificado por el usuario durante la creación.
* **Fecha de Creación**: Fecha en la que ha sido creada la aplicación Helm en el *Cluster*. 
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| que al ser pulsado, presenta dos opciones:

.. image:: /figuras/fig_mangue/158_mangue_acoes_helm.png
    :alt: Ações Helm
    :scale: 100 %
    :align: center
=====

      * **Editar Helm**: Al seleccionar la opción de editar se presenta la siguiente pantalla, a través de la cual el usuario puede cambiar el nombre y los argumentos de la aplicación Helm. 

      * **Eliminar Helm**: Al seleccionar esta opción se desinstala el Helm seleccionado del *Cluster*.
.. image:: /figuras/fig_mangue/159_mangue_add_helm.png
    :alt: Adiconar Helm
    :scale: 100 %
    :align: center
=====

Para crear un Helm es necesario pulsar el botón Añadir |icone_adicionar| es imprescindible especificar su nombre y seleccionar de la lista de Helms el nombre de la aplicación en el repositorio. También es posible especificar argumentos para la aplicación, algunas aplicaciones Helm requieren argumentos para realizar la configuración. 

Después de rellenar todos los campos necesarios, el botón ``Añadir Helm`` está disponible para ser pulsado. Al hacer clic en la plataforma Mangue.io se realiza la instalación de Helm, después de ser instalado presenta un mensaje de éxito. 

====

Server VS Code
--------------

El *Visual Studio Code* es un Ambiente de Desarrollo Integrado  (*Integrated Development Environment* - IDE) para el desarrollo de aplicaciones. Este IDE puede ser instalado en un *Cluster*, a través de un *Deployment*, permitiendo así que el IDE se ejecute dentro del navegador de un usuario. 

Para utilizar la funcionalidad de *Server VS Code* es necesario haber registrado previamente el *KubeConfig* del *Cluster* en la plataforma Mangue.io.

En la pantalla del *Server VS Code* se presenta una lista actualizada, con el *Visual Studio Code* en el *Cluster* actualmente. También es posible que el usuario realice la búsqueda del *Visual Studio Code* instalado por medio de su nombre.

.. image:: /figuras/fig_mangue/160_mangue_server_vscode.png
    :alt: Server VsCode
    :scale: 100 %
    :align: center
=====

A continuación describimos la información presente en la tabla de *VS Code*.

* **#**: Número secuencial del *VS Code* registrado en la plataforma Mangue.io.
* **Nombre**: Nombre del *VS Code* especificado por el usuario durante la creación.
* **Usuario**: Nombre del usuario que ha creado el *Visual Studio Code*.
* **Fecha de Creación**: Fecha de creación del *Visual Studio Code* en el *Cluster*. 
* **Réplicas**: Cantidad de réplicas del *deployment* disponibles y deseadas.
* **IP**: IP del *Visual Studio Code* para ser accedido en el navegador web.
* **Acciones**: Esta columna presenta el botón de ``Acción`` |icone_acao| al ser pulsado, muestra la opción de eliminar *VS Code*, como se muestra en la figura:

.. image:: /figuras/fig_mangue/161_mangue_excluir_vscode.png
    :alt: Excluir VsCode
    :scale: 100 %
    :align: center
=====

      * **Eliminar VS Code**: Al seleccionar la opción de eliminar, se quita el *VS Code* seleccionado del *Cluster*.

.. image:: /figuras/fig_mangue/162_mangue_add_vscode.png
    :alt: Add VsCode
    :scale: 100 %
    :align: center
=====

Para crear un *Visual Studio Code* es necesario hacer clic en el botón de Suma |icone_adicionar| y rellenar los campos siguientes:

* **Nombre del Servidor VS Code**: Nombre del servidor *Visual Studio Code* que se va a crear.
* **Tamaño del Servidor VS Code**: Tamaño del disco disponible para el *Visual Studio Code*. La medida del tamaño se establece en el campo Tipo de tamaño.
* **Tipo de Servicio**: El usuario puede seleccionar el tipo de servicio que se va a asignar al *deployment* del *Visual Studio Code*. Las opciones disponibles son: *Cluster IP*, *NodePort*, *Load Balancer* e *Ingress*.
* **Puerto**: El usuario puede seleccionar el puerto que se utiliza en el servicio.
* **Tipo de Tamaño**: Especifica la unidad de tamaño. Las opciones disponibles son: Gi y Mi.
* **Ingress Class**: Si el tipo de servicio seleccionado es *Ingress*, es necesario seleccionar el *Ingress Class* a ser utilizado por el servicio.
* **URL del Servidor VS Code**:  Si el tipo de servicio seleccionado es *Ingress*, es necesario especificar la ruta del *Ingress*. Ejemplo: /vscode
* **Activar Autenticación**: El usuario puede asignar una contraseña que es necesaria para acceder al Servidor *VS Code*.
* **Contraseña del Servidor VS Code**: Contraseña utilizada para acceder al Servidor *VS Code*.

====

Services, Load Balancing and Networking
=======================================

Los *Pods* nacen y mueren, y cuando mueren, mueren de verdad, no resucitan. Los controladores *ReplicaSets*, en particular, crean y eliminan *Pods* de forma dinámica (por ejemplo: aumentando o disminuyendo la escala). 

Aunque cada *Pod* tiene su propia dirección TCP-IP, ni siquiera estos pueden considerarse estables a lo largo del tiempo (por ejemplo, Protocolo de Configuración Dinámica de Direcciones de Red, en Inglés, *Dynamic Host Configuration Protocol - DHCP*). 

Esto puede crear un problema, si algún conjunto de *Pods* (llamado *back-end*) proporciona funcionalidad a otros *Pods* (llamado *front-end*) dentro de un *cluster* del Mangue.io; ¿Cómo estos *front-ends* descubren y controlan los *back-ends* que están en este conjunto? Es en este momento que se introducen los Servicios. 

Un Servicio en Mangue.io es una instancia del objeto *Service* del *Kubernetes*, que a su vez es una abstracción que define un conjunto lógico de *Pods* y una política por la cual es posible acceder a ellos. El conjunto de *Pods* segmentados por un servicio suele estar determinado por un conjunto de *Labels*. 

El menú *Services*, *Load Balancing and Networking* está dividido en dos submenús que corresponden a: *Servicios*, *Ingress*. Cada submenú tiene un propósito específico que se describe a continuación.

====

Servicios
---------

Es una forma abstracta de exponer una aplicación que se ejecuta en un conjunto de *pods* como un servicio de red. Con el *Kubernetes*, el usuario no necesita modificar su aplicación para utilizar un mecanismo de *Service Discovery* desconocido. 

El *Kubernetes* proporciona a los *pods* sus propias direcciones TCP-IP y un nombre *DNS* único para un conjunto de *pods* y puede equilibrar la carga entre ellos. Este submenú listará los servicios que existen en el *namespace* por el que el usuario está navegando.

El menú *Networking*/Servicios presenta todos los servicios de un *cluster* en un determinado *namespace*, en la tabla tenemos información listada como en la pantalla de abajo:

.. image:: /figuras/fig_mangue/163_mangue_servicos.png
    :alt: Serviços
    :scale: 100 %
    :align: center
=====

* **Servicio**: Representa el nombre del servicio creado, es el identificador principal de un servicio al ejecutar una búsqueda en la barra de búsqueda. 
* **Protocolo**: Se encarga de identificar el tipo de protocolo de este servicio, como por ejemplo: TCP, UDP. 
* **Tipo**: Representa el tipo de servicio creado en *Kubernetes*, hay tres tipos de servicio que son:

      * **NodePort**: Son servicios accesibles externamente a través del *range* de puertos de 30000 a 32767.

      * **ClusterIP**: Son servicios a los que sólo se puede acceder en la red interna del *cluster*.

      * **LoadBalancer**: Es un tipo de servicio existente con la finalidad de aprovisionar un *LoadBalancer* en la 7ª capa, para que la comunicación se realice con el servicio de la 4ª capa creado en el *cluster Kubernetes*.

* **Port**: Son los puertos en los que el servicio puede recibir peticiones.
* **Duración**: Responsable de identificar desde cuándo ha sido creada la estructura del servicio;
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| al ser pulsado, presenta tres opciones:

.. image:: /figuras/fig_mangue/164_mangue_acoes_servico.png
    :alt: Ações serviços
    :scale: 100 %
    :align: center
=====

A continuación se describe cada opción de este submenú:

* **Añadir Ingres**: *Ingress* es un servicio que puede ser configurado para proporcionar Servicios con URLs accesibles externamente. Un *Ingress Controller* es responsable de complementar el *Ingress*, normalmente con un balanceador de carga, aunque también puede configurar su enrutador de borde o *front-ends* adicionales para ayudar a manejar el tráfico. 

    Esta pantalla realiza la creación de un *Ingress* en dos etapas, inicialmente la creación de un balanceador de carga, y luego la creación del *Ingress* en la plataforma Mangue.io.
 
.. image:: /figuras/fig_mangue/165_mangue_add_ingress.png
    :alt: Add Ingress
    :scale: 100 %
    :align: center
=====

* **Nombre del Ingress**: En este campo el usuario debe informar un nombre que hace que este servicio se configure en la plataforma Mangue.io.
* **Generar LoadBalancer**: Después de informar el nombre del *ingress* el usuario debe hacer clic en el botón verde con el icono de un balanceador de carga |icone_loadbalancer| para iniciar el proceso de creación del balanceador de carga en la plataforma Mangue.io. El usuario debe esperar un *feedback* de alerta que se presenta en la esquina superior derecha de la pantalla informando del éxito o error de esta acción.
* **Añadir**: Después de crear con éxito el balanceador de carga, el usuario debe hacer clic en el botón ``Añadir`` para crear el servicio de *ingress* en la plataforma Mangue.io.

      * **Eliminar Servicio**: En la segunda opción del menú de acciones de servicios se encuentra la opción de eliminar, cuando se selecciona se abre un modal de confirmación, en el que se pide que se confirme la acción pulsando el botón ``Eliminar``. A continuación, se muestra el *feedback* de alerta en la esquina superior derecha de la pantalla, informando del éxito o del error.

.. image:: /figuras/fig_mangue/166_mangue_aviso_ingress.png
    :alt: Aviso Ingress
    :scale: 100 %
    :align: center
=====

Es importante tener en cuenta que esta acción es definitiva y elimina (borra) esta configuración de la plataforma Mangue.io, ya que se eliminan todas las referencias de este servidor de monitorización en la plataforma Mangue.io.

      * **Editar Servicio**: Esta opción del menú de acciones muestra la opción ``Editar Servicio``. Cuando se selecciona, la plataforma Mangue.io presenta el contenido del archivo en formato *JSON* con todas las configuraciones del servicio en *Kubernetes*. El usuario puede editar lo que sea necesario en este archivo y seleccionar el botón ``Enviar``. Esperar el *feedback* de la acción que abre el siguiente modal:

.. image:: /figuras/fig_mangue/167_mangue_editar_servico.png
    :alt: Editar Serviço
    :scale: 100 %
    :align: center
=====


Recomendamos que sólo los usuarios con experiencia en la sintaxis *YAML* o Kubernetes realicen cambios en el código de un servicio, ya que codificar (o cambiar) la sintaxis de forma incorrecta puede llevar a la pérdida de acceso a todo el ambiente de *clusters* existentes. 

El usuario puede utilizar el ratón para hacer clic en la línea (y la ubicación) deseada para empezar a escribir sus parámetros específicos del servicio, editando así la plantilla de código *YAML* que la plataforma presenta.

====

Ingress
-------

El *Ingress* expone las rutas HTTP y HTTPS desde fuera del *cluster* a los servicios dentro del *cluster*. El enrutamiento del tráfico se controla mediante reglas definidas en el recurso *Ingress*. 

Un *Ingress* puede ser configurado para proveer servicios con URLs accesibles externamente, *Load Balancing*, configuración para SSL / TLS. 

Un *Ingress Controller* se encarga de complementar el *Ingress*, normalmente con un balanceador de carga, aunque también puede configurar su enrutador de borde o *front-ends* adicionales para ayudar a manejar el tráfico. 

En este submenú, se listan los *Ingress* existentes en el *namespace* seleccionado en la pestaña de engranajes |icone_engrenagem| “Selección de configuración” de la plataforma Mangue.io.

Encima de la tabla, hay tres elementos con los que el usuario puede trabajar:

.. image:: /figuras/fig_mangue/053.1_mangue_pesquisar_atualização.png
    :alt: Pesquisar atualizações
    :scale: 100 %
    :align: center
=====

* **Acción de Búsqueda**: Si la lista que se presenta en esta pantalla es muy larga (ocupando más de una página), hay un campo que permite al usuario buscar por el nombre del *Update* deseado. Basta introducir una parte del nombre y pulsar “Enter” o hacer clic en el icono de "La lupa" |icone_lupa_verde|. Como resultado de esta búsqueda sólo se recuperan los *Updates* que contengan la palabra clave de la búsqueda.

* **Acción de Actualizar**: Basta hacer clic en el icono |icone_update|  para que Mangue.io actualice la interfaz con los valores más recientes de esta tabla de *Ingress*.

.. image:: /figuras/fig_mangue/169_mangue_ingress.png
    :alt: Ingress
    :scale: 100 %
    :align: center
=====

A continuación describimos la información de la lista que aparece en esta pantalla:

* **#**: Número secuencial del servidor de monitorización registrado en la plataforma Mangue.io.
* **Nombre**: Esta columna muestra el nombre del *Ingress* que fue informado durante el proceso de registro del *Ingress* en la plataforma Mangue.io.
* **Host**: Esta coluna apresenta a informação do nome do servidor (*Server Name*) que está registrado no DNS, ou o número do endereço TCP-IP deste servidor.
* **Servicio**: Esta columna presenta la información del servicio al que está asociado este *Ingress*.
* **Address**: Esta columna presenta el número de la dirección TCP-IP del *Ingress* que fue configurada en la plataforma Mangue.io.
* **Duración**: Esta columna presenta el tiempo en días transcurridos desde la fecha de creación del *Ingress* hasta la fecha actual en que el usuario está consultando esta lista.
* **Acciones**: Esta columna presenta el botón de ``Acción`` para eliminar *Ingress*, mediante el icono de "Papelera" |icone_lixo|. Al hacer clic en el icono, se solicita al usuario la confirmación para proceder a la eliminación del *ingress*, de acuerdo con la imagen que aparece a continuación:

.. image:: /figuras/fig_mangue/170_mangue_aviso_deletar_ingress.png
    :alt: Aviso deletar Ingress
    :scale: 100 %
    :align: center
=====

En caso de que el usuario haya incluido un nuevo *Ingress* recientemente, pero no encuentre el nombre en la lista, lo que puede hacer el usuario es pulsar el icono |icone_update| para que Mangue.io pueda actualizar la interfaz con la lista más reciente de esta tabla.

====

Namespaces
==========

El *Kubernetes* ofrece apoyo a múltiples *clusters* virtuales apoyados por un mismo *cluster* físico. Estos *clusters* virtuales son llamados *namespaces*. Los *namespaces* son identificados por un "nombre". Estos pueden contener diversos "recursos", y cada recurso debe tener su propio nombre único. El usuario puede crear el mismo recurso varias veces (repitiendo el mismo nombre), pero estos recursos deben configurarse en un *namespace* distinto.

*Namespaces* también apoyan la definición de cuotas, como por ejemplo un *namespace* para un ambiente de Producción y un *namespace* para un ambiente de Homologación.

Evidentemente, el ambiente computacional asignado al *namespace* Producción debe tener mayor capacidad de recursos computacionales del *cluster* que el *namespace* configurado para un ambiente de Homologación - ya que este ambiente tiene una carga de uso eventual. Las cuotas limitan la cantidad de recursos computacionales que un determinado *Namespace* puede consumir.

El menú *Namespaces* presenta una lista de todos los *namespaces* de un determinado *cluster*, en la tabla tenemos informaciones como: nombre del *namespace*, *status* y duración del *namespace*. Los *namespaces* consisten en diferentes áreas de trabajo que hacen parte de un *cluster*.

.. image:: /figuras/fig_mangue/171_mangue_namespaces.png
    :alt: Namespaces
    :scale: 100 %
    :align: center
=====

Para que el usuario pueda crear un *namespace*, debe hacer clic en el icono de suma  |icone_adicionar|, que presenta la siguiente pantalla donde el usuario puede configurar un nuevo *namespace*:

.. image:: /figuras/fig_mangue/172_mangue_add_namespace.png
    :alt: Adicionar namespace
    :scale: 100 %
    :align: center
===== 

La pantalla de arriba tiene un solo campo en el que el usuario debe rellenar el nombre que desea crear para el nuevo *namespace* y hacer clic con el cursor del ratón en el botón ``Añadir Namespaces``, para incluirlo en la plataforma. La plataforma Mangue.io presenta un *feedback* de esta acción en el campo superior derecho de la pantalla del navegador de internet.

Este nuevo *namespace* es creado dentro del *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración" de la plataforma Mangue.io.

Tras la inclusión de un nuevo *namespace*, si este nombre no aparece en la lista, el usuario puede hacer clic en el icono |icone_update| para que Mangue.io actualice la interfaz con la lista más reciente de esta tabla.

En la última columna de la tabla existe la opción de eliminar el *namespace*, al seleccionar esta columna se abre un modal de confirmación. Y si se confirma, aparece un *feedback* de creación para el usuario.

.. image:: /figuras/fig_mangue/171_mangue_namespaces.png
    :alt: Namespace deletar
    :scale: 100 %
    :align: center
=====

A continuación se describen los campos de la tabla presentada en esta pantalla:

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. 

    Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Esta columna presenta el nombre del *namespaces* que fue informado durante el proceso de registro de *namespaces* en la plataforma Mangue.io.
* **Status**: Identifica el estado actual del *namespaces*. Puede ser presentado por *Running*, *Pending* o “!” (signo de exclamación).

      * **Running** identifica que no hay ningún error con los *namespaces*.

      * **Pending** identifica algún estado de transición en los *namespaces*. Ya sea por actualización, inicialización del proceso del *container* o cualquier actividad que identifique un estado de transición.

      * **“!”** (signo de exclamación) identifica una alarma, es decir, que algo incorrecto ha ocurrido con los *namespaces*.

* **Cuota**:  Esta columna presenta un icono de un "ojo" |icone_exibir| que se queda activo en las líneas de *namespaces* que tengan alguna cuota definida. El usuario debe posicionar el cursor del ratón sobre el icono y la plataforma Mangue.io presenta una ventana *pop-up* con el nombre y las características de la cuota definida para este *namespace*.

.. image:: /figuras/fig_mangue/173_mangue_test_quota.png
    :alt: Teste cota
    :scale: 100 %
    :align: center
=====  

* **Duración**: Esta columna presenta el tiempo en días transcurridos desde la fecha de creación de los *namespaces* hasta la fecha actual en que el usuario está consultando esta lista.
* **Acciones**: Esta columna presenta el botón ``Acción`` |icone_acao| que al ser pulsado, presenta tres opciones como la figura siguiente:

.. image:: /figuras/fig_mangue/174_mangue_acoes_namespace.png
    :alt: Ações namespace
    :scale: 100 %
    :align: center
=====  

* **Añadir Labels**: Una etiqueta (*label*) permite al usuario asignar sus propias estructuras organizativas en objetos del sistema de una manera ligeramente acoplada, sin requerir que el *software* almacene estas asignaciones. Las etiquetas se crean con dos asignaciones "clave" y "valor" y se adjuntan a los objetos, como los *pods*. Las etiquetas (*labels*) deben utilizarse para especificar la identificación de los atributos de los objetos que son significativos y relevantes para los usuarios. Las etiquetas pueden utilizarse para organizar y seleccionar subconjuntos de objetos, información detallada en el enlace del pie de página del sitio de documentación de Kubernetes_.

.. _Kubernetes: https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/ 

.. image:: /figuras/fig_mangue/175_mangue_label_namespace.png
    :alt: Adicionar label namespace 
    :scale: 100 %
    :align: center
=====

Esta pantalla tiene dos campos y dos botones:

* **Llave**:  En este campo el usuario debe rellenar el nombre con el que se identifica la llave (*key*).
* **Valor**: En este campo el usuario debe rellenar con un número entero que es el valor de la llave.
* **Añadir**: El usuario debe hacer clic con el cursor del ratón sobre este botón para añadir la llave y su valor en la plataforma Mangue.io. Al hacer clic en este botón, la plataforma limpia ambos campos y crea una lista justo debajo. Si el usuario ha añadido una llave/valor equivocada, basta hacer clic en el botón ``Eliminar``, que el par de información en cuestión es eliminado, y el usuario puede registrar un nuevo par (llave/valor) con el contenido correcto.

.. image:: /figuras/fig_mangue/176_mangue_label_chave_valor.png
    :alt: Label chave valor
    :scale: 100 %
    :align: center
=====

* **Confirmar**: El usuario debe hacer clic en el botón ``Confirmar`` cuando haya completado la información de la(s) llave(s)/valor(es) necesaria(s) para los *namespaces*. Al hacer clic en el botón, la plataforma Mangue.io configura estas informaciónes, cerra la pantalla y presenta el *feedback* de la acción en la esquina superior derecha de la pantalla del navegador de Internet.

* **Añadir Cuota de Recursos**: Esta pantalla permite al usuario establecer la cantidad ideal de recursos computacionales que consume el *namespace* para mantener su rendimiento ideal, así como establecer su límite máximo de consumo de recursos computacionales.

La definición de una cuota puede afectar a otros servicios (*workloads*) registrados en la plataforma Mangue.io. Cuando el usuario define un límite de CPU y Memoria para un *namespace* si un *deployment* tiene varios *pods*, replicas o Autoescalador Horizontal, estos nunca superaran el límite de recursos computacionales establecido en la cuota. 

Por ejemplo: 

Si un *deployment* necesita iniciar una nueva réplica definida en el Autoescalador Horizontal, y el límite de CPU y Memoria ya ha sido alcanzado, la plataforma Mangue.io no inicia la nueva réplica, aunque los valores definidos en el Autoescalador Horizontal sean alcanzados, pero el límite de cuota no permite que haya recursos computacionales disponibles para esta nueva réplica.

.. image:: /figuras/fig_mangue/177_mangue_add_cota.png
    :alt: Adicionar cota recurso
    :scale: 100 %
    :align: center
=====

* **Nombre de la Cuota**: Informa el nombre con el que la cuota es identificada para los *namespaces* en la plataforma Mangue.io.
* **CPU Request**: En este campo el usuario debe rellenar un número entero que es el valor inicial de la cantidad de CPU que el *namespace* requiere para mantener el rendimiento ideal.
* **Memory Request**: En este campo el usuario debe rellenar un número entero que es el valor inicial de la cantidad de memoria que el *namespace* requiere para mantener el rendimiento ideal.
* **CPU Limit**: En este campo el usuario debe rellenar con un número entero que es el valor del límite máximo de cantidad de CPU que el *namespace* debe restringir para no agotar los recursos computacionales del *cluster*.
* **Memory Limit**: En este campo el usuario debe rellenar con un número entero que es el valor del límite máximo de la cantidad de memoria que el *namespace* debe restringir para no agotar los recursos computacionales del *cluster*.
* **Confirmar**: Cuando el usuario rellena todos los campos de este formulario debe pulsar el botón ``Confirmar`` para que la plataforma Mangue.io configure e incluya las cuotas de recursos a los *namespaces* seleccionados.

      * **Eliminar**: La tercera opción de este submenú permite al usuario eliminar (borrar) un *namespace* de forma permanente del *cluster* que fue seleccionado en la “pestaña” de configuraciones; y al hacer clic se abre la siguiente pantalla de interfaz solicitando la confirmación por parte del usuario:

.. image:: /figuras/fig_mangue/178_mangue_aviso_deletar.png
    :alt: Aviso deletar
    :scale: 100 %
    :align: center
=====

.. attention:: Esta es una acción extremadamente destructiva, ya que al eliminar un *namespace* también se eliminan **todos** los recursos y servicios presentes en él.

====

Nodes
=====

El menú *Nodes* muestra todos los *nodes* (máquinas virtuales) de un determinado *Cluster*. En *Overview Nodes* se puede ver gráficamente el consumo de recursos (CPU y memoria) de todos los *nodes* de un *Cluster* en un determinado período. 

El consumo de la CPU se mide en MilliCores y el de la memoria en MegaBytes, ambos en función del tiempo. 

Es permitido al usuario seleccionar el período deseado haciendo clic en los botones situados encima de los gráficos. Las opciones disponibles para el usuario son entre los últimos 30, 15, 7 y 1 día(s) y, en las últimas 12 horas. Para los períodos de 30, 15 y 7 días, las mediciones en función del tiempo son diarias y para los períodos de 1 día y 12 horas, son por hora. 

Se destaca en el color azul del gráfico de barras las cantidades de recursos utilizados en ese periodo seleccionado, ya sea por día o por hora, según elija el usuario, mientras que el color verde mide la cantidad total de recursos, es decir, que permanecen ociosos en ese periodo. 

La cantidad total de recursos de los *Nodes* de un *Cluster* tanto para la CPU como para la memoria está representada por la suma de estas dos medidas.  

.. image:: /figuras/fig_mangue/179_mangue_overview_nodes.png
    :alt: Overview Nodes
    :scale: 100 %
    :align: center
=====

.. image:: /figuras/fig_mangue/180_mangue_nodes.png
    :alt: Nodes
    :scale: 100 %
    :align: center
=====

Justo encima de la tabla, hay un elemento con el que el usuario puede actuar:

      * **Mostrar nodes por contrato**: Al seleccionar esta opción, aparece un campo en el que el usuario puede introducir el nombre del contrato por el que desea realizar su búsqueda.

A continuación la descripción de las columnas de esta tabla:

* **Nombre**: Nombre del *node*.
* **Status**: Corresponde al estado actual del *node*.

      * **Running**: Indica que el *node* está "sano".

      * **Failure**: Indica que se ha producido algún error con el *node*, o que actualmente el *node* no está disponible.

* **CPU Utilizada**: Representa el consumo actual del recurso de CPU de la máquina virtual (*node*). Este valor se expresa como una fracción de un número entero (decimales) de la cantidad de CPU existente en la infraestructura que compone la máquina virtual. La infraestructura computacional existente de la máquina virtual soporta y ejecuta microservicios (por ejemplo, el *deployment*), que consumen sólo una pequeña porción del recurso total de la CPU. Así, la aplicación muestra la cantidad decimal del recurso total de CPU consumido por la máquina virtual.
* **Memoria utilizada**: El consumo actual del recurso de Memoria RAM de la máquina virtual. Este valor se expresa en Gigabytes, a partir de la cantidad total de Megabytes de Memoria RAM existente en la infraestructura que conforma la máquina virtual (*node*). La infraestructura computacional existente de la máquina virtual (*node*) para soportar y ejecutar microservicios (por ejemplo, *deployment*), así que un microservicio consume sólo una pequeña parte del recurso de Megabytes de Memoria RAM de un *node*.

Para el usuario conocer los detalles de todos los *pods* de un *node* específico, basta pulsar con el cursor del ratón sobre el nombre del *node* y la plataforma Mangue.io presenta una sección con una lista de todos los *pods* que se ejecutan en el *node* seleccionado.

.. image:: /figuras/fig_mangue/181_mangue_pods.png
    :alt: Pods
    :scale: 100 %
    :align: center
=====  

La sección "Pods" presenta una tabla que enumera todos los *pods* que se ejecutan en este *node*. Presenta informaciones detalladas como el nombre, el nodo en el que se está ejecutando, el *status* actual del *pod*, la imagen, junto con su versión y su tiempo de vida (ver la descripción completa de los campos de esta tabla en el ítem Sección: PODs).

Cuando se necesite consultar los *logs*, o acceder al *prompt* del sistema operativo de un *pod* específico, en la columna “Acciones” el usuario debe pulsar con el cursor del ratón sobre el icono |icone_acao| para que la plataforma Mangue.io presente un submenú con la opción de acceso al *log* y a la línea de comandos del *pod* seleccionado.

Justo encima de la tabla, hay tres elementos con los que el usuario puede actuar:

.. image:: /figuras/fig_mangue/182_mangue_pesquisar_node.png
    :alt: Pesquisar Node
    :scale: 100 %
    :align: center
=====  

* **Acción de búsqueda**: Si la lista presentada en esta pantalla es muy larga (ocupa más de una página), hay un campo donde el usuario puede buscar por el nombre del *Update* deseado. Sólo tiene que introducir parte del nombre del *update* y pulsar ``Enter`` o hacer clic en el icono de "La lupa" |icone_lupa_verde|. Como resultado de esta búsqueda, sólo aparecen los *nodes* que contengan la palabra llave buscada.
* **Acción de actualización**: Basta hacer clic en el icono |icone_update| para que Mangue.io actualice la interfaz con la lista de nombres de *nodes* configurados en la plataforma Mangue.io.
* **Añadir Labels**: Si el usuario necesita añadir una (o varias) *labels* al *node*, debe hacer clic con el cursor del ratón en el icono de las etiquetas (labels) |icone_rotulo| y la plataforma Mangue.io presenta la siguiente pantalla:

.. image:: /figuras/fig_mangue/183_mangue_label_nods.png
    :alt: Label Nods
    :scale: 100 %
    :align: center
=====

* **Seleccionar nodes**: Al hacer clic en el campo se muestra una lista (*dropdown*) con todos los *nodes* configurados en la plataforma Mangue.io. El usuario sólo tiene que hacer clic con el cursor del ratón sobre el nombre del *node* deseado para seleccionar.
* **Nombre de la Label**: En este campo el usuario debe rellenar el nombre con el que se identifica la *label* (*key*).
* **Valor de la Label**: En este campo el usuario debe rellenar un número entero que es el valor de la llave.
* **Añadir**: El usuario debe hacer clic con el cursor del ratón sobre este botón para añadir la *label* y su valor en la plataforma Mangue.io. Al hacer clic en este botón, la plataforma Mangue.io limpia ambos campos y crea una lista a continuación. En el caso de que el usuario haya añadido una *label*/valor erróneo, basta hacer clic en el botón ``Eliminar``, y el par de información en cuestión es eliminado, el usuario puede registrar un nuevo par (llave/valor) con el contenido correcto.

.. note:: Añadir *labels* a los *nodes* puede ser importante para los usuarios que desean hacer configuraciones de *Node Affinity* a sus *Deployments*.

**Finalizar**: Este botón permite añadir la(s) label(s) seleccionada(s) a la plataforma Mangue.io. En la secuencia se muestra el *feedback* de esta acción. 

====

Migración de cluster
====================

Mangue.io es una plataforma de Gestión de Ambientes de Múltiples Orquestadores de *Containers*, que permite la orquestación, implementación (localización y programación) y operacionalización (ejecución) de *containers* de aplicaciones dentro de un *cluster* computacional (público o privado) o entre *clusters* computacionales (públicos y/o privados).

La plataforma opera en un modelo *multicloud* híbrido y, por lo tanto, permite a las empresas un control total, soporte para el sostenimiento de copias de seguridad (*backup*), replicación y migración de ambientes.
El menú Migraciones de *Cluster* se encarga de realizar la migración de múltiples recursos entre *clusters* - de público y/o privado a público y/o privado.

A través de la plataforma Mangue.io el usuario puede migrar el contenido completo de un *cluster* - con todos sus diversos tipos de *workloads* - a otro cluster.

La facilidad de migración de todo los tipos de *workloads* entre *clusters* facilita la creación de un ambiente de Múltiples Orquestadores de *Containers* preparado para escenarios de *Disaster Recovery*.

La plataforma Mangue.io es agnóstica a los proveedores de servicios (privados, públicos) y a través de la funcionalidad del menú Migraciones el usuario puede mantener, gestionar y operar diversas copias de sus *clusters* en múltiples orquestadores de *containers*, de forma simultánea y centralizada.

====

Proceso de Migración de Workloads
---------------------------------

El usuario puede observar que esta pantalla está segmentada en dos secciones: Migración entre Clusters y *Workloads*, el proceso de migración es sencillo y el usuario es guiado intuitivamente para completar el relleno de la pantalla en la plataforma Mangue.io.

A continuación presentamos el proceso para el correcto relleno de la pantalla de migración:

.. image:: /figuras/fig_mangue/184_mangue_migracao_clusters.png
    :alt: Migração clusters
    :scale: 100 %
    :align: center
=====

1. Seleccionar el *Cluster* **Origen** (Sección Migración)

* Este campo es un *dropdown list* y son listados los *clusters* configurados en el ítem Integrar *Cluster*.

2. Seleccione el *Cluster* **Destino** (Sección Migración)

* Este campo es un *dropdown list* y son listados los *clusters* configurados en el ítem Integrar *Cluster*.

3. Seleccionar *Namespace* (Sección *Workloads*)

* Este campo es un *dropdown list* y son listados los *namespaces* configurados en el ítem *Namespaces*.

* Si la línea situada debajo de este campo está punteada, significa que no hay ningún *namespace* configurado y disponible para la migración en el *cluster* de origen informado en el paso 1: Vea el ejemplo en la pantalla siguiente:

.. image:: /figuras/fig_mangue/185_mangue_workloads_tracejado.png
    :alt: Workloads
    :scale: 100 %
    :align: center
=====

* Cuando hay *namespaces* configurados, la plataforma Mangue.io presenta una línea continua debajo de este campo, véase el ejemplo siguiente:

.. image:: /figuras/fig_mangue/186_mangue_workloads_continua.png
    :alt: Workloads 
    :scale: 100 %
    :align: center
=====

4. Seleccionar el **Tipo** de *Workload* (Sección *Workloads*)

* Este campo es un *dropdown list* y presenta la lista de todos los tipos de *workloads* configurados en el elemento *Workloads*.

* Al hacer clic en este campo, la plataforma Mangue.io presenta una relación de *workloads* que pueden ser migradas de un *cluster* a otro (*Configmaps*, *Deployments*, *Daemonsets*, *Statefulsets*, *Ingresses, Services*).

* En *Kubernetes*, no hay ningún objeto, componente o cualquier tipo de construcción llamada *workload*. Sin embargo, el término suele utilizarse como una categoría general para las tareas y servicios que el usuario desea ejecutar en su *Cluster*.

5. Seleccionar el **Nombre** del *Workload* (Sección *Workloads*)

* Este campo es un *dropdown list* y son listados solo los nombres de *workloads* que forman parte del mismo tipo de *workload* seleccionado en el campo anterior.

* Cuando el usuario rellena todos los campos anteriores (*namespace*, tipo de *workload*) la plataforma Mangue.io presenta la lista de nombres disponibles y el usuario puede seleccionar uno de los nombres ya que cada línea está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. Cuando el usuario selecciona uno de los nombres, éste se añade a la lista de migración, como en el ejemplo siguiente:

.. image:: /figuras/fig_mangue/187_mangue_workloads.png
    :alt: Selecionar workloads
    :scale: 100 %
    :align: center
=====

* La plataforma Mangue.io permite añadir varios tipos de *workloads* para que la migración se pueda realizar en una sola etapa, según el ejemplo de la pantalla siguiente:

.. image:: /figuras/fig_mangue/188_mangue_workloads_lista.png
    :alt: Workloads lista
    :scale: 100 %
    :align: center
=====

6. **Confirmar**: 

* Después de seleccionados, los recursos se muestran en la tabla que contiene informaciones como: Nombre del recurso, Tipo de recurso, *Namespace*, *Cluster* de origen y *Cluster* de destino. La plataforma Mangue.io inicia el movimiento de los *workloads* entre los *clusters* seleccionados, y poco después, hay un *feedback* de esta acción que se presenta en la esquina superior derecha de la pantalla del navegador.

* Después de confirmar este procedimiento, la plataforma Mangue.io realiza la migración de todas las *workloads* seleccionadas entre los *clusters* indicados, se presenta un mensaje de *feedback* en la esquina superior derecha de la pantalla del navegador de Internet. 

====

Migración de Namespace
----------------------

Este menú es responsable por realizar la migración de múltiples recursos entre *namespaces* del mismo *Cluster*.

Esta pantalla está segmentada en dos secciones, al igual que la pantalla de **Migración** de Cluster: Migración entre *Namespaces* y *Workloads*, el proceso de migración es simple y el usuario es guiado de forma intuitiva para completar el proceso de llenado de la pantalla en la plataforma.

A continuación presentamos el proceso para el correcto relleno de la pantalla de migración:

.. image:: /figuras/fig_mangue/189_mangue_migracao_namespaces.png
    :alt: Migração entre namespace
    :scale: 100 %
    :align: center
=====

1. Seleccione el *Namespace* **Origen** (Sección Migración)

* Este campo es un *dropdown list* y son listados los *namespaces* del *Cluster*.

2. Seleccionar el *Namespace* **Destino** (Sección Migración)

* Este campo es un *dropdown list* y son listados los *namespaces* del Cluster.

3. Seleccionar el **Tipo** de *Workload* (Sección *Workloads*)

* Este campo es un *dropdown list* que lista todos los tipos de recursos disponibles para migración.

4, Seleccionar el **Nombre** de *Workload* (Sección *Workloads*)

* Este campo es un *dropdown list* y lista solo los nombres de los recursos que forman parte del mismo tipo de *workload* seleccionado en el campo anterior.

* Cuando el usuario rellena todos los campos anteriores (*namespace*, Tipo de *workload*) la plataforma Mangue.io presenta la lista de nombres disponibles y el usuario puede seleccionar uno de los nombres pues cada línea está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. Una vez que el usuario seleccione uno de los nombres, éste se anãnde a la lista de migración, tal y como se muestra en el siguiente ejemplo:

.. image:: /figuras/fig_mangue/190_mangue_workloads_tipo.png
    :alt: Workloads tipo
    :scale: 100 %
    :align: center
=====

* La plataforma Mangue.io permite añadir diversos tipos de *workloads* para que se pueda realizar en una sola etapa, según el ejemplo de la pantalla siguiente:

.. image:: /figuras/fig_mangue/191_mangue_workloads_lista.png
    :alt: Workloads lista
    :scale: 100 %
    :align: center
=====

5. **Confirmar**: 

* Una vez seleccionados, los recursos se muestran en la tabla que contiene informaciones como: Nombre del recurso, Tipo de recurso, *Namespace*, *Namespace* de origen y *Namespace* de destino. La plataforma Mangue.io inicia la movimentación de los *workloads* entre los *namespaces* seleccionados, y poco después, hay un *feedback* de esta acción que se presenta en la esquina superior derecha de la pantalla del navegador.

* Tras confirmar este procedimiento, la plataforma Mangue.io migra todos los *workloads* seleccionados entre los *namespaces* indicados, y se presenta un mensaje de *feedback* en la esquina superior derecha de la pantalla del navegador de Internet. 

====

Registry
========

El menú *Registry* presenta todos los *Docker Registries* integrados a la plataforma. *Docker Registry* ofrece un servicio de alojamiento de imágenes *Docker* análogo al que está disponible en Hub_, pero con la posibilidad de uso y alojamiento en una red interna. Los *Registries* pueden y deben ser utilizados como una alternativa para el almacenamiento de imágenes *docker* de los servidores y aplicaciones de una organización. 

En el menú *Registry* es posible conectarse a un *registry* privado, es decir, un servidor de registro de imágenes privado de la organización. O un servicio de registro de imagen público, como por ejemplo Docker Hub_.

En esta sección hay una tabla que contiene las informaciones de los *Registries* añadidos a Kubernetes, recordando que los *registries* son secretos (ver el ítem *Secrets*) creados por *namespace*.

Justo encima de la tabla, hay dos elementos con los que el usuario puede actuar:

.. image:: /figuras/fig_mangue/192_mangue_pesquisar_registry.png
    :alt: Pesquisar Registry 
    :scale: 100 %
    :align: center
=====

* **Acción de búsqueda**: Si la lista que se presenta en esta pantalla resulta muy larga (ocupando más de una página), existe un campo en el que se puede buscar por el nombre del *Registry* deseado. Sólo es necesario introducir parte del nombre del *update* y pulsar “Enter” o hacer clic en el icono de "La lupa" |icone_lupa_verde|. Como resultado de esta búsqueda aparecen sólo los *Registry* que contengan la palabra llave buscada.
* **Añadir un Registry**: Basta hacer clic en el signo de suma |icone_adicionar| para que el usuario pueda registrar un nuevo *Registry* en la plataforma. A continuación, aparece la siguiente pantalla:

.. image:: /figuras/fig_mangue/193_mangue_criar_edit_secret.png
    :alt: Criar Editar Secret para Registry 
    :scale: 100 %
    :align: center
=====

* **Nombre del Servidor**: Este campo es obligatorio y el usuario debe informar el nombre del servidor de *Registry* que desea configurar en la plataforma Mangue.io.
* **Username**: Este campo es obligatorio y el usuario debe introducir el *login* de usuario previsto en el sistema operativo del servidor de *registry* existente;
* **Email**: Este campo es obligatorio y el usuario debe introducir la dirección de correo electrónico del usuario que se utiliza para realizar la autenticación en el servidor de *registry*;
* **Contraseña**: Este campo es obligatorio y el usuario debe informar la contraseña del *login* de usuario, aprovisionado en el sistema operativo del servidor, que es utilizado para hacer la autenticación de este usuario en el servidor de *registry*.
* **Nombre Secret**: Nombre del *Secret* a ser creado para los datos del Registry.
* **Botón**  ``Confirmar``: Después de que el usuario haya cambiado todos los campos anteriores, debe hacer clic con el cursor del ratón en este botón para Confirmar los cambios informados para la plataforma Mangue.io.

A continuación se describen las columnas presentadas en esta lista de *registries*:

.. image:: /figuras/fig_mangue/194_mangue_registry_lista.png
    :alt: Registry lista 
    :scale: 100 %
    :align: center
=====

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. 

    Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Esta columna presenta el nombre del servidor de Registro de imagen creado;
* **Username**: Esta columna presenta el nombre de usuario que se utiliza para realizar la autenticación en el servidor de registro de imagen;
* **Email**: Esta columna presenta la dirección de correo electrónico del usuario que se utiliza para realizar la autenticación en el servidor de registro de imagen;
* **Contraseña**: Esta columna presenta la contraseña del usuario que se utiliza para realizar la autenticación en el servidor de registro de imagen.
* **URL del Servidor**: Esta columna presenta la url que el usuario utiliza para autenticar y descargar las imágenes desde el servidor de registro de imagen;
* **Duración**:  Esta columna indica el tiempo que lleva creada esa credencial de acceso al servidor de registro de imágenes en la plataforma;
* **Acciones**: Esta columna presenta el botón de ``Acción`` |icone_acao| al ser pulsado, presenta dos opciones como la figura siguiente:

.. image:: /figuras/fig_mangue/195_mangue_acoes_registry.png
    :alt: Ações registry 
    :scale: 100 %
    :align: center
=====

      * **Eliminar  Registry**: Acción responsable de eliminar la credencial de acceso al servidor de registro de imagen. Al seleccionar este botón, la plataforma Mangue.io solicita que se confirme la eliminación de la credencial. Recuerde que una vez confirmada, esta acción es irreversible. Si alguna aplicación del *Cluster* utiliza esta credencial para descargar el *container docker*, después de la eliminación esta acción para descargar el *container docker* falla, ya que la credencial fue eliminada.

.. image:: /figuras/fig_mangue/196_mangue_deletar_registry.png
    :alt: Deletar Registry 
    :scale: 100 %
    :align: center
=====  

      * **Editar Registry**: Acción responsable de proporcionar un mecanismo para actualizar las informaciones de una credencial de acceso a un servidor de registro de imágenes. Al seleccionar la acción "Editar Registry", aparece una pantalla con las informaciones previamente añadidas para la credencial en cuestión, permitiendo modificar los campos deseados y al pulsar el botón ``Confirmar``, la credencial es actualizada. Una alerta con feedback para la acción de actualización se genera en la esquina superior derecha de la pantalla del navegador de Internet.

.. image:: /figuras/fig_mangue/197_mangue_criar_editar_secret.png
    :alt: Criar Editar Secret para Registry  
    :scale: 100 %
    :align: center
=====

* **Nombre del Servidor**: En este campo el usuario puede cambiar el nombre del servidor de *Registry* existente.
* **Username**: En este campo el usuario puede cambiar el nombre de usuario que se utiliza para realizar autenticación en el servidor de *registry* de imagen;
* **Email**: En este campo el usuario puede cambiar el correo electrónico del usuario que se utiliza para realizar la autenticación en el servidor de *registry*;
* **Contraseña**: En este campo el usuario puede cambiar la contraseña de usuario que se utiliza para realizar la autenticación en el servidor de *registry*.
* **Botón**  ``Confirmar``: Después de que el usuario haya cambiado todos los campos anteriores, debe hacer clic con el cursor del ratón en este botón para confirmar los cambios informados para la plataforma Mangue.io.

====

Secrets
=======

*Secrets* (secretos) permiten almacenar y gestionar informaciones consideradas confidenciales o sensibles, tales como: contraseñas, *tokens*, *OAuth* y claves SSH. Emplear esta información a través de un *secret* es el modo más seguro y flexible que "expone" la información, en una definición de ciclo de vida de *Pod* o en una imagen de *container*. Los valores de un secreto se guardan en *BASE64*.

.. note:: Base 64 es un método para codificación de datos para transferencia en Internet (codificación MIME para transferencia de contenidos). Se utiliza a menudo para transmitir datos binarios a través de medios de transmisión que sólo se ocupan del texto. 

No significa que haya una cierta "capa" de encriptación en las informaciones, adicionalmente este es el enfoque más recomendado para almacenar informaciones sensibles.

Al seleccionar este menú se presenta una lista de todos los *secrets* presentes en el *Cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración" de la plataforma Mangue.io.

.. image:: /figuras/fig_mangue/198_mangue_lista_segredos.png
    :alt: Lista Secret
    :scale: 100 %
    :align: center
=====

El menú *Secret* contiene una tabla con las siguientes informaciones:

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. 

    Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Esta columna presenta el nombre del *Secret* utilizado en el momento de su configuración.
* **Tipo**: Tipo de secreto.
* **Duración**: Esta columna presenta el tiempo (en días) transcurrido desde la creación de este *secret*.
* **Acciones**: Esta columna presenta el botón ``Acción``, que es una papelera |icone_lixo_vermelho| que al ser pulsado elimina el *secret* de la misma fila. Al seleccionar la acción ``Eliminar Secret`` la plataforma Mangue.io pide al usuario que confirme la acción.

.. image:: /figuras/fig_mangue/199_mangue_aviso_deletar.png
    :alt: Aviso deletar 
    :scale: 100 %
    :align: center
=====

Es importante destacar que esta acción es irreversible cuando se confirma. Cualquier *workload* del *cluster* que esté asociada o utilice este *secret* puede presentar un error fatal (*crash*) durante su ejecución.

Si el usuario necesita conocer los contenidos almacenados de un *secret*, debe hacer clic en el nombre del *secret* para que la plataforma Mangue.io presente las informaciones específicas configuradas para el *secret* en una sección debajo de la lista.

Esta nueva sección de la pantalla presenta la lista de todos los componentes de un secret.

Para cada componente del *secret*, la plataforma Mangue.io presenta un icono de visualización del contenido del componente del *secret*. Este icono se representa con "ojo" |icone_exibir|, cuando el usuario hace clic en el icono, la plataforma Mangue.io presenta el contenido del componente como el ejemplo siguiente:

.. image:: /figuras/fig_mangue/200_mangue_valores.png
    :alt: Valores 
    :scale: 100 %
    :align: center
=====

Cuando el usuario hace clic sobre el icono de visualización de nuevo, la plataforma Mangue.io cierra la presentación del contenido del *secret* de la pantalla.

====

Schedule Task
=============

La plataforma Mangue.io puede programar tareas para ser realizadas en una fecha posterior, tareas como: 

* Actualizar *Deployment*.
* Escalar *Deployment*.
* Actualizar *ConfigMap*.

.. image:: /figuras/fig_mangue/201_mangue_agenda_tarefa.png
    :alt: Agenda tarefas
    :scale: 100 %
    :align: center
=====

En la página de *Schedule Task* se muestra una lista de las tareas programadas en la plataforma, también es posible buscar las tareas programadas por el nombre del recurso.

A continuación se describen las informaciones presentes en la tabla de tareas programadas.

* **#**: Número secuencial del *VS Code* registrado en la plataforma Mangue.io.
* **Fecha Programada**: Fecha para la que la tarea ha sido programada;
* **Tipo**: Tipo de tarea a ser realizada.
* **Detalles**: Detalles sobre la tarea a ser realizada.
* **Acciones**: Esta columna presenta el botón de ``Acción``, al ser pulsado, muestra las siguientes opciones:

.. image:: /figuras/fig_mangue/202_mangue_acoes_agendamento.png
    :alt: Ações agendamento
    :scale: 100 %
    :align: center
=====

      * **Editar Programación**: Al seleccionar la opción de edición, se presenta la pantalla con las informaciones de programación y es posible editarlas.

      * **Cancelar Programación**: Al seleccionar la opción de cancelar la programación, la fecha deseada es eliminada de la plataforma.

.. image:: /figuras/fig_mangue/203_mangue_agendar_tarefa.png
    :alt: Agendar tarefas 
    :scale: 100 %
    :align: center
=====


Para crear una tarea programada es necesario hacer clic en el botón de suma |icone_adicionar|  y es necesario rellenar los campos siguientes:

* **Fecha de Actualización**: Fecha y hora en que es ejecutada la tarea.
* **Tipo de Tarea**: Tipo de tarea a ser realizada, las opciones son:

      * Actualizar *Deployment*;

      * Escalar *Deployment*;

      * Actualizar *ConfigMap*.

.. image:: /figuras/fig_mangue/204_mangue_deployment.png
    :alt: Deployment
    :scale: 100 %
    :align: center
=====


En caso de seleccionar la opción de “Actualizar *Deployment*”, es necesario rellenar los nuevos campos, según la figura de arriba, de: 

* **Deployment**: El usuario debe seleccionar el *deployment* a ser actualizado. 
* **Nombre del Container**: El nombre del *container* a ser actualizado.
* **Versión del Container**: Versión para la cual el *Container* es actualizado.

.. image:: /figuras/fig_mangue/205_mangue_deployment_opcoes.png
    :alt: Deployment opções 
    :scale: 100 %
    :align: center
=====

Si se selecciona la opción de  ``Escalar Deployment``, es imprescindible rellenar los nuevos campos, según la figura de arriba: 

* **Deployment**: El usuario debe seleccionar el *Deployment* a ser actualizado.
* **Réplicas**: Cantidad de réplicas a las cuales el *Deployment* es escalado.

.. image:: /figuras/fig_mangue/206_mangue_configmap.png
    :alt: Configmap mapeando
    :scale: 100 %
    :align: center
=====

Si se selecciona la opción  ``Actualizar ConfigMap``, es necesario rellenar los nuevos campos, como se muestra en la figura de arriba, de:

* **ConfigMap**: El usuario debe seleccionar el *ConfigMap* que es actualizado.
* **Nombre del ConfigMap**: El usuario debe rellenar con el nombre del ConfigMap deseado.

Es posible añadir o eliminar archivos haciendo clic en los iconos |icone_adicionar_vermelho| y |icone_lixo_vermelho| respectivamente.

Los campos de un archivo *ConfigMap* son:

* **Nombre del Archivo**: El usuario debe introducir el nombre del archivo que es creado en el sistema operativo de la máquina virtual que utiliza ConfigMap.
* **Contenido del Archivo**: El usuario debe rellenar con el contenido específico del archivo a ser creado.

====

Storage
=======

Tratar con aplicaciones en *containers* tiene algunos desafíos, y uno de estos desafíos es cómo interactuar con los archivos en disco. Los archivos en disco de un *container* son efímeros, esto representa algunos problemas para aplicaciones no triviales empaquetadas en *containers*. 

Primero, cuando un *container* falla, el Mangue.io intenta reiniciarlo, pero los archivos en el disco se pierden, así el *container* empieza siempre con un estado limpio. 

En segundo lugar, cuando se ejecutan *containers* juntos en un *Pod*, generalmente es necesario compartir archivos entre esos *containers*. 

La abstracción de volumen de *Kubernetes* utilizada en Mangue.io resuelve estos dos problemas (para el ambiente Docker es diferente El Docker también tiene un concepto de volúmenes, aunque es un poco más flexible y menos gestionado. En Docker, un volumen es simplemente un directorio en el disco o en otro container.).

Por otro lado, un volumen de *Kubernetes* (utilizado por Mangue.io) tiene un tiempo de vida explícito, el mismo que el *Pod* que lo contiene. En consecuencia, un volumen supera a todos los *containers* que se ejecutan en el *Pod* y los datos se conservan en las reiniciaciones de ese mismo *container*. Naturalmente, cuando un *Pod* deja de existir, el volumen también deja de existir. Y quizás lo más importante, ya que *Kubernetes* soporta muchos tipos de volúmenes, y un *Pod* puede usar cualquier número de ellos simultáneamente, la plataforma Mangue.io también ha heredado esta capacidad. 

En su esencia, un Volumen es sólo un directorio, posiblemente con algunos datos, que son accesibles a los *containers* en un *Pod*. El directorio es la "ubicación", y su "contenido" está determinado por el tipo de volumen específico utilizado.

En la sesión de *Storage* el usuario encuentra los menús relacionados con la estructura del almacenamiento de datos persistentes en *Kubernetes*. Es posible navegar por tres estructuras diferentes:

* *StorageClass*
* *Persistent Volumes*
* *Persistent Volume Claims*

====

StorageClass
-------------

*StorageClass* son responsables de crear clases de *storage* de diferentes tipos, podemos ver el siguiente escenario como ejemplo:

    a. Un usuario tiene dos tipos de discos montados en dos *NFS servers* diferentes y desea utilizar el disco con más potencial de lectura y escritura para un tipo de aplicación y el disco con menos potencial de lectura y escritura para las otras aplicaciones.

    b. De este modo, el usuario debe crear dos *StorageClass* diferentes, cada un representa a un servidor *NFS*: uno para el disco que tiene el potencial de lectura y escritura más rápido y otro para el disco que tiene el potencial de lectura y escritura más bajo.

Cuando el usuario seleccionar el menú *Storage/StorageClass* la plataforma Mangue.io presenta la lista de todos los *StorageClass* que existen configurados en el *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem|  "Selección de configuración" de la plataforma Mangue.io. 

.. image:: /figuras/fig_mangue/207_mangue_storageclass.png
    :alt: StorageClass
    :scale: 100 %
    :align: center
=====

Las columnas de esta lista se describen a continuación:

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. 

    Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Nombre del *StorageClass*.
* **Provisioner**: Nombre del aprovisionador del *StorageClass*.
* **Duración**: Describe desde cuándo ha sido creado el recurso.
* **Acciones**: Esta columna presenta el botón de ``Acción``  |icone_acao| al ser pulsado, presenta la opción de eliminar el *StorageClass* seleccionado:

.. image:: /figuras/fig_mangue/208_mangue_deletar_storageclass.png
    :alt: Deletar StorageClass
    :scale: 100 %
    :align: center
=====

* Al seleccionar la acción ``Eliminar StorageClass``, la plataforma Mangue.io solicita al usuario la confirmación de la acción.

.. image:: /figuras/fig_mangue/209_mangue_aviso_deletar.png
    :alt: Aviso deletar
    :scale: 100 %
    :align: center
=====

Es importante destacar que esta acción es irreversible cuando se confirma. Cualquier *workload* del *cluster* que esté asociada, o utilice, a este *StorageClass*, puede presentar un erro fatal (*crash*) durante su ejecución.

====

PersistentVolume
----------------

*PersistentVolumes* (PV) es una porción del almacenamiento en el *cluster* que ha sido aprovisionado por un administrador o dinámicamente usando *StorageClass*. Es un recurso del *cluster*, al igual que un *node*. PVs son *plugins* de volumen como el recurso Volumes, pero tienen un ciclo de vida independiente de cualquier *Pod* individual que utilice el PV.

Cuando el usuario selecciona el menú *Storage/PersistentVolume* la plataforma Mangue.io presenta la lista de todos los *PersistentVolumes* que existen configurados en el *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración" de la plataforma Mangue.io. 

.. image:: /figuras/fig_mangue/210_mangue_pv.png
    :alt: Persistent volumes
    :scale: 100 %
    :align: center
=====  

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. 

    Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Capacity**: Esta columna presenta el tamaño/capacidad del *PersistentVolume* en Gigabytes.
* **Access Modes**: Esta columna presenta la configuración de acceso para este volumen, estos modos de acceso pueden ser tres, son:

      * **ReadWriteOnce**: El volumen es montado y puede recibir instrucciones de lectura y escritura sólo desde un único *node*.

      * **ReadOnlyMany**: El volumen es montado y tiene permiso solo de lectura, pero desde diferentes *nodes* simultáneamente, no se permite escritura.

      * **ReadWriteMany**: El volumen es montado y puede recibir instrucciones de lectura y escritura simultáneamente, pero desde diferentes *nodes*.

* **Reclaim Policy**: Cuando un usuario termina su volumen, puede eliminar los objetos de *Persistent Volumes Claim* de la API que permite recuperar el recurso (*reclaim*). La política de recuperación de un *PersistentVolume* indica al *cluster* que debe hacer con el volumen después de que se libere de su reivindicación. Actualmente hay tres políticas de recuperación:

      * **Retain**: La política (*retain*) permite la recuperación manual del recurso. Cuando se elimina el *PersistentVolumeClaim*, él sigue existiendo y el volumen se considera "liberado". Pero sigue sin estar disponible para otra reclamación porque los datos del reclamante anterior permanecen en el volumen.

      * **Delete**: En el caso de los volúmenes que admiten la política de recuperación de eliminación, esto elimina el objeto *PersistentVolume* de *Kubernetes*, así como el archivo de almacenamiento asociado en la infraestructura externa (por ejemplo, un volumen *AWS* *EBS*, *GCP PD* o *Azure Disk*).

      * **Recycle**: En esta última opción, la política de recuperación de un *PersistentVolume* permite al cluster realizar una limpieza básica.
 
* **Status**: Esta columna presenta la situación actual (*status*) de la solicitud de volumen, hay dos estados que se pueden mostrar:

      * **Bound**: Cuando las vinculaciones (*binding*) del tamaño del volumen corresponden al espacio designado en el ambiente computacional del *node*.

      * **Unbound**: Cuando las vinculaciones (*binding*) del tamaño del volumen no corresponden al espacio designado en el ambiente computacional del *node*.

* **StorageClass**: Esta columna presenta el nombre del *StorageClass* al que está asociado el *PersistentVolume*.
* **Age**: Esta columna presenta el tiempo (en días) transcurridos desde la creación de este *PersistentVolume*.
* **Acciones**: Esta columna presenta el botón de ``Acción``  |icone_acao| al ser pulsado, presenta la opción de eliminar el volumen seleccionado:

.. image:: /figuras/fig_mangue/211_mangue_deletar_volume.png
    :alt: Deletar volume
    :scale: 100 %
    :align: center
=====

* Al seleccionar la acción ``Eliminar Volumen``, la plataforma Mangue.io solicita al usuario que confirme la acción.

.. image:: /figuras/fig_mangue/212_mangue_aviso_deletar.png
    :alt: Aviso deletar
    :scale: 100 %
    :align: center
=====

Es importante destacar que esta acción es irreversible cuando se confirma. Cualquier *workload* del *cluster* que está asociado, o utiliza, este *PersistentVolume* puede presentar un error fatal (*crash*) durante su ejecución.

====

PersistentVolumeClaims
----------------------

Los *PersistentVolumeClaims* (PVC) son una solicitud de almacenamiento por parte de un usuario. Es similar a un *pod*. Los *pods* consumen recursos de los *nodes* y los PVCs consumen recursos PV. 

Los *pods* pueden solicitar niveles específicos de recursos (CPU y memoria). Los PVCs pueden solicitar tamaños específicos de almacenamiento y modos de acceso (por ejemplo, pueden ser montados *ReadWriteOnce*, *ReadOnlyMany*, o *ReadWriteMany*).

El menú *Storage/Persistent Volume Claims* muestra todos los PVCs presentes en un determinado *namespace* del *cluster*, la tabla presenta informaciones como:

.. image:: /figuras/fig_mangue/213_mangue_pvc.png
    :alt: Persistent volume claim
    :scale: 100 %
    :align: center
=====

* **# columna accionable**: Esta columna presenta una forma alternativa de eliminar (borrar) varias filas con un solo comando. 

    Cada fila está representada por un icono seleccionable |uCloud_icone_coluna_acionavel|. 

    Cuando el usuario elige una fila, o varias, la plataforma Mangue.io presenta el (los) icono(s) encima de esta columna, que representan acciones al usuario para ser ejecutadas de una sola vez para todas las filas seleccionadas. 

    En este caso es mostra el icono de "Papelera" |icone_lixo_vermelho| que permite eliminar todos los elementos indicados por el usuario con un solo comando;

* **Nombre**: Responsable de identificar el nombre del PVC. 
* **Capacidad**: Esta columna presenta el tamaño/capacidad del *PersistentVolumeClaim* en *Gigabytes*.
* **Status**: Se encarga de identificar el estado del PVC, generalmente pueden ser los siguientes estados:

      * **Bound**: Cuando el PVC fue creado con éxito.

      * **Pending**: Cuando está a la espera de alguna instrucción para que sea creada con éxito.

      * **Terminating**: Cuando está a la espera de alguna instrucción para que sea eliminado con éxito.

* **Provisioner**: Responsable por identificar cual *StorageClass* está usando el PVC.
* **Duración**: Esta columna presenta el tiempo (en días) transcurridos desde la creación de este PersistentVolume.
* **Acciones**: Esta columna presenta el botón de ``Acción`` |icone_acao| al ser pulsado, muestra la opción de eliminar el PVC seleccionado:

.. image:: /figuras/fig_mangue/211_mangue_deletar_volume.png
    :alt: Deletar volume
    :scale: 100 %
    :align: center
=====

* Al seleccionar la acción  ``Eliminar Volumen``, la plataforma Mangue.io solicita al usuario que confirme la acción.

.. image:: /figuras/fig_mangue/212_mangue_aviso_deletar.png
    :alt: Aviso deletar
    :scale: 100 %
    :align: center
=====

Es importante destacar que esta acción es irreversible cuando se confirma. Cualquier *workload* del *cluster* que está asociado, o utiliza, este *PersistentVolumeClaim* puede presentar un error fatal (*crash*) durante su ejecución.

====

Tareas
======

La plataforma Mangue.io es un ambiente que se comunica con el gestor de *containers* *Kubernetes* a través de *API-Restful*, de forma que cada vez que el usuario añade o reconfigura un recurso a través de la interfaz de Mangue.io, la plataforma envía una "tarea" a través de *API-Restful* al *cluster* *Kubernetes* para que esta tarea se ejecute.

Al final del procesamiento de la tarea, la plataforma Mangue.io recibe un mensaje de retroalimentación/respuesta del gestor de *Kubernetes* y lo muestra al usuario en la tabla de la interfaz. A continuación, la pantalla de Tareas muestra un ejemplo:

.. image:: /figuras/fig_mangue/214_mangue_tarefas.png
    :alt: Tarefas
    :scale: 100 %
    :align: center
=====

En la lista podemos encontrar el *status* de las tareas referidas al *cluster* que fue seleccionado en la pestaña de engranajes |icone_engrenagem| "Selección de configuración" de la plataforma Mangue.io:

* **Operación**: En esta columna se presenta una descripción sucinta de la tarea que fue ejecutada por el usuario a través de la interfaz de Mangue.io.
* **Cluster**: Esta columna muestra la identificación del *cluster* en el que se produjo la tarea.
* **Usuario**: Esta columna muestra la identificación del usuario que se conectó a la plataforma y solicitó la acción en la interfaz de Mangue.io.
* **Detalles**: En esta columna se muestra un icono de una letra “i”, en las líneas en que la columna *status* tenga el estado *Failed*, la plataforma Mangue.io muestra un *pop-up* con detalles del resultado de la tarea. 

    El usuario debe situar el cursor del ratón sobre la letra “i” y la plataforma Mangue.io presenta una pantalla *pop-up* con el contenido del mensaje de error retornado por *Kubernetes* a la plataforma Mangue.io. Vea un ejemplo a continuación:

.. image:: /figuras/fig_mangue/215_mangue_info_status.png
    :alt: Info status
    :scale: 100 %
    :align: center
=====

* **Fecha de inicio**: Esta columna muestra la fecha y la hora en que ha sido creada la tarea en la plataforma Mangue.io. Para el formato de fecha la presentación es: día/mes/año (norma brasileña - DD/MM/AAAA), para el formato de hora es: hora, minuto y segundo (formato de 24 horas - HH:MM:SS).
* **Creado en**: Esta columna presenta la cantidad de días transcurridos desde la fecha de inicio de la tarea (columna anterior).
* **Status**: Esta columna presenta el contenido del mensaje de retorno/respuesta del gestor de *Kubernetes* y presenta esta respuesta al usuario en tres *status* diferentes:

      * **SUCCESS**: Tarea enviada para *Kubernetes* y procesada con éxito;

      * **PENDING**: Tarea enviada para *Kubernetes* y está siendo procesada, hasta el momento no ha sido cerrada;

      * **FAILED**: La tarea enviada para *Kubernetes* y su procesamiento ha generado error/fallo durante el intento de la ejecución. 

Encima de la tabla, hay tres elementos con los que el usuario puede actuar:

.. image:: /figuras/fig_mangue/192_mangue_pesquisar_registry.png
    :alt: Pesquisar registry
    :scale: 100 %
    :align: center
=====

* **Acción de Búsqueda**: Si la lista presentada en esta pantalla es muy larga (más de una página), hay un campo donde el usuario puede buscar por parte del texto en la columna “Operación”. 

    Sólo tiene que introducir parte del nombre de la operación y pulsar “Enter”, o hacer clic en el icono de "Lupa" |icone_lupa_verde|. Como resultado de esta búsqueda, sólo apareceren las líneas que contengan la palabra clave de la búsqueda.

    Esta búsqueda distingue entre mayúsculas y minúsculas, de forma que el resultado de la búsqueda de la palabra “Eliminar” es diferente del resultado de la búsqueda de la palabra “eliminar”.

    Si la búsqueda no retorna ninguna incidencia, la lista aparece en blanco. Para volver a la lista inicial, el usuario debe borrar cualquier contenido/*string* de este campo, y hacer clic en el icono de "La lupa" |icone_lupa_verde| (buscar por el campo 'en blanco') y la plataforma Mangue.io presenta el contenido completo de la lista antes de cualquier búsqueda.

* **Acción de actualizar**: Basta hacer clic en el icono |icone_update| para que Mangue.io actualice la interfaz con el *status* más reciente de esta tabla de tareas.

====

Clusters Workloads
==================

Esta opción del menú lista todas las cargas de trabajo (*workloads*) existentes en todos los *clusters* integrados a la plataforma Mangue.io.

En primer lugar, es pertinente aclarar qué es exactamente una carga de trabajo (*workload*). En *Kubernetes*, no hay ningún objeto, componente o cualquier tipo de construcción llamada “carga de trabajo”. 

Sin embargo, el término se utiliza a menudo como una categoría general para las tareas y servicios que el usuario desea ejecutar en su *cluster*. Puede ser sinónimo de microservicios, aplicaciones, *containers* o procesos. Las cargas de trabajo, por lo general, son procesos de larga duración, pero también pueden ser de corta duración bajo demanda o *jobs* en lote.

La plataforma Mangue.io puede gestionar varios componentes que *Kubernetes* ofrece para gestionar y configurar sus cargas de trabajo. Se pueden listar los *pods* y los componentes que encapsulan los *pods*, como *ReplicaSets*, *Deployments*, *DaemonSets* y *StatefulSets*. 

A continuación, se detallan los componentes periféricos, como Servicios, *EndPoints* y *Ingress*.
Como se trata de un número muy grande de componentes, esta lista puede ser muy larga. A continuación se muestra un ejemplo de uno de estos componentes que aparecen en la pantalla:

.. image:: /figuras/fig_mangue/216_mangue_workloads.png
    :alt: Workloads
    :scale: 100 %
    :align: center
=====

* **# columna accionable**: Esta columna muestra el número secuencial *workload* en la lista presentada.
* **Nombre**: Esta columna muestra el nombre *workload* que fue creado durante el proceso de inclusión de este componente en la plataforma Mangue.io.
* **Tipo**: Esta columna presenta el tipo específico de componente(s) *workload(s)*.

      * *Deployments*

      * *Daemonsets*

      * *Horizontal Autoscaler*

      * *Pods*

      * *Statefulsets*

      * *Updates*

* **Réplicas**: Esta columna presenta la cantidad de réplicas activas que tiene este componente en el momento de la consulta.
* **Cluster**: Esta columna presenta el nombre del *cluster* al que está asociado el componente. La plataforma Mangue.io presenta todos los *clusters* con los que tiene configuración de integración.
* **Namespace**: Esta columna presenta el nombre del *namespace* al que está asociado el componente.

Si el usuario necesita visualizar todas las informaciones detalladas de un componente presente en la lista, basta hacer clic con el cursor del ratón sobre el nombre del componente y la plataforma Mangue.io presenta las mismas informaciones presentes en el menú *Workloads* (ejemplo de informaciones de un *deployment* abajo):

.. image:: /figuras/fig_mangue/217_mangue_deployment_info.png
    :alt: 
    :scale: 100 %
    :align: center
=====

Conclusión
==========

Este documento concluye la presentación y descripción del Mangue.io, una plataforma de Gestión de Ambientes de Múltiples Orquestadores de *Container* que entrega de forma continua, ágil, segura y productiva, las aplicaciones dirigidas a la implementación, pruebas y actualizaciones con *downtime* cero y *rollback* de *deployments*. 

----

**Equipo Ustore**

Manual de uso Mangue.io Ed. 4 Año 2023









.. |icone_engrenagem| image:: /figuras/fig_mangue/icone_engrenagem.png

.. |icone_lixo| image:: /figuras/fig_mangue/icone_lixo.png

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

.. |icone_loadbalancer| image:: /figuras/fig_mangue/icone_loadbalancer.png

.. |icone_rotulo| image:: /figuras/fig_mangue/icone_rotulo.png

.. |icone_engrenagem_azul| image:: /figuras/fig_mangue/icone_engrenagem_azul.png

.. |icone_sync| image:: /figuras/fig_mangue/icone_sync.png