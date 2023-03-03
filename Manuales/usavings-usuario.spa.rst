

.. image:: /figuras/fig_usavings/uSavings_media_sfundo.png
    :alt: logo usavings
    :align: center
======

uSavings - Manual de Utilización
++++++++++++++++++++++++++++++++


Soluciones de tecnologías de la información que permiten implementar una arquitectura de cómputo escalable, sólida y confiable en una nube distribuida.


------


Presentación
============

Este documento tiene como objetivo presentar las principales características y funcionalidades relacionadas con la aplicación “uSavings”. 

Este manual presenta los conceptos, pantallas, funcionalidades y comandos para el uso de este producto.

----

Visión y posicionamiento
========================

Este documento describe la aplicación uSavings, la visión y posicionamiento del producto debe entenderse considerando que está en constante desarrollo y evolución. Como resultado, las pantallas presentadas en este documento pueden estar sujetas a cambios en cualquier momento debido al desarrollo del software.

La tendencia actual, cada vez más fuerte, de migración de recursos de cómputo desde nubes privadas o entornos de *co-ubicación*, hacia el entorno de proveedores de nube pública, representa uno de los grandes desafíos para las organizaciones, que es la Gobernanza de Costos derivada de el alto uso de estos recursos informáticos y, en consecuencia, las empresas no son capaces de obtener las visiones adecuadas de estos costos en el futuro.

Actualmente, casi todas las plataformas de *Cloud Service Broker (CSB)* pueden presentar sugerencias de reducción de costos, sin embargo, la obtención de algunos valores depende de un servicio humano (o acción) para obtener dichos valores.

Los proveedores de servicios de nube pública proporcionan continua e ininterrumpidamente nuevas configuraciones de hardware (*flavor*) con características similares, pero a veces valores muy diferentes. 

En este punto, depende de un especialista en arquitectura buscar configuraciones de hardware posibles y compatibles.

La plataforma uSavings automáticamente completa estas actividades para que las comparaciones de configuraciones de hardware y/o costos recurrentes puedan presentarse más claramente al usuario de esta plataforma.

La plataforma uSavings realiza un inventario de todos los recursos de computación en la nube pública a través de su integración con la plataforma uCloud . Por lo tanto, la lista de recursos computacionales del servidor que se presenta en la interfaz de la Plataforma uSavings es una representación fiel de su entorno que se encuentra en el proveedor de servicios de nube pública, por lo tanto, la realidad existente en su entorno.

Todas las opciones alternativas de configuración de hardware se informan como **sugerencias**, ya que depende del usuario cambiar (reconfigurar) el hardware del recurso computacional (*flavor* ) en el mejor momento para su entorno.

Importante señalar que la Plataforma uSaving solo presenta **sugerencias**, ya que cualquier cambio de configuración de hardware (*flavor*) solo podrá realizarse con la infraestructura apagada (**fría**), de esta forma, el usuario debe gestionar el mejor momento (día y hora) para actuar sobre este cambio de configuración.

La integración con la Plataforma uCloud, permite al usuario visualizar las sugerencias presentadas en la interfaz de la Plataforma uSavings, para que pueda identificar correctamente el recurso computacional, y, a través de la Plataforma uCloud, ejecutar la tarea de cambiar la configuración del hardware (*flavor*) directamente en el entorno del proveedor de servicios de nube pública, sin necesidad de que el usuario inicie sesión en la consola del proveedor de nube pública.

====


¿ Qué es uSavings ?
-------------------

El uSavings es una herramienta que analiza en tiempo real el consumo de infraestructura de recursos de cómputo (máquinas virtuales, abreviadas como VMs) en las diferentes nubes, es a través de este análisis que la aplicación recomienda modificaciones. 

En caso de que la organización acepte o apoye esta sugerencia, tal decisión puede permitir el máximo ahorro financiero y la optimización de los recursos creados y/o ejecutados. 

La aplicación uSavings es un “cost advisor", es decir, un consultor de costos que le permite asesorar al usuario sobre cómo reducir los costos de su infraestructura, lanzada por la Plataforma uCloud, a través de diferentes proveedores de servicios en la nube - AWS, Azure, Google, IBM y VMWare.


====


¿ Cómo funciona ?
-----------------

La plataforma de uSavings obtiene y extrae información de los datos históricos de la Virtual Machine, es decir, desde la máquina virtual y desde el lanzamiento de cada proveedor de nube pública – la recopilación de estos datos comienza con la integración a la Plataforma del uCloud. 

La aplicación presenta un *Dashboard* consolidado y sugerencias de gasto de los clientes en cada proveedor de la nube, entregando así información precisa para una mejor toma de decisiones sobre los costos asignados de los recursos de infraestructura de la organización.

.. image:: /figuras/fig_usavings/001_organogram_usavings_usage.png
    :alt: organigrama operativo usavings
    :align: center
====

La imagen de arriba representa el organigrama de uSavings: en él, la máquina virtual de uCloud, es uno de los elementos principales de este flujo, como se muestra en el diagrama anterior. 


El siguiente elemento presentado es *Flavor*, permite saber cuánta memoria, vCPU y otros recursos son utilizados por la máquina. 

Por lo tanto, es desde el *Flavor* que sabes cuánto costa una máquina, en particular, a fin de mes. Con estos datos, es posible que la plataforma uSavings sugiera al cliente ahorros de recursos en la factura mensual.

.. image:: /figuras/fig_usavings/002_recorte_organograma.png 
    :alt: recorte del organigrama de usavings
    :align: center
==== 

El recorte en el organigrama, resalta la parte relevante del diagrama, representa la forma sugerente de la aplicación uSavings. 

Hay dos maneras de recomendar mejoras para una máquina virtual determinada: (i) por Flavor y (ii) por facturación.

* **Por Flavor** - uSavings verifica el *Flavor* asignado en la máquina y sugiere una posibilidad de mejora - esta mejora está relacionada con el costo beneficio - la aplicación publica los resultados en diferentes formatos (gráficos o porcentajes) y muestra cuál es el mejor cloud a se utilizar para ahorrar recursos, para la máquina virtual. Este parámetro, por deducción, significa que la máquina está encendida todo el tiempo.

* **Por Billing** - La facturación de la base de datos de uCloud admite múltiples nubes, difiere del alcance de la aplicación uSavings. La base de datos de uCloud puede admitir todos los tipos de billing disponibles. En la regla de negocio uSavings solo es posible realizar una sugerencia asertiva con billing para AWS y AZURE, como se muestra en la figura recortada de el diagrama, presentado arriba de este párrafo.


====


¿ Cómo ahorrar recursos ?
-------------------------

La ventaja de implementar uSavings en las organizaciones es la posibilidad de recibir información sobre recursos ociosos que fueron creados, e incluso ejecutados antes, actualmente no utilizados. Información que puede hacer posible el ahorro de recursos.

Debido a que la aplicación uSavings es una herramienta que analiza en tiempo real el consumo de la infraestructura de recursos de cómputo en las diferentes nubes, la aplicación uSavings muestra los recursos ociosos creados.

La herramienta es relevante para la toma de decisiones en las organizaciones, ya que al analizar la información que obtiene, la aplicación entrega resultados reales. Esto contribuye a una decisión organizacional capaz de generar ahorros financieros y optimizar los recursos creados y/o ejecutados.

La aplicación uSavings puede hacer referencia a sugerencias de reducción de configuración – *‘rightsizing’* de máquinas virtuales, si fueron creadas previamente con ‘super configuraciones’ y/o presentan un bajo consumo en el historial de rendimiento. **Dirige** la posibilidad de ampliar la relación costo-consumo, **no ejecutarla**. 

El propósito de implementar la plataforma uSavings es indicarle a la organización la posibilidad y/o camino para incrementar su ahorro de costos, en el 
próximo período de facturación del proveedor de servicios en la nube.

.. attention:: La organización a la que se le proporcionó la información, proporcionada por la aplicación uSavings, debe comunicarse con el proveedor de servicios en la nube para obtener información sobre el *‘rightsizing’*.

Al adquirir la plataforma uSavings, las organizaciones pueden tener a mano una valiosa herramienta estratégica y de inteligencia de negocios (*Business Inteligence*) que les indica la mejor manera de incrementar la relación “costo-beneficio” de sus infraestructuras virtuales y también la mejor forma de maximizar los recursos de las mismas máquinas creadas en proveedores de servicios en la nube.



Optimizaciones recomendadas después del monitoreo
-------------------------------------------------

Se pueden proponer las siguientes optimizaciones con base en las sugerencias de:

Rightsizing :
~~~~~~~~~~~

Consiste en sugerir la mejor combinación de CPU y memoria, con el objetivo de minimizar costos y maximizar el rendimiento. La herramienta recopila métricas de rendimiento para determinar el consumo de recursos promedio y máximo de una instancia durante un período de tiempo elegido, y recomienda una modificación a un tipo de configuración de máquina virtual 'VM', sea menos compuesto o apropiado para el proyecto.

Costos Comparativos :
-------------------

Presenta al usuario la lista actual de sus máquinas virtuales y una sugerencia de cuál sería la 'mejor configuración' en cada proveedor de nube. Permite al usuario evaluar qué proveedor tiene el costo más bajo en una determinada máquina virtual, en la fecha en que se obtuvo el valor 
de este costo.

Monitorear Recursos Ociosos :
-----------------------------

Supervisar los recursos inactivos, le permite comprobar si los recursos están en uso. El usuario-cliente puede monitorear los recursos creados y no utilizados.

Instancias Reservadas :
---------------------

Sobre la instancia reservada, la aplicación uSavings puede mostrarle al usuario-cliente que en el caso de cambiar de una máquina *on-demand* a una máquina reservada, la instancia reservada puede mostrar cuánto es posible ahorrar con relación a la máquina actual.

**Por ejemplo :**

Al utilizar el proveedor de AWS, las Instancias reservadas (*Reserved Instances - RIs*) de la *Amazon EC2* son una de las formas más obvias de controlar los costos de cómputo, lo que permite al usuario reservar capacidad de cómputo *EC2* a cambio de tarifas por hora significativamente reducidas.

Es importante señalar y reforzar al cliente/usuario que las Instancias reservadas (AWS, AZURE o instancia previa Google) no son instancias que el usuario pueda crear y ejecutar por un precio más bajo que las instancias normales. Y debe tenerse en cuenta que, no hay garantía de que estos 
servicios informáticos estén dedicados al cliente, o estén disponibles y accesibles los 365 días del año.

Si el proveedor de servicios en la nube necesita tener acceso a estos recursos informáticos, para otro tipo de tarea, el proveedor puede terminar estas instancias en cualquier momento (es decir, forzar la interrupción de estas maquinas virtuales) sin comunicación previa.

----

Menú inicial
============

La interfaz inicial que se presenta al usuario es un *Dashboard* que muestra un resumen de la infraestructura actual, direccionable y accesible a través de la plataforma uCloud. Al acceder a la interfaz de uSavings, el usuario se conecta automáticamente a sus 'VMs' de infraestructura de máquina virtual actual. 

De esta forma, el usuario visualiza los costes actuales de las máquinas virtuales existentes, puede comparar los costes de sus máquinas virtuales entre los distintos proveedores de servicios de infraestructura de nube pública.

El uSavings permite crear manualmente una lista de máquinas virtuales con configuraciones específicas (una configuración privada y/o 'imaginaria'), en el caso del usuario que quiera obtener la lista completa de sus máquinas virtuales y prefiera conectarse manual.

====


¿ Cómo acceder a la plataforma uSavings ?
-----------------------------------------

El acceso a la plataforma uSavings se realiza a través de la web, y se puede utilizar cualquiera de los navegadores: **Firefox**, **Google Chrome** o **Microsoft Edge**, en varios sistemas operativos, como **Microsoft Windows** 10 o 11.

.. attention::
    "Es importante señalar que la Plataforma uCloud no es compatible con Microsoft Internet Explorer (IE) en ninguna versión, ya que las tecnologías de este navegador están desactualizadas y no soportan la evolución de las páginas HTML actuales."

Para el acceso inicial, es necesario solicitar las credenciales al administrador - al recibir el enlace con la dirección y las credenciales de acceso, el usuario deberá utilizar su navegador preferido para acceder a la web y conectarse. Otra forma de acceder a la plataforma uSavings es directamente desde la plataforma uCloud, a través de su menú lateral izquierdo.

En caso de que el acceso se realice directamente en la web, se le mostra al usuario la imagen a continuación. En este momento debe ingresar las credenciales recibidas.

.. image:: /figuras/fig_usavings/003_tela_acesso_inicial.png 
    :alt: pantalla de login
    :align: center
====

El usuario debe llenar los campos de **‘login’** y **‘senha’**, con las credenciales recibidas del administrador de la plataforma. Haga clic en **'Entrar'**. Después de este procedimiento, se presenta la pantalla del *Dashboard*.

Si la pantalla del *Dashboard* no se muestra, significa que algunos de los campos están llenos de información inconsistente, es decir, *‘login‘* o ‘contraseña’ no existe y/o puede haber un error al escribir la información. Es importante comprobar y repetir la operación.

.. image:: /figuras/fig_usavings/004_tela_problema_acesso.png 
    :alt: pantalla de problema de acesso 
    :align: center
----

En caso de no poder iniciar sesión, se le presenta al usuario la imagen anterior, con la siguiente orientación: **(i)** verifique las credenciales y **(ii)** repita la operación.


====


Visión general
==============

En primer lugar, antes de ingresar a la sesión de Dashboard, es importante comprender el impacto de algunas herramientas existentes en el menú superior.

.. image:: /figuras/fig_usavings/005_recorte_menu_superior.png 
    :alt: recorte del menú superior
    :align: center
----

Para esto, en el recorte del menú superior, que se muestra arriba, se muestran los componentes relevantes, descritos en detalle a continuación, en orden: de izquierda a derecha.


Icono de Intercambio de Contrato
--------------------------------

Este icono |icone_ustore| es un punto relevante para realizar una reserva, partiendo de la premisa de que existe la posibilidad de que un usuario registrado en el uCloud ser parte de un grupo de usuarios. Por lo tanto, puede ser parte de más de un contrato. Y existe la posibilidad de seleccionar otro contrato, este contrato seleccionado puede contener otras características vinculadas a este contrato.

.. image:: /figuras/fig_usavings/006_troca_contrato.png 
    :alt: icono de intercambio de contrato
    :align: center
----

Este ícono de intercambio de contratos muestra todos los contratos en los que participa el usuario que inició sesión en la plataforma uSavings. Por lo tanto, el usuario puede cambiar entre ellos libremente. 

El intercambio de contrato puede implicar el intercambio de recursos que se presentan al usuario, ya que cada contrato puede tener una característica determinada, en la secuencia de este manual de usuario de uSavings se describe estos detalles.


Icono de configuración de Clouds
--------------------------------

Como introducción a la usabilidad de este fragmento de pantalla: |icone_configuracao|

Se puede decir que el término Clouds se utiliza para abstraer una agrupación de Flavors de una Cloud en particular de una nube en particular, siendo esto una agrupación de *Flavors* tanto reales como imaginarios.

.. image:: /figuras/fig_usavings/007_configuracoes_clouds.png 
    :alt: configuración de clouds
    :align: center
----

En el menú de configuración, hay una parte para la creación de *Clouds*, cambiar la actividad de *Clouds* y el área para crear nuevas *Clouds*.

.. image:: /figuras/fig_usavings/008_configuracao_alteracao_atividade.png 
    :alt: configuración de cambio de actividad
    :align: center
----

Icono Lista de cambios de idioma
--------------------------------

Este icono |icone_lista_troca_idioma| e permite cambiar el idioma en la plataforma uSavings, la 
plataforma originalmente está en portugués y se puede cambiar a español e inglés, solo haga clic en el icono con las banderas: |icone_bandeira_troca_idioma|

Icone Nombre de usuario logado
------------------------------

Este icono |icone_nome_usuario_logado| muestra el nombre de usuario que ha comenzado sesión en la plataforma uSavings. 

Icono de *LogOut*
-----------------

Este icono |icone_logout| desconecta al usuario de la plataforma.


Panel de control *Dashboard*
============================

La interfaz inicial de uSavings que se muestra al usuario es un panel de control *(Dashboard)*.

.. image:: /figuras/fig_usavings/009_menu_entrada_dashboard.png
    :alt: menú de entrada del dashboard
    :align: center
----

Este panel, imagen presentada arriba, muestra algunos datos en la pantalla que representa un resumen de la infraestructura direccionable actual accesible por la plataforma, estos datos están compuestos por segmentos llamados *Cards*.

.. image:: /figuras/fig_usavings/010_tela_inicial_dashboard_funcionalidades.png 
    :alt: pantalla de inicio: dashboard y caracteristicas
    :align: center
----

En la primera parte de la pantalla inicial, presentada en la imagen arriba, **solo se reflejan los servicios en la nube** que la organización **tiene en la plataforma uCloud** y **autoriza la integración**, el acceso por parte de la aplicación uSavings.

.. image:: /figuras/fig_usavings/011_container_conectado_plataforma_ucloud.png 
    :alt: contenedor conectado a la plataforma uCloud
    :align: center
----

En este caso, la imagen de lo contenedor conectado a la plataforma uCloud, muestra la lista de contenedores que participan en el contrato en el que se conecta el usuario. Esta autorización de acceso funciona desde el Acuerdo, como se muestra en el siguiente ejemplo:

.. note:: Cuando un contenedor particular de la plataforma uCloud está contenido en el Centro de Datos Virtual, que a su vez es parte de un contrato en el que participa el usuario que inició sesión en la plataforma uSavings.

De esta forma, se tiene acceso a los datos del contenedor, y solo después de este acceso y análisis de los datos, la plataforma uSavings puede sugerir mejoras de desempeño en uso.

El Dashboard permite una visualización rápida de cada una de las nubes conectadas a uCloud, las cuales se ven reflejadas en la aplicación uSavings. 

En caso de que la nube del usuario no se encuentre en uSavings, significa que la nube no se ha conectado a la plataforma uCloud.

A continuación, en este documento, se describen en detalle los cuatro cards que se muestran en la pantalla del Dashboard.

====


Latest Months
-------------

El primero *card* **Latest Months**, presenta la facturación ocurrida en el período relativo a los últimos seis (6) meses, es decir, se lista todos los montos invertidos en una determinada cuenta, para un período relativo a los últimos 6 meses.

.. image:: /figuras/fig_usavings/012_latest_months.png 
    :alt: Latest months
    :align: center
----

Este valor se recoge de valores generados por el *trabajo* uSavings, encargado de resumir la Billing de la plataforma uCloud.

.. image:: /figuras/fig_usavings/013_grafico_investimentos_real_versus_meses.png 
    :alt: grafico de inversiones en dolar x 6 ultimos meses 
    :align: center
----

El gráfico que se muestra en la imagen arriba presenta el valor del costo en Dólar versus el periodo requerido de los últimos 6 meses.

====



Consolidated Cost
-----------------

EL segundo *card* **Consolidated Cost** muestra algunas sugerencias en la pantalla del Dashboard, estas sugerencias están relacionadas con lo que contiene la máquina virtual “VM” seleccionada, es importante mencionar que todos los valores se presentan en dólares. 

La card muestra el *Flavor* y las regiones habilitadas para la máquina, la recopilación de esta información permite sugerir mejoras para optimizar su uso.

Este *card* detalla información sobre el porcentaje de ahorro, la diferencia de costos, el costo actual gastado, el costo optimizado y los *Flavors* utilizados y/o propuestos por la aplicación. Valores presentados en dólares.

.. image:: /figuras/fig_usavings/014_custos_consolidados.png 
    :alt: costos consolidados 
    :align: center
----

Al observar la imagen arriba, el porcentaje de 65,25% en el campo *Saving* representa el porcentaje de ahorro que la aplicación uSavings brinda como resultado, según la sugerencia cambiar *Flavor* dentro de la propia nube. 

Es decir, el usuario está realizando una búsqueda en la nube de AWS, los ahorros mostrados del 65,25% se pueden implementar al cambiar de *Flavor* dentro de la propia nube.

La información detallada en esta *Card* de costos consolidados presenta una gran cantidad de detalles para comprender la mejor combinación de CPU, memoria y disco, con un enfoque en la reducción de costos.

* **Saving** – Muestra el porcentaje de ahorro (en color verde) o gasto (en color rojo) en función del consumo actual y lo compara con las optimizaciones sugeridas;

* **Difference Cost** – Representa el mismo cálculo utilizado por Ahorro y revela la diferencia en Real (R$);

* **Current Cost** – Muestra el monto que se está gastando, en referencia al período en el que se recopiló el análisis.

* **Otimized Cost** – Indica el valor futuro si se aceptan e implementan los cambios sugeridos.

   * **Obs:** Todos los valores mostrados pueden cambiar durante el período, dependiendo del consumo traficado en las nubes.

====


Actual Flavor
-------------

Esta tercera *Card* presenta el *Flavor* de las máquinas seleccionadas de este contenedor, si se modifica carga la nueva información. La visualización de los porcentajes utilizados por *Flavor* se presenta mediante el gráfico circular y su representación ocurre por tipo, en el conjunto total de la infraestructura.

Todos los valores se muestran en dólares estadounidenses, sin gravamen de impuestos. Los precios provienen de la tabla importada directamente del proveedor de la nube e insertada en la base de datos de esta aplicación. El precio se calcula a partir del número de horas que componen el mes.

.. image:: /figuras/fig_usavings/015_grafico_actual_flavors.png 
    :alt: gráfico actual flavors 
    :align: center
----

La información contenida en la imagen arriba, se refiere al entorno de AWS, donde cada elemento difiere en términos de tamaño de memoria, vCPU, precio y sistema operativo y, al final, se presenta el valor del costo total de los *Flavors* que se utilizan actualmente.


====


Sugested Flavors
----------------

Este *Card* presenta otro tipo de gráfico, de la *Card Actual Flavors* demuestra cuánto sería la diferencia de la sugerencia de economía referenciada. Es decir, cuánto es posible ahorrar del recurso creado que está inactivo, al presentar la información de consumo actual y la sugerencia de consumo en un gráfico de columnas.

La columna azul representa el gasto corriente, la columna verde sugiere los ahorros que se pueden generar, en el caso de la aplicación de las sugerencias para mejorar el consumo de recursos presentadas por la plataforma uSavings.

.. image:: /figuras/fig_usavings/016_sugested_flavors.png 
    :alt: sugested flavors
    :align: center
----

Los gráficos y la información presentada son un **análisis inicial** del ahorro potencial de valores que la organización puede beneficiarse al adoptar las recomendaciones sugeridas por la plataforma uSavings.

Los valores presentados se refieren al período de recolección de datos (el intervalo mínimo inicial es de quince días). Cuanto más largo sea el tiempo de recopilación de información, más confiable está la estimación de ahorro calculada.

.. image:: /figuras/fig_usavings/017_tela_entrada_dashboard_1.2.png 
    :alt: pantalla de entrada dashboard (parte 1/2)
    :align: center
----

Este análisis inicial se calcula en función del uso, es decir, la ocupación de los recursos informáticos de las máquinas virtuales ‘VM’ dentro del periodo almacenado en la base de datos de la plataforma uSavings.

.. image:: /figuras/fig_usavings/018_tela_entrada_dashboard_2.2.png 
    :alt: pantalla de entrada dashboard (parte 2/2)
    :align: center
----

El resultado de este análisis es la sugerencia de la mejor combinación de CPU y memoria. Sugerencia dirigida a reducir costos y maximizar el rendimiento *(rightsizing)*. El análisis no hace el cálculo comparativo entre los valores de configuración de las máquinas virtuales ‘VMs’ en otros proveedores.

----

Menú Funcionalidades
====================

En el lado izquierdo del menú de entrada de la plataforma uSavings se enumeran los menús de funcionalidad, son: *Virtual Machines*, *Compare Clouds*, *Imaginary Cloud*, *Contenedor Hint* y el menú de acceso a la plataforma uCloud.

.. image:: /figuras/fig_usavings/019_submenu_funcionalidades.png
    :alt: submenú de funcionalidad
    :align: center
----

Virtual Machines
----------------

El menú Máquinas Virtuales muestra todas las máquinas virtuales en la infraestructura del usuario (es decir, el inventario de todas las máquinas virtuales ‘VMs’ de las cuentas que pertenecen a la organización).

.. image:: /figuras/fig_usavings/020_virtual_machines.png 
    :alt: maquinas virtuales
    :align: center
----

Esta vista permite la selección del contenedor específico para el análisis de costos y la sugerencia de cambio de *Flavor* en la misma nube que las máquinas virtuales enumeradas. Toda la información presentada se puede exportar en formato de informe csv.

.. image:: /figuras/fig_usavings/021_menu_virtual_machines.png 
    :alt: menú virtual machines
    :align: center
----

Es importante señalar que el contenedor apuntado debe estar contenido en uCloud, es decir, el contenedor a analizar debe estar conectado y sincronizado en la plataforma uCloud.

.. image:: /figuras/fig_usavings/022_selecionar_container.png
    :alt: seleccionar contenedor
    :align: center
----

Después de seleccionar el contenedor, la información se presenta en columnas, siguiendo el orden de la 1ª a la 6ª columna:

  * 1. el nombre de la máquina virtual;
  * 2. el *flavor* utilizado;
  * 3. se asigna el costo actual de la máquina si está encendida todo el mes;
  * 4. o flavor sugerido para la optimización;
  * 5. el costo mensual de flavor sugerido; 
  * 6. el valor anual de la máquina virtual.

.. image:: /figuras/fig_usavings/023_informacoes_container.png 
    :alt: información contenedor
    :align: center
----  

Las sugerencias mostradas *(Rightsizing)* se basan en el consumo CPU de máquinas virtuales, desde su creación hasta la actualidad. Se recopilan métricas y el cálculo se basa en promedios de consumo, luego se presenta la sugerencia.

El análisis del consumo de memoria puede ser parte del cálculo si el proveedor o las instancias están listos para proporcionar las métricas necesarias. Si la información no está disponible, se asume la memoria definida por el tipo (*flavor*) de la instancia implementada (*deployada*).

====


*Rightsizing* - sugerencia de cambio de *Flavor*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para recibir el resultado de la sugerencia de cambio de *Flavor*, el usuario debe seleccionar el contenedor deseado, como se muestra en la imagen seguiente. La aplicación uSavings genera el listado y la comparación de precios. Simplemente haga clic y espere.

.. image:: /figuras/fig_usavings/024_container_selecionado.png 
    :alt: contenedor seleccionado
    :align: center
----

Como resultado de esta operación, se desplega la imagem abajo, que muestra las diversas informaciones en bloques, tales como: *Flavor* y Costo Actual, Sugerencia de *Flavor* y el costo estimado de este nuevo *Flavor*. Finalmente, muestra el costo de reserva de *Flavor* estimado y sugerido para 1 año.

.. image:: /figuras/fig_usavings/025_resultado_estimado_selecao.png 
    :alt: resultado estimado en la seleción 
    :align: center
----

Caso de uso
~~~~~~~~~~~

Para comenzar el tutorial de este caso de uso, es importante recordar que las máquinas virtuales enumeradas provienen de la plataforma uCloud, por lo tanto, las nubes conectadas a uCloud deben contener las máquinas virtuales.

En caso de inexistencia de máquinas virtuales consultar el Manual de uCloud, en el tema: Cómo conectar e importar *Virtual Machine*.

**1º Paso :** 

Seleccione la nube *(contenedor)* que desea analizar.

.. image:: /figuras/fig_usavings/026_selecionar_nuvem_vm.png 
    :alt: seleccionar nube en vm 
    :align: center
----

**2º Paso :** 

Elija la región en la que se ejecuta la *Virtual Machine* seleccionada.

.. image:: /figuras/fig_usavings/027_selecionar_regiao_vm.png 
    :alt: seleccione región vm 
    :align: center
----

**3º Paso :** 

El resultado de la selección se muestra de acuerdo con la imagen *Resultado estimado en la seleción* posicionado sobre el tema de caso de uso, muestra la lista de todas las *Virtual Machines*. En esta misma pantalla, en la esquina superior derecha, puede exportar la lista de resultados en formato **.CSV**, simplemente haga clic en el botón **Export CSV**.

**4º Paso :**

Exporte el informe para verlo en una hoja de cálculo de Excel, en la máquina del usuario, el resultado esta similar a la imagen *Reporte exportado a Excel* presentado a continuación:

.. image:: /figuras/fig_usavings/028_relatorio_exportado_excel.png 
    :alt: reporte exportado a excel 
    :align: center
----

**5º Paso :**

Existe la opción de analizar la información de rendimiento, en la columna Rendimiento, como se destaca en la Figura 29. justo después de la columna Nome, la columna Performance muestra un icono con un símbolo * (asterisco). 

.. image:: /figuras/fig_usavings/029_coluna_performance.png 
    :alt: columna performance 
    :align: center
----

**6º Paso :** 

Al hacer clic en el icono * (asterisco), se muestra el informe de rendimiento:

.. image:: /figuras/fig_usavings/030_performance_maquinas.png 
    :alt: rendimiento de la maquina
    :align: center
----

El informe de rendimiento proporciona la visualización del gráfico con el consumo promedio de CPU y la memoria de la máquina virtual seleccionada, en un plazo aproximado de 15 a 20 días.


====



Compare Clouds
--------------

En la aplicación uSavings, la funcionalidad *“Compare Clouds”* permite realizar análisis comparativos. **Por Billing** o **Por Contenedor** de los costes entre la nube utilizada y las nubes elegidas para comparar.

.. image:: /figuras/fig_usavings/031_submenu_funcionalidades.png 
    :alt: submenú funcionalidad 
    :align: center
----

Para que las unidades estén disponibles, se requiere la integración con la plataforma uCloud, en este caso, las cuentas deben estar conectadas y sincronizadas, respetando las definiciones de las reglas de seguridad.

El *Compare Clouds* permite realizar análisis comparativos entre la propia nube, así como comparar con otras nubes. Además de comparar con nubes públicas que no están conectadas a la plataforma uCloud, como: IBM, AZURE, Google, AWS. 

Hay dos formas de realizar este análisis comparativo, comparar **por Billing** o **por Contenedor**.

.. image:: /figuras/fig_usavings/032_tela_inicial_compare_clouds.png 
    :alt: pantall de inicio compare clouds 
    :align: center
----

En la imagen arriba, se presentan dos barras con la posibilidad de realizar análisis comparativos:

* **Comparar por Billing** y 
* **Comparar por Contenedor**. 

Al hacer clic en la barra deseada, toma naranja, como se muestra en la imagen a continuación:

.. image:: /figuras/fig_usavings/033_selecao_compare_billing_compare_container.png 
    :alt: selección compare by billing o compare by container
    :align: center
----

Para reforzar, para que las unidades estén disponibles, **es fundamental** la integración con la plataforma uCloud.


====



Comparar por Billing
~~~~~~~~~~~~~~~~~~~~

Para permitir el análisis comparativo por Billing (Billetaje), es necesario que el emisor haya sido ejecutado en el contenedor indicado. Actualmente apoyamos, análisis comparativo por Billing a las nubes AWS y Azure, ver imagen arriba.

Antes de seleccionar el contenedor o nube a comparar, es necesario verificar si la plataforma de uCloud está emitido. Al menos uno (1) contenedor debe estar emitido y conectado a la plataforma uCloud.

.. note:: **Significado** do termo *ser emitido*: existe una factura de consumo en un período determinado, por lo menos (1) mes.   


====

   
**Paso a paso**

**1º Paso :** 

Para realizar el análisis comparativo, inicialmente, haga clic en el botón **Compare by Billing**. Verifique si la plataforma uCloud está emitida, al menos uno contenedor debe ser emitido y conectado a la plataforma.

====


**2º Paso :**

Seleccione la nube que contiene todos sus contenedors, Figura 34. Pulse en **AWS** o **AZURE**, luego haga pulse en **NEXT**.

.. image:: /figuras/fig_usavings/034_recorte_compare_billing.png 
    :alt: recorte compare by billing
    :align: center
----

En este caso, la nube **AWS** es seleccionado. Al presionar **NEXT**, la aplicación uSavings muestra la siguiente pantalla con la pregunta: «¿Qué nubes participarán en esta comparación?». Y pide al usuario que seleccione las nubes que quiere para realizar el análisis comparativo de los valores.

====


**3º Paso :**

Al seleccionar la nube, el usuario debe completar el período correspondiente al análisis en el calendario.

.. image:: /figuras/fig_usavings/035_selecao_periodo_bilhetagem_nuvem_comparada.png 
    :alt: selección periodo de emisión de boletos y nube para comparar 
    :align: center
----

El momento es importante, ya que los valores de la nube pueden cambiar debido al proveedor de la nube. Por esta razón, es posible elegir un cierto intervalo de tiempo. Este rango se calcula en función de la Billing generado por uCloud.

====


**4º Paso :**

Seleccione las nubes que participan en la análisis comparativa de valores. Esto incluye nubes que el usuario no necesariamente tiene conectadas a la plataforma uCloud, como nubes IBM y GOOGLE, de acuerdo con la imagen siguiente.

.. image:: /figuras/fig_usavings/036_selecionar_nuvens_analise_comparar_valores.png 
    :alt: seleccionar nubes para el analisis comparativo de valores 
    :align: center
----


**5º Paso :**

En este caso, al seleccionar cualquiera de las nubes públicas enumeradas, la siguiente pantalla es para elegir la región. Es importante saber que esta región corresponde al *Flavor* registrado en la base de datos.

.. image:: /figuras/fig_usavings/037_escolher_regiao_nuvem_1.png 
    :alt: elegir región por nube 1 
    :align: center
----

.. image:: /figuras/fig_usavings/037_escolher_regiao_nuvem_2.png 
    :alt: elegir región por nube 2
    :align: center
----

**6º Paso :**

Después de seleccionar la región por nube, la aplicación uSavings presenta la imagen *resultado después de eligir la región* con el resultado completo para la región seleccionada. Y un botón que te permite borrar la región, por la posibilidad de error y elegir otra región.

.. image:: /figuras/fig_usavings/038_resultado_escolha_regiao.png 
    :alt: resultado después de eligir la región 
    :align: center
----

Para que sea posible el análisis comparativo por Facturación (Emisión), es necesario que el emisor haya sido ejecutado en el contenedor indicado. 

Actualmente admitimos la evaluación comparativa de Billing para las nubes de AWS y Azure. Y, para que **las unidades estén disponibles, se requiere la integración con la plataforma uCloud**. En este caso, las cuentas deben estar conectadas y sincronizadas, respetando las definiciones de las reglas de seguridad.

====


Comparar por Contenedor
~~~~~~~~~~~~~~~~~~~~~~~

La segunda comparación que ofrece la aplicación uSavings es el análisis por Contenedor. Es necesario seleccionar y avanzar la secuencia del proceso para obtener el resultado deseado, que es el análisis comparativo por envase. Para que el proceso suceda, es fundamental seleccionar otra nube, además de la nube inicial elegida.

.. image:: /figuras/fig_usavings/039_selecao_comparativo_container.png 
    :alt: selección de comparativa por contenedor 
    :align: center
----

**Paso a paso**

**1º Paso :** 

Para realizar el análisis comparativo, inicialmente, haga clic en el botón **Compare by Contenedor**.

.. image:: /figuras/fig_usavings/040_selecionar_container_nuvem_compara.png 
    :alt: seleccione el contenedor y la nube para comparar
    :align: center
----

**2º Paso :**

Seleccione el contenedor como se muestra en la imagen de abajo, para compararlo con la nube anterior que se muestra en la imagen, vea la imagen anterior, el recorte ubicado en el lado izquierdo.

.. image:: /figuras/fig_usavings/041_selecionar_container_nuvem.png 
    :alt: seleccionar contenedor o nube 
    :align: center
----

**3º Paso :**

Seleccione la región y haga clic en Siguiente para finalizar la operación y obtener el resultado.

.. image:: /figuras/fig_usavings/042_tela_escolha_regiao_cloud.png 
    :alt: pantalla de elección de la región por nube
    :align: center
----

.. image:: /figuras/fig_usavings/043_comparativo_container_nuvem.png 
    :alt: comparación por contenedor versus nube
    :align: center
----

Se mostra el resultado y así el usuario llega al último step.

Después de realizar el análisis comparativo y presentar el resultado, este documento sigue con la descripción del siguiente paso, cuando los datos comparativos están en pantalla.

====


Analizar y Exportar la información recopilada
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

La plataforma uSavings permite al usuario navegar por cada una de estas unidades de información y se las seleccionar de acuerdo con la necesidad de información.

**4º Paso :**

Análisis y exportación de la información recopilada.

La imagen abajo presenta algunas tarjetas que demuestran valores sobre las sugerencias en la misma nube y en las nubes elegidas. Los resultados pueden verse directamente en la aplicación uSavings o exportarse a un informe en formato .csv

.. image:: /figuras/fig_usavings/044_cards_precos_consolidados.png 
    :alt: cards de precios consolidadas
    :align: center
----

La plataforma uSavings permite al usuario navegar por cada una de estas unidades de información y seleccionarlas de acuerdo con la necesidad de información. Esta comparación de nubes permite ver que hay dos tipos de comparación: *ON DEMAND* y *RESERVED*.

.. image:: /figuras/fig_usavings/045_representacao_grafica_preco_nuvem.png 
    :alt: representación gráfica de los precios de las nubes
    :align: center
----

La columna verde es el análisis que muestra el valor más bajo, ya que representa el costo más bajo, este costo es la sugerencia de intercambio de *Flavor* dentro de la propia nube. Las columnas centrales representan las estimaciones de las demás nubes, con relación a la columna de la derecha (color azul) que representa la nube actual con el valor de costo actual del contrato.

Al descargar la pantalla, la segunda parte de la comparativa de *Flavors* **versus** nubes, se muestra la combinación de CPU, memoria y su costo.

.. image:: /figuras/fig_usavings/046_tela_resultado.png 
    :alt: pantalla de resultados
    :align: center
----

En esta pantalla se puede ver la comparativa de *Flavors* y nubes. Además, al pasar el cursor sobre los diferentes *Flavors*, se mostrará la combinación de CPU, memoria y su respectivo costo. En esta tabla también es posible cambiar las sugerencias realizadas por uSavings, si no conviene al uso del usuario y de la organización.

La imagen arriba muestra los detalles por cada *Virtual Machine* y costos por nube, el usuario puede desplazarse y ver el costo de *Flavor* en distintas nubes.

Al hacer clic en esta información, se abre un menú que le permite al usuario cambiar el *Flavor* sugerido en la nube.

Si selecciona otro *Flavor*, la aplicación uSavings le pregunta si desea cambiarlo por otros similares o parecidos. Si es así, todas las máquinas virtuales *g1-small* se calcula como *e2-small*. Ver el informe exportado en formato.csv imagen siguiente:

.. image:: /figuras/fig_usavings/047_relatorio_exportado_csv.png 
    :alt: informe exportado en .csv
    :align: center
----

Este procedimiento no cambia el *Flavor* de las *Máquinas Virtuales* en las nubes, solo calcula las estimaciones de cambio de *Flavor* que se deben realizar en la consola de las nubes o en la plataforma uCloud.

====


Imaginary Cloud
---------------

La penúltima función del submenú uSavings se denomina *«Imaginary Cloud»*.

.. image:: /figuras/fig_usavings/048_submenu_funcionalidade.png 
    :alt: submenú de características
    :align: center
----

El submenu *Imaginary Cloud* te permite crear un entorno imaginario, con la intención de predecir el costo de la infraestructura del usuario/cliente al usar las diferentes nubes públicas.

.. image:: /figuras/fig_usavings/049_tela_inicial_imaginary_cloud.png 
    :alt: pantalla de inicio imaginary cloud
    :align: center
----

En la pantalla de inicio de *Imaginary Cloud* se pueden ver los Contenedores creados y es posible Eliminar el Contenedor. Así como la visualización de las *Virtual Machines*. *Load Balancer*, *Storage*, *IP* y *Database*. A continuación, el detalle de las pantallas y la descripción de las columnas de estos 5 ítems:

.. image:: /figuras/fig_usavings/050_tela_imaginary_vm.png 
    :alt: pantalla imaginary maquina virtual
    :align: center
---- 

En la pantalla *Imaginary Virtual Machine*, son diez las piezas de información presentadas de izquierda a derecha:

  * **(i)** Eliminar maquina virtual; 
  * **(ii)** Nombre; 
  * **(iii)** Memoria; 
  * **(iv)** vCPU;
  * **(v)** Precio corriente en dólares; 
  * **(vi)** Sistema operativo; 
  * **(vii)** IBM; 
  * **(viii)** Google; 
  * **(ix)** Azure; 
  * **(x)** AWS.

.. image:: /figuras/fig_usavings/051_tela_imaginary_load_balancer.png 
    :alt: pantalla imaginary load balancers
    :align: center
----

La pantalla *Imaginary Load Balancers* muestra ocho piezas de información en la pantalla, de izquierda a derecha:

  * **(i)** Eliminar load balancer; 
  * **(ii)** Nombre; 
  * **(iii)** Instancias; 
  * **(iv)** Reglas; 
  * **(v)** Datos por mes; 
  * **(vi)** AZURE; 
  * **(vii)** GCP; 
  * **(viii)** AWS.

.. image:: /figuras/fig_usavings/052_tela_imaginary_storage.png 
    :alt: pantalla imaginary storage
    :align: center
----

La pantalla *Imaginary Storage* muestra seis piezas de información en la pantalla, de izquierda a derecha:

  * **(i)** Eliminar storage; 
  * **(ii)** Nombre; 
  * **(iii)** Cantidad de IP; 
  * **(iv)** GCP; 
  * **(v)** AZURE; 
  * **(vi)** AWS.

.. image:: /figuras/fig_usavings/053_tela_imaginary_ip.png 
    :alt: pantalla imaginary ip
    :align: center
----

La pantalla *Imaginary IP* muestra seis piezas de información en la pantalla, de 
izquierda a derecha:

  * **(i)** Eliminar IP; 
  * **(ii)** Nombre; 
  * **(iii)** Cantidad de IP; 
  * **(iv)** GCP; 
  * **(v)** AZURE; 
  * **(vi)** AWS.

.. image:: /figuras/fig_usavings/054_tela_imaginary_database.png 
    :alt: pantalla imaginary database
    :align: center
----

En la pantalla Imaginary Database, las diez piezas de información presentadas de izquierda a derecha:

  * **(i)** Eliminar Database; 
  * **(ii)** Nombre; 
  * **(iii)** vCPUs; 
  * **(iv)** Memoria; 
  * **(v)** Storage; 
  * **(vi)** Banco de datos; 
  * **(vii)** Multi-Zone; 
  * **(viii)** AWS; 
  * **(ix)** AZURE; 
  * **(x)** GCP.

.. image:: /figuras/fig_usavings/055_imaginary_clouds_containers.png 
    :alt: imaginary clouds pantalla de contenedores
    :align: center
----

A partir de este entorno, el usuario puede crear un entorno imaginario (contenedor) y eliminar los contenedores creados.

.. image:: /figuras/fig_usavings/056_criar_ambiente_imaginario.png 
    :alt: crear pantalla de entorno imaginario contenedor
    :align: center
----

.. image:: /figuras/fig_usavings/057_tela_deletar_ambiente_imaginario_container.png 
    :alt: eliminar pantalla de entorno imaginario contenedor
    :align: center
----

El ambiente Imaginary Cloud permite la creación de máquinas, importar desde un archivo.csv con el inventario de infraestructura, permite la creación de un contenedor y presentación de una pantalla con el costo de las diferentes nubes.

Estas pantallas de entorno imaginario son el resultado de la intención de predecir el coste de la infraestructura del usuario/cliente al utilizar las diferentes nubes públicas. Y cada una de estas columnas representa el costo de lo que se lograría, incluido el costo de la migración.

Después de toda esta imaginación de escenarios, la aplicación brinda documentación en formato.csv, lista para importar y usar en reuniones de toma de decisiones.

.. image:: /figuras/fig_usavings/058_criar_container_imaginario.png 
    :alt: crear contenedor imaginario
    :align: center
----

Después de crear el contenedor imaginario, podemos seguir creando otros recursos y comparar sus precios para las diferentes nubes, mostrando también cuál sería la nube que proporciona el precio más bajo para los datos deseados.

.. image:: /figuras/fig_usavings/059_criar_virtual_machine.png 
    :alt: crear virtual machine
    :align: center
----

Comenzando con la creación de la Máquina Virtual, tenemos una serie de entradas que se deben rellenar, comenzando con el campo Nombre a otras opciones como vCPU, memoria y sistema operativo deseado, además, se debe estipular cuánto presupuesto habría que "pagar" por esta Máquina Virtual.

.. image:: /figuras/fig_usavings/060_import_export_csv.png
    :alt: import y export csv
    :align: center
----

Después de su creación, los resultados se presentan en la pantalla, en dos formatos: 

 * **(i)** Los gráficos que relacionan las máquinas virtuales con los Flavors deseados para cada una de las nubes que cubre el producto; 

 * **(ii)** Un cuadro formato.csv que se puede exportar a la necesidad del usuario de información distinta de las presentadas en el gráfico, si el gráfico no es suficiente o satisfactorio.

.. image:: /figuras/fig_usavings/061_comparativo_criar_load_balancer.png 
    :alt: comparación al crear load balancer
    :align: center
----

Tenemos la opción de crear un *Balanceador de Carga* imaginario de la misma manera, con 4 *inputs* esta creación también requiere un nombre - El Nombre de entrada se requiere para todas las opciones de creación - y 3 nuevos *inputs*: 

* Instancias, 
* Reglas de transferencia y 
* Datos por mes en GB.

Los resultados se presentan en formato de tabla, que muestra el precio del servicio deseado para cada Cloud. Vale la pena mencionar que en este *ejemplo de creación de Load Balancer*, la nube de AZURE tiene el valor más bajo, en segundo lugar, la nube de AWS, y finalmente, el costo más alto en este ejemplo es la nube de GCP. Es así como la aplicación uSavings sugiere el ahorro de los recursos contratados para la toma de decisiones en la organización. 


.. image:: /figuras/fig_usavings/062_criar_storage_imaginary_cloud.png 
    :alt: crear storage en imaginary cloud
    :align: center
----

Siguiendo el proceso, crea un Storage de la misma manera, con 4 entradas que consisten en las entradas: 

* Nombre, 
* Instancias, 
* Cantidad de transacciones y 
* Tamaño en GB.

.. image:: /figuras/fig_usavings/063_criar_storage.png 
    :alt: crear storage
    :align: center
----

Después de crear un *Storage*, la pantalla de presentación es similar a la visualización del *Load Balancer*.

.. image:: /figuras/fig_usavings/064_resultado_criacao_storage.png 
    :alt: resultado de la creación de la storage
    :lign: center
----

Para la penúltima opción de creación tenemos la IP, que sigue la misma lógica, requiriendo solo 2 *Inputs*: 

* Nombre y 
* Cantidad de IPs. 

.. image:: /figuras/fig_usavings/065_criar_ip.png 
    :alt: crear ip
    :align: center
----

El formato de presentación de la pantalla IP es similar a los elementos ya explicados anteriormente en este manual. La última opción por describir para la creación imaginaria es la Database. 

.. image:: /figuras/fig_usavings/066_criar_database_imaginary_cloud.png 
    :alt: crear database en lo imaginary cloud
    :align: center
----

Para que la operación tenga éxito se necesita rellenar nombre, vCPU, memoria en GB, Almacenamiento en GB, motor que se utiliza y, si debe ser multizona, o no. 

.. image:: /figuras/fig_usavings/067_criar_database_imaginary_cloud_2.png 
    :alt: crear database en lo imaginary cloud
    :align: center
----

Después de la creación también se recibe una tabla con los datos que se crearon y los precios de mercado existentes.

Si el usuario lo considera necesario eliminar el *Imaginary Cloud*, después de crear todos estos elementos, hay la opción de eliminar cualquiera de ellos en cualquier momento, en caso de eliminar los elementos dentro del contenedor se debe hacer clic en el símbolo de la papelera a la izquierda de la tabla. 

Para eliminar el contenido o debe hacer clic en él y rellenar un modal con el nombre del elemento que desea eliminar.

====


Contenedor Hint
---------------

La última función de menú uSavings es el *Contenedor Hint*, presenta recursos que aparentemente no se están utilizando o están generando costos supuestamente innecesarios. 

.. image:: /figuras/fig_usavings/068_container_hint.png 
    :alt: menú contenedor hint
    :align: center
----

La funcionalidad está disponible para cuentas conectadas e integradas con el Cloud.

.. image:: /figuras/fig_usavings/069_selecao_tipo_nuvem_container.png 
    :alt: selección por tipo de nube o contenedor
    :align: center
----

Al conectar la cuenta de nube pública a la plataforma uCloud se presenta la imagen de arriba. La pantalla permite seleccionar los tipos de proveedores de nube:

  * **(i)** GCP; 
  * **(ii)** AWS; 
  * **(iii)** AZURE; 
  * **(iv)** VMWare o seleccione un contenedor.

.. image:: /figuras/fig_usavings/070_tela_recursos_nao_utilizados.png 
    :alt: pantalla de recursos no utilizados
    :align: center
----

El usuario debe seleccionar una de las cuatro nubes que quiere buscar para averiguar qué recursos aparentemente no se utilizan o generan costos supuestamente innecesarios.

Después de seleccionar la nube deseada, la pantalla presenta una lista que le permite buscar las siguientes características:

* **Disks** - Enumera los discos creados y no asociados a ninguna máquina virtual;

* **Public IP** - Enumera las direcciones IP públicas que se han solicitado en algún momento que generan costos y no están asociadas a ninguna máquina virtual;

* **Disk Snapshot** - Enumera todas las instantáneas de los discos creados, no distingue cuáles de ellos deben o no deben eliminarse;

* **VM Snapshot** - Enumera todas las instantáneas de las máquinas virtuales creadas, no distingue cuáles de ellas deben o no deben eliminarse.

* **Load Balancer** - Enumera todos los Load Balancer creados, pero no distingue cuáles de ellos deben o no deben borrarse.

* **Virtual Machine** - Enumera todas las máquinas virtuales creadas.

Así, el usuario puede realizar la búsqueda y averiguar qué recursos no se utilizan o generan costes innecesarios para la organización.

----

uCloud
======

El último menú de funcionalidad presenta la posibilidad de ir a la plataforma uCloud solamente con un hacer de clic en este menú, la aplicación uSavings envía el usuario a la plataforma uCloud.

-------

Conclusión
==========

Así, este documento concluye la descripción general de los procedimientos requeridos para su uso. La lectura de este manual de usuario permite a el usuario de la aplicación utilizar sus funciones correctamente.

====


**Equipo Ustore**



uSavings Manual de utilización - Edición 2 v.7 - 02/05/2022. Revisión 22/11/2022.



.. |icone_ustore| image:: /figuras/fig_usavings/icone_ustore.png 

.. |icone_configuracao| image:: /figuras/fig_usavings/icone_configuracao.png

.. |icone_lista_troca_idioma| image:: /figuras/fig_usavings/icone_lista_troca_idioma.png

.. |icone_bandeira_troca_idioma| image:: /figuras/fig_usavings/icone_bandeira_troca_idioma.png

.. |icone_nome_usuario_logado| image:: /figuras/fig_usavings/icone_nome_usuario_logado.png

.. |icone_logout| image:: /figuras/fig_usavings/icone_logout.png