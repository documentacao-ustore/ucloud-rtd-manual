
.. figure:: /figuras/ucloud.png
   :alt: Logo uCLoud
   :scale: 60 %
   :align: center
   
----


Release do Trimestre: Junho | Julho | Agosto - Ano 2022
=======================================================
Plataforma uCloud versão: *Update tags 5.3-b56 e 1.0-account90*

----


Apresentação
============


Este release da Plataforma uCloud é uma ferramenta de comunicação fundamental ao trabalho de divulgação e difusão das novidades sobre o produto, inovações geradas na área de desenvolvimento.


O release além de ser um material informativo com conteúdo relevante sobre as entregas de um ou mais incrementos na aplicação, tem como objetivo fornecer resultado ao investimento dos clientes, obter parecer e noticiar o progresso, seja de aprimoramento, melhorias ou correções. Realmente oferece a visibilidade adequada no processo de desenvolvimento do produto.


----


Notícias 
========


As novidades  deste período sobre a plataforma uCloud abrange as sete (7) novas implementações, as treze (13) melhorias realizadas na categoria *Cloud* pela demanda na adequação às mudanças nesses provedores, quarenta (40) aprimoramentos globais da plataforma uCloud e as trinta  e quatro (34) ações corretivas, sendo nove (09) relacionadas as nuvens, dez (10) relativas a uCloudOPS e quinze (15) pertencentes ao *Billing*.

Tópicos a serem descritos neste documento:

* Novas implementações;


* Adequações às nuvens públicas e privadas;


* Aprimoramento da plataforma uCloud;


* Ações corretivas.


----


Novas Implementações
====================

Este tópico apresenta as sete novas implementações e insere *hyperlinks* em alguns termos que encaminham o leitor a ampliar seu conhecimento a respeito de determinada implementação. Ao acessar informações detalhadas sobre cada um deles, no manual de uso do uCloud, hospedado no repositório/*wiki* da Ustore.


1. **Budget**
 
Esta nova implementação corresponde a um relatório baseado em consumo que tem como objetivo definir o orçamento total referente a um determinado período, seja mensal, trimestral, semestral ou anual. 

As informações detalhadas sobre o uso do Budget_ podem ser acessadas no repositório/*wiki* que abriga o manual de uso do uCloud.

.. _Budget: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/usr-manual.html#budget


----


2. **Customização do branding a nível de Contrato**

A branding do portal Multicloud é permitida através da personalização definida por contrato. O cliente usuário pode selecionar as características da sua marca (Empresa) representada no portal Multicloud como as cores, a logomarca, entre outras.


----


3. **Dimensão**

Para evitar recursos iguais sendo tagueados de formas diferentes, a dimensão foi criada para agrupar *tags* distintas a recursos do mesmo contexto. Para isso, foram criadas operações lógicas e um filtro, com o intuito de identificar no *Billing* quais recursos pertencem a uma determinada dimensão.

O detalhamento das informações a respeito da implementação Dimensão_ podem ser acessadas no repositório/*wiki* que hospeda o manual de uso do uCloud.


.. _Dimensão: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/usr-manual.html#dimensao


----


4. **Import e Export de ofertas de serviço em (XML + YAML)**

Nessa nova funcionalidade é possível importar e exportar uma mesma oferta de uma nuvem qualquer contanto que esteja vinculada ao Portal uCloud. Antes era possível importar e exportar arquivos em formato JSON, então foram adicionadas as opções de importar e exportar os arquivos também em formato XML e YAML. [tag 5.3-b43 10ago]


----


5. **Import de credenciais do Google no Secret Manager da AWS**

Secret Manager é um repositório onde são gravadas as informações que somente o usuário tem acesso. Para importar os dados credenciais da Google deste usuário, a ação deve ser feita através do uCloud para que estes sejam transferidos do repositório escondido da AWS. [tag 5.3-b16 28jul]


----


6. **Permissões a Nível de Conta**

Esta nova funcionalidade otimiza o processo de permissão de um usuário. Nesta modalidade de permissão a nível de conta, o usuário pode realizar as ações a partir do perfil de permissão criado para ele, seja básico ou avançado. Este usuário tem o poder de administrar diversos contratos vinculados a uma conta, de acordo com as permissões que lhe foram concedidas.


----


7. **Relatório de Monitoramento de Consumo V1** 

Nova funcionalidade do uCloud que trata do detalhamento completo dos gastos, divididos por Nuvens, Contratos e Recursos. São gerados diferentes tipos de relatórios, para cada tipo de divisão (Nuvem/Contrato/Recurso), separando um por vez e organizando-os do maior para o menor consumo. Além de comparar com os gastos dos meses anteriores, proporcionando ao cliente informações necessárias para que se possa avaliar se houve queda ou aumento dos gastos.

O detalhamento das informações podem ser lidas no manual de uso do uCloud, menu Financeiro, que abriga o submenu Relatórios > Painéis baseados em consumo,  neste encontra-se o Relatório_ de Monitoramento de Consumo v1.

.. _Relatório: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/usr-manual.html#relatorio-de-monitoramento-de-consumo


----


Adequação às mudanças ocorridas em Nuvens
=========================================


Amazon Web Services (AWS)
-------------------------


Em relação à interação com o provedor de serviço de nuvem pública Amazon Web Services (AWS) lista-se a melhoria a seguir:


* A partir desta adequação pode ser realizado o *Import* do Container unicamente para o faturamento. [tag 5.2-b45 05jul]


Microsoft Azure (Azure)
-----------------------


Relativo à interação com o provedor de serviço de nuvem pública Microsoft AZURE, pode-se listar três melhorias:


* Alteração da interface gráfica do botão de criação do *Scaling Group* [tag 5.3-b12 27jul];

* Para a melhor experiência do usuário, opta-se por ocultar o campo de Grupo de Segurança dos VDCs [tag 5.2-b72 21jul];

* Realizar o *Import* do Container somente para o faturamento [tag 5.2-b57 13jul].


Google Cloud Platform (GCP)
---------------------------


No que concerne à interação com o provedor de serviço de nuvem pública Google Cloud Platform (GCP), houveram oito melhorias listadas na sequência:


+--------------------------------------------------+-----------------+
|FEATURE                                           |VERSÃO           |
+==================================================+=================+
|O botão para associar o disco à VM recebe nova    |tag 5.2-b38 22jun|
|interface gráfica                                 |                 |
+--------------------------------------------------+-----------------+
|Aprimoramento no contrato padrão do usuário ao    |tag 5.2-b46 05jul|
|criar uma Máquina Virtual de Banco de Dados       |                 |
+--------------------------------------------------+-----------------+
|Adição do detalhamento de *loadbalancers* de um   |tag 5.2-b46 05jul|
|*Scaling Group*                                   |                 |
+--------------------------------------------------+-----------------+
|Adaptação do *Import* do Container do tipo Google |tag 5.2-b48 07jul|
+--------------------------------------------------+-----------------+
|Inclusão das novas regiões, são elas:             |tag 5.2-b64 18jul|
+--------------------------------------------------+-----------------+
|* Melbourne, Vitória, Oceania:                                      |
|       australia-southeast2                                         |
+--------------------------------------------------------------------+
|* Delhi, Região da Capital Nacional, Ásia:                          |
|       asia-south2                                                  |
+--------------------------------------------------------------------+
|Refinamento da seleção para associar a subrede ao |tag 5.3-b30 03ago| 
|*Import* do Container                             |                 |
+--------------------------------------------------+-----------------+
|Associação de zona ao criar VM                    |tag 5.3-b36 08ago|
+--------------------------------------------------+-----------------+
|Novos filtros de faturamento:                     |tag 5.2-b57 13jul|
+--------------------------------------------------+-----------------+
|* **Discount**:                                                     |
|                                                                    |
|O tipo de crédito com desconto é usado para valores recebidos       | 
|após um limite de gasto contratual a ser atingido.                  |
+--------------------------------------------------------------------+
|Nos relatórios do *Cloud Billing* disponíveis no console, este é    |
|listado como “Descontos com base em gastos (contratuais)".          | 
+--------------------------------------------------------------------+
|* **Free tier**:                                                    |
|Alguns serviços oferecem "uso gratuito de recursos até os limites   |
|especificados". Nesses serviços, os créditos são aplicados para     |
|implementar o uso de nível gratuito.                                |
+--------------------------------------------------------------------+
|* **Promotion**:                                                    |
|O tipo de crédito promocional inclui o teste gratuito do *Google    | 
|Cloud* e créditos de campanha de marketing ou outras concessões para| 
|usá-lo. Quando disponíveis, os créditos promocionais são            | 
|considerados uma forma de pagamento e são aplicados automaticamente |
|para reduzir a fatura total.                                        |
+--------------------------------------------------------------------+




* O botão para associar o disco à VM recebe nova interface gráfica [tag 5.2-b38 22jun];

* Aprimoramento no contrato padrão do usuário ao criar uma máquina virtual de banco de dados [tag 5.2-b46 05jul];

* Adição do detalhamento de *loadbalancers* de um *Scaling Group* [tag 5.2-b46 05jul];

* Adaptação do *Import* do Container do tipo Google [tag 5.2-b48 07jul];

* Inclusão das novas regiões, são elas [tag 5.2-b64 18jul]:


  * Melbourne, Vitória, Oceania: australia-southeast2.
  
  * Delhi, Região da Capital Nacional, Ásia: asia-south2.

* Refinamento da seleção para associar a subrede ao *Import* do Container [tag 5.3-b30 03ago];

* Associação de zona ao criar VM [tag 5.3-b36 08ago];

* Novos filtros de faturamento [tag 5.2-b57 13jul]:


  * **Discount**: o tipo de crédito com desconto é usado para valores recebidos após um limite de gasto contratual a ser atingido. Nos relatórios do *Cloud Billing* disponíveis no console, este é listado como “Descontos com base em gastos (contratuais)”.
  
  * **Free tier**: Alguns serviços oferecem "uso gratuito de recursos até os limites especificados". Nesses serviços, os créditos são aplicados para implementar o uso de nível gratuito.
  
  * **Promotion**: o tipo de crédito promocional inclui "Teste gratuito do Google Cloud e créditos de campanha de marketing ou outras concessões para usar o Google Cloud". Quando disponíveis, os créditos promocionais são considerados uma forma de pagamento e são aplicados automaticamente para reduzir a fatura total.


Huawei Cloud (Huawei)
---------------------

Em relação à interação com o provedor de serviço de nuvem pública Huawei nenhuma ocorrência de alteração, nova implementação ou funcionalidade.


IBM Cloud (IBM)
---------------

Em relação à interação com o provedor de serviço de nuvem pública IBM nenhum registro de correção, alteração, nova funcionalidade ou implementação.


VMware 6.5 ou superior (vCenter/vSphere)
----------------------------------------

No tocante à interação com o *hypervisor VCenter/vSphere*, relaciona-se a seguinte melhoria:


* A política de agendamento para *Scaling Group* permite ao usuário criar a política que define o momento de criar nova(s) máquina(s) [tag 5.3-b36 08ago].


VMWare vCloud (vCloud)
----------------------


Em relação à interação com o *hypervisor vCloud* nenhuma ocorrência de alteração, correção, nova implementação ou funcionalidade.

----


Aprimoramento da plataforma uCloud
==================================


A Ustore renova a plataforma uCloud em conformidade com a evolução contínua das inovações no setor de *cloud computing* - ambiente dinâmico que permite acesso remoto a *softwares*, armazenamento de arquivos e processamento de dados por meio da Internet. 


Logo, a prática da melhoria contínua adotada no aprimoramento da plataforma uCloud em *Account*, OPS e *Billing*, associada à produtividade, resulta na lista das melhorias globais a seguir:

1.

* Criação de *user* no *Account*:  Atalho para criar usuário direto no menu Administração, submenu *Account*. [tag 1.0-account68 04jul]

2.

* Listagem em ordem alfabética de container e VDC na tela de criação de um grupo de segurança: Ao listar os VDCs na criação de grupo de segurança, a exibição está em ordem alfabética. [tag5.2-b39 23jun]

3.

* Listagem em ordem alfabética de container e VDC na tela de criação de uma rede: A tela de criação de uma rede apresenta a lista em ordem alfabética de container e VDC. [tag5.2-b39 23jun]

4.

* Listagem em ordem alfabética por container e VDC na criação de IP Público: No momento de criar o IP Público a lista apresentada, do container e do VDC, está em ordem alfabética. [tag5.2-b39 23jun]

5.

* Reforço na segurança da interface do uCloud: Foram efetuadas melhorias na segurança no *Front-End* do uCloud. [tag 5.2-b43 30jun]

6.

* O idioma do usuário pode ser trocado a nível de conta, além do nível de usuário existente: Então uma conta pode ter um idioma e ser vista pelo idioma que o usuário determinar. [tag 1.0-account66 22jun]

7.

* Persistência da troca de idioma do usuário: A plataforma mantém o idioma escolhido no primeiro acesso. [tag 5.2-b61 14jul]

8.

* Persistência do idioma no envio de e-mails dentro do portal: A plataforma mantém o idioma escolhido no envio de e-mails. [tag 5.2-b73 21jul]

9.

* Adaptação da listagem dos perfis de permissionamento e visualização na interface gráfica: a lista dos perfis aparece por cima do modal, facilitando a visualização. [tag 5.2-b47 06jul]

10.

* Criação de *Tags* virtuais com a mesma chave, mas com valores diferentes: Esta melhoria permite a criação de uma ou mais *Tags* com chaves iguais e valores diferentes. [tag 5.2-b49 07jul]

11.

* Atualização do CORE.sql do uCloud: Agiliza de maneira significante a resposta do ambiente. [tag 5.2-b52 12jul]

12.

* Atualização das cotas em toda a plataforma uCloud: A unificação das cotas em todos os ambientes padroniza a visualização das cotas do usuário nas funcionalidades de contrato e grupo. [tag 5.2-b52 12jul]

13.

* No menu da funcionalidade de Configuração, o submenu Geral contempla a adição do botão (ON/OFF) na ativação automática e do uCloud v.2, este botão indica que a função está habilitada ou desabilitada. [tag 5.2-b55 13jul]

14.

* Atualização do formato de recuperação da senha. [tag 5.2-b60 14jul]

15.

* Aprimoramento na customização do *branding* a nível de contrato. [tag 5.3-b08 26jul]

16.

* No menu Tarefas, na lista de tarefas em operação a coluna “Ações” permite ao usuário cancelar ou pausar uma *Task* independente do status, contanto que a porcentagem esteja abaixo de 99%. [tag 5.2-b69 20jul]

17.

* Atualização na funcionalidade “*Checkbox*” associando todas as VMs no contrato e no grupo. [tag 5.3-b43 melhoria 10ago]

18.

* No Menu Administração, ao clicar no submenu Contratos e selecionar um determinado Contrato da lista, é permitido "Adicionar Administradores" seja usuário ou grupo de usuários. Para facilitar a busca, foi adicionada uma barra de pesquisa, que entrega como resultado o nome de um usuário ou um grupo. [tag 5.3-b54 17ago.]  

19.

* Criação de cota por quantidade de VM/Instância por contrato. [tag 5.3-b36 nova funcionalidade 08ago] 

20.

* Adaptação de *Workflow* para suportar o encadeamento de diversas tarefas (de forma sequencial e/ou paralela, sem número máximo) de *workflows* existentes no portal. [tag 5.3-b50 nova funcionalidade 15ago] 

21.

* Aprovação de *task* ao exceder cota: Quando um usuário excede a cota existente no contrato automaticamente o administrador percebe que o usuário precisa de mais cota. Assim, o administrador pode aprovar ou não essa solicitação. [tag 5.3-b53 nova funcionalidade 16ago]

22.

* Nova apresentação no Relatório Financeiro na interface de dados do *Billing*. [tag 1.0-account79 01ago]

23.

* Opção *CentOS7* para criação de *ResourceKey*: requisito da nuvem atendido com o acréscimo do *CentOS7* como Sistema Operacional para taguear USN. [tag 5.3-b09 nova funcionalidade 26jul]

24.

* Kubernetes para criar *ResourceKey*: acréscimo do Kubernetes como Sistema Operacional como requisito do Google para taguear máquinas Kubernetes. [tag 5.2-b45 fix 05jul]

25.

* O menu Perfil de *Tag* Virtual aprimora a experiência de uso ao permitir nomes semelhantes na criação do perfil de *tag* virtual e impedir o uso de caracteres especiais. [tag 5.2-b57 13jul]

26.

* Incremento do perfil de Tag Virtual ao incluir o campo *uCloudIdentifier* que será usado como referência. Está aplicado nas operações do container e dos bilhetadores. [tag 5.2-b65 18jul]  

27.

* O menu Catálogo de Serviços após a refatoração do ponto de transmissão e recepção de informação *endpoint* detalha o resultado somente quando o usuário solicita a busca. [tag 5.2-b58 13jul]

28.

* Associar o mesmo preço de *USN Tag* para vários contratos: foi eliminada a restrição de *tag* para apenas um contrato. [tag 5.2-b65 18jul]

29.

* O menu Tarefas recebe a atualização do registro de *taks* nas atividades ocorridas no *Billing* dentro do portal. [tag 5.3-b09 26jul] 

30.

* Adição de variáveis ao criar uma *tag* virtual. [tag 5.3-b49 15ago]

31.

* Relatório de monitoramento de consumo: Adição do Identificador Único Universal (UUID) do container, otimiza o fechamento da fatura do contrato que monitora o consumo. [tag 5.3-b18 28jul]

32.

* A tela de Resumo detalhado da fatura incrementa o carregamento de dados e torna a entrega mais rápida no resultado da requisição na sua interface. [tag 5.3-b22 29jul]

33.

* Melhoria na visualização do fechamento de faturas com usuários multicontratos: Um usuário vinculado a mais de um contrato, tem a opção de ver o fechamento da fatura com os gastos de cada contrato específico individualmente. [tag 5.3-b46 10ago]

34.

* *"Checkbox"* de selecionar todos os VDC de um contrato. [tag 1.0-account88 10ago]

35.

* *"Loader"* para carregamento atrasado do uCloud. [tag 5.3-b15 nova funcionalidade 28jul]

36.

* Campo de pesquisa para subredes dentro da tela de máquina virtual. [tag 5.2-b72 21jul]

37.

* Reativada a funcionalidade de *stop* de VM. [tag 5.2-b72 21jul]

38.

* Listagem de dados detalhados de *Billing*. [tag 5.3-b09 26jul]

39.

* Forma como o relatório consolidado apresenta os dados. [tag 5.3-b11 27jul]

40.

* Criação de persistência na validação de recursos que não estão no contrato para criação de máquina virtual e *Scaling Group*. [tag 5.2-b47 06jul]


----


Ações corretivas globais
========================



Este tópico lista as ações corretivas realizadas pela nossa equipe de desenvolvimento, identificadas em consequência dos *reports* gerados na experiência de uso e *quality assurance*. 

As ações corretivas de *fix* e *bugs* podem referir-se a: 


* Adequações às nuvens e;


* Na plataforma uCloud em *Account*, *OPS* e *Billing*.

----


Adequações às nuvens
--------------------



Amazon Web Services (AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~


Em relação à interação com o provedor de serviço de nuvem pública Amazon Web Services (AWS), pode-se listar uma ação corretiva:

1.

* Criação do Balanceador com o Grupo de Segurança selecionado. [tag 1.0-account65 fix 20ago]



Microsoft Azure (Azure)
~~~~~~~~~~~~~~~~~~~~~~~

Em relação à interação com o provedor de serviço de nuvem pública Microsoft AZURE, são listadas as seguintes correções:

2.

* Persistência ao adicionar um *loadbalancer* a uma máquina virtual da Azure. [tag 5.2-b51 fix 08jul]

3.

* Alteração no cálculo dos discos da Azure. [tag 5.3-b45 fix 10ago]

4.

*  Foi ocultado o botão de "Edit Subnet" que antes gerava inativação dos *inputs* no momento da criação de subredes. [tag 5.2-b72 fix 21jul]



Google Cloud Platform (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Em relação à interação com o provedor de serviço de nuvem pública Google Cloud Platform (GCP), pode-se listar as seguintes correções:

5.

* Chamada em *loop* da tela de *storage*. [tag5.2-b38 fix 22jun]

6.

* Criação de um *loadbalancer*, e a retificação na mensagem de erro. [tag 5.2-b46 fix 05jul]



Huawei Cloud (Huawei)
~~~~~~~~~~~~~~~~~~~~~

Em relação à interação com o provedor de serviço de nuvem pública Huawei Cloud, não houve nenhuma alteração, correção, nova implementação ou nova funcionalidade.



IBM Cloud (IBM)
~~~~~~~~~~~~~~~


Em relação à interação com o provedor de serviço de nuvem pública IBM Cloud, é listada a seguinte correção:

7.

* As listagens dos recursos são disponibilizadas por filtragem de regiões na hora da criação de redes. [tag 5.2-b64 bug 18jul]



VMware vCloud
~~~~~~~~~~~~~


Em relação à interação com o hypervisor de nuvem privada VMware 6.5 (ou superior), pode-se listar as seguintes correções:

8.

* VMware clonava uma VM de *Scaling Group*. [tag 5.2-b62 fix 14jul]

9.

* Gerenciamento de escalonamento baseado nas *policies* (Métricas) de escrita e leitura de disco. [tag 5.3-b14 fix 28jul]


----


Na Plataforma uCloud
--------------------



**OPS**

10.


* Filtro VDC no grupo. [tag 5.2-b65 fix 18jul] 

11.

* Filtro VDC na empresa. [tag 5.2-b65 fix 18jul]

12.

* Persistência da logo do portal no primeiro acesso. [tag5.2-b39 fix 23jun]

13.

* Tela de VDC em *loop*. [tag 5.2-b44 fix 05jul]

14.

* Persistência do dado no preço do custo total a partir do *amount* exibido em tela. [tag 5.2-b54 fix 13jul]

15.

* Travamento da tela de *Dashboard* do uCloud ao realizar *login*. [tag 5.3-b17 fix 28jul]

16.

* Adição de VM a um *Workflow*. [tag 5.3-b51 fix 16ago]

17.

* Operações de subrede. [tag 5.3-b54 fix 17ago]

18.

* Persistência das Novas traduções no *Dashboard*. [tag 5.2-b44 fix 05jul]

19.

* *Query* para VM. [tag 5.3-b39 fix 08ago]




**Billing**

20.

* *Pop-up VirtualTags*. [tag 5.2-b45 fix 05jul]

21.

* Dados duplicados no *pop-up* de detalhes da fatura do usuário. [tag 5.2-b45 fix 05jul]

22.

* Relatório CSV detalhado para preencher a coluna USN. [tag 5.2-b45 fix 05jul]

23.

* Não listar recursos marcados com USN. [tag 5.2-b45 fix 05jul]

24.

* *NullPointer* para obter a moeda no processo de cálculo da fatura. [tag 5.2-b65 fix 18jul]

25.

* Adição de coluna ao relatório financeiro do *Billing*. [tag 5.3-b02 fix 22jul]

26.

* *Nullpoint* no faturamento do relatório consolidado do *Billing*. [tag 5.3-b02 fix 22jul] 

27.

* Dados encontrados na geração de relatório detalhado. [tag 5.3-b06 fix 25jul]

28.

* Ação realizada para entregar valores no contrato. [tag 5.3-b06 fix 25jul]

29.

* Sumarização por Container do Relatório PDF. [tag 5.3-b23 fix 29jul]

30.

* Relatório PDF de faturas fechadas. [tag 5.3-b31 fix 03ago]

31.

* *Export* de CSV do relatório financeiro. [tag 5.3-b35 fix 05ago]

32.

* Cálculo USN. [tag 5.2-b58 fix 13jul]

33.

* Chamada de tela de minha fatura por grupo para carregamento de dados. [tag 5.3-b25 fix 01ago]

34.

* Eliminado o problema no Relatório detalhado vindo vazio. [tag 5.3-b46 fix 10ago]



----

.

Neste release é evocado o princípio da norma ISO 9001, elaborada pela Organização Internacional de Normalização (no Brasil conhecida como ABNT NBR ISO 9001). A qual objetiva estabelecer normas consistentes que aumentam a qualidade nos processos aplicados e redundam na melhoria contínua e ajustes nas funcionalidades, em busca da gestão da qualidade e excelência empresarial. 

O apresentado acima refere-se ao princípio da gestão da qualidade citada na norma ISO 9001.

Em resumo, o documento apresenta:

* Sete (7) novas implementações;
* Treze (13) melhorias realizadas na categoria *Cloud* pela demanda na adequação às mudanças nesses provedores;
* Quarenta (40) aprimoramentos globais da plataforma uCloud e;
* Trinta  e quatro (34) ações corretivas, sendo:
    *  Nove (09) relacionadas às nuvens;
    *  Dez (10) relativas a uCloudOPS e;
    *  Quinze (15) pertencentes ao *Billing*. 

Portanto, conclui-se o release trimestral, correspondente aos lançamentos ocorridos nos meses de junho, julho e agosto do corrente ano, na plataforma uCloud, inovações geradas na área de desenvolvimento da Ustore.

