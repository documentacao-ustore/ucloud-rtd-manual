uCloud - Notas de Lançamento Junho|Julho|Agosto - 2022
======================================================

.. figure:: /figuras/ucloud.png
   :alt: Logo uCLoud
   :scale: 50 %
   :align: center
   
----

Plataforma uCloud versão: *Update tags 5.3-b56 e 1.0-account88*

Apresentação
============

A Ustore renova a plataforma uCloud em conformidade com a evolução contínua das inovações no setor de *cloud computing*, um ambiente dinâmico que permite acesso remoto a *softwares*, armazenamento de arquivos e processamento de dados por meio da Internet. 

Neste lançamento é evocado o princípio da norma ISO 9001, elaborada pela Organização Internacional de Normalização (no Brasil conhecida como ABNT NBR ISO 9001). A qual objetiva estabelecer normas consistentes que aumentam a qualidade nos processos aplicados e redundam na melhoria contínua e ajustes nas funcionalidades, em busca da gestão da qualidade e excelência empresarial. 

As melhorias apresentadas a seguir referem-se ao princípio da gestão da qualidade citada na norma ISO 9001, realizada durante os meses de junho, julho e agosto do corrente.

Notícias 
========

Esta nota de lançamento divulga as trinta e três melhorias globais realizadas em alguns menus de funcionalidades do portal, catorze adequações elaboradas às mudanças das nuvens e as sete novas implementações. Estão categorizadas em:

* Nuvens públicas e privadas;

* Aprimoramento da plataforma uCloud em Account, uCloudOPS e *Billing*;

* Novas implementações.

Nuvens Públicas e Privadas
==========================

Amazon Web Services (AWS)
-------------------------

Em relação à interação com o provedor de serviço de nuvem pública Amazon Web Services (AWS):

* A partir desta nota pode ser realizado o Import do Container unicamente para o faturamento.

Microsoft Azure (Azure)
-----------------------

Relativo à interação com o provedor de serviço de nuvem pública Microsoft AZURE, podemos listar três melhorias:

* Alteração da interface gráfica do botão de criação do Scaling Group;

* Para a melhor experiência do usuário, opta-se por ocultar o campo de Grupo de Segurança dos VDCs;

* Realizar o Import do Container somente para o faturamento.

Google Cloud Platform (GCP)
---------------------------

No que concerne à interação com o provedor de serviço de nuvem pública Google Cloud Platform (GCP), houveram oito melhorias listadas na sequência:

* O botão para associar o disco à VM recebe nova interface gráfica;

* Aprimoramento no contrato padrão do usuário ao criar uma DBVM;

* Adição do detalhamento de *loadbalancers* de um Scaling Group;

* Adaptação do Import do Container do tipo Google;

* Inclusão das novas regiões, são elas:

  * Melbourne, Vitória, Oceania: australia-southeast2.
  
  * Delhi, Região da Capital Nacional, Ásia: asia-south2.

* Refinamento da seleção para associar a subrede ao Import do Container.

* Associação de zona ao criar VM.

* Novos filtros de faturamento:

  * **Discount**: o tipo de crédito com desconto é usado para valores recebidos após um limite de gasto contratual a ser atingido. Nos relatórios do Cloud Billing disponíveis no console, este é listado como “Descontos com base em gastos (contratuais)”.
  
  * **Free tier**: Alguns serviços oferecem "uso gratuito de recursos até os limites especificados". Nesses serviços, os créditos são aplicados para implementar o uso de nível gratuito.
  
  * **Promotion**: o tipo de crédito promocional inclui "Teste gratuito do Google Cloud e créditos de campanha de marketing ou outras concessões para usar o Google Cloud". Quando disponíveis, os créditos promocionais são considerados uma forma de pagamento e são aplicados automaticamente para reduzir a fatura total.

IBM Cloud
---------

No que se refere à interação com o provedor de serviço de nuvem pública IBM Cloud, é listada a seguinte melhoria:

* As listagens dos recursos são disponibilizadas por filtragem de regiões na hora da criação de redes.

VMware 6.5 ou superior (vCenter/vSphere)
----------------------------------------

No tocante à interação com o hypervisor VMware 6.5 ou superior, relaciona-se a seguinte melhoria:

* A política de agendamento para Scaling Group permite ao usuário criar a política que define o momento de criar nova(s) máquina(s).

Aprimoramento da plataforma uCloud em Account, uCloudOPS e *Billing*
====================================================================

Na Ustore a prática da melhoria contínua adotada no aprimoramento da plataforma uCloud, associada à produtividade, resulta na lista a seguir:

* Criação de user no Account:  Atalho para criar usuário direto no menu Administração, submenu Account.

* Listagem em ordem alfabética de container e VDC na tela de criação de um grupo de segurança: Ao listar os VDCs na criação de grupo de segurança, a exibição está em ordem alfabética.

* Listagem em ordem alfabética de container e VDC na tela de criação de uma rede: A tela de criação de uma rede apresenta a lista em ordem alfabética de container e VDC.

* Listagem em ordem alfabética por container e VDC na criação de IP Público: No momento de criar o IP Público a lista apresentada, do container e do VDC, está em ordem alfabética.

* Reforço na segurança da interface do uCloud: Foram efetuadas melhorias na segurança no *Front-End* do uCloud.

* O idioma do usuário pode ser trocado a nível de conta, além do nível de usuário existente: Então uma conta pode ter um idioma e ser vista pelo idioma que o usuário determinar.

* Persistência da troca de idioma do usuário: A plataforma mantém o idioma escolhido no primeiro acesso. 

* Persistência do idioma no envio de e-mails dentro do portal: A plataforma mantém o idioma escolhido no envio de e-mails.

* Adaptação da listagem dos perfis de permissionamento e visualização na interface gráfica: a lista dos perfis aparece por cima do modal, facilitando a visualização.

* Criação de *Tags* virtuais com a mesma chave, mas com valores diferentes: Esta melhoria permite a criação de uma ou mais *Tags* com chaves iguais e valores diferentes.

* Atualização do CORE.sql do uCloud: Agiliza de maneira significante a resposta do ambiente.

* Atualização das cotas em toda a plataforma uCloud: A unificação das cotas em todos os ambientes padroniza a visualização das cotas do usuário nas funcionalidades de contrato e grupo. 

* No menu da funcionalidade de Configuração Geral contempla a adição do botão (ON/OFF) na ativação automática e do uCloud v.2, este botão indica que a função está habilitada ou desabilitada. 

* Atualização do formato de recuperação da senha.

* Aprimoramento na customização do *branding* no menu de funcionalidades do *Billing* para a versão mobile, com o objetivo de garantir a melhor visualização nas opções modo *light* e *dark*.

* No menu Tarefas, na lista de tarefas em operação a coluna “Ações” permite ao usuário cancelar ou pausar uma *Task* independente do status, contanto que a porcentagem esteja abaixo de 99%. 

* Atualização na funcionalidade “*Checkbox*” associando todas as VMs no contrato e no grupo.

* No Menu Administração ao clicar em Contratos e selecionar um determinado Contrato da lista, é permitido "Adicionar Administradores" seja usuário ou grupo de usuários. Para facilitar a busca, foi adicionada uma barra de pesquisa, que entrega como resultado o nome de um usuário ou um grupo.

* Criação de cota por quantidade de VM/Instância por contrato. 

* Adaptação de *Workflow* para suportar o encadeamento de diversas tarefas (de forma sequencial e/ou paralela, sem número máximo) de *workflows* existentes no portal. 

* Aprovação de *task* ao exceder quota: Quando um usuário excede a cota existente no contrato automaticamente o administrador percebe que o usuário precisa de mais cota. Assim, o administrador pode aprovar ou não essa solicitação.

* Nova apresentação no Relatório Financeiro na interface de dados do *Billing*.

* Opção *CentOS7* para criação de *ResourceKey*: requisito da nuvem atendido com o acréscimo do *CentOS7* como Sistema Operacional para taguear USN.

* Kubernetes para criar *ResourceKey*: acréscimo do Kubernetes como Sistema Operacional como requisito do Google para taguear máquinas Kubernetes.

* O menu Perfil de Tag Virtual aprimora a experiência de uso ao permitir nomes semelhantes na criação do perfil de tag virtual e impedir o uso de caracteres especiais.

* Incremento do perfil de Tag Virtual ao incluir o campo *uCloudIdentifier* que será usado como referência. Está aplicado nas operações do container e dos bilhetadores.  

* O menu Catálogo de Serviços após a refatoração do ponto de transmissão e recepção de informação ‘*endpoint*’ detalha o resultado somente quando o usuário solicita a busca.

* Associar o mesmo preço de *USN Tag* para vários contratos: foi eliminada a restrição de *tag* para apenas um contrato.

* O menu Tarefas recebe a atualização do registro de *taks* nas atividades ocorridas no *Billing* dentro do portal. 

* Adição de variáveis ao criar uma tag virtual.

* Melhoria no Relatório de monitoramento de consumo: Adição do Identificador Único Universal - UUID do container, otimiza o fechamento da fatura do contrato que monitora o consumo.

* A tela de Resumo detalhado da fatura incrementa o carregamento de dados e torna a entrega mais rápida no resultado da requisição na sua interface.

* Melhoria na visualização do fechamento de faturas com usuários multicontratos: Um usuário vinculado a mais de um contrato, tem a opção de ver o fechamento da fatura com os gastos de cada contrato específico individualmente.

Novas Implementações
====================

Neste relato a Ustore divulga as sete inovações ocorridas na plataforma uCloud, a seguir descritas de forma resumida:

1. **Budget**: Corresponde a um relatório baseado em consumo que tem como objetivo definir o orçamento total referente a um determinado período, seja mensal, trimestral, semestral ou anual. Este relatório possibilita monitorar o uso do Budget.

2. **Customização do branding a nível de Contrato**: A branding do portal Multicloud é permitida através da personalização definida por contrato. O cliente usuário tem as características da sua marca (Empresa) representada no portal Multicloud como as cores, a logomarca, entre outras.

3. **Dimensão**: Para evitar recursos iguais sendo tagueados de formas diferentes, a dimensão foi criada para agrupar *tags* distintas a recursos do mesmo contexto. Para isso, foram criadas operações lógicas e um filtro, com o intuito de identificar no *Billing* quais recursos pertencem a uma determinada dimensão.

4. **Import e Export de ofertas de serviço em (XML + YAML)**: Nessa nova funcionalidade é possível importar e exportar uma mesma oferta de uma nuvem qualquer contanto que esteja vinculada ao Portal uCloud. Antes era possível importar e exportar arquivos em formato JSON, então foram adicionadas as opções de importar e exportar os arquivos também em formato XML e YAML.

5. **Import de credenciais do Google no Secret Manager da AWS**: Secret Manager é um repositório onde são gravadas as informações que somente o usuário tem acesso. Para importar os dados credenciais da Google deste usuário, a ação deve ser feita através do uCloud para que estes sejam transferidos do repositório escondido da AWS.

6. **Permissões a Nível de Conta**: Esta nova funcionalidade otimiza o processo de permissão de um usuário. Nesta modalidade de permissão a nível de conta, o usuário pode realizar as ações a partir do perfil de permissão criado para ele, seja básico ou avançado. Este usuário tem o poder de administrar diversos contratos vinculados a uma conta, de acordo com as permissões que lhe foram concedidas.

7. **Relatório de Monitoramento de Consumo V1**: Nova funcionalidade do uCloud que trata do detalhamento completo dos gastos, divididos por Nuvens, Contratos e Recursos. São gerados diferentes tipos de relatórios, para cada tipo de divisão (Nuvem/Contrato/Recurso), separando um por vez e organizando-os do maior para o menor consumo. Além de comparar com os gastos dos meses anteriores, proporcionando ao cliente informações necessárias para que se possa avaliar se houve queda ou aumento dos gastos.

Em resumo, o documento apresenta as catorze (14) melhorias realizadas na categoria nuvens públicas e privadas pela demanda na adequação às mudanças nesses provedores. Os trinta e três (33) aprimoramentos globais da plataforma uCloud. Além das sete (7) novas implementações. Assim, conclui-se o documento com as notas de lançamento deste trimestre correspondente aos meses de junho, julho e agosto do corrente ano.