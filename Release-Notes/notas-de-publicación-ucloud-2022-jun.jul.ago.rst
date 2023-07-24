.. figure:: /figuras/ucloud.png
   :alt: Logo uCLoud
   :scale: 60 %
   :align: center
   
----

.. centered:: Português_     -     Español     -     English_

.. _Português: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Release-Notes/nota-de-lançamento-ucloud-2022-jun.jul.ago.html 

.. _English: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Release-Notes/press-release-ucloud-2022-jun.jul.aug.html 

====

2022.06-08
++++++++++

Notas de publicación: uCloud
============================

Período: Junio | Julio | Agosto 

Versión: `Update tags 5.3-b56 y 1.0-account88`

====

Presentación
============

Ustore renueva la plataforma uCloud en línea con la continua evolución de las innovaciones en el sector de *cloud computing*, un ambiente dinámico que permite el acceso remoto a softwares, almacenamiento de archivos y procesamiento de datos a través de Internet.

Este lanzamiento evoca el principio de la norma ISO 9001, desarrollada por la *Organización Internacional de Normalización* (en Brasil conocida como ABNT NBR ISO 9001). El objetivo es establecer normas consistentes que aumenten la calidad de los procesos aplicados y resulten en una mejora continua y ajustes en la funcionalidad, en busca de gestión de calidad y excelencia empresarial.

Las mejoras que se presentan a continuación se refieren al principio de gestión de la calidad citado en la norma ISO 9001, realizadas durante los meses de junio, julio y agosto del año en curso.


====

Noticias
========


Esta nota de publicación divulga las treinta y tres mejoras globales realizadas en algunos menús de funcionalidades del portal, catorce ajustes elaborados para los cambios en la nube y las siete nuevas implementaciones. Están clasificadas en:

* Nubes públicas y privadas;

* Mejora de la plataforma uCloud en *Account*, *uCloudOPS* y *Billing*;

* Nuevas implementaciones.

====

Nubes Públicas y Privadas
=========================

*Amazon Web Services (AWS)*
---------------------------

En relación a la interacción con el proveedor de servicios de nube pública Amazon Web Services (AWS):

* A partir de esta nota se puede ser realizado el *Import* del *Container* únicamente para la facturación.

*Microsoft Azure (Azure)*
-------------------------

Con respecto a la interacción con el proveedor de servicios de nube pública Microsoft AZURE, podemos enumerar tres mejoras:

* Cambio de la interfaz gráfica del botón de creación de *Scaling Group*;

* Para una mejor experiencia del usuario, optamos por ocultar el campo de Grupo de Seguridad de los VDCs;

* Realizar el *Import* del *Container* sólo para la facturación.

*Google Cloud Platform (GCP)*
-----------------------------

En cuanto a la interacción con el proveedor de servicios de nube pública *Google Cloud Platform* (GCP), se han introducido ocho mejoras que se enumeran a continuación:

* El botón para asociar el disco con la VM obtiene una nueva interfaz gráfica;

* Mejora en el contrato estándar del usuario al crear una DBVM;

* Adición del detallamiento de *loadbalancers* de un *Scaling Group*;

* Adaptación del *Import* de *Containers* del tipo Google;

* Inclusión de las nuevas regiones, que son:

  * Melbourne, Victoria, Oceanía: australia-southeast2.
  
  * Delhi, Región de la Capital Nacional, Asia: asia-south2.

* Perfeccionamiento de la selección para asociar la subred al Import del Container.

* Asociación de zonas al crear VM.

* Nuevos filtros de facturación:

  * **Discount**: El tipo de crédito con descuento se utiliza para los valores recibidos tras alcanzar un límite de gasto contractual. En los informes de *Cloud Billing* disponibles en la consola, esto aparece como "Descuentos Basados en el Gasto (contractual)".
  
  * **Free tier**: Algunos servicios ofrecen "uso gratuito de recursos hasta unos límites especificados". En estos servicios, los créditos se aplican para implementar el uso de nivel gratuito.

  * **Promotion**: El tipo de crédito promocional incluye "Prueba gratuita de Google Cloud y créditos para campañas de marketing u otras concesiones para utilizar Google Cloud". Cuando están disponibles, los créditos promocionales se consideran una forma de pago y se aplican automáticamente para reducir la factura total.



VMware 6.5 ou superior (vCenter/vSphere)
----------------------------------------

En cuanto a la interacción con el hipervisor VMware 6.5 o superior, se relaciona la siguiente mejora:

* La política de programación de Scaling Group permite al usuario crear la política que define el momento de crear nuevas máquinas.

====

Perfeccionamiento de la plataforma uCloud en *Account*, *uCloudOPS* y *Billing*
===============================================================================

En Ustore la práctica de perfeccionamiento continuo adoptado en la mejora de la plataforma uCloud, asociado a la productividad, resulta en la siguiente lista:

* Creación de *User* en *Account*:  Atajo para crear un usuario directamente en el menú Administración, submenú *Account*.

* Listado en orden alfabético del *container* y del VDC en la pantalla de creación de un grupo de seguridad: Al listar los VDCs en la creación de un grupo de seguridad, la visualización es en orden alfabético.

* Listado en orden alfabético de *container* y VDC en la pantalla de creación de una red: La pantalla de creación de una red muestra el listado en orden alfabético del *container* y del VDC.

* Listado en orden alfabético por *container* y VDC en la creación de la IP Pública: Al crear la IP Pública, el listado que se muestra, del *container* y del VDC, está en orden alfabético.

* Mejora de la seguridad de la interfaz de uCloud: Se han realizado mejoras de seguridad en el *Front-End* de uCloud.

* El idioma del usuario se puede cambiar a nivel de cuenta, además del nivel de usuario existente: Así, una cuenta puede tener un idioma y ser vista por el idioma que el usuario determine.

* Persistencia en el cambio de idioma del usuario: La plataforma conserva el idioma elegido en el primer acceso.

* Persistencia del idioma al enviar correos electrónicos dentro del portal: La plataforma mantiene el idioma elegido al enviar correos electrónicos.

* Adaptación del listado de perfiles de permisos y visualización en la interfaz gráfica: el listado de perfiles aparece encima del modal, facilitando la visualización.

* Creación de *Tags* virtuales con la misma clave, pero con diferentes valores: Esta mejora permite la creación de una o más *Tags* con claves iguales y valores diferentes.

* Actualización de CORE.sql de uCloud: Agiliza significativamente la respuesta del ambiente.

* Actualización de cuotas en toda la plataforma uCloud: La unificación de las cuotas en todos los ambientes estandariza la visualización de las cuotas de los usuarios en la funcionalidad de los contratos y los grupos. 

* En el menú de la funcionalidad de Configuración, el submenú General contempla la adición del botón (ON/OFF) en la activación automática y de uCloud v.2, este botón indica que la función está habilitada o deshabilitada.

* Actualización del formato de recuperación de contraseñas.

* Mejora en la customización del *branding* en el menú de funcionalidades del *Billing* para la versión *mobile*, con el fin de asegurar la mejor visualización en las opciones de modo claro y oscuro.

* En el menú Tareas, en la lista de tareas en operación la columna "Acciones" permite al usuario cancelar o pausar una *Task* independientemente del *status*, en tanto que el porcentaje sea inferior al 99%.

* Actualización en la funcionalidad "*Checkbox*" asociando todas las VMs en el contrato y en el grupo. 

* En el Menú Administración haciendo clic en el submenú Contratos y seleccionando un determinado Contrato de la lista, es permitido "Añadir Administradores" sea un usuario o un grupo de usuarios. Para facilitar la búsqueda, se ha añadido una barra de búsqueda que ofrece como resultado el nombre de un usuario o de un grupo.

* Creación de cuota por cantidad de VM/Instancia por contrato.

* Adaptación de *Workflow* para soportar el encadenamiento de varias tareas (de forma secuencial y/o paralela, sin número máximo) de *Workflows* existentes en el portal.

* Aprobación de *Task* al exceder la cuota: Cuando un usuario excede la cuota existente en el contrato, automáticamente el administrador se da cuenta de que el usuario necesita más cuota. Así, el administrador puede aprobar o no esta solicitud.

* Nueva presentación en el Informe Financiero en la interfaz de datos del *Billing*.

* Opción CentOS7 para creación de *ResourceKey*: requisito de la nube atendido con la adición de CentOS7 como Sistema Operativo para etiquetar USN.

* Kubernetes para crear *ResourceKey*: adición de Kubernetes como Sistema Operativo como requisito de Google para etiquetar máquinas Kubernetes.

* El menú Perfil de Tag Virtual mejora la experiencia de uso permitiendo nombres similares en la creación del perfil de *Tag* Virtual y evitar el uso de caracteres especiales.

* Incremento del perfil de *Tag* Virtual incluyendo el campo *uCloudIdentifier* que es utilizado como referencia. Se aplica a las operaciones de container y taquilleros.   

* El menú Catálogo de Servicios después de refactorizar el punto de transmisión y recepción de información '*endpoint*' detalla el resultado sólo cuando el usuario solicita la búsqueda.

* Asociar el mismo precio de *USN Tag* para varios contratos: se ha eliminado la restricción de *Tag* para un solo contrato.

* El menú Tareas recibe la actualización del registro de *Taks* en las actividades ocurridas en *Billing* dentro del portal.

* Se añaden variables al crear un Tag virtual.

* Mejora en el informe de supervisión del consumo: La incorporación del Identificador Único Universal - UUID del *container*, optimiza el cierre de la factura del contrato que monitorea el consumo.

* La pantalla de resumen detallado de la factura, incrementa la carga de datos y hace más rápida la entrega de resultados de la petición en su interfaz. 

* Mejora en la visualización del cierre de facturas con usuarios multicontratos: Un usuario vinculado a más de un contrato, tiene la opción de ver el cierre de la factura con los gastos de cada contrato específico de forma individual.

====

Nuevas Implementaciones
=======================

En este informe, Ustore da a conocer las siete innovaciones que han tenido lugar en la plataforma uCloud, que se describen brevemente a continuación:

1. **Budget**: Corresponde a un informe basado en el consumo que tiene como objetivo definir el presupuesto total para un periodo determinado, que puede ser mensual, trimestral, semestral o anual. Este informe permite controlar la utilización del *Budget*.

2. **Customización del Branding a nivel de contrato**: El *Branding* del portal Multicloud se permite a través de la personalización definida contractualmente. El cliente usuario tiene las características de su marca (Empresa) representadas en el portal Multicloud, como los colores, el logotipo, etc.

3. **Dimensión**: Para evitar que recursos idénticos sean etiquetados de formas diferentes, la dimensión fue creada para agrupar *Tags* distintos a recursos del mismo contexto. Así, se crearon operaciones lógicas y un filtro con el fin de identificar en el *Billing* qué recursos pertenecen a una determinada dimensión.

4. **Import y Export de ofertas de servicios en (XML + YAML)**: En esta nueva funcionalidad es posible importar y exportar una misma oferta desde cualquier nube mientras se encuentre vinculada al Portal uCloud. Anteriormente era posible importar y exportar archivos en formato JSON, luego se añadieron las opciones de importar y exportar archivos también en formato XML e YAML.

5. **Import de credenciales del Google en el Secret Manager de AWS**: *Secret Manager* es un repositorio donde se guarda las informaciones a la que sólo el usuario tiene acceso. Para importar los datos de las credenciales de Google de este usuario, la acción debe realizarse a través de uCloud para transferirlos desde el repositorio oculto de la AWS.

6. **Permisos a nivel de cuenta**: Esta nueva funcionalidad optimiza el proceso de permisos de un usuario. En este modo de permiso a nivel de cuenta, el usuario puede realizar las acciones a partir del perfil de permiso creado para él, sea básico o avanzado. Este usuario tiene la facultad de gestionar varios contratos vinculados a una cuenta, de acuerdo con los permisos que se le hayan concedido.

7. **Informe de Supervisión de Consumo V1**: Nueva funcionalidad de uCloud que se ocupa del detallamiento completo de los gastos, divididos por Nubes, Contratos y Recursos. Se generan diferentes tipos de informes, para cada tipo de división (Nube/Contrato/Recurso), separando uno a uno y organizándolos desde el más alto al más bajo consumo. Además de comparar con los gastos de los meses anteriores, proporcionando al cliente las informaciones necesarias para evaluar si hubo una disminución o un aumento de los gastos.

En resumen, el documento presenta las catorce (14) mejoras realizadas en la categoría de nube pública y privada por la demanda en la adecuación a los cambios de estos proveedores. Las treinta y tres (33) mejoras globales de la plataforma uCloud. Además de las siete (7) nuevas implantaciones. Con esto concluye el documento con las notas de publicación de este trimestre correspondientes a los meses de junio, julio y agosto del presente año.
