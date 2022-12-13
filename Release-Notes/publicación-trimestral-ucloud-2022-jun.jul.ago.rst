.. figure:: /figuras/ucloud.png
   :alt: Logo uCLoud
   :scale: 50 %
   :align: center
   
----


Publicación (Trimestral) Junio | Julio | Agosto - Año 2022
=========================================
Plataforma uCloud versión: *Update tags 5.3-b56 y 1.0-account90*


—-


Presentación
==========


Este boletín de la Plataforma uCloud es una herramienta de comunicación esencial para la difusión de las novedades sobre el producto y las innovaciones generadas en el área de desarrollo.
Las Notas de Publicación, además de ser un material informativo con contenido relevante sobre las entregas de uno o varios incrementos en la aplicación, tienen como objetivo proporcionar resultados a la inversión de los clientes, obtener asesoramiento e informar de los avances, ya sean de perfeccionamiento, mejoras o correcciones. Realmente proporciona la visibilidad adecuada en el proceso de desarrollo del producto.




Noticias 
========


Las novedades o lanzamientos de este periodo sobre la plataforma uCloud abarcan las siete (7) nuevas implantaciones, las trece (13) mejoras realizadas en la categoría *Cloud* por la demanda en la adecuación a los cambios en estos proveedores, cuarenta (40) mejoras globales de la plataforma uCloud y las treinta y cuatro (34) acciones correctivas, siendo nueve (09) relacionadas con las nubes, diez (10) relacionadas con uCloudOPS y quince (15) pertenecientes al *Billing*. 


* Nuevas implementaciones;


* Adecuaciones a las nubes públicas y privadas;


* Perfeccionamiento de la plataforma uCloud;


* Acciones correctivas.








Nuevas implementaciones
==================


Este tópico presenta las siete nuevas implementaciones e inserta *hyperlinks* en algunos términos que direccionan el lector a ampliar su conocimiento sobre determinada implementación, accediendo a informaciones detalladas sobre cada una de ellas, en el manual del usuario uCloud, alojado en el repositorio / wiki de Ustore.



1.  **Budget**


El *Budget* es un informe basado en el consumo creado con el objetivo de definir un presupuesto total para un periodo determinado (denominado Intervalo), ya sea mensual, trimestral, semestral o anual. Este informe basado en el consumo, además de definir un presupuesto total, permite visualizarlo con un desglose de los costes de *Budgets*.


Cuando se traduce del inglés al portugués, *"budget"* se refiere a la palabra "presupuesto" y corresponde a una nueva implementación en el Portal uCloud, definida por un informe basado en el consumo que tiene como objetivo fijar el presupuesto total para un período y permite las previsiones de costes. 




Accediendo al *Budget*
--------------------




Para acceder al submenú *Budget* en el portal uCloud, el usuario debe hacer clic en el menú Administración, y luego en el submenú Contratos. En la pantalla siguiente se muestra la lista de todos los contratos existentes.


.. figure:: /figuras/fig_budget/01_budget_contrato.png
   :alt: Budget Contrato  
   :align: center


----




Al seleccionar en la lista el contrato deseado, aparece una nueva pantalla con los detalles del contrato. La pantalla de detalles del contrato puede considerarse una de las más grandes de la plataforma uCloud, ya que presenta diecisiete tipos de datos diferentes, exhibiendo las tarjetas:


  * 1.General; 
  * 2.Categorías de Precios;
  * 3.Precio de los Recursos;
  * `4.Budgets`;
  * 5.Contrato Primario;
  * 6.Administradores; 
  * 7.Reglas de Facturación;
  * 8.Políticas de Alertas; 
  * 9.Cuota del Contrato;
  * 10.Datos de la Empresa 
  * 11.Virtual Datacenters Concedidos; 
  * 12.Usuarios; 
  * 13.Grupos; 
  * 14.Datos de Facturación;
  * 15.Perfiles de Aprovisionamiento del Contrato y sus Permisos;
  * 16.Productos;
  * 17.Perfil de Facturación por Container.




.. figure:: /figuras/fig_budget/02_budget_tela_contrato.png
   :alt: Budget tela contrato 
   :align: center


----
  


En esta pantalla de detalle del contrato, el usuario debe utilizar la barra de desplazamiento y navegar hasta encontrar la cuarta `tarjeta` llamada *Budget* que se muestra a continuación:


.. figure:: /figuras/fig_budget/03_contrato_budget.png
   :alt: Contrato tela Budget  
   :align: center


----






La `Tarjeta Budget` exhibe dos botones, `[REFRESH]` y `[+Añadir]`. 


.. attention:: |atencao| En este ejemplo de imagen, los *Budgets* aún no han sido creados, de modo que está en blanco, con el símbolo de atención. 
   
Al hacer clic en el botón `"+ Añadir"`, se presenta el modal "Crear Budget", y a partir de ahí, el usuario inicia la primera creación.


.. figure:: /figuras/fig_budget/03_budget_adicionar.png
   :alt: Budget Adicionar 
   :align: center


---- 






Creando *Budget* y *Sub Budget*
-------------------------------


El modal "Crear *Budget*", presenta los campos: nombre, intervalo, mes, *"checkbox"* para seleccionar si el informe es recurrente, el valor por coste o por cantidad consumida.


A continuación, se muestran los detalles de los `Sub Budgets` como: desambiguación, selección del *container*, valor y los botones `[+Incluir Subbudget] [Cancelar]` y `[Crear]`.




.. important:: La desambiguación es responsable por el propósito del Sub Budget, por lo tanto, al hacer clic en el "Checkbox", el usuario visualiza y puede filtrar uno de los cinco tipos de elementos existentes: Account Master - Container - Cloud Type - Dimensión - TagUsn.


.. figure:: /figuras/fig_budget/04_criar_budget.png
   :alt: Criar Budget 
   :align: center


---- 
  


Tras pulsar el botón `[+Añadir]`, se presenta la pantalla de creación del *Budget* como se muestra en la imagen anterior, en ella el usuario debe rellenar todos los campos y configurar la generación del informe basado en el consumo.




* `Nombre`: Espacio destinado al nombre del *Budget*. 
* `Intervalo`: Presentado como un menú desplegable, este campo es responsable por el período deseado para la creación del informe (mensual, trimestral, semestral o anual).




.. figure:: /figuras/fig_budget/05_criar_budget_preencher_intervalo.png
   :alt: Preencher intervalo 
   :align: center


---- 
 
            
En el proceso de crear y configurar el *Budget*, el usuario tiene la opción de seleccionar en la plataforma el "Intervalo" que pretende generar en el informe. A continuación se detallan las pantallas correspondientes a los cuatro tipos de intervalos permitidos en esta creación.




Intervalo Trimestral
~~~~~~~~~~~~~~~~~~~~


.. figure:: /figuras/fig_budget/05_budget_trimestral.png
   :alt: Budget trimestral 
   :align: center


---- 




Al observar la figura anterior, en el espacio "Intervalo", es necesario hacer clic en la opción "Trimestral", como resultado la interfaz presenta un "*checkbox*" con cuatro opciones de periodo, situada al lado de la `tarjeta` "Detalles de los *Sub Budgets*". El usuario debe seleccionar de acuerdo con el trimestre que desea generar el informe.


La aplicación permite al usuario elegir cualquiera de los trimestres disponibles dentro del periodo de un año, comenzando siempre a partir del mes elegido, situado en el campo "Seleccione el mes".




 
Intervalo Semestral
~~~~~~~~~~~~~~~~~~~ 


.. figure:: /figuras/fig_budget/05_budget_semestral.png
   :alt: Budget semestral 
   :align: center


---- 
  
En el menú desplegable "Intervalo", al seleccionar la opción "Semestral", la *tarjeta* referente a los periodos presentados como intervalos semestrales aparece al lado de los detalles del *Sub Budget*, en forma de *“checkbox”*.  


La aplicación genera dos alternativas con los semestres disponibles dentro del periodo de un año. Comenzando a partir del mes elegido que se encuentra en el campo "Seleccione el mes".




Intervalo Anual
~~~~~~~~~~~~~~~


.. figure:: /figuras/fig_budget/05_budget_anual.png 
   :alt: Budget anual 
   :align: center


---- 




Al seleccionar el intervalo anual, aparece una lista con todos los meses correspondientes al periodo de 1 año, a partir del mes seleccionado en el campo "Seleccione el mes".  


Permite crear un *Sub Budget* para cada mes del año, sea manualmente o marcando la opción "igual para todos los meses". 


Al incluir un *Sub Budget*, el mismo se añade para todos los meses, recordando que el valor del *Budget* se refiere al año. 




.. attention:: Al crear Sub Budgets para todos los meses del año, la suma debe limitarse al valor total del Budget.




Intervalo Mensual
~~~~~~~~~~~~~~~~


La pantalla de Intervalo Mensual se presenta al continuar con el proceso de rellenar los campos de la pantalla "*Crear *Budget*". Para el intervalo mensual, el informe contempla el mes elegido.




En la secuencia siguiente, el usuario debe completar los espacios restantes, completando este modal para la creación de *Budget*:




* `Seleccione el mes`: En este campo el usuario debe rellenar con el mes y el año deseado para marcar la fecha inicial del informe, o seleccionar una fecha personalizada.


.. figure:: /figuras/fig_budget/06_criar_budget_mes.png
   :alt: Budget mensal 
   :align: center


---- 
  


* `Budget Recurrente`: Responsable por la activación, o no, del informe continuo. 


Esta funcionalidad habilita la creación automática. 


Por ejemplo, en el mes siguiente, se creará otro *Budget*, en el caso de trimestral y semestral, se creará un mes después del último mes del periodo. 
  
.. figure:: /figuras/fig_budget/07_criar_budget_recorrente.png
   :alt: Criar budget recorrente  
   :align: center


---- 




* `Valor`: Campo que hace referencia al valor del informe.
 
En este espacio, el usuario debe rellenar el campo Valor con la cantidad disponible para el *Budget*, y seleccionar si este valor es por coste o por cantidad consumida. 




* `Por coste o por cantidad consumida`: *“Checkbox”* responsable de indicar qué unidad del `Budget` se utiliza como referencia para mostrar el informe en pantalla, por coste (valor en BRL) o por cantidad consumida (valor en *amount* de los recursos). Estas opciones se encuentran en la parte derecha del campo de relleno del valor. 




Después de rellenar estos datos, se deben completar los campos sobre los detalles de los *Sub Budgets*. En este caso, el usuario debe seleccionar el tipo de desambiguación que desea en el informe, si es de *Container*, *Account Master*, *CloudType*, *Dimensión* o *TagUsn*.




.. note:: Es posible añadir los Sub Budgets a nuestro Budget principal, limitándose a la regla de que el valor de éste tiene que ser igual a la suma de los valores de sus Sub Budgets. Si el valor representa un número mayor o menor, el botón de creación del Budget permanece desactivado y el "saldo restante" difiere de 0.


.. figure:: /figuras/fig_budget/08_desambiguação.png
   :alt: Desambiguação  
   :align: center


---- 
    
Seleccionado el tipo de Desambiguación, el siguiente punto es rellenar el valor de *Sub Budgets*, en la *tarjeta* "Detalles del Sub Budget".  


.. figure:: /figuras/fig_budget/09_criar_budget_valor.png
   :alt: Criar budget valor 
   :align: center 


---- 




En este paso, el valor del *Sub Budget* debe rellenarse, y cuando se introduce el valor deseado, el saldo restante se presenta justo debajo del campo de valor.




Una vez completados todos los datos, el usuario debe pulsar el botón "Incluir Subbudget" para finalizar la inclusión. Como resultado de la operación, la pantalla exhibe la lista de *Sub Budget* incluido como se muestra en la imagen siguiente:




.. important:: El saldo restante corresponde al valor que indica el saldo restante del Budget, equivale al valor del Budget sustraído por la suma del valor de todos los Sub Budgets.  El botón "Crear Budget" permanece desactivado si el saldo restante es diferente de 0. 


.. figure:: /figuras/fig_budget/10_criar_budget_incluir_sub.png 
   :alt: Criar budget incluir sub 
   :align: center


---- 
  


Para crear el segundo *Budget*, el usuario debe seguir los pasos detallados anteriormente en el ciclo de creación del primer *Budget*. Proceda al punto "Detalles de los Sub Budgets" que se muestra a continuación:


.. figure:: /figuras/fig_budget/08_desambiguação.png
   :alt: Desambiguação   
   :align: center


----  


En este flujo, para detallar el `Sub Budget` con una desambiguación distinta, basta seleccionar un tipo diferente del utilizado anteriormente, y haciendo clic en *"Dimensión"*, el campo al lado permanece disponible para la selección de una determinada dimensión.


.. figure:: /figuras/fig_budget/12_subbudget_detalhes.png
   :alt: Subbudget detalhes  
   :align: center


----
  


Al rellenar el valor deseado, es necesario observar la cantidad disponible en el área "Saldo restante", situada debajo del espacio "Valor". Tras completarlo, basta con pulsar el botón "Incluir SubBudget" al lado del hueco "Valor", para que el *Sub Budget* de desambiguación del tipo "Dimensión" creado se una al *Sub Budget* de desambiguación del tipo *"Container"* generado anteriormente. 


Ambos se muestran en el listado de abajo:




.. figure:: /figuras/fig_budget/14_subbudget_criado.png
   :alt: Subbudget criado 
   :align: center


----
  
 
Para finalizar el proceso de creación de *Budgets* y *Sub Budgets*, basta con pulsar el botón ``Crear`` situado en la parte inferior derecha de la pantalla.




Editando Budget 
---------------


Para editar un *Budget*, basta el usuario acceder al menú Administración, y luego hacer clic en el submenú Contratos, la plataforma exhibe la lista de todos los contratos existentes.


En ella, el usuario debe hacer clic en el contrato relacionado al `Budget` que desea editar. La pantalla cargada presenta los detalles de este contrato, siendo necesario utilizar la barra de desplazamiento y navegar hasta encontrar la cuarta tarjeta *Budget*. 


En esta `tarjeta` se muestran cinco columnas: Nombre, Intervalo, Fecha de inicio, Valor y Acciones.


La columna "Acciones" permite al usuario realizar dos ejecuciones representadas por los iconos `[Editar]` y `[Eliminar]`.


.. figure:: /figuras/fig_budget/15_editar_budgets.png
   :alt: Editar budgets  
   :align: center


----




Al pulsar el botón `[Editar]` en el *Budget* elegido, se muestra el modal de edición con toda las informaciones previamente rellenadas.


.. figure:: /figuras/fig_budget/16_editar_budget.png
   :alt: Editar budget 
   :align: center


----
  


En esta pantalla es posible cambiar el nombre, el mes, el valor, si el *Budget* es por coste o por cantidad consumida, y además, se pueden hacer cambios en los *Sub Budgets*. Resaltando que hay una limitación del intervalo, después de la creación de un *Budget* es imposible cambiarlo.




.. important:: En resumen, los Sub Budgets creados no se modifican, es necesario eliminar y añadir el nuevo Budget.








Visualizando el Informe de Costes de `Budgets`
----------------------------------------------


Para visualizar el Informe de Costes de `Budgets`, el usuario debe hacer clic en el menú Financiero y, a continuación, en el submenú Informes. Esta visualización permite al usuario mantenerse informado sobre las previsiones de costes en detalle.


En este flujo se presenta la pantalla `Financiero`, en esta interfaz se puede elegir entre acceder a la propia factura o gestionarla, desde uno de los grupos o contratos administrados por el usuario conectado. 


Es necesario seleccionar el periodo, mes y año deseado, para mostrar los resultados basados en estas fechas. A continuación, se presentan dos clases de paneles basados en el consumo y factura. 


El primer tópico  `“Paneles Basados en el Consumo”` agrupa siete tipos de informes: 


1. Historial de Servicio; 
2. Coste Cadenciado;
3. Coste Relacional del Producto;
4. Visualización de Recursos;
5. **Costes de Budgets**;
6. Informe de Monitoreo de Consumo;
7. Informe Basado en Límite de Coste.


El segundo tópico `“Paneles Basados en Factura”` reúne cinco tipos de paneles:  


1. Mi factura;
2. Financiero;
3. Informe Consolidado de Facturación;
4. Cuenta Master; 
5. Tendencia de Facturación.   




Para acceder al `Informe de Costes de Budgets`, el usuario debe hacer clic en la opción `Coste de Budgets`, que se muestra en la siguiente pantalla:


.. figure:: /figuras/fig_budget/17_painéis_consumo.png
   :alt: Painéis baseados em consumo  
   :align: center


----
  


En la pantalla de "Detalles de los Costes de Budgets", el usuario debe seleccionar un contrato, haciendo clic en el contrato deseado se muestra la siguiente pantalla:


.. figure:: /figuras/fig_budget/18_detalhamento_custos.png
   :alt: Detalhamento de custos 
   :align: center


----
  


Al hacer clic en "Período", el icono calendario es exhibido por la plataforma, el usuario debe seleccionar el mes o los meses deseados. Por último, debe pulsar en buscar.


.. figure:: /figuras/fig_budget/19_detalhamento_período.png
   :alt: Detalhamento período 
   :align: center 


----




Al final de la selección del periodo, como resultado de la búsqueda, el sistema filtra todos los `budgets` dentro del periodo determinado.


.. figure:: /figuras/fig_budget/20_detalhe_subbudget.png
   :alt: Detalhamento subbudget 
   :align: center 


----
  


Al visualizar la lista de los **Budgets**, se muestra en pantalla la siguiente información:


1. Período;
2. Cantidad Consumida por los `Sub Budgets` en Porcentaje;
3. Nombre;
4. Intervalo;
5. Tipo: Por Coste o por Cantidad consumida;
6. Valor Consumido por sus `Sub Budgets`;
7. Barra de Consumo;
8. Valor Asignado para el `Budget`.




Al hacer clic en el *Budget* para visualizar los *Sub Budgets*, la interfaz ofrece las informaciones necesarias para que el usuario pueda comprender los costes, que son:


1. Período;
2. Cantidad que la Desambiguación consume del valor asignado para el `Sub Budget` en porcentaje;
3. Nombre;
4. Tipo de Desambiguación;
5. Valor consumido de la Desambiguación;
6. Barra de Consumo;
7. Valor asignado para el `sub budget`.




.. note:: Al elegir un *Budget* que tenga un intervalo trimestral, semestral o anual, la plataforma sólo muestra los *Sub Budgets* correspondientes al periodo seleccionado. En esta opción, la plataforma entiende que se trata de un periodo incompleto de este *Budget*. Para presentar todos los meses, debe elegirse el período completo del presupuesto.


—-


—-


2. **Personalización del *branding* a nivel de contrato**: El *branding* del portal Multicloud es permitido a través de la personalización definida por contrato. El cliente usuario puede seleccionar las características de su marca (empresa) representada en el portal Multicloud como los colores, el logotipo, entre otros.




—-


3. **Dimensión**
~~~~~~~~~~~~




La Dimensión es una nueva implementación de la plataforma uCloud, y fue creada para agrupar `Tags` de diferentes nomenclaturas, pero que forman parte del mismo contexto, que están etiquetados en diferentes nubes. De esta manera, se evita que los mismos recursos sean etiquetados de diferentes maneras. 


Así, se elaboraron operaciones lógicas y un filtro, con el fin de identificar en el *Billing* qué recursos pertenecen a una determinada dimensión. Para entender mejor los dos puntos que construyen este concepto, observe los siguientes ejemplos:




1. Unifica un conjunto de `Tags` que son diferentes pero que tienen el mismo significado/función.


 * Por ejemplo:


   * product: ETC
   * Product: eTc
   * producT: CTE




Como se puede observar, los `Tags` anteriores expresan lo mismo, aunque son divergentes en su forma escrita. Es importante recordar que se pueden **aplicar en diferentes nubes**, pero en los mismos recursos, donde deberían comportarse igualmente.


Así, al unificar este grupo de `Tags` en una dimensión, es posible identificar todos los recursos que están dentro de este contexto, y así tener una nueva forma de visualización de Informes, `Budget` y `Forecast`.




2. Crea expresiones lógicas.


 * Por ejemplo:
 
   * product: EFG & departamento:TI


En el ejemplo de arriba, la expresión representa que esta dimensión desea todos los recursos que tengan los `Tags`: “product: EFG & departamento:TI”. Esta expresión es considerada simple, sin embargo, algo más complejo puede ser construido a partir de lo que se puso implementado.




Creando una Dimensión
~~~~~~~~~~~~~~~~~~~~


Para crear una dimensión, el usuario debe hacer clic en el menú Financiero, y luego en el submenú Utilidades, que exhibe dos opciones que se muestran en la siguiente imagen: 


1. **Dimensión**; 
2. Tags Virtuales.


.. image:: /figuras/fig_ucloud_findimensao/1_dimensão_menu_financeiro.png
   :alt: Financeiro Dimensão_menu_financeiro
   :align: center
----
  


Al seleccionar la opción "Dimensión", se presenta la lista de dimensiones generadas anteriormente, como se muestra en la figura siguiente:
  
.. image:: /figuras/fig_ucloud_findimensao/02_dimensão_listagem.png
   :alt: Financeiro Dimensão_listagem
   :align: center
----




En caso de que ésta sea la primera dimensión creada por el usuario, ninguna lista se presenta en la pantalla, como se muestra en la siguiente figura:




.. image:: /figuras/fig_ucloud_findimensao/03_dimensão_listagem_vazia.png
   :alt: Financeiro Dimensão_listagem_vazia
   :align: center
----
  


En la parte superior izquierda de la pantalla aparece el botón "Crear dimensión", sobre el que el usuario debe pulsar para iniciar el proceso de creación.


Después de pulsado, se muestra la pantalla inicial de creación de la "Dimensión", como se puede ver en la siguiente figura: 
  


.. image:: /figuras/fig_ucloud_findimensao/04_dimensão_inicio.png
   :alt: Financeiro Dimensão_inicio
   :align: center
----




Para entender mejor la función de cada campo, conviene observar los detalles a continuación:


* Nombre de la dimensión: En este campo el usuario debe rellenar el nombre de la dimensión a guardar.


* Estructura + : Este botón presenta dos opciones que el usuario puede aplicar a la estructura de su "Dimensión":


* Agrupación de *Tags*;


   * *Tag*. 




.. attention:: |atención| Es importante señalar que esta estructura debe ser una expresión lógica pensada previamente. Por lo tanto, para agrupar los `tags` es necesario ponerlos primero en un grupo.


* Estructura: Corresponde al bloque situado al final de la pantalla, donde el usuario tiene una mejor visualización de la estructura que está siendo montada.


* Botón "Guardar": Una vez rellenados los datos por completo, el usuario debe pulsar el botón "Guardar" para que los datos no se pierdan.




Creando una Agrupación de *Tags*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




Tras rellenar el nombre de la "Dimensión", el usuario debe crear un grupo para su estructura. Al pasar el cursor del ratón por la opción "Agrupación de *Tags*", aparece el siguiente mensaje:




.. image:: /figuras/fig_ucloud_findimensao/05_dimensão_mensagem_grupo_expandida.png
   :alt: Financeiro Dimensão_mensagem_grupo_expandida
   :align: center
----


Una vez seleccionado, el modal de creación del grupo se muestra, donde el nombre de la agrupación de `Tags` debe ser rellenado y luego guardado.


.. image:: /figuras/fig_ucloud_findimensao/06_dimensão_criar_grupo.png
   :alt: Financeiro Dimensão_criar_grupo
   :align: center
----


  


Una vez realizada la acción, debajo de la función **"Estructura +"**, aparece el nombre del grupo creado y, junto a él, dos botones de acción:


* Símbolo de suma "+" para crear otro(s) grupo(s) o añadir *Tag(s)*;


* Icono de una basurera para eliminar el grupo creado.


Al lado de estos iconos, aparece la siguiente información:




.. image:: /figuras/fig_ucloud_findimensao/07_dimensão_mensagem_estrutura_expandida.png
   :alt: Financeiro Dimensão_mensagem_estrutura_expandida
   :align: center
----


.. attention:: |atención| Es importante señalar que si la construcción de la "Dimensión" no se ajusta a las condiciones mostradas en el mensaje, el botón "Guardar" queda inhabilitado para su activación.


En la imagen de abajo, también se puede ver que en la función de Estructura, en la parte inferior de la pantalla, el grupo está representado por (    ).




.. image:: /figuras/fig_ucloud_findimensao/08_dimensão_grupo_estrutura.png
   :alt: Financeiro Dimensão_grupo_estrutura
   :align: center
----  






Creando *Tag*
~~~~~~~~~~~~~


Al hacer clic en el icono de suma "+" al lado del grupo creado y situando el cursor del ratón sobre la opción `Tag` aparece el siguiente mensaje:




.. image:: /figuras/fig_ucloud_findimensao/09_dimensão_mensagem_tag_expandida.png
   :alt: Financeiro Dimensão_mensagem_tag_expandida
   :align: center
----


Al hacer clic en `Tag`, el modal de creación de `Tag` es mostrado:




.. image:: /figuras/fig_ucloud_findimensao/10_dimensão_modal_tag.png
   :alt: Financeiro Dimensão_modal_tag
   :align: center
----


  
El primer paso del usuario es seleccionar una de las `companies` listadas en el menú desplegable.




.. image:: /figuras/fig_ucloud_findimensao/11_dimensão_lista_company.png
   :alt: Financeiro Dimensão_lista_company
   :align: center
----


  
Después de seleccionar la `company` deseada, el botón "Filtrar" al lado del menú desplegable queda disponible para activación, como se ejemplifica en la imagen siguiente:




.. image:: /figuras/fig_ucloud_findimensao/12_dimensão_filtrar.png
   :alt: Financeiro Dimensão_filtrar
   :align: center
----


  
Si la `company` ya dispone de `Tags`, se muestra un listado de `Tags` con las claves y valores de los últimos tres meses. La pantalla exhibe el número de páginas abajo del listado y las informaciones recuperadas en bloques de 10, 25, 50 o 100 filas.




.. image:: /figuras/fig_ucloud_findimensao/13_dimensão_company_tag.png
   :alt: Financeiro Dimensão_company_tag
   :align: center
----


  


El usuario debe seleccionar el `Tag` deseado, mostrado en la lista, y automáticamente se muestran la Clave y el Valor del `Tag` creado.


  


.. image:: /figuras/fig_ucloud_findimensao/14_dimensão_company_tag_escolhida.png
   :alt: Financeiro Dimensão_company_tag_escolhida
   :align: center
----




Al finalizar el llenado del modal, el usuario debe hacer clic en el botón "Guardar" que se encuentra en la parte inferior derecha de la pantalla.
  


.. image:: /figuras/fig_ucloud_findimensao/15_dimensão_modal_segunda_tag.png
   :alt: Financeiro Dimensão_modal_segunda_tag
   :align: center
----




Si una `company` no tiene `Tags` y el usuario desea crearlos, basta introducir la Clave y el Valor en los últimos campos, como se muestra en la imagen de arriba, dejando los campos centrales vacíos.


Una vez hecho esto, la pantalla de creación de "Dimensión" debe aparecer de la siguiente manera: 


.. image:: /figuras/fig_ucloud_findimensao/16_dimensão_grupo_e_tag.png
   :alt: Financeiro Dimensão_grupo_e_tag
   :align: center
----




Según la imagen anterior, se puede percibir que la "Dimensión" tiene un sistema jerárquico, en el que primero hay un grupo insertado en la estructura, y sólo después de la creación del grupo siguen los `Tags`.
 
Después de inicializar el proceso de creación de una "Dimensión", es necesario añadir los otros `Tags` del mismo contexto para que formen parte del grupo.


Así, el usuario debe hacer clic en el signo de suma "+" que aparece al lado de Estructura, donde figuran dos **operadores lógicos** </> OR e </> AND. 




Utilizando el Operador Lógico
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  


Los operadores lógicos forman parte del lenguaje de programación y se utilizan con el objetivo de crear expresiones de tipo verdaderas y falsas. Estas se usan para unir dos expresiones divergentes y elaborar una expresión condicional más compleja. 




.. image:: /figuras/fig_ucloud_findimensao/17_dimensão_operadores_lógicos_closeup.png
   :alt: Financeiro Dimensão_operadores_lógicos_closeup
   :align: center
----




Para entender mejor su aplicación, a continuación se detallan las informaciones sobre los dos operadores utilizados en la creación de "Dimensión".


 * </> “OR”: En una expresión, si sólo una de ellas es verdadera, ésta se considera totalmente verdadera y es ejecutada.


 * </> “AND”: En una expresión, si una de ellas es falsa, ésta se considera totalmente falsa y no es ejecutada.


Para entender mejor su uso, el usuario debe seguir el proceso de creación.  


Al situar el cursor del ratón sobre la opción del operador </> “OR”, aparece el siguiente mensaje:




.. image:: /figuras/fig_ucloud_findimensao/18_dimensão_operador_ou_closeup.png
   :alt: Financeiro Dimensão_operador_ou_closeup
   :align: center
----




Es decir, aunque uno de los `Tags` no exista, la acción se realiza sólo con el `Tag` existente.


Cuando se pone el ratón sobre el operador </> AND, aparece el siguiente mensaje:




.. image:: /figuras/fig_ucloud_findimensao/19_dimensão_operador_e_closeup.png
   :alt: Financeiro Dimensão_operador_e_closeup
   :align: center
----




Es decir, al buscar los `Tags`, si sólo uno de los `Tags` es inexistente, la acción es detenida.


En este ejemplo, se ha seleccionado el operador "AND" (en lengua inglesa), y la confirmación de la acción se presenta en el cambio de ambas estructuras:




.. image:: /figuras/fig_ucloud_findimensao/20_dimensão_operador_selecionado.png
   :alt: Financeiro Dimensão_operador_selecionado
   :align: center
----


  
Una vez finalizado este primer proceso de creación de "Tag", el usuario debe crear el segundo "Tag", repitiendo el flujo de creación detallado anteriormente.


Al finalizar este paso, se muestra la estructura final de una dimensión y, para guardarla, basta pulsar el botón "Guardar", situado en la esquina inferior derecha de la pantalla, como se muestra en la figura siguiente:


.. image:: /figuras/fig_ucloud_findimensao/21_dimensão_estrutura_completa.png
   :alt: Financeiro Dimensão_estrutura_completa
   :align: center
----




Al finalizar esta acción, la "Dimensión" guardada aparece en el listado de Dimensión.




Listado de Dimensión
~~~~~~~~~~~~~~~~~




Para listar la "Dimensión" recién creada, normalmente la pantalla muestra el listado. Al consultar la pantalla "Listado de Dimensión", en caso de que no se actualice automáticamente, el usuario debe pulsar el botón "Actualizar" situado en la esquina superior derecha de la pantalla.


A continuación, la pantalla que muestra la lista debe exhibir la "Dimensión" creada, como aparece en la figura siguiente:




.. image:: /figuras/fig_ucloud_findimensao/22_dimensão_listagem_final.png
   :alt: Financeiro Dimensão_listagem_final
   :align: center
----




La pantalla de arriba "Listado de Dimensión" muestra en la parte superior derecha el nombre del contrato, el símbolo de la funcionalidad "Tareas" y el nombre del usuario conectado.


En esta pantalla el usuario puede elegir entre crear una nueva dimensión, editar una dimensión existente o eliminar una dimensión creada. Presenta los dos botones que permiten "Crear dimensión" o "Actualizar" la lista de dimensiones.


En esta lista se presentan las columnas "Nombre" y "Acciones", las informaciones pueden ser personalizadas y recuperadas haciendo clic en los bloques de 10, 25, 50 o 100 líneas. La columna "Acciones" permite las operaciones "Editar" y "Eliminar".   




Editando una Dimensión
~~~~~~~~~~~~~~~~~~~~~




Para editar una dimensión, el usuario debe hacer clic en el botón correspondiente a la edición en la columna "Acciones" del listado de "Dimensión", como se detalla a continuación:




.. image:: /figuras/fig_ucloud_findimensao/23_dimensão_botão_editar.png
   :alt: Financeiro Dimensão_botão_editar
   :align: center
----


  
Al hacerlo, se muestra la pantalla con la estructura montada y finalizada, como se ejemplifica a continuación. Este ejemplo, utilizando una nueva dimensión, contiene Grupos y `Tags` variados.




.. image:: /figuras/fig_ucloud_findimensao/24_dimensão_estrutura_completa.png
   :alt: Financeiro Dimensão_estrutura_completa
   :align: center
----




Observando la figura anterior, se nota el icono de la basurera. Es decir, el usuario tiene tanto la posibilidad de crear otros grupos y añadir más `Tags`, así como de eliminarlos.  


También se puede constatar que a cada acción realizada, la Estructura, situada en la parte inferior de la página, se modifica.


Para que los cambios tengan efecto, es necesario que el usuario pulse el botón "Guardar" situado al lado de la función de Estructura, ubicado en la parte inferior derecha de la página.




Donde se utiliza la "Dimensión"
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Actualmente, esta implementación agrupa *Tags* y los agrupan en la "Dimensión" creada, facilitando la visualización categorizada en otras funcionalidades de la plataforma.


Además, la "Dimensión" se utiliza en el modal "Crear Budget" que se incluye en la *tarjeta* denominada "Detalles de Sub Budgets" en la desambiguación_ .




.. _desambiguação: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/usr-manual.html#criando-budget-e-sub-budget






—-




4. **Import y Export de ofertas de servicios en (XML + YAML)**: En esta nueva funcionalidad es posible importar y exportar una misma oferta desde cualquier nube, siempre que esté vinculada al Portal uCloud. Anteriormente era posible importar y exportar archivos en formato JSON, ahora se han añadido las opciones de importar y exportar los archivos también en formato XML e YAML. [tag 5.3-b43 10ago]


5. **Import de credenciales del Google en el Secret Manager de la AWS**: Secret Manager es un repositorio donde se almacena las informaciones cuyo acceso está reservado al usuario. Para importar los datos credenciales de Google de este usuario, la acción debe realizarse a través de uCloud para que sean transferidos desde el repositorio escondido de AWS. [tag 5.3-b16 28jul]


6. **Permisos a nivel de Cuenta**: Esta nueva funcionalidad optimiza el proceso de permisos de un usuario. En esta modalidad de permisos a nivel de cuenta, el usuario puede realizar las acciones desde el perfil de permisos creado para él, ya sea básico o avanzado. Este usuario tiene la facultad de gestionar diversos contratos vinculados a una cuenta, según los permisos que se le hayan concedido.


7. **Informe de Monitoreo de Consumo V1**: 


El informe de Monitoreo de Consumo (v1) es una nueva funcionalidad del portal uCloud, que se ocupa del seguimiento de facturación y del detalle completo de los gastos, categorizados por Nubes (por ejemplo, *AWS* y *Azure*), Contratos y Recursos.  




En este documento se generan diferentes tipos de índices, que pueden ser tablas, informes y gráficos, para cada tipo de clase (Recurso, Contrato y Nube). Estos se titulan en los tópicos: 


  1. *Historial de Facturación*;
  2. *Factura por Contrato/Proyecto*;
  3. *Mayores Variaciones en esta Factura* y
  4. *TOP 3 Contratos por Nube en Detalle*.




.. attention:: |atención| Cada una de estas categorías está separada y organizada del mayor al menor consumo. 




Además, el **Informe de Monitoreo de Consumo (v1)**, denominado brevemente como **IMC.v1**, compara los gastos del mes en curso con los del mes anterior, proporcionando a la empresa las informaciones necesarias para que se pueda evaluar el desembolso y tener un control eficiente de las posibles caídas o aumentos de consumo. 






Accediendo al IMC.v1
~~~~~~~~~~~~~~~~~~




Para generar el Informe de Monitoreo de Consumo (v1) en el portal uCloud, el usuario debe acceder al menú "Financiero", identificado en la esquina inferior izquierda. Y a continuación hacer clic en el submenú "Informes".




.. figure:: /figuras/fig_ucloud_fin_rmcv1/1_Menu_Financeiro.png 
   :alt: Menu_Financeiro
   :align: center 


----
  


En la pantalla siguiente se muestran todas las opciones relacionadas con el acceso y la gestión de las facturas de los grupos o contratos que el usuario administra.


  
.. figure:: /figuras/fig_ucloud_fin_rmcv1/2_Financeiro_painéis.png 
   :alt: Financeiro_painéis
   :align: center 


----






Haciendo clic en el submenú "Informes", el tópico "Paneles basados en el Consumo" permite acceder a los informes relacionados con el consumo del mes en curso introducido en la búsqueda por el usuario.


.. figure:: /figuras/fig_budget/17_painéis_consumo.png 
   :alt: Painéis_baseados_consumo
   :align: center 


----
  


En él se agrupan siete tipos de informes, uno de los cuales es el **Informe de Monitoreo de Consumo - IMC.v1**.






.. figure:: /figuras/fig_ucloud_fin_rmcv1/4_Descrição.png 
   :alt: Descrição
   :align: center 


----
  


Al hacer clic en esta opción, el usuario puede generar el documento deseado.






Creación del IMC.v1
~~~~~~~~~~~~~~~~




Tras hacer clic en **Informe de Monitoreo de Consumo (v1) - IMC.v1**, se abre una nueva pantalla en la que el usuario puede seleccionar el mes y el año que desea visualizar, así como filtrar los contratos deseados.






.. figure:: /figuras/fig_ucloud_fin_rmcv1/5_RMConsumo.png 
   :alt: Relatório Monitoramento Consumo v1 
   :align: center 


----
  




En este mismo modal, se muestran dos botones: 




* [**GENERAR INFORME**] Permanece disponible para la activación cuando se selecciona al menos un contrato.
* [**SELECCIONAR TODO**]. Se refiere al filtro de los contratos. Se pueden ver las barras de desplazamiento y de búsqueda.






.. figure:: /figuras/fig_ucloud_fin_rmcv1/6_Seleção_mês_e_ano.png 
   :alt: Seleção_mês_e_ano
   :align: center 


----






La barra de desplazamiento, situada en el lado derecho, ayuda al usuario a navegar por el modal en busca del contrato pretendido. La barra de búsqueda facilita la consulta, el usuario sólo tiene que escribir las letras iniciales del contrato.






.. figure:: /figuras/fig_ucloud_fin_rmcv1/7_Barras_rolagem_pesquisa.png 
   :alt: Barras_rolagem_pesquisa
   :align: center 


----
  






Tras hacer clic en “Generar Informe”, se abre una nueva pantalla en la que aparece el mes seleccionado por el usuario y los botones [*DOWNLOAD*] y [GENERAR NUEVO INFORME].






.. figure:: /figuras/fig_ucloud_fin_rmcv1/8_Download_recorte_RMCv1.png 
   :alt: Desbloquear_download
   :align: center 


----




El desbloqueo del botón [*DOWNLOAD*] sólo se realiza cuando los datos se compilan en la plataforma y la misma proporciona el informe del período y del contrato seleccionado. 








En el ejemplo de la siguiente pantalla, la plataforma informa que el "usuario no tiene informes generados para los contratos y períodos seleccionados" y pide al usuario que pulse sobre [GENERAR NUEVO INFORME]. 


Para la ejecución de la descarga del archivo, basta con que el usuario haga clic en el botón citado.






.. figure:: /figuras/fig_ucloud_fin_rmcv1/9_Gerar_relatório.png 
   :alt: Gerar_relatório
   :align: center 


----  






En el caso de no disponer de datos, los informes no quedan disponibles para el mes seleccionado, el botón [*DOWNLOAD*] aparece inactivo (color gris) y la plataforma emite el mensaje mencionado en el ejemplo anterior e impreso en la imagen de arriba.




Cuando hay datos por publicar para el periodo seleccionado por el usuario, la plataforma comunica al usuario que el informe está en proceso de recopilación de datos.




Siguiendo el *status* en el menú de Tareas
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




En el flujo de crear el IMC.v1, la plataforma presenta dos tipos de situación, según el perfil del usuario que está conectado a la plataforma. El *status* de la tarea en la parte superior de la pantalla difiere, para cada tipo de usuario un procedimiento, según la secuencia descrita:




**Caso 1:** 




* **Usuario admin**: Al abrir la funcionalidad “Tareas”, hay que observar la ventana de "Aprobaciones pendientes" que muestra las columnas: Operación, Usuario, Detalles, Progreso, Fecha de inicio, Duración, *Status* y Acciones. 




**Caso 2:** 




* **Usuario user**: Al crear el informe, debe solicitar al administrador de su contrato que apruebe la tarea solicitada.




**Procedimiento:**


En la columna "Acciones" situada en la ventana "Aprobaciones Pendientes" **el usuario admin** del contrato debe aprobar la acción "Generar Informe". En el caso del **usuario user**, debe solicitar al administrador del contrato que realice o no la aprobación de la tarea.






.. figure:: /figuras/fig_ucloud_fin_rmcv1/10_Tarefas.png 
   :alt: Tarefas
   :align: center 


----




Luego debe esperar la actualización del "Status" que puede ser: En ejecución (*Running*); Fallo (*Failed*) o Éxito (*Successfull*).




Una vez que el proceso de creación del nuevo informe fue exitoso, los datos fueron compilados en la plataforma uCloud. 






Habilitación del *Download* del IMC.v1
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




Una vez creado con éxito el nuevo informe, el usuario debe repetir el flujo para descargarlo, ya que los datos están recopilados en la plataforma uCloud.  


A continuación, es necesario seleccionar de nuevo, el mismo período y los contratos que se desea buscar las informaciones previamente creadas. 
 


.. figure:: /figuras/fig_ucloud_fin_rmcv1/11_Fluxo.png
   :alt: Fluxo_gerar_relatório
   :align: center 


----






En este punto, el usuario debe observar si el botón [GENERAR INFORME] está habilitado (color naranja), en caso afirmativo, significa que el flujo para descargar el IMC.v1 prosigue, los datos están previamente preparados y pueden ser extraídos en formato de informe.




Durante este proceso, la plataforma desbloquea el botón [*Download*] y lo muestra en color verde, como se observa en la siguiente imagen. 






.. figure:: /figuras/fig_ucloud_fin_rmcv1/12_Relatório_gerado.png 
   :alt: Relatório gerado
   :align: center 


---- 






El usuario debe verificar el mensaje que la plataforma presenta: "Informe generado para los contratos y el periodo seleccionado. Puedes descargarlo o generar uno nuevo con las mismas configuraciones".




Al final de esta secuencia de actividades, para ejecutar la descarga del archivo IMC.v1 deseado, el usuario debe hacer clic en el botón [*DOWNLOAD*].






Visualizando el IMC.v1
~~~~~~~~~~~~~~~~~~~~~




Tras generar y descargar el **Informe de Monitoreo de Consumo (v1) - IMC.v1**, se presenta un ejemplo que se describe a continuación:




**Portada**




El documento presenta una portada con las siguientes informaciones:
 
1. Nombre de la empresa;
2. Fecha de Facturación;
3. Texto normalizado sobre la facturación de los consumos en las nubes.




Tal como se muestra a continuación:








.. figure:: /figuras/fig_imcv1_spa/1_portada.png 
   :alt: imcv1 portada
   :align: center 


----
  




**1 - Resumen Ejecutivo** 




En el resumen ejecutivo se presenta un texto explicativo que describe la variación de los valores y el porcentaje que se ha producido en la factura del mes en curso en comparación con el mes anterior, conforme el ejemplo:






.. figure:: /figuras/fig_imcv1_spa/2_resumen_ejecutivo.png 
   :alt: resumen ejecutivo
   :align: center 


----






**1.1 - Historial de Facturación**




Después del resumen ejecutivo, está el Historial de Facturación, que presenta una tabla con el período seleccionado por el usuario, en la que se muestra el valor de la nube deseada en Reales (R$) y Unidad de Servicio de Nube (USN), y la tasa de variación en porcentaje del mes anterior y también del mes actual. 




.. attention::  |atención| Unidad de Servicio de Nube (USN) es un modelo de tarificación de los servicios de nube, asignado a las empresas que están asociadas a las esferas gubernamentales. 


.. important:: La USN pretende establecerse como un método predecible, lineal y flexible para obtener una cantidad específica a cobrar por los servicios de computación en nube.


.. note:: |nota| La métrica USN consiste en establecer un valor de referencia específico para cada tipo de servicio en la nube, según las métricas individuales asociadas al consumo de recursos.








.. figure:: /figuras/fig_imcv1_spa/3_historial_de_facturación.png 
   :alt: historial de facturación
   :align: center 


----




Según el ejemplo de arriba, se comparan los gastos del mes actual con los del mes anterior, mostrando si hubo un aumento o disminución del consumo para cada contrato específico, también exhibe el porcentaje y las posibles variaciones del mes anterior al actual.


Además, esta parte de la implementación expone una regla básica: sólo se especifican los 5 mayores gastos, es decir, se divulgan los contratos que tuvieron mayor consumo durante el mes en curso, junto con los valores de cada uno separadamente.


Esta regla tiene como objetivo mantener el documento más compacto, evitando hacerlo largo, según los ejemplos siguientes: 




* Primer ejemplo nube *AWS*




.. figure:: /figuras/fig_imcv1_spa/4_visualización_ejemplo1aws.png 
   :alt: visualización
   :align: center 


----




Para la complementación y mejor visualización, esta parte del documento genera también un gráfico circular, que contiene las mismas informaciones de los gastos de la tabla de forma ilustrativa, separando los contratos por colores para una mejor comprensión del usuario.




*Segundo ejemplo de gráfico circular nube *AWS*:








.. figure:: /figuras/fig_imcv1_spa/5_grafico_circular_ejemplo2aws.png 
   :alt: Ejemplo
   :align: center 


---- 




.. note:: |nota| En el caso de más de una nube, el informe sigue el mismo formato de presentación e informaciones.






* Tercer ejemplo nube *Azure*:






.. figure:: /figuras/fig_imcv1_spa/6_nube_azure_ejemplo3.png 
   :alt: Exemplo azure
   :align: center 


----




**2 - Factura por Contrato/Proyecto**




En la Factura por Contrato/Proyecto, es informado, en primer lugar, el gasto general de los contratos para cada nube, como se muestra en el resumen ejecutivo, con sus valores en R$ y USN.






.. figure:: /figuras/fig_imcv1_spa/7_factura_por_contrato.png 
   :alt: factura por contrato
   :align: center 


---- 
 




A continuación de la tabla hay un gráfico que contiene la proporción de estos consumos en porcentaje, como se muestra a continuación:




Al igual que en el Historial de Facturación, en la Factura por Contrato/Proyecto, también se genera un gráfico para la complementación y mejor visualización del usuario, conteniendo las mismas informaciones de los gastos de la tabla de forma ilustrativa, demostrando la proporción de los gastos por nube.






 
.. figure:: /figuras/fig_imcv1_spa/8_proporción_de_nubes.png 
   :alt: proporción de nubes
   :align: center 


----






Tras el gráfico, la siguiente imagen expone y especifica **todos** los contratos de cada nube (además de los cinco mayores mostrados en el historial de facturación), siendo resaltados los proyectos más recientes.




El ejemplo de la siguiente tabla detalla los costes de la nube, sus contratos y el valor total, presentados en R$ y USN.






.. figure:: /figuras/fig_imcv1_spa/9_tabla1_ejemplo_aws.png
   :alt: exemplo tabla aws
   :align: center
----




.. figure:: /figuras/fig_imcv1_spa/10_tabla2_ejemplo_azure.png
   :alt: exemplo tabla azure
   :align: center 


---- 




.. note:: |nota| Tenga en cuenta que en el caso de más de una nube, el informe sigue el mismo patrón de presentación e informaciones.




**3 - Mayores Variaciones en esta Factura**




En las "Mayores Variaciones en esta Factura" se presentan en una tabla, todas las variaciones de los contratos del mes de cada proveedor específico, comparando el valor del mes anterior con el valor del mes actual, demostrando la variación de su valor total en porcentaje, por lo tanto, esta parte del documento es un complemento de la "Factura por Contrato/Proyecto".




Esta tabla considera únicamente las variaciones más relevantes, con un corte que contiene, en primer lugar, las mayores o iguales a quince por ciento (>=15%) y, en consecuencia, las menores o iguales a quince por ciento negativo (<= -15%). A continuación, un ejemplo:








.. figure:: /figuras/fig_imcv1_spa/11_mayores_variaciones.png 
   :alt: mayores variaciones
   :align: center 


----






Las **variaciones positivas** (>=15%) se destacan en el **tono azul**, al igual que las **variaciones negativas** (<= -15%) se destacan en el **tono rojizo**. 


Se puede observar que cuanto mayor es la variación, más oscuro es el tono.






.. figure:: /figuras/fig_imcv1_spa/12_mayores_variaciones_ejemplo2.png
   :alt: mayores variaciones 2
   :align: center 


----




Además, el contrato con mayor valor de variación se destaca y presenta las informaciones sobre sus recursos de forma detallada. Este gráfico contiene **todos los recursos del contrato** y sus gastos, informando cuáles fueron los cambios en su consumo y utilización. El gráfico también señala cuáles fueron los recursos que más gastaron en el mes, como se ejemplifica en la siguiente imagen:






.. figure:: /figuras/fig_imcv1_spa/13_cambio_aws.png
   :alt: cambio aws
   :align: center 


---- 








.. figure:: /figuras/fig_imcv1_spa/14_cambio_aws_lista1.png
   :alt: cambio aws lista1
   :align: center 








.. figure:: /figuras/fig_imcv1_spa/15_cambio_aws_lista2.png 
   :alt: cambio aws lista2
   :align: center 


---- 








.. figure:: /figuras/fig_imcv1_spa/16_cambio_azure.png 
   :alt: cambio azure
   :align: center 


----






Justo después del gráfico de barras, se presenta una tabla descriptiva, con las columnas *Producto* y *Importe total* *(R$)* de las cantidades de cada recurso invertido de forma separada y específica, desde el importe más alto al más bajo.


.. figure:: /figuras/fig_imcv1_spa/17_cambio_azure_tabla1.png
   :alt: tabla descriptiva 1
   :align: center 






.. figure:: /figuras/fig_imcv1_spa/18_cambio_azure_tabla2.png
   :alt: tabla descriptiva 2 
   :align: center 


----


.. note:: |nota| En el caso de más de una nube, el informe sigue el mismo patrón de presentación e información.




**4 - TOP 3 Contratos por Nube en Detalle**




Por último, se expone un índice que contiene el recorte de los tres contratos que tuvieron mayor consumo en cada nube, y los recursos que representan el mayor impacto en cada una de ellas. El informe presenta cada una de las nubes utilizadas por la empresa, el nombre de los contratos y sus valores totales en R$ y USN, como se presenta en el siguiente ejemplo:








.. figure:: /figuras/fig_imcv1_spa/19_detalle_aws.png 
   :alt: detalle
   :align: center 


----




A continuación, se publica de manera más detallada el resumen de cuánto cuesta cada producto al contrato, especificándolos y evidenciando el porcentaje sobre los gastos totales de cada contrato. Esta información se demuestra mediante un gráfico ilustrativo como se muestra el siguiente ejemplo: 






.. figure:: /figuras/fig_imcv1_spa/20_detalle_aws_lista1.png
   :alt: detalle aws lista 1
   :align: center 




.. figure:: /figuras/fig_imcv1_spa/21_detalle_aws_lista2.png
   :alt: detalle aws lista2
   :align: center 






.. figure:: /figuras/fig_imcv1_spa/22_detalle_azure_lista1.png
   :alt: detalle azure lista1
   :align: center 


----






.. attention:: |atención| En el caso de más de una nube, el informe sigue el mismo patrón de presentación e información.




Por último, cabe destacar que la implementación **Informe de Monitoreo de Consumo (v1) IMC.v1**, auxilia en el control de los gastos mensuales, presentándolos y comparándolos con el mes anterior.


Esta actualización cuenta con un amplio índice, que contiene tablas, informes y gráficos que van desde lo más general a lo más específico, proporcionando a la empresa y, en consecuencia, al usuario, todas las informaciones y herramientas necesarias que permiten un control total sobre sus inversiones y proyectos.








—-






Adecuación a los Cambios Realizados en las Nubes Públicas y Privadas
==========================


Amazon Web Services (AWS)
-------------------------


En cuanto a la interacción con el proveedor de servicios de nube pública Amazon Web Services (AWS), se enumeran las siguientes mejoras:

+--------------------------------------------------+-----------------+
|*FEATURE*                                         |VERSIÓN          |
+==================================================+=================+
|A partir de esta adecuación, se puede realizar el |tag 5.2-b45 05jul|
|*Import* del *Container* unicamente para la       |                 |
|facturación.                                      |                 |
+--------------------------------------------------+-----------------+


Microsoft Azure (Azure)
-----------------------


En cuanto a la interacción con el proveedor de servicios de nube pública Microsoft AZURE, se pueden enumerar tres mejoras:

+--------------------------------------------------+-----------------+
|*FEATURE*                                         |VERSIÓN          |
+==================================================+=================+
|Cambio de la interfaz gráfica del botón de        |tag 5.3-b12 27jul|
|creación del *Scaling Group*.                     |                 |
+--------------------------------------------------+-----------------+
|Para una mejor experiencia del usuario, se ha     |tag 5.2-b72 21jul|
|optado por ocultar el campo de Grupo de Seguridad |                 | 
|de VDCs.                                          |                 |
+--------------------------------------------------+-----------------+
|Realizar el *Import* del *Container* únicamente   |tag 5.2-b57 13jul|
|para la facturación.                              |                 |
+--------------------------------------------------+-----------------+



Google Cloud Platform (GCP)
---------------------------


En cuanto a la interacción con el proveedor de servicios de nube pública Google Cloud Platform (GCP), se han introducido ocho mejoras que se enumeran a continuación:

+--------------------------------------------------+-----------------+
|*FEATURE*                                         |VERSIÓN          |
+==================================================+=================+
|El botón para asociar el disco a la VM obtiene    |tag 5.2-b38 22jun|
|una nueva interfaz gráfica.                       |                 |
+--------------------------------------------------+-----------------+
|Mejora en el contrato estándar del usuario al     |tag 5.2-b46 05jul|
|crear una Máquina Virtual de Base de Datos.       |                 |
+--------------------------------------------------+-----------------+
|Incorporación de los detalles de *loadbalancers*  |tag 5.2-b46 05jul|
|de un *Scaling Group*.                            |                 |
+--------------------------------------------------+-----------------+
|Adaptación del *Import* del *Container* del tipo  |tag 5.2-b48 07jul|
|*Google*.                                         |                 |
+--------------------------------------------------+-----------------+
|Inclusión de nuevas regiones, éstas son:          |tag 5.2-b64 18jul|
+--------------------------------------------------+-----------------+
|* Melbourne, Victoria, Oceanía:                                     |
|       australia-southeast2                                         |
+--------------------------------------------------------------------+
|* Delhi, Región de la Capital Nacional, Asia:                       |
|       asia-south2                                                  |
+--------------------------------------------------+-----------------+
|Refinamiento de la selección para asociar la      |tag 5.3-b30 03ago| 
|subred al *Import* del *Container*.               |                 |
+--------------------------------------------------+-----------------+
|Asociación de zona al crear VM.                   |tag 5.3-b36 08ago|
+--------------------------------------------------+-----------------+
|Nuevos filtros de facturación:                    |tag 5.2-b57 13jul|
+--------------------------------------------------+-----------------+
|* **Discount**:                                                     |
|                                                                    |
|El tipo de crédito con descuento es utilizado para los importes     | 
|recibidos después de haber alcanzado un umbral de gasto contractual.|
+--------------------------------------------------------------------+
|En los informes de *Cloud Billing* disponibles en la consola, esto  |
|aparece como "Descuentos basados en el gasto (contractuales)".      | 
+--------------------------------------------------------------------+
|* **Free tier**:                                                    |
|Algunos servicios ofrecen "uso gratuito de recursos hasta los       |
|límites especificados". En estos servicios, los créditos            |
|se aplican para implementar el uso de nivel gratuito.               |
+--------------------------------------------------------------------+
|* **Promotion**:                                                    |
|El tipo de crédito promocional incluye prueba gratuita de *Google   | 
|Cloud* y créditos para campañas de marketing u otras concesiones    | 
|para usarlo. Cuando están disponibles, los créditos promocionales   | 
|se consideran una forma de pago y se aplican automáticamente para   |
|reducir la factura total.                                           |
+--------------------------------------------------------------------+



Huawei Cloud (Huawei)
---------------------------------------


En cuanto a la interacción con el proveedor de servicios de nube pública de Huawei, no se produjo ningún cambio, nueva implementación o funcionalidad.




IBM Cloud (IBM)
-------------------


En cuanto a la interacción con el proveedor de servicios de nube pública IBM no hay registro de corrección, cambio, nueva funcionalidad o implementación.




VMware 6.5 o superior (vCenter/vSphere)
----------------------------------------


En cuanto a la interacción con el hipervisor VCenter/vSphere, destacamos la siguiente mejora:

+--------------------------------------------------+-----------------+
|*FEATURE*                                         |VERSIÓN          |
+==================================================+=================+
|La política de programación para *Scaling Group*  |tag 5.3-b36 08ago|
|permite al usuario crear la política que define   |                 |
|el momento de crear nueva(s) máquina(s).          |                 |
+--------------------------------------------------+-----------------+
 


VMWare vCloud (vCloud)
------------------


En relación a la interacción con el hipervisor vCloud no se ha producido ningún cambio, corrección, nueva implementación o funcionalidad.




Perfeccionamiento de la plataforma uCloud
=============================


Ustore renueva la plataforma uCloud en consonancia con la continua evolución de las innovaciones en el sector de *cloud computing*, ambiente dinámico que permite el acceso remoto a softwares, almacenamiento de archivos y procesamiento de datos a través de Internet.


Por lo tanto, la práctica del perfeccionamiento continuo adoptada en la mejora de la plataforma uCloud en *Account*, *OPS* y *Billing*, unida a la productividad, resulta en la siguiente lista de mejorías globales:


+-----------------------------------------------------+-----------------+
|*FEATURE*                                            |VERSIÓN          |
+=====================================================+=================+
|Creación de user en *Account*:  Acceso directo para  |tag 1.0-account68|
|crear un usuario en el menú Administración,          |            04jul|
|“submenú Account”.                                   |                 | 
+-----------------------------------------------------+-----------------+
|Listado por orden alfabético del *container* y VDC   |tag 5.2-b39 23jun|
|en la pantalla de creación de un grupo de seguridad: |                 |
|Al listar los VDCs en la creación de este grupo,     |                 |
|visualización ordenada.                              |                 |
+-----------------------------------------------------+-----------------+
|Listado por orden alfabético del *container* y VDC   |tag 5.2-b39 23jun|
|en la pantalla de creación de una red: La pantalla   |                 |
|de creación de una red presenta el listado ordenado  |                 |
|de *container* y VDC.                                |                 |
+-----------------------------------------------------+-----------------+
|Listado en orden alfabético por *container* y VDC    |tag 5.2-b39 23jun|
|al crear la IP Pública: Al crearla, el listado       |                 |
|ordenado del *container* y del VDC es exhibido.      |                 |
+-----------------------------------------------------+-----------------+
|Mejora de la seguridad de la interfaz del uCloud:    |tag 5.2-b43 30jun|   
|Se han realizado avances en la seguridad del         |                 |
|*Front-End*.                                         |                 |
+-----------------------------------------------------+-----------------+
|El idioma del usuario puede cambiarse a nivel de     |tag 1.0-account66|  
|cuenta, además del nivel de usuario existente:       |            22jun|
|Así una cuenta puede tener un idioma y ser vista por |                 |
|el idioma que el usuario determinar.                 |                 |
+-----------------------------------------------------+-----------------+
|Persistencia en el cambio de idioma del usuario:     |tag 5.2-b61 14jul|
|La plataforma mantiene el idioma elegido en el       |                 |
|primer acceso.                                       |                 |
+-----------------------------------------------------+-----------------+
|Persistencia del idioma en el envío de correos       |tag 5.2-b73 21jul|   
|electrónicos dentro del portal: La plataforma        |                 |
|mantiene el idioma elegido al enviar                 |                 |
|correos electrónicos.                                |                 |
+-----------------------------------------------------+-----------------+
|Adaptação daAdaptación del listado de perfiles       |tag 5.2-b47 06jul|   
|de permisos y visualización en la interfaz gráfica:  |                 |
|El listado de perfiles aparece por encima del modal, |                 |
|optimiza visualizar.                                 |                 |
+-----------------------------------------------------+-----------------+
|Creación de *Tags* virtuales con la misma clave y    |tag 5.2-b49 07jul|   
|valor diferentes: Esta mejora permite la creación de |                 |
|una o más *Tags* con claves iguales y valores        |                 |
|diferentes.                                          |                 |
+-----------------------------------------------------+-----------------+
|Actualización del CORE.sql de uCloud: Agiliza        |tag 5.2-b52 12jul| 
|significativamente la respuesta del entorno.         |                 |
+-----------------------------------------------------+-----------------+
|Actualización de las cuotas en toda la plataforma    |tag 5.2-b52 12jul|  
|uCloud: Su unificación en todos los ambientes        |                 |
|estandariza la visualización de las cuotas de los    |                 |
|usuarios en las funcionalidades de los contratos     |                 |
|y de los grupos.                                     |                 | 
+-----------------------------------------------------+-----------------+
|En el menú de la funcionalidad de Configuración, el  |tag 5.2-b55 13jul|
|submenú General contempla la adición del botón       |                 |
|(ON/OFF) en la activación automática y del uCloud    |                 |
|v.2, este botón indica que la función está activada  |                 |
|o desactivada.                                       |                 | 
+-----------------------------------------------------+-----------------+
|Actualización del formato de recuperación de         |tag 5.2-b60 14jul|
|contraseñas.                                         |                 | 
+-----------------------------------------------------+-----------------+
|Mejora en la personalización del *branding* a nivel  |tag 5.3-b08 26jul| 
|de contrato.                                         |                 |
+-----------------------------------------------------+-----------------+
|En el menú Tareas, en su lista de tareas en          |tag 5.2-b69 20jul|  
|operación, la columna "Acciones" permite al usuario  |                 |
|cancelar o pausar una *Task* independientemente del  |                 |
|*status*, a condición de que el porcentaje sea       |                 |
|inferior al 99%.                                     |                 |
+-----------------------------------------------------+-----------------+
|Actualización en la funcionalidad "*Checkbox*"       |tag 5.3-b43 10ago|
|asociando todas las VMs en el contrato y en el grupo.|                 |
|[mejora]                                             |                 |
+-----------------------------------------------------+-----------------+
|En el Menú Administración haciendo clic en el        |tag 5.3-b54 17ago| 
|submenú Contratos y seleccionando un determinado     |                 |
|Contrato de la lista, es permitido                   |                 |
|"Añadir Administradores" sea usuario o grupo de      |                 | 
|usuarios. Para facilitar la búsqueda, se ha          |                 |
|incorporado una barra de búsqueda que ofrece como    |                 |
|resultado el nombre de un usuario o de un grupo.     |                 |
+-----------------------------------------------------+-----------------+
|Creación de cuota por cantidad de VM/Instancia por   |tag 5.3-b36 08ago| 
|contrato.                                            |                 |
|[nueva funcionalidad]                                |                 |
+-----------------------------------------------------+-----------------+
|Adaptación de *Workflow* para soportar la            |tag 5.3-b50 15ago| 
|secuenciación de diversas tareas (de manera          |                 |
|secuencial y/o en paralelo, sin número máximo) de    |                 |
|*workflows* existentes en el portal.                 |                 |
|[nueva funcionalidad]                                |                 |
+-----------------------------------------------------+-----------------+
|Aprobación de *task* por exceder cuota: Cuando un    |tag 5.3-b53 16ago| 
|usuario excede la cuota existente en el contrato,    |                 |
|automáticamente el administrador se da cuenta de que |                 |
|el usuario necesita más cuota. Así, el administrador |                 |
|puede aprobar o no esta solicitud.                   |                 |
|[nueva funcionalidad]                                |                 |
+-----------------------------------------------------+-----------------+
|Nueva presentación en el Informe Financiero en la    |tag 1.0-account79| 
|interfaz de datos del *Billing*.                     |            01ago|
+-----------------------------------------------------+-----------------+
|Opción *CentOS7* para creación de *ResourceKey*:     |tag 5.3-b09 26jul|                  
|requisito de la nube cumplido al añadir *CentOS7*    |                 |
|como Sistema Operativo para etiquetar USN.           |                 |
|[nueva funcionalidad]                                |                 |
+-----------------------------------------------------+-----------------+
|Kubernetes para crear *ResourceKey*: adición de      |tag 5.2-b45 05jul|           
|Kubernetes como Sistema Operativo como requisito de  |                 |
|Google para etiquetar máquinas Kubernetes.           |                 |
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+
|El menú Perfil de *Tag* Virtual mejora la experiencia|tag 5.2-b57 13jul| 
|del uso al permitir nombres similares en la creación |                 |
|del perfil de tag virtual e impedir el uso de        |                 |
|caracteres especiales.                               |                 |
+-----------------------------------------------------+-----------------+
|Incremento del perfil de *Tag Virtual* incluyendo    |tag 5.2-b65 18jul| 
|el campo *uCloudIdentifier* que se utiliza como      |                 |
|referencia. Está aplicado en las operaciones del     |                 |
|*container* y de los billetes.                       |                 |
+-----------------------------------------------------+-----------------+
|El menú Catálogo de Servicios tras refactorizar el   |tag 5.2-b58 13jul| 
|punto de transmisión y recepción de información      |                 | 
|'*endpoint*' detalla el resultado sólo cuando el     |                 | 
|usuario solicita la búsqueda.                        |                 |
+-----------------------------------------------------+-----------------+
|Asociar el mismo precio de *USN Tag* para varios     |tag 5.2-b65 18jul| 
|contratos: se ha eliminado la restricción de *Tag*   |                 |
|para un único contrato.                              |                 |
+-----------------------------------------------------+-----------------+
|El menú Tareas recibe la actualización del registro  |tag 5.3-b09 26jul| 
|de *task* en las actividades ocurridas en el         |                 |
|*Billing* dentro del portal.                         |                 |
+-----------------------------------------------------+-----------------+
|Adición de variables al crear un *Tag virtual*.      |tag 5.3-b49 15ago| 
+-----------------------------------------------------+-----------------+
|Informe de monitoreo del consumo: Adición del        |tag 5.3-b18 28jul| 
|Identificador Único Universal - UUID del *container*,|                 |
|optimiza el cierre de la factura del contrato que    |                 |
|monitorea el consumo.                                |                 |
+-----------------------------------------------------+-----------------+
|La pantalla de Resumen detallado de la factura       |tag 5.3-b22 29jul| 
|incrementa la carga de datos y acelera la entrega    |                 |
|del resultado de la solicitud en su interfaz.        |                 |
+-----------------------------------------------------+-----------------+
|Mejora en la visualización del cierre de facturas con|tag 5.3-b46 10ago| 
|usuarios multicontratos: Un usuario vinculado a más  |                 |
|de un contrato, tiene la opción de ver el cierre de  |                 |
|la factura con los gastos de cada contrato específico|                 |
|de forma individual.                                 |                 |
+-----------------------------------------------------+-----------------+
|*Checkbox* de seleccionar todos los VDC de un        |tag 1.0-account88|  
| contrato.                                           |            10ago|
+-----------------------------------------------------+-----------------+
|*Loader* para la carga retrasada de uCloud.          |tag 5.3-b15 28jul|
|[nueva funcionalidad]                                |                 |
+-----------------------------------------------------+-----------------+
|Campo de búsqueda para subredes dentro de la pantalla|tag 5.2-b72 21jul| 
|de la máquina virtual.                               |                 |
+-----------------------------------------------------+-----------------+
|Reactivación de la función de *stop* de VM.          |tag 5.2-b72 21jul|
+-----------------------------------------------------+-----------------+
|Listado de datos detallados del *Billing*.           |tag 5.3-b09 26jul|
+-----------------------------------------------------+-----------------+
|Manera como el informe consolidado presenta          |tag 5.3-b11 27jul|
|los datos.                                           |                 |
+-----------------------------------------------------+-----------------+
|Creación de persistencia en la validación de recursos|tag 5.2-b47 06jul| 
|que no están en el contrato para creación de máquina |                 |
|virtual y *Scaling Group*.                           |                 |
+-----------------------------------------------------+-----------------+    



Acciones Correctivas Globales
===================


Este tópico enumera las acciones correctivas llevadas a cabo por nuestro equipo de desarrollo, identificadas como resultado de los *reports* generados en la experiencia del uso y *quality assurance*. Las acciones correctoras de *fix* y *bugs* pueden referirse a: Adecuaciones a las nubes y mejoras de la plataforma uCloud en *Account*, *OPS* y *Billing*.




Adecuaciones a las nubes
===================


Amazon Web Services (AWS)
---------------------------------------


En cuanto a la interacción con el proveedor de servicios de nube pública Amazon Web Services (AWS), se puede enumerar una acción correctiva:

+-----------------------------------------------------+-----------------+
|*FEATURE*                                            |VERSIÓN          |
+=====================================================+=================+
|Creación del Balanceador con el Grupo de Seguridad   |tag 1.0-account65| 
|seleccionado.                                        |            20ago|
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+



Microsoft Azure (Azure)
------------------------------


En cuanto a la interacción con el proveedor de servicios de nube pública Microsoft AZURE, se enumeran las siguientes correcciones:

+-----------------------------------------------------+-----------------+
|*FEATURE*                                            |VERSIÓN          |
+=====================================================+=================+
|Persistencia al añadir un *loadbalancer* a una       |tag 5.2-b51 08jul| 
|máquina virtual de Azure.                            |                 |
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+
|Cambio en el cálculo de los discos Azure.            |tag 5.3-b45 10ago|
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+
|Se ha ocultado el botón *"Edit Subnet"*, que antes   |tag 5.2-b72 21jul| 
|provocaba la inactivación de *inputs* a la hora de   |                 |
|crear subredes.                                      |                 |
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+


Google Cloud Platform (GCP)
--------------------------------------


En cuanto a la interacción con el proveedor de servicios de nube pública Google Cloud Platform (GCP), se pueden enumerar las siguientes correcciones:

+--------------------------------------------------+-----------------+
|*FEATURE*                                         |VERSIÓN          |
+==================================================+=================+
|Llamada en *loop* desde la pantalla de *storage*. |tag 5.2-b38 22jun|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Creación de un *loadbalancer*, y la rectificación |tag 5.2-b46 05jul| 
|del mensaje de error.                             |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+ 


Huawei Cloud (Huawei)
------------------------------


En cuanto a la interacción con el proveedor de servicios de nube pública Huawei Cloud, no hubo ningún cambio, corrección, nueva implementación o nueva funcionalidad.


IBM Cloud
-----------


En cuanto a la interacción con el proveedor de servicios de nube pública IBM Cloud, se enumera la siguiente corrección:

+--------------------------------------------------+-----------------+
|*FEATURE*                                         |VERSIÓN          |
+==================================================+=================+
|Los listados de los recursos se ponen a           |tag 5.2-b64 18jul|  
|disposición filtrando las regiones a la hora de   |                 |
|la creación de las redes.                         |                 | 
|[bug]                                             |                 |
+--------------------------------------------------+-----------------+


VMware vCloud
-------------------


En cuanto a la interacción con el hipervisor de la nube privada VMware 6.5 (o superior), se pueden enumerar las siguientes correcciones:

+--------------------------------------------------+-----------------+
|*FEATURE*                                         |VERSIÓN          |
+==================================================+=================+
|VMware clonaba una VM de *Scaling Group*.         |tag 5.2-b62 14jul|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Gestión de escalamiento basada en las *policies*  |tag 5.3-b14 28jul| 
|(Métricas) de escritura y lectura del disco.      |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+




Plataforma uCloud
===============


**OPS** 

+--------------------------------------------------+-----------------+
|*FEATURE*                                         |VERSIÓN          |
+==================================================+=================+
|Filtro VDC en el grupo.                           |tag 5.2-b65 18jul|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Filtro VDC en la empresa.                         |tag 5.2-b65 18jul|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+             
|Persistencia del logotipo del portal en el primer |tag5.2-b39 23jun | 
|acceso.                                           |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Pantalla VDC en *loop*.                           |tag 5.2-b44 05jul| 
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Persistencia del dato en el precio de coste total |tag 5.2-b54 13jul| 
|a partir del *amount* mostrado en pantalla.       |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Bloqueo de la pantalla del *dashboard* de uCloud  |tag 5.3-b17 28jul|
|al realizar el *login*.                           |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Adición de VM a un *workflow*.                    |tag 5.3-b51 16ago|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Operaciones de subred.                            |tag 5.3-b54 17ago|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Persistencia de las nuevas traducciones en el     |tag 5.2-b44 05jul|
|el *Dashboard*.                                   |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|*Query* para VM.                                  |tag 5.3-b39 08ago|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+


**Billing**

+--------------------------------------------------+-----------------+
|FEATURE                                           |VERSÃO           |
+==================================================+=================+
|*Pop-up VirtualTags*                              |tag 5.2-b45 05jul|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Datos duplicados en el *pop-up* de los detalles de|tag 5.2-b45 05jul|  
|los detalles de la factura del usuario.           |                 | 
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Informe CSV detallado para rellenar la columna en |tag 5.2-b45 05jul|  
|USN.                                              |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|No listar recursos marcados con USN.              |tag 5.2-b45 05jul|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|*NullPointer* para obtener la moneda en el proceso|tag 5.2-b65 18jul|  
|de cálculo de la factura.                         |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Adición de una columna al informe financiero del  |tag 5.3-b02 22jul| 
|*Billing*.                                        |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|*Nullpoint* en la facturación del informe         |tag 5.3-b02 22jul|    
|consolidado del *Billing*.                        |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Datos encontrados al generar el informe detallado.|tag 5.3-b06 25jul| 
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Acción realizada para entregar los valores en el  |tag 5.3-b06 25jul| 
|contrato.                                         |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Resumen por *Container* del Informe PDF.          |tag 5.3-b23 29jul|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Informe PDF de las facturas cerradas.             |tag 5.3-b31 03ago|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|*Export* de CSV del informe financiero.           |tag 5.3-b35 05ago|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Cálculo USN.                                      |tag 5.2-b58 13jul|
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Llamada de pantalla de mi factura por grupo para  |tag 5.3-b25 01ago|
|la carga de datos.                                |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
|Eliminado el problema del Informe Detallado que   |tag 5.3-b46 10ago|
|aparecía vacío.                                   |                 |
|[fix]                                             |                 |
+--------------------------------------------------+-----------------+
 


====


====




En esta nota se evoca el principio de la norma ISO 9001, elaborada por la Organización Internacional de Normalización (en Brasil conocida como ABNT NBR ISO 9001). Su objetivo es establecer normas consistentes que aumenten la calidad de los procesos aplicados y redundan una mejora continua y ajustes en las funcionalidades, en busca de una gestión de calidad y excelencia empresarial. 

Todo lo anterior se refiere al principio de la norma ISO 9001.


En resumen, el documento presenta:
* Siete (7) nuevas implantaciones; 
* Trece (13) mejoras realizadas en la categoría *Cloud* debido a la demanda en la adaptación a los cambios en estos proveedores; 
* Cuarenta (40) mejoras globales de la plataforma uCloud;  
* Treinta y cuatro (34) acciones correctivas; 
* Nueve (09) relacionadas con las nubes; 
* Diez (10) relativas a uCloudOPS; 
* Quince (15) pertenecen al *Billing*. 


Por tanto, se concluye las notas de publicación del trimestre correspondiente a los meses de junio, julio y agosto del presente año.








.. |atencao| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/hand-stop-o.png?raw=true

.. |nota| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/hand-pointer-o.png?raw=true

.. |importante| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/warning.png?raw=true