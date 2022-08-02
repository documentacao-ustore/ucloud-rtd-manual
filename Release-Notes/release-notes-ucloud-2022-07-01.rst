uCloud - Notas Maio - 2022
===========================

.. figure:: /figuras/ucloud_logo_peq.png
   :alt: Logo uCLoud
   :scale: 50 %
   :align: center

----

Plataforma uCloud versão: `Update tag 5.2-b35`


Apresentação
============

Em geral, o profissional de infraestrutura de TI utiliza diversos consoles para provisionar recursos computacionais, seja dentro da organização (datacenter privado) ou em algum provedor de nuvem. A computação em nuvem é uma evolução dos serviços e produtos de tecnologia da informação sob demanda, chamada por Brantner et al., 2008 de *Utility Computing*, a qual objetiva fornecer componentes básicos como: armazenamento, processamento e largura de banda de uma rede através de provedores especializados com um custo baixo por unidade utilizada. Na contemporaneidade, manter-se atualizado e preparado, em todas as «consoles» é um desafio para este profissional.

Na tentativa de aumentar a produtividade e reduzir o grau de dependência destes consoles o mercado desenvolveu o conceito de Infraestrutura como Código (IaaC - Infrastructure as a Code). Este conceito endereça somente o momento do provisionamento inicial (mesmo com o uso de scripts para instalação de padrões e softwares), podem existir demandas em que o profissional de TI deverá conectar-se à console do ambiente, para executar alguma intervenção na infraestrutura que não seja possível mediante o conceito de IaaC. Estar conectado e ficar alternando entre os diversos consoles de nuvem, demanda uma grande especialização e conhecimento do profissional de TI.

As plataformas de CSB (*Cloud Service Broker*) foram desenvolvidas para ocupar esse nicho e concentrar o inventário dos recursos computacionais de nuvens públicas e privadas em uma única interface e que transfere ao usuário o controle e a operação destes recursos multi-nuvem.

Como mencionado, o próprio mercado desenvolveu as metodologias de provisionamento de recursos computacionais através de scripts automatizados (também chamados de *playbooks*). Dentre estes formatos existem alguns que o mercado mundial adotou mais largamente, pode-se citar o Ansible, Terraform e Puppet.

O mercado também criou a demanda de programar a execução de uma sequência de diversos *scripts* dentro de um fluxo controlado e encadeado, de forma que um erro em um destes *scripts* pode interromper todo o fluxo para evitar o provisionamento de uma infraestrutura computacional sem a devida qualidade.

Atenta à evolução constante do mercado brasileiro e às demandas dos nossos usuários, a Ustore apresenta as novas implementações, as correções, as integrações, as atualizações no menu de funcionalidades e sua descrição detalhada. 

Além da ampliação do conceito existente, este release notes detalha o update ocorrido na plataforma uCloud, constante na *(tag.5.2-b35)* atendendo às diversas demandas mercadológicas dos nossos clientes, capazes de transformar a forma de gerenciar nuvens públicas e privadas com a plataforma uCloud.


Novas implementações
====================

As novidades apresentadas a seguir foram categorizadas em:

* As ações corretivas para adequação às mudanças ocorridas nos provedores de nuvens;
* As integrações realizadas no portal;
* Atualizações globais em alguns menus de funcionalidades do  portal.

Além das inovações mais robustas, elencadas em três temas. Estas novas implementações serão descritas, em detalhe, no transcorrer deste documento.

#. Account 
#. TAGs Virtuais
#. Oracle Cloud Infrastructure


Ações Corretivas
================

Neste release notes estão listadas todas as ações corretivas implementadas, motivadas devido certas situações reportadas à nossa equipe de desenvolvimento.


Amazon Web Services (AWS)
-------------------------

Em relação à interação com o provedor de serviço de nuvem pública AWS, não houve nenhuma alteração, correção, nova implementação ou nova funcionalidade.


Microsoft Azure (Azure)
-----------------------

Em relação à interação com o provedor de serviço de nuvem pública Microsoft AZURE, podemos listar as seguintes alterações:

#. Adaptação do Scaling Group para se adequar a atualização no modelo de resposta enviado pela nuvem.  Após esta implementação, ao criar um Scaling Group o processo cria automaticamente um Grupo de Instâncias, a serem gerenciadas por este Scaling Group.
#. Ajuste ao modelo de tratamento da deleção de discos associados a Máquinas Virtuais. Essa melhoria foi necessária por haver mudança na maneira como a deleção é feita na nuvem. Adaptação no PMC para acompanhar esta melhoria.


Google Cloud Plataform (GCP)
----------------------------

Em relação à interação com o provedor de serviço de nuvem pública Google Cloud Platform (GCP), podemos listar as seguintes alterações:

* Nova execução no funcionamento dos Listeners e Membros de um Balanceador.
* Adição do suporte ao criar o Balanceador utilizando o protocolo HTTP.
* Aplicação de regras de UDP (*User Datagram Protocol*) para Grupos de Segurança.
* Inclusão das novas regiões, são elas:

  * Columbus, Ohio, América do Norte: us-east-5
  * Dallas, Texas, América do Norte: us-south1
  * Madri, Espanha, Europa: europe-southwest1
  * Milão, Itália, Europa: europe-west8
  * Paris, França, Europa: europe-west-9

Huawei Cloud (Huawei)
---------------------

Em relação à interação com o provedor de serviço de nuvem pública Huawei Cloud, não houve nenhuma alteração, correção, nova implementação ou nova funcionalidade.

IBM Cloud
---------
Em relação à interação com o provedor de serviço de nuvem pública IBM Cloud, podemos listar a seguinte alteração:

#. Implementação da regra de negócio para desabilitar a edição da única NIC *(Network Interface Card)* da Máquina Virtual.

VMware 6.5 ou superior (vCenter/vSphere)
----------------------------------------

Em relação à interação com o hypervisor de nuvem privada VMware 6.5 (ou superior), podemos listar as seguintes alterações:

#. Atualização na forma de criar sub-rede para se adequar a nova versão do uSDN.
#. Comportamento anômalo corrigido, várias conexões abriam ao mesmo tempo.

VMware vCloud
-------------

Em relação à interação com o hypervisor de nuvem privada VMware 6.5 (ou superior), podemos listar as seguintes alterações:

- Correção da importação de container.
- Atualização da API para a versão 35.0.

Integrações
===========
- Houve uma implementação e melhoria da comunicação com o agente de monitoramento (Mangue/uCloud).

Atualizações
============

Abaixo relacionamos a lista de atualizações que foram implementadas na Plataforma uCloud:

#. Ampliação da cobertura de traduções dos elementos ou itens do portal, tanto para a língua espanhola como a língua inglesa.
#. Atualização da tabela de preço dos flavors.
#. Revisão da comunicação nas mensagens de exceção do portal, foco na interação do usuário com o conteúdo e  experiência de uso.

Menu Virtual Datacenter (VDC)
-----------------------------

#. Redução do tempo de carregamento dentro da tela de edição do VDC de um container.

Menu Perfis de Visualização
---------------------------

#. Adição dos módulos uLog e uMonitor como opção de seleção em Perfis de Visualização.

Descritivo das Novas Implementações
===================================

Abaixo descreveremos as características técnicas e operacionais de três das novas implementações que foram aplicadas para esta nova versão/release da Plataforma uCloud.
Neste capítulo estão elencadas as novas implementações e serão esclarecidas no transcorrer deste documento.

#. Account 
#. TAGs Virtuais
#. Oracle Cloud Infrastructure (OCI) - *apenas as funcionalidades de operação*.

Descrição de Account
====================

A Plataforma uCloud pode ser implantada de duas formas diferentes:

A. Instalação dedicada *(on-premises)*

Para o cenário da instalação dedicada *(on-premises)* a funcionalidade de Account pode não ser aplicada,provavelmente esta instalação pertence somente a uma única empresa, e esta empresa não compartilhará a Plataforma uCloud entre outras organizações. Ainda neste cenário, vamos assumir que a instalação da Plataforma uCloud será utilizada apenas na(s) nuvem(ns) própria(s) (públicas e/ou privadas).

B. Instalação compartilhada como serviço *(SaaS - Software as a Service)*

A funcionalidade Account foi concebida para o cenário de instalação compartilhada *(SaaS)*, onde a empresa (chamaremos de **organização**) tem o objetivo de prestação de serviço de 'Cloud Service Broker' com a Plataforma uCloud entre suas diversas operações (regionais ou internacionais) e para seus diversos clientes-finais.

O cenário acima descrito da Plataforma uCloud *SaaS* é ideal para provedor de serviço de conectividade/comunicação (**organização**) que pode compartilhar a Plataforma uCloud entre suas operações regionais e, também, entre os seus clientes finais que desejam os benefícios de uma operação, governança financeira e *billing*.

Esta funcionalidade auxilia o gerenciamento e o controle do ambiente da organização, de maneira centralizada, por sua regra de negócio possibilita criar as “Contas” e alocar os Contratos, os Grupos e os seus Usuários (elementos pertencentes ao universo "*Switch Roles*”).

Possibilita organizar e compartilhar os recursos entre as “Contas” criadas, além de aplicar as políticas de controle de serviço aos **contratos**, **grupos** e **usuários**, otimizando a melhoria da governança. Esta nova modelagem insere a camada “Conta” no menu **Administração** a qual representa um novo processo para promover o alinhamento em torno da funcionalidade “Contas” e, assim, conduzir as organizações a obter um maior controle.

Esta funcionalidade “**Contas**” tem como objetivo entregar à organização a possibilidade de segmentar clientes por porte (máquinas virtuais), por volume de receita (custos financeiros), possibilita entender o desempenho por “Conta” e filtrar o seu histórico por linha de negócio.

Segmentação por Quantidade de Máquinas Virtuais (Exemplo)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para exemplificar uma forma de como cobrar pela “oferta de serviço” de Gerenciamento Centralizado Nuvem pela Plataforma uCloud, utilizaremos o exemplo de 'níveis de consumo' de infraestrutura computacional com base no número de Máquinas Virtuais Gerenciadas pela Plataforma do uCloud, denominado de “Tier”. Os Tiers representam o modelo de cobrança existente na funcionalidade "Contas", a regra de negócio criada estabelece contabilizar os recursos obtidos e gerados por uma determinada conta.

No portal, os Tiers são categorizados nos níveis de A a J (1 a 10) e calculados a partir das regras estabelecidas com a utilização de dois parâmetros: - certo número de máquinas virtuais  gera determinado custo máximo *(número de máquinas versus custo/valor)*. No caso de uma conta criada, ao atingir um dos parâmetros, imediatamente, a aplicação escala para o próximo nível. Segue a descrição dos níveis dos Tiers:

+--------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+
| **Tier**           |  **A** |  **B** |  **C** |  **D** | **E**  |  **F**  |  **G**  |  **H**  |  **I**  |  **J**  |
+====================+========+========+========+========+========+=========+=========+=========+=========+=========+
|| **Quantidade de** ||       ||       ||       ||       ||       ||        ||        ||        ||        ||        |
|| **Máqs.Virtuais** || ≤ 20  || ≤ 30  || ≤ 50  || ≤ 75  || ≤ 100 || ≤ 150  || ≤ 200  || ≤ 250  || ≤ 300  || ≤ 500  |
+--------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+
| **Valor Mensal**   | $1.500 | $3.000 | $4.000 | $6.000 | $8.000 | $16.000 | $24.000 | $32.000 | $40.000 | $64.000 |
+--------------------+--------+--------+--------+--------+--------+---------+---------+---------+---------+---------+

.. attention:: ATENÇÃO: Todas as quantidades e valores acima apresentados são meramente ilustrativos, servem apenas como exemplos.

Exemplo de Casos de Uso
------------------------

* *Contrato Empresa Galáxia (qtde. VMs 20)*:

Apenas no objetivo de exemplificar um cenário, iremos descrever oferta de serviços de utilização da Plataforma uCloud na modalidade SaaS (Software como Serviço) para a empresa Galáxia, e na sua “Conta” existem 20 máquinas virtuais (ativas e gerenciadas pela  Plataforma uCloud), se enquadra no nível Tier “A” - sendo o valor mensal a ser investido pela Empresa Galáxia será R$ 1,500 reais ou dólares (a depender do país que a empresa está estabelecida). Uma observação importante, caso a conta utilize somente 18 máquinas, esta ainda será classificada no Tier “A”.

Segmentação por Contas
----------------------
Existem duas classes de “Contas” elas estão categorizados em dois tipos, as contas do tipo **Integrator** e do tipo **Producer**, detalhadas a seguir:

* **A. Conta Integrator**
  Esta conta é responsável por criar os perfis das contas integrator e producer, ao criar estes perfis alimenta os tiers e os pacotes, além de estabelecer, a conta producer sua regra de uso. 
  
  * Para exemplificar: 
  
  Funciona como uma espécie de *cluster*, aglomerando ou categorizando outras corporações.

  * Por exemplo:

    Para o caso de uma **corporação** multinacional utilizando uma conta Integrator, ela pode ser considerada “Conta Integrator” para os países que a compõem: México, Brasil, Chile e Colômbia.

    A corporação é responsável por criar outras contas e escalar as permissões de outros usuários. Ela tem como particularidade a lista de todas as contas producer, a lista de todos os contratos associados e pode aplicar as regras de negócio.

* **B. Conta Producer**
  Esta conta producer pertence à organização que consome o recurso, representa uma unidade de menor agrupamento e pode operar todo o portal.

  * Por exemplo:

    Na continuação do exemplo acima, esta corporação multinacional cria as “contas producer” para as organizações que pertencem a ela dentro de um determinado país listado acima, no Brasil, a organização possui as empresas A e B que administram os contratos a1 e b1.

Abaixo segue uma ilustração que apresenta o conceito completo da abrangência da funcionalidade ***Account*** implementada na Plataforma uCloud. Os nomes e denominações utilizados são meramente ilustrativos.

.. figure:: /figuras/ucloud_arquitetura_conceitual003.png
   :align: center

----

As Contas Producer podem ter um administrador ou mais (neste nível o perfil deste usuário é de um Administrador do Sistema - ex.: root), os contratos param de ser criados quando o recurso da conta corporativa acaba, os perfis de visualização e permissionamento obedecem a regra de negócio aplicada pela conta integrator.

A estratégia da utilização da funcionalidade “Contas” entrega uma melhor percepção de valor ao nível de hierarquia que se quer organizar os dados dentro do contexto da organização, ao facilitar seu trânsito nos níveis operacionais, gerenciais e executivos.

Com a criação desta funcionalidade o administrador da conta pode gerenciar as permissões de visualização e permissionamento de cada **usuário** dentro de cada **grupo**, contido em determinado **contrato**. Deste modo, o acesso é negado por padrão, sendo concedido apenas quando as permissões especificarem ‘permitir’.

Adicionalmente, a funcionalidade “Contas” possibilita utilizar as políticas de controle que estabelecem as barreiras de proteção de permissão e visualização aos usuários, a depender das características de tipo de usuário, grupo e contrato a que pertença.

Ao estabelecer esses padrões de permissão, acessos e visualizações aos recursos, organiza e qualifica o privilégio que cada usuário terá dentro dos ambientes dos provedores de nuvem pública em que cada contrato/grupo/usuário pertence, criando assim, permissões diferentes e necessárias para criar controles minuciosos em cada conta.

Descrição de TAGs Virtuais
==========================

Num contexto amplo, uma *TAG* (um rótulo ou uma etiqueta) é uma palavra chave que assina ou identifica um determinado recurso computacional (ou serviço decorrente da existência deste) armazenado em um provedor de nuvem, repositório ou banco de dados. As *TAGs* são um tipo de metadado, capazes de fornecer informação que descreve o dado, isto facilita a busca automatizada para a  recuperação de informações. Uma *TAG* é um rótulo no qual o usuário atribui uma **Chave** e um **Valor** a um recurso computacional de nuvem pública.

No cenário de qualquer tipo de nuvem, o dado contido nas *TAGs* é utilizado juntamente com outras formas de tagueamento que os provedores de nuvem aplicam para classificar as informações a respeito dos seus recursos. Assim, as TAGs auxiliam à pesquisa, organização, identificação, gerenciamento e, por fim, a filtragem dos recursos utilizados de qualquer provedor de nuvem, por exemplo: AWS, Azure, Google, entre outras.

Estas TAGs (etiquetas) após vinculadas a um recurso  são utilizadas para categorizar estes recursos para que possam ser classificados por: finalidade, propriedade, critério ou localidade. Por exemplo: o usuário ou a organização, podem definir um conjunto de *TAGs* para as instâncias do Amazon EC2, da sua conta, para auxiliar a rastrear o proprietário e/ou o nível do agrupamento (empilhamento de valores - stack) de cada recurso computacional de nuvem pública consumido.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual001.png
   :align: center

----

.. note:: A figura acima é um exemplo e as informações presentes são meramente ilustrativas.

Na imagem acima utilizamos duas máquinas virtuais como exemplo para ilustrar a vinculação de TAG a recursos. Um detalhe que é muito pouco mencionado é que os provedores de serviço de nuvem pública não permitem vincular TAGs a todos os seus produtos e/ou serviços (consulte a documentação do provedor para saber quais recursos são passíveis de terem uma TAG vinculada ao recurso).

No exemplo acima vinculamos “**duas** TAGs diferentes” ao mesmo recurso (máquina virtual) desta forma induzimos que os relatórios financeiros por TAG totalizaram o valor do custo da TAG duas vezes (o mesmo valor em cada TAGs) e, para este exemplo, nesta situação dobrar o custo dentro do mesmo período.

Mas devemos ressaltar que para o ambiente do provedor de serviço de nuvem pública, uma vez criada uma TAG esta não será vinculada automaticamente a qualquer recurso (ou serviços decorrentes da existência do recurso). O usuário deve primeiro criar a(s) TAG(s) e depois vincular manualmente a(s) TAG(s) ao(s) recurso(s) desejado(s). Por ser um processo manual e executado por um usuário no console do provedor de serviço de nuvem, o recurso de TAGs pode consumir muito tempo do Administrador de Custos de nuvem pública. Pode existir uma quantidade muito grande de linhas no arquivo de billing/bucket para o Administrador de Custos verificar. Este processo de verificação e de vinculação de TAGs é contínuo e manual.

.. important:: Pelo fato das TAGs serem acessíveis a muitos serviços nos provedores de nuvens, é relevante evitar adicionar dados privados ou confidenciais às *TAGs virtuais*, como por exemplo: identificação pessoal, informação confidencial ou sigilosa.
 
A Plataforma do uCloud sincroniza e recebe o conteúdo do arquivo de billing (CSV) do provedor de serviço de nuvem pública e, consequentemente, recebe todas as TAGs existentes no provedor.
 
 
As TAGs Virtuais da Plataforma uCloud
-------------------------------------

Mencionamos acima que o processo de vincular uma TAGs a um recurso é manual, consome muito tempo e, principalmente, não se repete de forma automática para novos serviços de um recurso que já tenha uma TAG vinculada.

A nova funcionalidade de TAGs Virtuais da Plataforma uCloud cria uma automação para o processo de vinculação de TAGs a recursos existentes no ambiente do provedor de serviço de nuvem pública.

O processamento de TAG Virtual da Plataforma uCloud, pode vincular automaticamente uma TAG específica a um recurso a ser selecionado com base em *Nome de Produto* e/ou *Família de Produto* e/ou *Identificador do Recurso*. Importante ressaltar que a conjunção “e/ou” demonstra o alto grau de granularidade que o usuário pode selecionar para atender ao uso específico de sua necessidade.

Vejamos abaixo como a nova implementação de TAGs Virtuais permite automatizar a vinculação de TAGs em recursos.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual002.png
   :align: center

----

.. note:: A figura acima é um exemplo e as informações presentes são meramente ilustrativas.


No exemplo acima, sempre que a Plataforma uCloud executar a sincronização do arquivo CSV de *billing/bucket*, **automaticamente** as TAGs serão vinculadas para todos os registros (linhas) recursos no arquivo de billing os quais a correlação de *Product Name* ou *Product Family* ou *Identificador do Recurso* for encontrada.

As “TAGs Virtuais” são aplicadas nos recursos da nuvem (por exemplo: máquinas virtuais, bancos de dados) para que seja possível criar classificações por projetos, divisões por centro de custos, entre outros tipos de agrupamentos. Estas chaves e valores de TAGs podem ou não ser refletidas nos *reports* de *billing* disponíveis para consulta somente através do console do provedor de nuvem pública. Assim, os recursos importados do arquivo de *bucket/billing* que existe nos provedores das nuvens públicas que por quaisquer política destes provedores deixam de indexar a etiqueta ao recurso do serviço de nuvens, podem receber uma “*TAG Virtual*”. Mas é muito importante ressaltar que essas “TAGs Virtuais” existem somente na base de dados da Plataforma uCloud, não sendo escrita (ou sincronizada) para o *bucket/billing* que existe no ambiente do provedor de serviço de nuvem pública.

Este é um serviço único e está disponível com a nova implementação da Plataforma uCloud para facilitar a classificação dos recursos utilizados nas **diversas nuvens** por meio da “*TAG Virtual*”. A TAG Virtual deve ser criada pela organização cliente, ela pode ser baseada no perfil de categorização, de acordo com o recurso utilizado e a necessidade de identificação no relatório financeiro, seja por finalidade, propriedade, critério ou localidade, entre outros.

A “*TAG Virtual*” deve ser aplicada pelo cliente usuário dentro do portal uCloud, no intuito de possibilitar a identificação automatizada do recurso que deixou de ser taggeado pelos diversos provedores de nuvens por distintas regras e políticas internas de cada um deles. Após a aplicação da “*TAG Virtual*”  como recurso da plataforma uCloud e em seguida, aplicar por meio do Accountant *virtual-tag-applier*, e a normalização delas, utilizando o Accountant *virtual-tag-normalizer*. Deste modo, será facilitada a visualização das informações para a tomada de decisão, registradas nos relatórios financeiros, em relação a utilização dos recursos providos pelas diversas nuvens que não foram tagueados previamente pela própria nuvem. 

As organizações que utilizam processos automatizados para gerenciar a infraestrutura incluem as TAGs adicionais específicas para automatização, em geral, criam agrupamentos relevantes a fim de organizar os recursos nas dimensões técnicas, comerciais e de segurança. 

Normalização de TAGs Virtuais
-----------------------------

Importante mencionar que a existência contínua de um recurso no provedor de serviço de nuvem, gera novos serviços ou produtos que decorrem da existência/manutenção do recurso na nuvem do provedor de serviço de nuvem pública (ex.: *snapshots*).

Quando um cliente solicita a criação de uma cópia de segurança da imagem de disco (*snapshot*) um novo snapshot pode, não necessariamente, receber a vinculação de um TAG no processo de TAGs Virtuais

Para cobrir esta lacuna existe a nova funcionalidade de **Normalização de TAGs**.

Este processo executa uma comparação de cada linha do arquivo de *billing* e quando encontra um recurso “sem TAG Virtual” mas esta linha é um novo serviço/produto de um recurso com uma TAG Virtual, este processo EFETUA UMA CÓPIA da TAG Virtual do recurso principal mesmo que a sua combinação de *ProductName, ProductFamily, Identificador do Recurso*, não tenha sido capaz de vincular a TAG Virtual.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual003.png
   :align: center

----

.. note:: A tabela acima é um exemplo e as informações presentes são meramente ilustrativas.

Este processo pode levar algum tempo, pois é executado com comparação de *string* de caracteres de cada linha do **billing** individualmente.

Com este processo a Plataforma uCloud complementa a nova funcionalidade de TAGs Virtuais, mas deve ser executada somente quando o usuário Administrador de Custos identifica que existem recursos sem TAGs Virtuais. 

Quando utilizar
----------------

A partir desta nova implementação, direcionada à classificação, normalização e visualização das informações obtidas dos diversos provedores de nuvem pública, a nova funcionalidade “TAGs Virtuais” possibilita "*etiquetar/taguear*", ou seja, marcar os recursos que por alguma regra ou definição, não tenha sido possível encontrar registrada no billing de determinado provedor de nuvem utilizado pela organização ou cliente usuário.

Uma vez que, cada nuvem apresenta distintos relatórios de recursos utilizados, a dificuldade para o profissional de TI conseguir normalizar e entender a classificação apresentada pelas diversas nuvens, ou até informação suprimida por ausência de TAGs que agrupam em formato relevante, informações preciosas, sejam elas quantitativa, qualitativa ou financeira, facilitando à organização e/ou ao seu cliente usuário a possibilidade de tomada de decisão assertiva, ao utilizar esta nova implementação, nomeada de “TAGs Virtuais”. Desenvolvida pela Ustore como solução para atender esta ausência, demandada nos “*reports*" que têm comportamento semelhante nos diversos provedores de nuvem, como AWS, Azure, Google entre outros.

O portal uCloud gera o report financeiro, este relatório recupera informações por nome de produto ou por TAG. É o portal ucloud que oferece este serviço único de “TAGs Virtuais” que possibilita e/ou facilita o gerenciamento e a classificação de certos recursos que deixaram de receber TAGs na nuvem, como dito anteriormente, por regras ou políticas internas estabelecidas pelos próprios provedores. 

É necessário utilizar esta nova implementação, quando a organização e o cliente usuário precisam recuperar informações por TAG ou nome de produto de forma distinta, nas diversas nuvens, uma vez que cada provedor de nuvem, como o Google, a AWS e o Azure tratam o relatório de registro de billing de forma diferenciada. E cada um deles utiliza nomenclaturas próprias para cada tipo de recurso ofertado. 

Ao aplicar as “TAGs Virtuais” nos recursos da nuvem (por exemplo: bancos de dados e máquinas virtuais) é possível criar classificação por divisões de centros de custos, projetos e outros tipos de agrupamentos.

A nova implementação do portal uCloud possibilita apresentar no relatório financeiro informes gerados de acordo com o que foi classificado ou “tagueado” pelo usuário para agrupar ou identificar informações, seja por nome de produto, finalidade, propriedade, critério ou localidade, entre outros.

.. note:: As chaves e os valores de TAGs podem ou não ser refletidas no relatório  (report) de bilhetagem (billing) das diversas nuvens. As TAGs não têm significado semântico no Amazon EC2, são interpretadas como uma sequência de caracteres.

Assim, os recursos importados do arquivo de billing das nuvens públicas que por quaisquer políticas destes provedores deixam de indexar a etiqueta ao recurso do serviço de nuvens, podem receber uma “*TAG Virtual*” dentro do portal. 

Restrições das TAGs
-------------------

No caso da aplicação das “TAGs Virtuais”, existem algumas dicas e restrições básicas a serem aplicadas:

* **Número máximo de TAGs por recurso**: 50
* **Tamanho máximo da chave**: 128 caracteres
* **Tamanho máximo do valor**: 256 caracteres
* **Caracteres permitidos**: Os caracteres permitidos nos serviços são: letras (a-z, A-Z), números (0-9) e espaços representáveis, além dos seguintes caracteres: + - = . _ : / @.

* Para habilitar etiquetas de instância em metadados, as chaves de etiquetas de instância permitem usar letras (a-z, A-Z), números (0-9) e os seguintes caracteres: + - = . , _ : @. Evitar espaços ou /, e não podem formar apenas . (um ponto), .. (dois pontos) ou _index.


.. note:: Para qualquer recurso, cada chave da etiqueta deve ser exclusiva e pode ter apenas um valor.

.. important:: ATENÇÃO: As chaves e os valores de TAGs são *Case Sensitive*, em outras palavras diferenciam **MAIÚSCULAS de minúsculas**.

.. warning:: O prefixo **aws** é reservado para uso da Amazon Web Service (AWS). Não é possível editar nem excluir a chave ou o valor de uma TAG quando ela tem uma chave de TAG com esse prefixo. As TAGs com o prefixo aws: não contam para as TAGs por limite de recurso.

Como utilizar
-------------

Esta nova implementação possibilita taguear os recursos ausentes de marcação na bilhetagem das nuvens, seja por regra ou definição. O que resulta em ganho de informação relevante daqueles recursos que deixariam de ser categorizados e recuperados. 

Existem algumas estratégias comuns de marcação que auxiliam na identificação e gerenciamento de recursos na nuvem, para organizar recursos e para alocar custos, além de várias categorias de marcação na nuvem, por exemplo na AWS:

* **Técnicas**
* **Automação**
* **Comerciais**
* **Segurança**

As TAGs adicionais apresentam maior eficiência por criar agrupamentos, TAGs técnicas, TAGs para automação, TAGs comerciais, TAGs de segurança. Dentre elas podemos citar algumas: Nome, ID do aplicativo, Função do aplicativo, Cluster, Ambiente, Versão, Data/Hora, Aceitar/Recusar, Segurança, Projeto. Proprietário, Centro de custo/Unidade de negócios, Cliente, Confidencialidade e Conformidade.

.. note:: Comportamento da TAG na Nuvem AWS: As TAGs criadas pelo sistema que iniciam com **aws**: são reservadas para uso da AWS, não é possível editar nem excluir uma TAG que inicia com o prefixo aws. Em relação ao limite de criar TAG, cada recurso pode ter no máximo 50 TAGs criadas pelo usuário.

Podemos resumir que o processo de utilização da funcionalidade de TAGs Virtuais se aplicam em dois momentos distintos:

1. **Criação e Automação do uso de TAGs Virtuais;**

  a. Provisionar um nome de identificação para **um único** perfil de TAGs Virtuais com todas as vinculações de TAGs com base na combinação de *Product Name* e/ou *ProductFamily* e/ou *Identificador do Recurso*.
  b. Vincular Perfil de TAGs Virtuais ao identificador de nuvem (*container*).
  c. Executar o processamento e sincronização do arquivo de Billing/Bucket.
  d. Visualização dos relatórios Financeiros na Plataforma uCloud usando a totalização por **TAGs**.
  e. Se for identificado que ainda existem recursos SEM TAGs (lembrar existem recursos que o provedor de serviço de nuvem pública não vincula a nenhuma TAG; ou que a combinação de *ProductName, ProductFamily, Identificador de Recurso*, não foi suficiente para associar a totalidade de linhas do arquivo de *billing*), a Plataforma uCloud permite endereçar esta ausência de TAGs com o processo seguinte.

2. **Normalização de TAGs Virtuais;**

  a. Este processo somente deve ser aplicado quando a combinação existente no Perfil de TAGs Virtuais não consegue aplicar TAGs para todos recursos.
  b. Este processo deve ser executado APENAS UMA VEZ por mês pois demanda um certo tempo para completar a normalização de todas as linhas do billing no período do mês corrente. *Este processo deve ser inicializado manualmente e normaliza as TAGS Virtuais apenas e somente para um único período, não é recorrente ou automático*.

A seguir a tela que apresenta a nova implementação no portal uCloud:

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual004.png
   :align: center

----

Com a adição da nova funcionalidade no portal e a possibilidade de empregar as “TAGs Virtuais” para recuperar a informação previamente tagueada do recurso utilizado em qualquer provedor de nuvem, de forma única, onde a utilização pode ocorrer em dois fluxos, a seguir detalhados:

1. Vinculação de uma TAG para um recurso da nuvem através da especificação de uma sequência de caracteres que identifica um **[ProductName]** e/ou **[ProductFamily]** e/ou **[Identificador da Nuvem]**.

  a. Para esse fluxo o usuário pode especificar, por exemplo, que o recurso pertencente ao *ProductName Amazon Elastic Compute Cloud*, no [ProductFamily] **Data Transfer**, vinculado ao identificador da nuvem i-0e85640d78d096974 tenha as TAGs especificadas no formulário, mesmo que essas TAGs não sejam fornecidas pela nuvem.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual005.png
   :align: center

----

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual008.png
   :align: center

----

  b. Vincular o Perfil de TAGs Virtuais criado, à nuvem (*container*) provisionada na Plataforma uCloud

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual009.png
   :align: center

----

2. Normalização das TAGs para recursos onde na família dos produtos não é retornado TAGs pela nuvem.

  a. Para esse fluxo, será possível habilitar que no ato da coleta de dados de bilhetagem da nuvem, os recursos obtidos que não venham por padrão com a TAG do provedor de nuvem, sejam normalizados com as TAGs que estão associadas a este recurso.

    * Se já houver uma TAG com a mesma chave do outro lado, a TAG não será sobrescrita.
    * Todos os *hyper Identifiers* que pertencerem ao mesmo [productName].

No momento de exportar o relatório de faturamento as “TAGs Virtuais” retornam normalizadas, de acordo com os recursos usados nas TAGs.

.. figure:: /figuras/ucloud_menu_configuracao_tag_virtual010.png
   :align: center

----

A figura acima apresenta a aplicação das “TAGs virtuais'', por meio do Accountant *virtual-tag-applier*, e sua normalização, utilizando o Accountant *virtual-tag-normalizer*.


Oracle Cloud Infrastructure (OCI)
---------------------------------

Com a necessidade das organizações de manter um desempenho consistente, elas tendem a adotar a estratégia de utilizar vários provedores de nuvens públicas. Para atender a esta demanda, a Ustore lança a nova implementação “Oracle Cloud Infrastructure (OCI)”, integrando a nuvem pública OCI ao portal uCloud.

Este novo release da Plataforma uCloud, disponibiliza somente as funcionalidade de operação de infraestrutua OCI, de acordo com a lista de funcionaldades abaixo listada.

A partir deste release notes, o nosso portal passa a dar suporte à nuvem, disponibiliza os recursos e funcionalidade de Operação do embitne OCI listados a seguir:



+-------------------------+-------------------------+------------------------+---------------------+
| **Import de Container** | **Sync de Container**   | **Grupo de Segurança** | **Rede**            |
+=========================+=========================+========================+=====================+
| Máquina Virtual         | Máquina Virtual         | Criar                  | Criar               |
+-------------------------+-------------------------+------------------------+---------------------+
| Rede                    | Rede                    | Deletar                | Deletar             |
+-------------------------+-------------------------+------------------------+---------------------+
| Sub-rede                | Sub-Rede                | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| Grupo de Segurança      | Grupo de Segurança      | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| Região                  | Região                  | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| Flavors                 | Flavors                 | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| Templates               | Templates               | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| Storages                | Storages                | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| IP Público              | IP Público              | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
|                         |                         |                        |                     |
| **Sub-rede**            | **Máquina Virtual**     | **Disco Órfão**        | **IP Público**      |
+=========================+=========================+========================+=====================+
| Criar                   | Iniciar                 | Criar                  | Criar               |
+-------------------------+-------------------------+------------------------+---------------------+
| Deletar                 | Parar                   | Deletar                | Deletar             |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Reiniciar               | Anexar a uma VM        | Anexar a uma VM     |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Performance da VM       | Desanexar de uma VM    | Desanexar de uma VM |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Criar                   | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Deletar                 | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Atualizar               | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Criar Disco             | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Deletar Disco           | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Criar Snapshopt         | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Deletar Snapshopt       | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Criar Placa de Rede     | .                      | .                   |
+---------------------------+-----------------------+------------------------+---------------------+
| .                       | Deletar Placa de Rede   | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Anexar Disco a VM       | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Desanexar Disco a VM    | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
|                         |                         |                        |                     |
| **Par de Chaves**       |  **Balanceador**        | **Invent. Recursos**   | **Storage**         |
+=========================+=========================+========================+=====================+
| Criar                   | Criar                   | Listar                 | Criar Bucket        |
+-------------------------+-------------------------+------------------------+---------------------+
| Deletar                 | Deletar                 | Criar TAG              | Deletar Bucket      |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Anexar Máquina          | Editar TAG             | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| .                       | Desanexar Máquina       | Deletar TAG            | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
|                         |                         |                        |                     |
| **DNS**                 | **Scaling Group**       | **Banco de Dados**     | **VPN**             |
+=========================+=========================+========================+=====================+
| Criar                   | Criar                   | Criar                  | Criar               |
+-------------------------+-------------------------+------------------------+---------------------+
| Deletar                 | Deletar                 | Deletar                | Deletar             |
+-------------------------+-------------------------+------------------------+---------------------+
| Adicionar Registro      | .                       | Reiniciar              | Listar              |
+-------------------------+-------------------------+------------------------+---------------------+
| Deletar Registro        | .                       | DBVM Performance       | .                   |
+-------------------------+-------------------------+------------------------+---------------------+
| Editar Registro         | .                       | .                      | .                   |
+-------------------------+-------------------------+------------------------+---------------------+



Deve-se salientar que a atual lista das funcionalidades acima está diretamente relacionada com a disponibilidade de funcionalidades presentes no atual conjuto de desenvolvimento de software (*SDK - Software Development Kit*) publicado pela Oracle, e que foi utilizado pela equipe de DevOps da Ustore (maio/2022) para a integração com a Oracle Cloud Infrastructure.

O desenvolvimento contínuo tanto da equipe de DevOps da Ustore, como a ampliação das novas funcionalidades presentes em outras evoluções do SDK Oracle, permitem no futuro a evolução de releases e/ou versões da Plataforma uCloud, que serão relacionadas nos futuros Release Notes da Plataforma uCloud.

.. note:: No presente momento neste Release Notes (maio, 2022) a API e o SDK para o OCI ainda não permite o suporte completo para implementação de coleta e cálculo de *billing* da infraestrutura presente no ambiente OCI. Aguardamos a evolução do SDK e API Oracle Cloud Infrastructure para implementar a funcionalidade de *billing* para OCI.

Este conjunto de novas funcionalidades implementadas e descritas, contidas neste documento, geraram o desenvolvimento desta nova versão (`update tag 5.2-b35`). Assim, a Ustore reafirma o constante compromisso de evolução da plataforma e o alinhamento às necessidades do mercado e dos seus clientes.