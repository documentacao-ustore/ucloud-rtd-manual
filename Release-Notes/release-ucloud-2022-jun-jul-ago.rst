
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


+--------------------------------------------------+-----------------+
|FEATURE                                           |VERSÃO           |
+==================================================+=================+
|A partir desta adequação pode ser realizado o     |tag 5.2-b45 05jul|
|*Import* do Container unicamente para faturamento |                 |
+--------------------------------------------------+-----------------+



Microsoft Azure (Azure)
-----------------------


Relativo à interação com o provedor de serviço de nuvem pública Microsoft AZURE, pode-se listar três melhorias:


+--------------------------------------------------+-----------------+
|FEATURE                                           |VERSÃO           |
+==================================================+=================+
|Alteração da interface gráfica do botão de criação|tag 5.3-b12 27jul|
|do *Scaling Group*                                |                 |
+--------------------------------------------------+-----------------+
|Para a melhor experiência do usuário, opta-se por |tag 5.2-b72 21jul|
|ocultar o campo de Grupo de Segurança dos VDCs    |                 |
+--------------------------------------------------+-----------------+
|Realizar o *Import* do Container somente para     |tag 5.2-b57 13jul|
|o faturamento                                     |                 |
+--------------------------------------------------+-----------------+



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
|Adaptação *Import* do Container do tipo *Google*  |tag 5.2-b48 07jul|
+--------------------------------------------------+-----------------+
|Inclusão das novas regiões, são elas:             |tag 5.2-b64 18jul|
+--------------------------------------------------+-----------------+
|* Melbourne, Vitória, Oceania:                                      |
|       australia-southeast2                                         |
+--------------------------------------------------------------------+
|* Delhi, Região da Capital Nacional, Ásia:                          |
|       asia-south2                                                  |
+--------------------------------------------------+-----------------+
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




Huawei Cloud (Huawei)
---------------------

Em relação à interação com o provedor de serviço de nuvem pública Huawei nenhuma ocorrência de alteração, nova implementação ou funcionalidade.


IBM Cloud (IBM)
---------------

Em relação à interação com o provedor de serviço de nuvem pública IBM nenhum registro de correção, alteração, nova funcionalidade ou implementação.


VMware 6.5 ou superior (vCenter/vSphere)
----------------------------------------

No tocante à interação com o *hypervisor VCenter/vSphere*, relaciona-se a seguinte melhoria:


+--------------------------------------------------+-----------------+
|FEATURE                                           |VERSÃO           |
+==================================================+=================+
|A política de agendamento para *Scaling Group*    |tag 5.3-b36 08ago|
|permite ao usuário criar a política que define    |                 |
|o momento de criar nova(s) máquina(s)             |                 |
+--------------------------------------------------+-----------------+


VMWare vCloud (vCloud)
----------------------


Em relação à interação com o *hypervisor vCloud* nenhuma ocorrência de alteração, correção, nova implementação ou funcionalidade.

----


Aprimoramento da plataforma uCloud
==================================


A Ustore renova a plataforma uCloud em conformidade com a evolução contínua das inovações no setor de *cloud computing* - ambiente dinâmico que permite acesso remoto a *softwares*, armazenamento de arquivos e processamento de dados por meio da Internet. 


Logo, a prática da melhoria contínua adotada no aprimoramento da plataforma uCloud em *Account*, OPS e *Billing*, associada à produtividade, resulta na lista das melhorias globais a seguir:


+-----------------------------------------------------+-----------------+
|FEATURE                                              |VERSÃO           |
+=====================================================+=================+
|Criação de *user* no *Account*:  Atalho para criar   |tag 1.0-account68|
|usuário direto no menu Administração, submenu Account|            04jul|
+-----------------------------------------------------+-----------------+
|Listagem em ordem alfabética de container e VDC na   |tag 5.2-b39 23jun|
|tela de criação de um grupo de segurança: Ao listar  |                 |
|os VDCs na criação deste grupo, exibição em ordem    |                 |
+-----------------------------------------------------+-----------------+
|Listagem em ordem alfabética de container e VDC na   |tag 5.2-b39 23jun|
|tela de criação de uma rede: A tela de criação de uma|                 |
|rede apresenta a lista em ordem de *Container* e *VDC|                 |
+-----------------------------------------------------+-----------------+
|Listagem em ordem alfabética por container e VDC na  |tag 5.2-b39 23jun|
|criação de IP Público: No momento de criá-lo, a lista|                 |
|do container e VDC é apresentada em ordem alfabética |                 |
+-----------------------------------------------------+-----------------+
|Reforço na segurança da interface do uCloud:         |tag 5.2-b43 30jun|
|Foram efetuadas melhorias na segurança no *Front-End*|                 |
+-----------------------------------------------------+-----------------+
|O idioma do usuário pode ser trocado a nível de conta|tag 1.0-account66|
|além do nível de usuário existente:                  |            22jun|
|Então uma conta pode ter um idioma e ser vista pelo  |                 |
|idioma que o usuário determinar                      |                 |
+-----------------------------------------------------+-----------------+
|Persistência da troca de idioma do usuário:          |tag 5.2-b61 14jul|
|A plataforma mantém o idioma escolhido no primeiro   |                 |
|acesso                                               |                 |
+-----------------------------------------------------+-----------------+
|Persistência do idioma no envio de e-mails dentro do |tag 5.2-b73 21jul|
|portal: A plataforma mantém o idioma escolhido ao    |                 |
|enviar e-mails                                       |                 |
+-----------------------------------------------------+-----------------+
|Adaptação da listagem dos perfis de permissionamento |tag 5.2-b47 06jul|
|e visualização na interface gráfica: A lista dos     |                 |
|perfis aparece por cima do modal, otimiza visualizar |                 |
+-----------------------------------------------------+-----------------+
|Criação de *Tags* virtuais com a mesma chave e valor |tag 5.2-b49 07jul|
|diferentes: Esta melhoria permite a criação de uma ou|                 |
|mais *Tags* com chaves iguais e valores diferentes   |                 |
+-----------------------------------------------------+-----------------+
|Atualização do CORE.sql do uCloud: Agiliza de maneira|tag 5.2-b52 12jul|
|significante a resposta do ambiente                  |                 |
+-----------------------------------------------------+-----------------+
|Atualização das cotas em toda a plataforma uCloud:   |tag 5.2-b52 12jul|
|Sua unificação, em todos os ambientes, padroniza a   |                 |
|visualização das cotas do usuário nas funcionalidades|                 |
|de contrato e grupo                                  |                 |
+-----------------------------------------------------+-----------------+
|No menu da funcionalidade de Configuração, o submenu |tag 5.2-b55 13jul|
|Geral contempla a adição do botão (ON/OFF)na ativação|                 |
|automática e do uCloud v.2, este botão indica que a  |                 |
|função está habilitada ou desabilitada               |                 |
+-----------------------------------------------------+-----------------+
|Atualização do formato de recuperação da senha       |tag 5.2-b60 14jul|
+-----------------------------------------------------+-----------------+
|Aprimoramento na customização do *branding* a nível  |tag 5.3-b08 26jul|
|de contrato                                          |                 |
+-----------------------------------------------------+-----------------+
|No menu Tarefas, em sua lista de tarefas em operação,|tag 5.2-b69 20jul|
|a coluna “Ações” permite ao usuário cancelar ou      |                 |
|pausar uma *Task* independente do status, contanto   |                 |
|que a porcentagem esteja abaixo de 99%               |                 |
+-----------------------------------------------------+-----------------+
|Atualização na funcionalidade “*Checkbox*” associando|tag 5.3-b43 10ago|
|todas as VMs no contrato e no grupo                  |                 |
|[melhoria]                                           |                 |
+-----------------------------------------------------+-----------------+
|No Menu Administração ao clicar no submenu Contratos |tag 5.3-b54 17ago|
|e selecionar um determinado Contrato da lista, é     |                 |
|permitido "Adicionar Administradores" seja usuário ou|                 |
|grupo de usuários.                                   |                 | 
|Para facilitar a busca, foi adicionada uma barra de  |                 |
|pesquisa, que entrega como resultado o nome de um    |                 |
|usuário ou um grupo                                  |                 |
+-----------------------------------------------------+-----------------+
|Criação de cota por quantidade de VM/Instância por   |tag 5.3-b36 08ago|
|contrato                                             |                 |
|[nova funcionalidade]                                |                 |
+-----------------------------------------------------+-----------------+
|Adaptação de *Workflow* para suportar o encadeamento |tag 5.3-b50 15ago|
|de diversas tarefas de forma sequencial e/ou paralela|                 |
|sem número máximo de *workflows* existentes no portal|                 |
|[nova funcionalidade]                                |                 |
+-----------------------------------------------------+-----------------+
|Aprovação de *task* ao exceder cota: Quando um       |tag 5.3-b53 16ago|
|usuário excede a cota existente no contrato,         |                 |
|automaticamente o administrador percebe que o usuário|                 |
|precisa de mais cota. Assim, o administrador pode    |                 |
|aprovar ou não essa solicitação                      |                 |
|[nova funcionalidade]                                |                 |
+-----------------------------------------------------+-----------------+
|Nova apresentação no Relatório Financeiro na         |tag 1.0-account79| 
|interface de dados do *Billing*                      |            01ago|
+-----------------------------------------------------+-----------------+
|Opção *CentOS7* para criação de *ResourceKey*:       |tag 5.3-b09 26jul|                  
|Requisito da nuvem atendido com o acréscimo do       |                 |
|*CentOS7* como Sistema Operacional para taguear USN  |                 |
|[nova funcionalidade]                                |                 |
+-----------------------------------------------------+-----------------+
|Kubernetes para criar *ResourceKey*: Acréscimo do    |tag 5.2-b45 05jul|             
|Kubernetes como Sistema Operacional como requisito do|                 |
|Google para taguear máquinas Kubernetes              |                 |
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+
|O menu Perfil de *Tag* Virtual aprimora a experiência|tag 5.2-b57 13jul| 
|de uso ao permitir nomes semelhantes na criação do   |                 |
|perfil de tag virtual e impedir o uso de caracteres  |                 |
|especiais                                            |                 |
+-----------------------------------------------------+-----------------+
|Incremento do perfil de *Tag* Virtual ao incluir o   |tag 5.2-b65 18jul|
|campo *uCloudIdentifier* que é usado como referência.|                 |
|Está aplicado nas operações do container e dos       |                 |
|bilhetadores                                         |                 |
+-----------------------------------------------------+-----------------+
|O menu Catálogo de Serviços após a refatoração do    |tag 5.2-b58 13jul|
|ponto de transmissão e recepção de informação        |                 | 
|*endpoint* detalha o resultado somente quando o      |                 | 
|usuário solicita a busca                             |                 |
+-----------------------------------------------------+-----------------+
|Associar o mesmo preço de *USN Tag* para vários      |tag 5.2-b65 18jul|
|contratos: Foi eliminada a restrição de *tag* para   |                 |
|apenas um contrato                                   |                 |
+-----------------------------------------------------+-----------------+
|O menu Tarefas recebe a atualização do registro de   |tag 5.3-b09 26jul|
|*taks* nas atividades ocorridas no *Billing* dentro  |                 |
|do portal                                            |                 |
+-----------------------------------------------------+-----------------+
|Adição de variáveis ao criar uma *Tag* virtual       |tag 5.3-b49 15ago|
+-----------------------------------------------------+-----------------+
|Relatório de monitoramento de consumo: Adição do     |tag 5.3-b18 28jul|
|Identificador Único Universal (UUID) do container,   |                 |
|otimiza o fechamento da fatura do contrato que       |                 |
|monitora o consumo                                   |                 |
+-----------------------------------------------------+-----------------+
|A tela de Resumo detalhado da fatura incrementa o    |tag 5.3-b22 29jul|
|carregamento de dados e torna a entrega mais rápida  |                 |
|no resultado da requisição na sua interface          |                 |
+-----------------------------------------------------+-----------------+
|Melhoria na visualização do fechamento de faturas com|tag 5.3-b46 10ago|
|usuários multicontratos: Um usuário vinculado a mais |                 |
|de um contrato, tem a opção de ver o fechamento da   |                 |
|fatura com os gastos de cada contrato específico     |                 |
|individualmente                                      |                 |
+-----------------------------------------------------+-----------------+
|*Checkbox* de selecionar todos os VDC de um contrato |tag 1.0-account88|
|                                                     |            10ago|
+-----------------------------------------------------+-----------------+
|*Loader* para carregamento atrasado do uCloud        |tag 5.3-b15 28jul|
|[nova funcionalidade]                                |                 |
+-----------------------------------------------------+-----------------+
|Campo de pesquisa para subredes dentro da tela de    |tag 5.2-b72 21jul|
|máquina virtual                                      |                 |
+-----------------------------------------------------+-----------------+
|Reativada a funcionalidade de *stop* de VM           |tag 5.2-b72 21jul|
+-----------------------------------------------------+-----------------+
|Listagem de dados detalhados de *Billing*            |tag 5.3-b09 26jul|
+-----------------------------------------------------+-----------------+
|Forma como o relatório consolidado apresenta os dados|tag 5.3-b11 27jul|
+-----------------------------------------------------+-----------------+
|Criação de persistência na validação de recursos que |tag 5.2-b47 06jul|
|não estão no contrato para criação de máquina virtual|                 |
|e *Scaling Group*                                    |                 |
+-----------------------------------------------------+-----------------+




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


+-----------------------------------------------------+-----------------+
|FEATURE                                              |VERSÃO           |
+=====================================================+=================+
|Criação do Balanceador com o Grupo de Segurança      |tag 1.0-account65|
|selecionado                                          |            20ago|
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+

1.

* Criação do Balanceador com o Grupo de Segurança selecionado. [tag 1.0-account65 fix 20ago]



Microsoft Azure (Azure)
~~~~~~~~~~~~~~~~~~~~~~~

Em relação à interação com o provedor de serviço de nuvem pública Microsoft AZURE, são listadas as seguintes correções:


+-----------------------------------------------------+-----------------+
|FEATURE                                              |VERSÃO           |
+=====================================================+=================+
|Persistência ao adicionar um *loadbalancer* a uma    |tag 5.2-b51 08jul|
|máquina virtual da Azure                             |                 |
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+
|Alteração no cálculo dos discos da Azure             |tag 5.3-b45 10ago|
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+
|Foi ocultado o botão de "Edit Subnet" que antes      |tag 5.2-b72 21jul| 
|gerava inativação dos *inputs* no momento da criação |                 |
|de subredes                                          |                 |
|[fix]                                                |                 |
+-----------------------------------------------------+-----------------+


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

