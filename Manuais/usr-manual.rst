uCloud - Manual de Usuário
++++++++++++++++++++++++++

.. figure:: /figuras/ucloud_logo_peq.png
   :alt: Logo uCLoud
   :align: center

----

Introdução Visão Geral
======================

As organizações empresariais adotaram a nuvem como solução para gerenciar seus ambientes e adotam uma combinação de nuvens privadas e públicas, o grande desafio atual é o gerenciamento destes ambientes híbridos de diversas nuvens (hybrid multi-cloud) de forma a alcançar uma visão unificada, bem como obter um controle dos custos financeiros de forma centralizada, uma vez que cada organização empresarial tem uma necessidade e enfrenta diferentes desafios. 

A Plataforma do uCloud foi desenvolvida para estes cenários, independente de quantos provedores (públicos e/ou privados) existam, o usuário poderá interagir com suas plataformas de Infraestrutura como Serviço (Infrastructure as a Service – IaaS), Plataforma como Serviço (Platform as a Service – PaaS).
Como mencionado anteriormente, o uCloud está posicionado como uma plataforma de Cloud Service Broker – CSB (broker de serviços em nuvem) que permite gerenciar múltiplos provedores de serviços de nuvem, tanto privados quanto provedores de nuvem pública.

Uma plataforma de CSB como a Plataforma do uCloud permite às organizações atuar em cinco pontos fundamentais para o gerenciamento de ambientes híbridos multi-nuvem, são eles:

Governança Financeira
---------------------

Além do controle da infraestrutura, a Plataforma do uCloud permite que empresas usuárias desta plataforma possam estabelecer limites, tanto financeiros quanto quantitativos de recursos (cotas). Estes limites financeiros ou de infraestrutura, podem ser aplicados em três níveis:

* Para um provedor público em geral (ver o ítem Contratos, no Menu Administração)
* Para um grupo de usuários (ver o item Grupos, no Menu Administração)
* Para um usuário/indivíduo (ver o item Usuários, no Menu Administração)

Desta forma, a organização aplicará critérios de governança financeira e controle de custos, como também poderá acompanhar os custos do seu ambiente híbrido de multi-nuvem através de uma única interface. 

A adoção da aplicação de limites (cotas) financeiros e/ou recursos computacionais em diversos níveis alcança o nível de usuário, assim o controle de custos será efetivo e permitirá evitar que o orçamento da organização seja surpreendida em situações que o custo da infraestrutura computacional seja exorbitante ou acima dos valores pré-estabelecidos.

Outro aspecto da Plataforma do uCloud é a redução de custo de certificação e treinamento dos especialistas, em cada uma das interfaces de cada provedor (público e/ou privado), visto que o emprego de uma interface de uso e gerenciamento único e simples, permite extrair mais produtividade do ambiente do provedor de nuvem. Mesmo que o usuário não tenha treinamento ou certificação no console específico do provedor (público e/ou privado), a Plataforma do uCloud possibilitará ao usuário provisionar um recurso computacional no ambiente desejado de forma simples e fácil.

Billing (Faturamento dos Serviços)
----------------------------------

A Plataforma do uCloud viabiliza às organizações empresariais a informação dos custos recorrentes referente ao uso dos recursos computacionais na(s) operação(ões) em um ambiente híbrido multi-nuvem. Este é apenas um dos pontos que faz parte da prática de Cloud Financial Management - FinOps (Gestão financeira da nuvem).

Importante ressaltar que, individualmente, a Plataforma do uCloud não atende a todos os três pilares da prática de FinOps por default. A Ustore possui outros produtos que podem ser complementares e o conjunto de produtos tem potencial para atuar como um ambiente capaz de englobar e atender a prática de FinOps.

O quesito suportado pelo uCloud é o ponto de Informação (Inform), os outros pontos desta melhor prática de FinOps: a Otimização e a Operação pertencem aos outros produtos do portfólio da Ustore que complementa a Plataforma do uCloud.

Deve-se esclarecer que a Plataforma do uCloud não cria ou gera valores de recursos computacionais, estes valores são gerados nos provedores de nuvem pública dos quais a Plataforma do uCloud extrai (download) o arquivo de billing (faturamento) destes provedores e adiciona estas informações em suas bases de dados internas. Para que, posteriormente, de acordo com os critérios comerciais do contrato possam ser aplicados e estes custos calculados e convertidos para a moeda corrente no Brasil. 

Desta forma, o usuário permanece informado da evolução dos custos e poderá acompanhar se estes custos encontram-se dentro dos critérios da governança financeira da organização.

Geralmente estes custos são apresentados em arquivos de texto não estruturados (Comma-separated Values – CSV) gerados a cada período (média de 8 horas) e a Plataforma do uCloud adiciona a informação deste arquivo CSV para a sua base de dados interna de forma a agilizar e simplificar a apresentação destes valores na tela do usuário.

Exclusivamente, os usuários com um perfil específico podem ‘visualizar custos’ e permanecer informados dos valores de consumo dos seus recursos computacionais totais em cada provedor de nuvem (pública e/ou privada). Isto permite que o usuário possa acompanhar os custos acumulados dos recursos computacionais ativos nos provedores de serviços de nuvem.

Monitoração da Infraestrutura
-----------------------------

Uma funcionalidade importante da Plataforma do uCloud é a recente implementação do módulo de gerência de eventos (monitoração) que permite coletar eventos e alarmes que foram gerados nos ambientes de nuvem (público e/ou privado), ativar notificações e criar relatórios customizados. 

Todas essas facilidades reduzem os custos para as organizações, uma vez que elimina a necessidade de contratação de serviços de monitoração dos provedores, pois tal serviço pode representar altos custos os quais podem impactar de forma negativa no orçamento (ultrapassar o limite) destinado para infraestrutura de nuvem pública. 

Esta funcionalidade permite integrar a um ambiente de gerenciamento de Service Desk para controle IT Service Management (gerenciamento de serviços de TI).

Inventário (Assessment)
-----------------------

A Plataforma do uCloud se conecta aos provedores de nuvem através do cadastramento de credenciais de acesso específicas de cada provedor de serviço de nuvem (público e/ou privado). Para esta finalidade as empresas devem providenciar credenciais de modo “operativo”. 

Esta credencial operativa é fornecida pelo administrador do serviço de nuvem e são credenciais que são geradas nas contas dos provedores que somente tem permissão de interagirem com a console do provedor público de nuvem através de uma API, não são credenciais normais com informações padrão de login e senha. Desta forma, a segurança e as regras de regulamentação de segurança da informação estão previstas e atendidas em sua totalidade.

Uma vez que as credenciais operativas são configuradas na Plataforma do uCloud, a primeira atividade é sincronizar as configurações e o inventário de recursos computacionais existentes no provedor (máquinas virtuais – workloads). Este inventário de máquinas virtuais é extraído e adicionado nas bases de dados do uCloud, de forma que a apresentação na tela do usuário seja rápida.

Com este inventário disponível diretamente dentro da Plataforma do uCloud, o usuário poderá operar cada uma das máquinas virtuais, independente de qual é o provedor de nuvem que este recurso está provisionado. Veja a seguir as possíveis operações a serem aplicadas aos recursos computacionais existentes nos provedores de nuvem (público e/ou privado).

Importante mencionar que a Plataforma do uCloud não possui nenhum recurso computacional, estes recursos existem nas nuvens dos provedores de serviço de nuvem pública ou nos ambientes de virtualização (hypervisors) instalados em seu Data Center privado. Através da API Rest a Plataforma do uCloud, envia ações (tarefas) para o gerenciador de ambiente de nuvem específico (público e/ou privado) para que estes então executem a ação desejada.

O usuário poderá acompanhar o resultado de qualquer uma das ações de operação nos recursos computacionais de forma quase que imediata, vale lembrar que não é a Plataforma do uCloud que executa as ações, e sim, o ambiente onde a máquina virtual existe (seja ele público e/ou privado). Este é o encarregado de executar a tarefa enviada através da API Rest. 

Caso o resultado não seja refletido na interface da tela do usuário, o console destino pode levar um certo tempo para executar esta tarefa e somente após o término da execução da tarefa o resultado será apresentado na interface do uCloud. 

Existe uma opção de menu onde o usuário poderá acompanhar o percentual de andamento destas tarefas, seu resultado de sucesso ou a mensagem de erro referente a alguma restrição do ambiente destino. 

Importante ressaltar que podem existir restrições aplicadas ao usuário provisionado na Plataforma do uCloud, restrições ao usuário porque ele pode haver exaurido seu limite, sua cota financeira ou de recursos computacionais, desta forma a Plataforma do uCloud gerar um aviso de erro: “limite de cota excedido” por exemplo. Estes cenários serão descritos no menu Tarefas.

Operação da Infraestrutura
--------------------------

A menção operar significa ao leitor que é a capacidade do usuário comandar certas ações diretamente nestas máquinas virtuais, como ações de: parar (shutdown), reiniciar (restart), suspender (suspend), remover (delete), para citar algumas operações básicas.

Através da interface da Plataforma do uCloud, o usuário pode enviar comandos para os consoles de cada provedor de nuvem, além das ações acima listadas. Este também pode visualizar as informações das configurações específicas da máquina virtual, bem como alterar ou adicionar algum recurso extra a esta máquina virtual (por exemplo: placa de rede, disco, grupo de segurança, snapshot, entre outros).

Em relação aos provedores de serviço de nuvem pública, a Plataforma do uCloud está preparada para se conectar com as seguintes plataformas de nuvem pública:

* Amazon Web Services (**AWS**)
* Google Cloud Plataform (**GCP**)
* Microsoft **Azure**
* IBM Cloud
* Huawei Cloud
* Oracle Cloud Infrastructure (**OCI** - *Roadmap*)

Atualmente, a Plataforma do uCloud está preparada para se conectar com as seguintes plataformas (hypervisors) de gerenciamento de ambiente de nuvem privada:

* **VMware** (vCenter Versões 5.0, 5.1, 5.5, 6.0, 6.5, 6.7);
* **vCloud**
* Hyper-v (Windows 2008R2, Windows 2012, Windows 2012R2 e Windows 2016)
* **Openstack** 
* **Xen Server** 
* XCP-NG
* KVM

A Plataforma do uCloud, além das funções de CSB (*Cloud Service Broker*), também é um agregador de funcionalidades que permite aos usuários, de forma simples e centralizada, o controle de diversos consoles de gerenciadores de ambientes virtualizados (*hypervisors*) seja do ambiente privado on-premises quanto do ambiente de fornecedores de nuvem pública. Agrega as funcionalidades de monitoração, fluxo de trabalho na nuvem (*Cloud Workflow*) e possibilita implementar um repositório biblioteca centralizado de arquivos (playbooks) de referência para uso de ferramentas de infraestrutura como código (*Infrastructure as a Code*).

Integração e Interoperabilidade entre Plataformas (*API Ucloud*)
----------------------------------------------------------------

Interoperabilidade é a habilidade de dois ou mais sistemas (computadores, meios de comunicação, redes, software e outros componentes de tecnologia da informação) de interagir e de intercambiar dados de acordo com um método definido, de forma a obter os resultados esperados. Interoperabilidade define se dois componentes de um sistema, desenvolvidos com ferramentas diferentes, de fornecedores diferentes, podem ou não atuar em conjunto.

A comunicação entre estes 'sistemas' se baseia no consumo de uma interface de programação de aplicação (API) que possibilita o envio e recebimento de chamadas para execução de alguma atividade ou extrair de algum tipo de informação armazenada.  A sigla API deriva da expressão inglesa Application Programming Interface que, traduzida para o português, pode ser compreendida como uma interface de programação de aplicação. Ou seja, API é um conjunto de normas que possibilita a comunicação entre plataformas através de uma série de padrões e protocolos.

Por meio de APIs, desenvolvedores podem estabelecer comunicação (interoperabilidade) entre softwares e aplicativos capazes de se comunicar com outras plataformas.

O principal exemplo é a integração nativa e direta da Plataforma do uCloud com a console dos provedores de nuvem pública, toda esta é executada através da interoperabilidade via API dos  consoles dos provedores.

Outro exemplo bastante comum do uso da plataforma uCloud é a emissão de invoices de bilhetagem para sistemas de showback e chargeback, bem como o envio de informações e alertas sobre recursos gerenciados.

Nossos clientes (e/ou integradores) podem utilizar a documentação da API da Plataforma do uCloud com suas plataformas internas, de forma a complementar ou automatizar certas atividades ou ações que estão além das capacidades nativas da Plataforma do uCloud. Por exemplo: consultar e extrair da Plataforma do uCloud o custo da fatura dos valores de um provedor de nuvem pública através de uma aplicação financeira/contábil para a emissão da Nota Fiscal.

A Plataforma do uCloud possui uma documentação da sua API, mas o acesso a documentação completa deve ser solicitada à Equipe de Atendimento ao Cliente (contato@usto.re) para que seja criada e enviada uma credencial de acesso à documentação da Plataforma do uCloud.
A Equipe Ustore está preparada para auxiliar e avaliar as demandas de interoperabilidade e integração entre a Plataforma do uCloud e as plataformas que possuem e permitem o uso de API’s para a interoperabilidade.

Arquitetura da Plataforma do uCloud
-----------------------------------

Abaixo apresentamos uma arquitetura de referência para a Plataforma do uCloud com os seus componentes, os provedores e as integrações nativas.

.. figure:: /figuras/uCloud_future_vision-small.jpg
   :alt: Arquitetura de Referência da Plataforma uCloud
   :align: center

----

A Plataforma do uCloud se comunica com o console dos provedores através da API Rest, assim toda ação executada ou configurada nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada. A Ustore tem o compromisso de manter o desenvolvimento constante das suas Plataformas de Software e aplicar as melhores práticas (best practices) de DevOps vigentes no mercado de TI, na atualidade. Nosso compromisso versa na manutenção da compatibilidade de integração para que as mais recentes mudanças e implementações no console dos provedores, e de todos os softwares com os quais mantemos interoperabilidade, de forma que as novas funcionalidades estejam sempre disponíveis através da interface da Plataforma do uCloud. Utiliza-se um conjunto de práticas e ferramentas projetadas para aumentar a capacidade de uma organização fornecer aplicativos e serviços mais rapidamente do que os processos tradicionais de desenvolvimento de software.

Acesso a Plataforma uCloud
==========================

O acesso à plataforma é feito através de um endereço de Internet, o usuário deve utilizar um navegador de Internet (Internet browser) e inserir o endereço da URL/link, assim o usuário visualiza a tela inicial de apresentação. Os navegadores de Internet compatíveis com a Plataforma do uCloud são: Microsoft Edge versão 86.x, Google Chrome versão 85.x, Firefox verão 80.x ou Opera versão 71.x.

.. attention::
    *Importante ressaltar que a Plataforma do uCloud não é compatível com o Microsoft Internet Explorer (IE) em qualquer versão, pois as tecnologias deste navegador se encontram desatualizadas e não suportam a evolução das atuais páginas HTML.*
	
Após iniciar uma sessão de Internet browser, o endereço/caminho para o acesso a aplicação deve ser preenchido conforme exemplo abaixo, da seguinte forma:

- Link de exemplo com Endereço IP: ``http://<ucloudserverTCP_IP_Address>:80``

- Link de exemplo com Nome de Servidor: ``http://ucloud_Server_Name.com/``

Após entrar com o endereço corretamente, a tela do usuário será similar a figura abaixo:

.. figure:: /figuras/uCloud_acesso_platafform_001.png
   :alt: Tela de Login da Plataforma uCloud
   :align: center

----

As credenciais para o login e senha devem ter sido provisionadas previamente na Plataforma do uCloud, por um usuário com perfil de Administrador (ou outro usuário com esta permissão).

O usuário deverá informar nos campos os seus dados de login e senha e clicar com o cursor do mouse sobre o botão Entrar.

Caso as credenciais de acesso não tenham sido provisionadas, não existam ou em último caso, o usuário não se recorde das corretas informações das suas credenciais, não terá acesso a plataforma. Ver o item Solicitação de Nova Senha, no caso de o usuário esquecer algum tipo de informação para proceder com o login de acesso à Plataforma do uCloud.

Após inserir suas credenciais de acesso (nome do usuário e senha), efetuar o procedimento de login, ao usuário será apresentada a tela inicial da Plataforma do uCloud.

.. figure:: /figuras/uCloud_acesso_platafform_002.png
   :alt: Dashboard uCloud
   :align: center

----

Siga para o próximo tópico para a descrição detalhada das características da tela inicial (Dashboard) da Plataforma do uCloud.

Menu de Usuário
===============

A barra de menu do usuário fica localizada à esquerda da tela e, inicialmente, é apresentada no modo expandido, como na figura abaixo:
  
.. figure:: /figuras/uCloud_menu_usuario_001.png
   :align: center


Algumas opções de menu possuem um submenu, as quais são apresentadas quando o usuário posiciona o mouse sobre a indicação (sinal de menor “<”). Ao clicar sobre este ícone, a interface apresenta o submenu desta opção ao usuário, ver o exemplo na figura abaixo:

.. figure:: /figuras/uCloud_menu_usuario_002.png
   :align: center

----

É possível ao usuário optar pela redução da apresentação da barra de Menu do Usuário para o modo de Somente Ícones, para ter uma maior área de apresentação. Para alternar entre o Menu do Usuário Modo Expandido e o Menu do Usuário Modo Ícones, existe um elemento gráfico verde com três barras, de fácil identificação para o usuário. Este elemento estará presente em qualquer tela da Plataforma do uCloud.
Quando o usuário clica sobre este elemento, a barra do Menu de Usuário será alternada para o Modo Ícones, conforme o exemplo na figura abaixo:

.. figure:: /figuras/uCloud_menu_usuario_003.png
   :align: center

----

Quando a barra de Menu do Usuário está em modo ícone, os submenus serão apresentados conforme a figura abaixo:

.. figure:: /figuras/uCloud_menu_usuario_004.png
   :align: center

----

As páginas seguintes detalham cada uma das opções do menu de usuário e suas respectivas funcionalidades.

Menu Administração 
==================

Ao apresentar alguns conceitos sobre o ambiente de administração do uCloud, é importante esclarecer alguns pontos sobre a Plataforma do uCloud, nos conceitos existem três termos que serão amplamente utilizados no ambiente do uCloud;

* **Contrato**: é a forma com o qual se define a relação *comercial* entre o provedor e a empresa que o contratou. No contrato são definidos os custos, a margem financeira, taxa de conversão de moeda, custos de recursos (opcional) e a cota (limite) global que pode ser uma cota financeira ou uma cota de recursos computacionais.

* **Grupo**: é uma forma lógica definida unicamente dentro da Plataforma do uCloud que pode definir um grupo de usuários (ex.: DevOps), um departamento (ex.: vendas), uma iniciativa (ex.: VDI), ao qual vários usuários estão associados sendo parte integrante deste grupo. Estes ‘grupos’ não existem nos provedores de nuvem (público e/ou privado) existem somente dentro da Plataforma do uCloud.

* **Usuário**: Um usuário é a entidade que possui acesso identificado à Plataforma do uCloud para efetuar ações nos recursos computacionais dos provedores (público e/ou privado).

A figura abaixo exemplifica, em uma imagem, a relação entre estes três termos e é primordial que o usuário utilize esta figura como referência para entender as relações;
  
.. figure:: /figuras/uCloud_menu_administracao_contrato_002.png
   :align: center

----

É importante entender que um **Contrato** pode possuir vários grupos e cada *Grupo* pode conter vários *Usuários*. Entretanto, a Plataforma do uCloud permite somente que um Usuário faça parte de apenas um grupo e um único Grupo esteja vinculado a exclusivamente um contrato.

A seguir, neste documento, será descrito que ao configurar as cotas (limites financeiros ou de recursos) do contrato, estes limites serão compartilhados/divididos por cada um dos grupos existentes e, por consequência, os usuários estão limitados às cotas do grupo ao qual estão incluídos.

É possível notar, na figura anterior, o termo Virtual Data Center (VDC) este termo é uma alocação lógica de máquinas virtuais que permite às organizações definir um (ou mais) grupo(s) de servidor(es) que faz(em) parte de uma nuvem. Um VDC pode representar um departamento, uma subsidiária ou um grupo de usuários. Veja mais informações no item Virtual Data Center.

A opção Administração apresenta campos que variam de acordo com o perfil do usuário que está acessando o sistema naquele momento. O uCloud possui cinco perfis diferentes.

#. **Usuários do sistema**: são os usuários regulares que acessam o sistema para consumir os recursos. Existe a possibilidade de *Usuários com perfil apenas de leitura*, que podem designar usuários regulares mas limitados em somente para acessar a Plataforma do uCloud para visualizar as informações. 
#. **Usuários Administradores de Contrato**: são os usuários que estão associados a um contrato e sobre este contrato podem definir regras de bilhetagem, provisionar e alterar outros usuários na plataforma.
#. **Usuários Administradores de Grupo**: são usuários que estão associados a um grupo de usuários, eles podem provisionar e alterar outros usuários na plataforma.
#. **Usuários Gestores Financeiros**: usuários com perfil para acessar as informações financeiras do uCloud.
#. **Usuários Administradores**: São usuários com perfil de acesso total e podem efetuar intervenções globais nas configurações da plataforma. Este perfil de usuário é exclusivo da Ustore ou de um único perfil de usuário da organização que efetuou a aquisição das licenças da Plataforma do uCloud. Este usuário administrador possui permissão para gerenciar todas as funcionalidades e recursos globais ofertados pela plataforma.

.. note::
  |atencao| *O Perfil Administrador não será coberto neste documento. Entre em contato com seu ponto focal na Ustore para obter o documento específico: Manual do Administrador da Plataforma uCloud.
  Por segurança, melhores práticas e por padrão, existe apenas um (01) usuário provisionado com este tipo de perfil*.
	
Menu Administração / Usuários
-----------------------------

A Plataforma do uCloud possui bancos de dados próprios que armazenam as informações dos usuários como login e senha de forma segura e criptografada. A tela inicial do Menu Administração apresenta a lista de usuários provisionados, a informação de login de um usuário, o grupo ao qual o usuário está associado e o tipo do seu perfil deste login.

De acordo com o tipo de perfil do usuário que está acessando o sistema, a Plataforma do uCloud apresentará somente a relação de usuários que o perfil que está registrado e ativo pode gerenciar ou administrar.

.. figure:: /figuras/uCloud_menu_administracao_usuario_001.png
   :align: center

----

Para proceder com o acesso à Plataforma do uCloud deve-se provisionar (cadastrar) um usuário com seu respectivo login e senha de acesso.

Abaixo estão descritas as colunas apresentadas nesta lista de usuários:

* **Botão Criar Usuário**: Quando selecionado este botão, o processo está descrito no item Criando Novo Usuário, veja na página 41.
* **Login**: Esta coluna apresenta as credenciais de login do usuário. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de login de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Nome**: Esta coluna apresenta o nome do usuário que foi informado durante o processo do seu provisionamento na Plataforma do uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de nomes de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Grupo**: Esta coluna apresenta o grupo principal do usuário que foi informado durante o processo do seu provisionamento na Plataforma do uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Perfil**: Esta coluna apresenta o perfil do usuário que foi informado durante o processo do seu provisionamento na Plataforma do uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de perfis de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Busca Rápida**: O usuário poderá observar que logo abaixo do nome de cada coluna existe um campo em ‘branco’, este campo permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de eventos de login. Basta preencher o campo em ‘branco’ com uma sequência de caracteres que possam ser relevantes e a Plataforma do uCloud atualizará a tela de forma a representar este padrão de busca.
* **Coluna Perfil**: O campo de busca rápida, na coluna Perfil, possui um controle avançado em forma de um "*dropdownlist*" que permite aplicar um **filtro** de ‘tipo perfil’ para que a lista apresentada fique restrita somente à opção que foi selecionada. Para isto, basta clicar com o cursor do mouse neste campo, a Plataforma do uCloud apresenta as opções de filtragem./

.. figure:: /figuras/uCloud_menu_administracao_usuario_002.png
   :align: center

---- 

Um usuário, provisionado, deve estar vinculado a apenas um dos seis **Tipos de Perfil** disponíveis, e esta definição decorre de qual função este usuário pode estar associado. Destes seis tipos, apenas *dois (02)* perfis (perfil *Usuário* e *Auditor*) são utilizados no dia a dia das operações na Plataforma do uCloud.

O perfil **Auditor** tem uma função muito restrita, mas muito importante no controle e gerenciamento de custos do ambiente de recursos computacionais em nuvem (público e/ou privado).

O perfil **Usuário** é o mais fundamental e mais flexível, pois este pode assumir diferentes níveis de permissões e funções de operação, gerenciamento e administração do ambiente empresarial no uCloud.

Abaixo descrevemos os quatro tipos básicos de perfil de usuários na Plataforma do uCloud:

* **Usuário**: é o perfil universal e todo outro perfil tem como premissa ser provisionado como um usuário da Plataforma do uCloud e que deve estar vinculado a um grupo e está limitado as permissões (acesso a menus) e cotas (limites financeiros ou de recursos) que podem ser individuais ou compartilhadas do grupo. Importante ressaltar que qualquer outro perfil descrito abaixo, são variações deste perfil inicial.
  * Este usuário não possui permissão de alterar nenhuma das suas permissões, as quais foram estabelecidas durante o seu provisionamento. Apenas um usuário com perfil de Administrador de Grupo e/ou de Contrato, poderá redefinir os limites (cotas) e permissões deste perfil de usuário.
  * Este usuário está identificado na listagem com a marca (flag) gráfica: ``user``

* **Usuário Administrador de Contrato**: é um usuário, anteriormente provisionado, que está cadastrado no campo Administrador na tela de Contratos. Este perfil de usuário tem permissão de provisionar novos usuários bem como alterar alguns campos da tela de Contrato.

  * Este usuário possui permissão de alterar algumas das suas permissões estabelecidas durante o seu provisionamento, bem como alterar algumas das suas próprias permissões bem como as permissões de outros usuários. Apenas um usuário com perfil de Administrador de Grupo e/ou de Contrato, poderá redefinir os limites (cotas) e permissões deste perfil de usuário.
  * Este usuário está identificado na listagem com a marca (flag) gráfica: ``user`` - o termo User + uma estrela parcialmente preenchida - indica que este usuário é um Administrador de Contrato.

* **Usuário Administrador de Grupo**: é um usuário, anteriormente provisionado, que está cadastrado no campo Administrador do Grupo na tela de Grupos. Este usuário possui permissão de alterar algumas de suas permissões estabelecidas durante o seu provisionamento, bem como alterar algumas das suas próprias permissões bem como as permissões de outros usuários. Apenas um usuário com perfil de Administrador de Grupo e/ou de Contrato, poderá redefinir os limites (cotas) e permissões deste perfil de usuário.

  * Este usuário está identificado na listagem com a marca (flag) gráfica: ``user`` - o termo User + uma estrela não preenchida - indica que este usuário é um Administrador de Grupo.

* **Usuário Administrador de Contrato e Administrador de Grupo**: A Plataforma do uCloud permite que um usuário possa estar associado como Administrador de um Grupo e, simultaneamente, Administrador de um Contrato este usuário está identificado na listagem com a marca (flag) gráfica: ``user``, e uma estrela estará completamente preenchida indicando que este usuário é um Administrador de Grupo e de Contrato.

  * Esta dupla associação de perfil, permite a este usuário um alto nível de controle e administração do ambiente da empresa 

* **Auditor**: é um usuário que tem acesso ao menu da Gestão Financeira e realiza o acompanhamento do faturamento do portal, bem como define as regras de precificação do contrato.

  * Este usuário, por premissa básica, não está associado a nenhuma permissão para operação e alteração de qualquer que sejam os recursos computacionais em qualquer provedor de serviço de nuvem (público e/ou privado). Este perfil tem acesso unicamente a análise financeira e de custos do contrato ao qual este usuário está vinculado, por intermédio de um grupo.
  * Este usuário está identificado na listagem com a marca (flag) gráfica: ``Auditor``, o termo indica que este usuário é um Auditor do Contrato.

Os outros quatro perfis (Administrator, Service, VDI User, VDI Administrator) são perfis internos da Plataforma do uCloud, não serão cobertos neste documento. Entre em contato com seu ponto focal na Ustore para obter os documentos específicos: Manual do Administrador da Plataforma uCloud e Manual do Ambiente VDI Ustore.


Visualizando um Usuário
-----------------------
Na listagem de usuários é possível visualizar as informações de um usuário,  basta clicar com o mouse sobre a linha na qual o usuário se apresenta, a Plataforma do uCloud exibirá a tela com todas as informações do usuário provisionado na plataforma. Nesta tela é possível adicionar novas configurações ao perfil de um usuário. A tela de visualização de detalhes de um usuário está dividida em seções e será descrita abaixo:

.. figure:: /figuras/uCloud_menu_administracao_usuario_003.png
   :align: center

----

* **Seção Geral**: A primeira seção desta tela apresenta os dados gerais do perfil do usuário provisionado na Plataforma do uCloud. Por meio desta tela será possível alterar alguns campos referentes ao usuário.

  * **Botão de Excluir Usuário**: Este botão pode ser usado para remover o usuário provisionado na Plataforma do uCloud de forma definitiva e irreversível. Basta o usuário clicar com o cursor do mouse sobre o botão, e será apresentada a tela solicitando a confirmação da ação, conforme a tela abaixo:

.. figure:: /figuras/uCloud_menu_administracao_usuario_004.png
   :align: center

----

Após a confirmação da Exclusão do usuário, este usuário e suas credenciais de acesso ficam indisponíveis imediatamente de forma irreversível, não sendo possível recuperar as informações deste usuário. Se a exclusão for acidental, este usuário deverá ser provisionado novamente.
  * **Ícone de Edição Ativo** |icone_edita_on|: Todos os campos que possuem o ícone de edição ativo são passíveis de terem seu conteúdo altera.
  * **Ícone de Edição Inativo** |icone_edita_on|: Todos os campos que possuem o ícone de edição inativo ou não são passíveis de terem seu conteúdo alterado através desta tela (ex.: valores das cotas de grupo) ou o perfil do usuário que está registrado e acessando esta tela, não possui permissão para alterar o conteúdo do(s) campo(s).
  * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma do uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma do uCloud.
  * **Ícone de Cancelamento** |icone_cancela_vermelho|: Caso o usuário tenha clicado sobre o ícone de edição por engano ou não deseja que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna para os valores iniciais, antes de proceder qualquer preenchimento ou alteração.
  * **Barra de Rolagem**: Esta seção possui um grande conjunto de campos, para a completa visualização de todos o usuário deve utilizar a barra de rolagem ao lado direito desta seção. Se o usuário rolar o mouse, a tela desce e apresenta os campos que não estavam sendo visualizados, conforme a tela abaixo:
  * **Apenas Leitura** : Este campo configura um usuário que não tem permissão de efetuar nenhuma ação através da Plataforma do uCloud, mas seu login está ativo e ele possui a capacidade de visualizar todas as telas, as quais ele tenha permissão.

    * Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o seu perfil permita proceder a alteração. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.
  
  * **Autenticação Multifator**: Este campo indica se este usuário terá seu processo de autenticação na plataforma (login) sendo verificado duplamente, antes de aprovar que este usuário tenha acesso a Plataforma do uCloud. Para isto ocorrer, será enviada uma mensagem no número de serviço móvel do celular cadastrado.

    * Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o seu perfil permita proceder a alteração. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.
  
  * **Ativar Cota de Faturamento**: Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o perfil permita alterar. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.
  * **Aprovação do Administrador**: Este campo configura que todas as ações e solicitações efetuadas na interface da Plataforma do uCloud, deste usuário, deverão ser aprovadas por um usuário Administrador do Grupo. Esta é uma funcionalidade para aumentar o controle de governança de custos e operações.

    * Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o perfil permita alterar. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.


* **Seção Permissões do Usuário**: Quando o usuário é criado ele herda/recebe todas as permissões definidas no Grupo ao qual ele pertence (ver próxima seção), bem como as permissões estabelecidas no Contrato. Esta tabela é opcional, mas permite adicionar, ou revogar, as permissões que este usuário possui para efetuar ações, ou acessar menus, na Plataforma do uCloud.
  * **Botão Editar** : Para acrescentar ou revogar permissões para o usuário, o Administrador (ou usuário com autorização) deve clicar neste botão para que a Plataforma do uCloud possa apresentar a tela que seja possível realizar o procedimento de adicionar ou excluir permissões específicas para este usuário. Veja exemplo abaixo:
  Esta tela possui duas colunas distintas;

  À esquerda são as permissões previamente adicionadas ao usuário. Ao lado de cada permissão existe um campo do tipo “check box” que ao ser selecionado exclui (revoga) a respectiva permissão deste usuário.

  À direita estão as permissões disponíveis na Plataforma do uCloud que podem ser adicionadas ao perfil individual deste usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, adiciona a respectiva permissão deste usuário.
    * **Utilizar as permissões padrões**: Ao selecionar este campo “check box”, e confirmar a ação, o usuário receberá todas as permissões de usuário disponíveis na Plataforma do uCloud.
    * **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o mouse no botão Aplicar para confirmar as alterações - de forma definitiva e imediata - para o usuário que está visualizando/alterando. Terminada esta ação a Plataforma do uCloud fechará esta tela e retorna à tela anterior, com seu conteúdo atualizado, apresentando a nova relação de permissões do usuário.

* **Seção Políticas de Permissionamento do Usuário (eventual)**: Esta seção somente será apresentada para usuários que foram provisionados na Plataforma uCloud com o "checkbox" Criar Usuário na Nuvem habilitado. Esta seção apresenta todas as políticas de permissionamento únicas e específicas do ambiente do provedor de serviço de nuvem pública. Estas políticas são ‘importadas’ durante o processo de sincronização do container, e permitem um alto nível de controle granular das capacidades (permissões) que o usuário pode efetuar dentro do ambiente do provedor de serviço de nuvem. Quando o usuário é recém provisionado, este pode estar associado a nenhuma política de permissionamento, será necessário configurar manualmente as permissões.  
  * **Botão Editar**: Este botão permite ao usuário Administrador (ou usuário com autorização) acrescentar ou revogar políticas de permissionamento do ambiente do provedor de serviço de nuvem. Para isto, ele deve clicar no botão ‘Editar’ a partir daí será permitido ao usuário administrador adicionar ou excluir permissões específicas para o usuário desejado. Veja exemplo abaixo:
  Esta tela possui duas colunas distintas;

  * À esquerda são as políticas de permissionamento previamente adicionadas ao usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, exclui (revoga) a respectiva permissão deste usuário.
  * À direita estão as políticas de permissionamento disponíveis do ambiente do provedor de serviço de nuvem pública que podem ser adicionadas ao perfil individual deste usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, adiciona a respectiva permissão deste usuário.
  * **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação, a Plataforma do uCloud fechará esta tela e retornará à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.
   
* **Seção Permissões do Grupo**: Esta seção somente apresenta as permissões que foram definidas nas configurações do Grupo ao qual este usuário está vinculado. A Plataforma do uCloud não permite que as permissões listadas aqui possam ser alteradas através desta tela. Para ter contato e conhecer as permissões definidas no grupo, veja o item Administração / Grupos. Se forem necessárias alterações de qualquer permissão listadas aqui, estas alterações devem ser efetuadas nas configurações do Grupo.

* **Seção Grupos Secundários**: Nesta seção é possível associar um usuário a mais de um grupo na Plataforma do uCloud. Na seção Geral, é possível verificar o Grupo principal ao qual o usuário está vinculado.
   * **Botão Editar**: Para vincular este usuário a um grupo secundário, ou desvincular este usuário de um grupo secundário, o Administrador (ou usuário com autorização) deve clicar neste botão Editar para que a Plataforma do uCloud possa apresentar a tela que permite desvincular o usuário de grupos secundários. Veja exemplo abaixo:
   * À direita estão listados os grupos que estão vinculados ao contrato do grupo principal ao qual este usuário foi provisionado originalmente. A Plataforma do uCloud lista somente os grupos que estão vinculados ao contrato vigente. Ao lado de cada grupo existe um campo do tipo “check box” que, quando selecionado, vincula o grupo selecionado a este usuário.
   * À esquerda estão listados os grupos secundários que este usuário está vinculado. Ao lado de cada grupo existe um campo do tipo “check box” que, quando selecionado, desvincula o grupo selecionado deste usuário.
   * **Botão Aplicar**: Após certificar que todas as vinculações, ou remoção, foram configuradas, o usuário deve clicar no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.
  
* *Seção Perfis de Visualização*: Esta seção permite que o administrador do contrato possa selecionar quais opções do Menu do Usuário, este usuário poderá visualizar. Através desta funcionalidade, o administrador pode personalizar como este usuário interage com a Plataforma do uCloud. É possível acompanhar o processo de definição destes perfis no item Configurações / Perfis de Visualização. Esta configuração retira ou adiciona as opções da barra de Menu de Usuário, de forma que para o usuário não há como saber que tal função existe. A possibilidade de saber, seria acompanhar outro usuário utilizando a plataforma com outras opções de Menu de Usuário visíveis.
   * **Botão Adicionar**: Para adicionar este usuário a um perfil de visualização, ou desvincular este usuário de um grupo secundário, o Administrador (ou usuário com autorização) deve clicar neste botão Adicionar para que a Plataforma do uCloud possa apresentar a tela que possibilita associar o usuário a um dos perfis de visualização configurados na plataforma. Veja exemplo abaixo:
   * Pode-se informar parte do nome de um grupo e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud apresente uma lista com todos os grupos que possuem a mesma sequência de caracteres informados. Este campo é sensível a maiúsculas e/ou minúsculas, somente irá listar os Perfis de Visualização que combinam exatamente com a parte do texto que foi digitado (se nada for listado, digitar o texto com outra combinação de maiúsculas e ou minúsculas.

   * **Botão Salvar**: Após certificar que vinculou o usuário ao Perfil de Visualização correto, o usuário deve clicar com o botão do mouse no botão Salvar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

.. note:: |atencao| *Importante ressaltar que os perfis listados na tela exemplo não existem e foram criados apenas para fins ilustrativos.*

* **Seção Últimos Logins**: Nesta seção serão listados todos os eventos em que este usuário se conectou (login) na Plataforma do uCloud. Veja a tela exemplo abaixo:
   * **Data do Login**: Este campo apresenta a data e a hora em que o usuário inicia uma sessão na Plataforma do uCloud, utilizando o seu login. A informação está apresentada no formato de data no padrão brasileiro (Dia/Mês/Ano Hora:Minuto:segundo).
   * **Data de Logout**: Este campo apresenta a data e a hora em que o usuário encerra uma sessão na Plataforma do uCloud, utilizando o seu login. A informação está apresentada no formato de data no padrão brasileiro (Dia/Mês/Ano Hora:Minuto:segundo).
   * **Tempo da Sessão**: Este campo apresenta o total de tempo que este login de usuário permanecer conectado a Plataforma do uCloud, no formato de horas, minutos e segundos (ex.: 6h 18m 33s).
   * **IP Remoto**: Este campo apresenta o número do endereço TCP-IP o qual o usuário estava associado, quando iniciou a sessão com a Plataforma do uCloud.
   * **Busca Rápida**: O usuário pode notar que logo abaixo do nome de cada coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de eventos de login. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma do uCloud atualizará a tela de forma a representar este padrão de busca.

* **Seção Máquinas Virtuais**: Esta seção apresenta uma lista das máquinas virtuais (VMs) ou cargas de trabalho (workloads) que foram criadas por este usuário, durante uma sessão ativa na Plataforma do uCloud.
   * **Busca Rápida**: O usuário pode notar que logo abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de máquinas virtuais (VMs) deste usuário. Basta preencher o campo em branco com uma sequência de caracteres que possa ser relevante e a Plataforma do uCloud atualiza a tela de forma a representar este padrão de busca.

Criando Novo Usuário
--------------------

Antes de tratar da criação de um usuário é importante estabelecer que para a Plataforma do uCloud um Usuário está vinculado a um Grupo e um Grupo está vinculado a um Contrato [Usuário<Grupo<Contrato].
Desta forma, antes de iniciar a criação de um novo usuário, é importante verificar a existência do grupo ao qual este usuário será associado. Para criar um usuário é necessário selecionar a opção **Criar Usuário** conforme indicado abaixo. 

.. figure:: /figuras/uCloud_menu_usuario_022.png
   :align: center

----

A seguir a descrição do correto preenchimento dos campos desta tela, para provisionar um usuário na Plataforma do uCloud, são eles:

* **Grupo**: Este campo é obrigatório e o usuário deve informar um grupo previamente provisionado na Plataforma do uCloud, pois não será possível continuar o cadastramento de um usuário sem vincular este novo usuário a um grupo existente.

.. figure:: /figuras/uCloud_menu_usuario_017.png
   :align: center

----

   * Pode-se informar parte do nome de um grupo e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo:
   * Quando encontrado o Grupo ao qual este novo usuário deverá estar vinculado, basta selecioná-lo e o campo se preencherá com o grupo específico.
   * *Importante ressaltar que será possível associar este usuário a mais de um grupo, caso seja necessário. Mas estes grupos devem estar vinculados a somente um único Contrato.*

* **Nome**: Este campo é obrigatório e deve ser preenchido com o nome do usuário que se está provisionando.
* **Login**: Este campo é obrigatório e deve ser preenchido com a sequência de caracteres que será utilizada para identificar o usuário durante o processo de login no uCloud.
* *Senha*: Este campo é obrigatório e deve ser preenchido com a sequência de caracteres da senha do usuário. Importante ressaltar que esta sequência deve ser maior do que quatro (04) caracteres alfanuméricos. Deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”, conforme a documentação encontrada no site da Azure. A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres e deve conter caracteres de três das seguintes categorias:
   * Letras maiúsculas e minúsculas (A a Z)
   * Números de base 10 (de 0 a 9)
   * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' <>,.? /) – Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política.

* **Confirmar Senha**: Este campo é obrigatório e deve ser preenchido com a mesma sequência de caracteres informados no campo anterior. Caso a sequência informada neste campo seja diferente da anterior, será apresentado um pop-up com uma mensagem de erro na tela.

.. figure:: /figuras/uCloud_menu_usuario_018.png
   :alt: Menu de Usuário
   :align: center

----

* **Email**: Este campo é obrigatório, nele deve ser informado um endereço de correio eletrônico (e-mail) válido. Este endereço de correio eletrônico será fundamental durante o processo de redefinição de senha pelo usuário, pois a Plataforma do uCloud utiliza este e-mail para o envio de uma mensagem que permite ao usuário criar uma senha, para ele, de forma automática.

.. attention::
    A Plataforma do uCloud **não efetua** qualquer validação prévia referente a existência do e-mail informado ou seu efetivo funcionamento. No caso de inexistência do e-mail destino, ou erro em sua digitação, o usuário ficará impossibilitado de executar a redefinição da sua senha de acesso. Neste caso deverá contactar o administrador do seu grupo/contrato.

* **Telefone**: Este campo é obrigatório, e deve ser preenchido com um número de telefone de serviço móvel celular, utilizar o seguinte formato:
   * **Dois (02)** números que identificam o código de área do número de telefone de serviço móvel celular (XX). Não é necessário informar o número ‘zero (0)’ que antecede ao código de área no padrão brasileiro.
   * **nove (09)** números que identificam o número de telefone do serviço móvel celular do usuário. Não é necessário informar qualquer outro caractere para separação dos grupos de números de telefone serviço móvel celular.
   * Exemplo de preenchimento: ``(11)999991234``

* **Cargo**: Este campo é obrigatório, mas é meramente informativo para identificar o cargo do usuário que se deseja provisionar.
* **Empresa**: Este campo é obrigatório, mas é meramente informativo para identificar a organização a qual este usuário está associado.
* **Tipo de Cota**: Este campo é obrigatório, trata-se de um campo do tipo “drop down list”, quando o usuário clicar sobre este será apresentada a lista das opções de tipos de cota disponíveis para provisionar um usuário, veja as opções abaixo:

.. figure:: /figuras/uCloud_menu_usuario_019.png
   :alt: Tipo de Cota de Usuário
   :align: center

----

* **Cota de Grupo**: Quando selecionada esta opção o usuário compartilha dos limites (cotas) financeiros ou de recursos computacionais que estão definidos nas configurações do Grupo. Usuários com cota de grupo devem ficar atentos nas informações apresentadas na tela inicial (dashboard – veja item Dashboard) uma vez que a Plataforma do uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites disponíveis no grupo ao qual o usuário está vinculado.
* **Cota de Usuário**: Quando selecionada esta opção pelo usuário, a Plataforma do uCloud solicita que sejam informados os limites (cotas) financeiros ou de recursos computacionais específicos e individuais para este usuário, conforme a tela abaixo;
 
.. figure:: /figuras/uCloud_menu_usuario_020.png
   :alt: Cota Individual de usuário
   :align: center

----

* **Cota de CPU**: Este campo é obrigatório e deve ser informado um número inteiro que representa o limite máximo de consumo do recurso computacional de CPUs para todas as máquinas virtuais criadas nos provedores de serviço de nuvem (público e/ou privado), por este usuário.
* **Cota de Faturamento**: Este campo é opcional e deve ser informado um número inteiro que será estabelecido como limite máximo referente aos valores financeiros dos custos de consumo dos recursos computacionais para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado).
* **Cota de Memória**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Memória para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado). Pode ser selecionado o limite em Gigabytes ou um limite em Terabytes.
* **Cota de Disco**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Disco para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado). Pode ser selecionado o limite em Gigabytes ou um limite em Terabytes.
* **Cota de IPs Públicos**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de IPs Públicos para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado).
* Em outras palavras, os usuários sem cota individual podem consumir a cota definida no Grupo; quando definida uma cota para um usuário, uma parte da cota do Grupo é alocada para o usuário, esta parte da cota do Grupo não será acessível a outros usuários do Grupo.
* Quando um usuário se registra, ele deve observar as informações apresentadas na tela inicial (dashboard – veja item Dashboard na página ) pois a Plataforma do uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites definidos para este usuário.

.. note:: |atencao| *Usuários com cotas individuais: esta cota individual será subtraída (retirada) da cota do Grupo ao qual este usuário está vinculado.* 

* **Habilitar Primeiro Acesso**: Este campo é um campo opcional do tipo de seleção  “check box”, que permite que o usuário possa alterar sua senha de acesso no primeiro acesso deste usuário a Plataforma do uCloud. Quando selecionado, a Plataforma do uCloud irá apresentar um ‘pop-up’ solicitando ao usuário informar uma nova senha, para substituir a senha inicialmente provisionada para este usuário,

.. warning:: A Plataforma do uCloud não irá permitir que o usuário inicie uma sessão ativa sem antes o usuário substituir a senha originalmente informada. Após o usuário informar a nova senha, será armazenada de forma encriptada nas bases de dados internas, neste momento a sessão do usuário se torna ativa para iniciar a o uso da Plataforma do uCloud normalmente.

* **Ativar Autenticação Multifator**: Este campo é um campo de seleção “check box” que indica se este usuário terá seu processo de autenticação na plataforma (login) sendo verificado duplamente antes de aprovar que este usuário tenha acesso a Plataforma do uCloud. Será enviada uma mensagem para o correio eletrônico informado no campo **e-mail** com um link/url para o usuário confirmar a segunda etapa de autenticação.
* **Ativar cota de Faturamento**: Este campo é um campo de seleção “check box” que indica se este usuário terá seu faturamento computado constantemente na relação de consumo de Faturamento (ver item Financeiro).
* **Administrador precisa aprovar a realização de atividades**: Este campo é um campo de seleção "checkbox" que indica todas as ações e solicitações efetuadas na interface da Plataforma do uCloud, elas devem ser aprovadas por um usuário Administrador do Grupo. Esta é uma funcionalidade destinada a aumentar o controle de governança de custos e operações.
* 
  * Na prática, qualquer novo recurso computacional (uma nova máquina virtual) que este usuário solicitar através da interface do uCloud: a solicitação não será enviada para o provedor de serviço de nuvem (público e/ou privado) de forma imediata, a solicitação ocorrerá em 2 tempos. No primeiro momento, ela aguarda a aprovação do Administrador do Grupo. No segundo tempo, após a aprovação do administrador do grupo (se aprovada) a solicitação segue no processo de criação/alteração solicitada por este usuário.

* **Criar Usuário na Nuvem**: Este campo é um campo de seleção "checkbox" que indica as credenciais de login e senha deste usuário (informadas acima), elas serão enviadas ao provedor de serviço de nuvem pública para que seja provisionado um usuário com as mesmas credenciais de acesso no provedor de serviço de nuvem pública selecionado abaixo.
   * **Containers**: Este campo é obrigatório e do tipo “Dropdown” quando o usuário clica com o cursor do mouse, a Plataforma do uCloud lista todos os containers configurados na Plataforma do uCloud. O usuário deve selecionar um provedor da lista.

.. figure:: /figuras/uCloud_menu_usuario_021.png
   :alt: Menu de Usuario
   :align: center

----

* **Permissões**: O usuário recebe/herda todas as permissões definidas no Grupo ao qual ele pertence, bem como as permissões estabelecidas no Contrato e por último as permissões específicas deste usuário. Esta tabela é opcional, ela permite adicionar ou revogar as permissões que este usuário recebe, o que permite efetuar ações ou acessar menus na Plataforma do uCloud. São cento e trinta e duas (132) permissões disponíveis que podem ser associadas ao usuário (todas ou apenas uma parte). Qualquer alteração efetuada nas permissões disponíveis (inclusão ou revogação) será aplicada de forma imediata no login deste usuário após a confirmação. Veja o item Configurações / Perfis de Permissionamento para uma forma alternativa de criar grupos de permissões customizados para sua empresa
   * **Botão Criar**: Após todos os campos obrigatórios e opcionais para provisionar o novo usuário estarem preenchidos o usuário pode clicar com o cursor do mouse no botão verde Criar, assim a Plataforma do uCloud provisiona o novo usuário em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, significa que algum campo obrigatório permanece sem preenchimento (o usuário deve checar e corrigir) ou a sequência de caracteres da senha do login deve ser inferior a quatro (04) caracteres.

Administração / Grupos
----------------------

Na Plataforma uCloud, o termo Grupo estabelece um conceito que permite alocar uma determinada quantidade de recursos computacionais, ou recursos financeiros, que poderão ser consumidos por todos os usuários que estão vinculados ao grupo, criando assim uma pequena ‘célula’ de governança financeira. A Plataforma do uCloud pode conter diversos Grupos para que a governança financeira fique mais próxima do cenário real da organização.

Importante ressaltar que o conceito de ''Grupos" existe somente para a Plataforma do uCloud e não existe nada similar nos provedores de serviço de nuvem pública ou privada.

Um Grupo de usuários pode ser um Departamento, uma Unidade de Negócio, um Centro de Custos, uma Filial. Quando se define um limite de quantidade de recursos computacionais ou um limite financeiro para um grupo, significa que a Plataforma do uCloud registra este limite. 

Se este recurso ultrapassar os limites estabelecidos para o grupo, da parte de qualquer usuário vinculado a este grupo, a Plataforma do uCloud nega (bloqueia) a criação ou alteração de determinada quantidade de recurso computacional, uma vez que este novo recurso computacional não poderá ultrapassar estes limites.

Estes limites podem ser ajustados a qualquer momento (aumento ou redução) da parte dos usuários com perfil de Administrador de Grupo ou Administrador de Contrato, apenas eles estão habilitados para alterar os valores limites (cotas) estabelecidos no grupo.

.. figure:: /figuras/uCloud_menu_grupo_001.png
   :alt: Menu de Usuario
   :align: center

----

A seguir a descrição das colunas apresentadas nesta lista de grupos:

* **Botão Criar Grupo**; Quando selecionado este botão o processo está descrito no item.

* **Nome**: Esta coluna apresenta o nome do Grupo. Como forma de simplificar a visualização, é possível clicar com o botão do mouse no título desta coluna, o resultado apresentado na Plataforma do uCloud apresenta a classificação da lista de grupos de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Contrato**: Esta coluna apresenta o nome do Contrato ao qual este grupo está associado. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no nome do contrato de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Admin**: Esta coluna apresenta o nome do login de usuário que foi associado no campo de Administrador do Grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no nome do login de usuário de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Cota de CPU**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de CPU que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor da quantidade de CPU de forma crescente ou decrescente.

* **Cota de Memória**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Memória que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor da quantidade de memória de forma crescente ou decrescente.

* **Cota de Disco**: Esta coluna apresenta o número inteiro que representa o limite (cota) valor total de Disco de Armazenamento que foi definido para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor total do Disco de Armazenamento de forma crescente ou decrescente.

Visualizando Grupo
------------------

Estando na listagem de grupos é possível visualizar algumas informações de um grupo, para isto, basta clicar com o mouse sobre a linha à qual um grupo faz parte e a Plataforma do uCloud apresentará a tela com todas as informações de um grupo provisionado na plataforma. Através desta tela é possível adicionar novas configurações ao perfil de um usuário.

A tela de visualização de detalhes de um usuário está dividida em seções, descrita abaixo;

.. figure:: /figuras/uCloud_menu_grupo_002.png
   :alt: menu de usuário
   :align: center

----

* **Botão de Excluir Grupo** Este botão pode ser usado para remover o grupo provisionado na Plataforma do uCloud de forma definitiva e irreversível. Basta o usuário clicar com o cursor do mouse sobre o botão, e será apresentada uma tela solicitando a confirmação da ação, conforme a tela abaixo;

.. figure:: /figuras/uCloud_menu_grupo_003.png
   :alt: menu de usuário
   :align: center

----

* Após a confirmação da Exclusão do grupo, este grupo e as configurações associadas a este estarão indisponíveis imediatamente de forma irreversível, não sendo possível recuperar as informações deste grupo. Se a exclusão for acidental, este usuário deverá ser provisionado novamente, ver o item  na página.

.. warning:: A Plataforma do uCloud não permite remover um grupo quando existem ainda usuários vinculados ao grupo. Antes de excluir um grupo da plataforma certifique que todos seus usuários foram desvinculados do referido grupo para que seja possível a remoção do grupo seja definitiva.
	
* **Seção Geral**: Esta seção da tela apresenta as informações sobre o grupo que está provisionado e os campos apresentados nesta seção podem ter seu conteúdo alterado através desta tela. O que define a condição de alteração está relacionado com o ícone de edição a seguir;
   * **Ícone de Edição Ativo**: Todos os campos que possuem o ícone de edição ativo são passíveis de ter seu conteúdo alterado.
   * **Ícone de Edição Inativo**: Todos os campos que possuem o ícone de edição inativo ou não são passíveis de terem seu conteúdo alterado através desta tela (ex.: valores das cotas de grupo) ou o perfil do usuário que está registrado e acessando esta tela, não possui permissão para alterar o conteúdo do(s) campo(s).
   * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma do uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma do uCloud.
   * **Ícone de Cancelamento** |icone_cancela_vermelho|: Caso o usuário tenha clicado sobre o ícone de edição por engano, ou não deseja que as alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho, para cancelar as alterações e o conteúdo do campo irá retornar para os valores iniciais, antes de qualquer preenchimento ou alteração.

* **Seção Permissões**: O Grupo recebe (herda) todas as permissões definidas no Contrato ao qual este grupo está vinculado. Esta tabela é opcional, mas permite adicionar ou revogar as permissões que este grupo possui para efetuar ações ou acessar menus na Plataforma do uCloud.

.. figure:: /figuras/uCloud_menu_grupo_004.png
   :alt: menu de usuário
   :align: center

----

   * **Botão Editar**; Para acrescentar ou revogar permissões para o usuário Administrador do Grupo (ou usuário autorizado com perfil semelhante ao administrador), basta clicar neste botão para que a Plataforma do uCloud apresente a tela para adicionar ou excluir permissões específicas para este grupo.

.. figure:: /figuras/uCloud_menu_grupo_005.png
   :alt: menu de usuário
   :align: center

----

Abaixo descreveos os campos desta tela:

* Esta tela possui duas colunas distintas, à esquerda são as permissões definidas no Contrato que são repassadas para o Grupo vinculado ao contrato. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, exclui (revoga) a respectiva permissão deste usuário.
* À direita estão as permissões disponíveis na Plataforma do uCloud que podem ser adicionadas ao grupo. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, adiciona a respectiva permissão deste usuário.
* **Utilizar as permissões padrões**: Ao selecionar este campo “checkbox”, e confirmar a ação, o Grupo receberá todas as permissões disponíveis na Plataforma do uCloud.
* **Botão Aplicar**: Após o usuário certificar-se de que todas as alterações necessárias foram configuradas (inclusões ou exclusões),ele deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o grupo que se está alterando. Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

* **Seção Virtual Data Center**: Nesta seção são listados todos os Virtual Data Centers (VDC) associados a este grupo. Um Virtual Data Center é um agrupamento ‘lógico’ de determinados recursos computacionais de nuvem (templates, flavors, redes, regiões globais, storage e máquinas virtuais) que possibilita um controle de governança financeira para a empresa. O usuário vinculado a este grupo, que possui um (ou mais) Virtual Data Center, somente poderá consumir os recursos computacionais disponíveis neste Virtual Data Center. Para mais informações veja no item Menu Virtual Data Center.

.. figure:: /figuras/uCloud_menu_grupo_006.png
   :alt: menu de usuário
   :align: center

----

* **Botão Editar** |botao_editar|; Para vincular um Grupo a um Virtual Data Center, o usuário Administrador do Grupo (ou usuário com autorização) deve clicar neste botão para que a Plataforma do uCloud possa apresentar a tela para adicionar ou excluir um Virtual Data Center vinculado a este grupo.

.. figure:: /figuras/uCloud_menu_grupo_007.png
   :alt: menu de usuário
   :align: center

----

* Esta tela possui duas colunas distintas, à esquerda estão apresentados os Virtual Data Centers (VDCs) que foram vinculados a este Grupo (no momento do seu provisionamento). Ao lado de cada VDC existe um campo do tipo “checkbox” , ao selecioná-lo a Plataforma do uCloud exclui (desvincula) o VDC deste grupo.
* À direita estão apresentados os Virtual Data Centers (VDCs) que estão vinculados ao contrato deste, ao qual este grupo pertence e que permite ser vinculado a este Grupo. Ao lado de cada VDC existe um campo do tipo “checkbox” , quando selecionado, vincula o VDC ao Grupo.
* **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o grupo que se está alterando. Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.
* **Coluna Ações / Botão Kick-Off** ; Este botão permite desvincular o Virtual Data Center do Grupo em uma ação. Basta o usuário clicar com o mouse no botão Kick-Off para que o VDC seja desvinculado do Grupo, de forma definitiva e imediata, para o grupo que se está alterando. Importante ressaltar que esta ação não solicita validação para o usuário.

* **Seção Usuários**: Esta seção da tela apresenta a lista de todos os usuários que estão vinculados ao grupo e o respectivo consumo individual de recursos computacionais. Através desta tela o usuário com perfil de Administrador do Grupo, pode acompanhar qual(is) usuário(s) consome(m) mais recursos computacionais nos provedores de nuvem (público e/ou privado);

.. figure:: /figuras/uCloud_menu_grupo_008.png
   :alt: menu de usuário
   :align: center

----

* **Botão Criar Usuário**; Este botão permite provisionar um novo usuário na Plataforma do uCloud já vinculando este novo usuário ao grupo que se está visualizando. Esta é a metodologia recomendada pela Ustore para provisionar novos usuários para acessar o ambiente. Quando clicar com o botão do Mouse sobre este botão, a Plataforma do uCloud apresenta a tela de Criando Novo Usuário.
* **Botão Adicionar Usuário Existente**; Este botão permite vincular um usuário existente a este grupo. Quando o usuário clicar com o cursor do mouse neste botão será apresentada uma tela;

.. figure:: /figuras/uCloud_menu_grupo_009.png
   :alt: menu de usuário
   :align: center

----

* É necessário preencher o campo desta tela com alguns caracteres do login do usuário que se deseja associar e a Plataforma do uCloud apresenta uma lista com os logins de usuário que possuam os caracteres informados em sua identificação de login. Selecionar o usuário desejado com o botão do mouse e depois confirmar a ação através do botão verde OK. Esta tela será encerrada e a lista de usuários do grupo será atualizada - como resultado apresenta este usuário, neste grupo.

Esta seção da tela possui uma lista com colunas, descritas a seguir;

* **Login** : Esta coluna apresenta as credenciais de login do usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de login de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Cota de CPU** : Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de CPU que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor da quantidade de CPU de forma crescente ou decrescente.

  * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
  * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de Faturamento** : Esta coluna apresenta o número que representa o limite (cota) do valor financeiro que foi definido para o usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor financeiro de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de Memória** : Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Memória que for definida para este usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor da quantidade de memória de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de Disco** : Esta coluna apresenta o número inteiro que representa o limite (cota) valor total de Disco de Armazenamento que for definido para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor total do Disco de Armazenamento de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de IPs Públicos** : Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Endereços TCP-IP Públicos que foram definidos para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor da quantidade de IPs Públicos de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Uso da CPU**: Esta coluna apresenta a quantidade consumida do recurso computacional CPU por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor total de consumo do recurso CPU de forma crescente ou decrescente.
* **Uso da Memória**: Esta coluna apresenta a quantidade consumida do recurso computacional de Memória por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor total de consumo do recurso Memória de forma crescente ou decrescente.
* **Uso do Disco**: Esta coluna apresenta a quantidade consumida do recurso computacional Disco de Armazenamento por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista dos usuários com base no valor total de consumo do recurso Disco de Armazenamento, de forma crescente ou decrescente.
* **Uso de IP**: Esta coluna apresenta a quantidade consumida do recurso computacional Endereços TCP-IP Público por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor total de consumo do recurso Endereço IP, de forma crescente ou decrescente.

* **Ações**: Esta coluna apresenta ícones que demonstram se o usuário está provisionado consumindo as cotas do Grupo ou possui cota individual. Para usuários com cotas individuais, existe um botão para editar os limites (cotas) dos recursos computacionais ou financeiros de um usuário com cotas individuais.
   * **Ícone de Cota de Grupo** |icone_cota_grp|; Este ícone será apresentado nas linhas de usuários que estão associados a cota de grupo.
   * **Ícone de Cota de Usuário** |icone_cota_indv|; Este ícone será apresentado nas linhas de usuários que estão associados a cota individual.
   * **Botão Editar Cotas** |botao_editar|; Este botão é apresentado somente nas linhas de usuários que estão associados às cotas individuais. Exclusivamente estará ativo se o perfil do usuário que está registrado e acessando esta tela for um administrador de grupo ou de contrato e possuir a permissão para alterar o conteúdo do(s) campo(s). Quando for pressionado o botão 'Editar Cotas' a Plataforma do uCloud apresenta a tela abaixo:

.. figure:: /figuras/uCloud_menu_grupo_010.png
   :alt: menu de grupo
   :align: center

----

* **Cota de CPU**: Alterar, se necessário, o novo valor de limite de quantidade do recurso computacional das CPUs.
* **Cota de Memória**: Alterar, se necessário, o novo valor de limite de quantidade do recurso computacional de Memória.
* **Cota de Disco**: Alterar, se necessário, o novo valor de limite de quantidade do recurso computacional do Disco de Armazenamento.
* **Cota de IPs Públicos**: Alterar, se necessário, o novo valor de limite de quantidade do recurso computacional de Endereços TCP-IP Público.
* **Cota de Faturamento**: Alterar, se necessário, o novo valor do limite (cota) do valor financeiro que for definido para o usuário.
* **Botão Editar**: Após checagem de que todas as alterações necessárias foram configuradas, o usuário deve clicar com o botão do mouse no botão Editar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está alterando.

Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando as novas cotas do usuário.

Criando Novo Grupo
------------------

O conceito de Grupos criado unicamente para a Plataforma do uCloud,  não existe nada semelhante em qualquer provedor de recursos computacionais de nuvem (público e/ou privado).
Para a Plataforma do uCloud um “Grupo” tem duas atribuições básicas que são:

#. Permite organizar usuários de forma a identificar um departamento, um centro de custo, uma iniciativa, apenas para citar alguns pontos.
#. Pode estabelecer um limite (cotas de recursos ou financeiro) para os usuários vinculados ao grupo, de como será possível consumir os recursos computacionais de nuvem (público e/ou privado).

Para criar um grupo é preciso provisionar, previamente, um Contrato na Plataforma do uCloud, e vincular o grupo a um contrato existente.
Importante ressaltar que somente os usuários com perfil de Administrador de Contrato, ou Administrador de Grupo estão habilitados para provisionar um grupo na Plataforma do uCloud.
Abaixo se apresenta a tela para provisionar um grupo na Plataforma do uCloud;

.. figure:: /figuras/uCloud_menu_grupo_011.png
   :alt: menu de grupo
   :align: center

----

* **Nome**: *Este campo é obrigatório* e deve ser preenchido com o nome do grupo.
* **Contrato**: *Este campo é obrigatório* e deve ser informado o nome do contrato, ao qual o grupo está vinculado. Pode-se informar parte do nome de um contrato e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo.

.. figure:: /figuras/uCloud_menu_grupo_012.png
   :alt: menu de grupo
   :align: center

----

Serão listados apenas os contratos aos quais o perfil do usuário tem a permissão de visualizar. Assim que selecionado o grupo ficará vinculado ao contrato.

Assim que um contrato é selecionado, a Plataforma do uCloud apresenta, na coluna à direita desta tela, o grupo de Permissões que foram definidas no Contrato.

.. figure:: /figuras/uCloud_menu_grupo_013.png
   :alt: menu de grupo
   :align: center

----

Todos os usuários que pertencem ao grupo recebem as mesmas permissões. Existem duas formas diferentes que podem ser utilizadas neste momento para repassar as permissões do contrato para o grupo.

  * **Utilizar as permissões padrões**: Esta opção engloba um conjunto padrão de permissões para o grupo, assim todos os usuários herdam este grupo de permissões padrão.
  * **Definir manualmente as permissões**: Ao lado de cada linha de permissão existe um campo do tipo “check box”, ao ser selecionado, adiciona a respectiva permissão ao grupo e aos usuários pertencentes a este grupo. Este processo é detalhado, pois existem mais de cento e sessenta permissões na Plataforma do uCloud. Se o “check box” existente no topo da tabela for selecionado, significa marcar todas as permissões de uma única vez.
  * **Apenas permissões de leitura**: Este campo é do tipo “radio button” ao ser selecionado configura que este grupo (e os usuários que o compõem) estão restritos a visualizar as informações do ambiente de nuvem. Os usuários vinculados a este grupo não possuem permissão de criação e/ou modificação de qualquer recurso computacional nos provedores de nuvem (público e/ou privado).

* **Cota de IPs Públicos**: Este campo é obrigatório e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo de Endereços TCP-IP Públicos que poderão ser consumidos por todos os usuários do grupo.
* **Cota de CPU**: Este campo é obrigatório e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais das CPUs que poderão ser consumidos por todos os usuários do grupo.
* **Cota de Memória**: Este campo é obrigatório e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais de Memória que poderão ser consumidos por todos os usuários do grupo. Pode ser selecionado o limite em Megabytes ou em Gigabytes.
* **Cota do Disco**: Este campo é obrigatório e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais de Disco de Armazenamento que poderá ser consumido por todos os usuários do grupo. Pode ser selecionado o limite em Gigabytes, Megabytes ou em Terabytes.
* **Botão Criar**: Após preencher todos os campos obrigatórios e opcionais para provisionar o novo grupo, o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma do uCloud provisione o novo grupo em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório foi deixado sem preenchimento.

Após o usuário confirmar a ação de criar um grupo, a Plataforma do uCloud encerra a tela anterior e retorna para a tela com a lista de grupos e o grupo recém criado se apresenta nesta lista.

Administração / Contrato
------------------------

Uma grande vantagem para as empresas quando adotam a Plataforma do uCloud é o controle e monitoração da Governança de Custos e de Recursos Computacionais.

Permitir a governança de custos em ambientes híbridos de multi-nuvem (público e/ou privado) facilita as empresas a manterem os limites definidos dos seus investimentos (orçamento) dentro dos objetivos de negócio das organizações usuárias da Plataforma do uCloud.

O Contrato é o ponto principal onde a organização usuária do uCloud estabelece a forma como gerencia os aspectos comerciais, os limites financeiros (ou dos recursos computacionais), define seus valores para recursos computacionais de forma individualizada (válido somente para uma nuvem privada), vincula os grupos e os usuários.

Quando os valores dos recursos computacionais de nuvens públicas são totalizados em outras moedas, no contrato se estabelece a forma da conversão da moeda estrangeira para a moeda local (e o valor de conversão é fixo ou variável) e as taxas de impostos aplicadas aos custos do contrato.

No contrato, a organização pode estabelecer a data inicial e sua expiração (prazo do contrato). Ao estabelecer a data do prazo do contrato, a organização poderá definir se os recursos computacionais existentes no provedor de nuvem pública, deverão ser removidos definitivamente de forma manual (um a um) ou de forma automática (remoção de todos os recursos automaticamente).

A maneira de configurar um contrato pode variar de organização para organização, por isso, abaixo estão listados alguns exemplos de configuração:

#. Um contrato pode abranger mais de um provedor de nuvem: desta forma todos os provedores serão controlados dentro dos mesmos padrões do contrato. Esta modalidade é muito útil quando os custos são fixos e não existe negociação dos valores de recursos computacionais. Desta forma, os custos estão centralizados em um único ponto.

#. Um contrato pode estar vinculado a apenas um provedor de nuvem: desta forma o contrato limita os custos de forma mais granular e permite criar grupos que consumam apenas recursos computacionais deste provedor. Desta forma, todos os custos de um único provedor estão centralizados em um único ponto.

#. Dois contratos podem estar vinculados a um mesmo provedor de nuvem: esta forma é a mais indicada quando a organização e o provedor de nuvem renegociam os custos dos recursos computacionais. Como existem dois momentos diferentes (custos anteriores à renegociação e custos após a renegociação) e cada contrato reflete as margens e valores dos diferentes períodos de cada negociação. Desta forma, os custos de cada momento da negociação estão centralizados em um único ponto.

#. Um contrato para cada filial fiscal (CNPJ) da empresa: desta forma é possível efetuar a governança de custos de cada unidade fiscal da organização, caso cada uma destas filiais tenham liberdade de contratação de provedores de nuvem de forma individual. Desta forma, os custos de cada filial terá a sua própria governança de custos de serviços de computação em nuvem (público e/ou privado).

O contrato é o primeiro item a ser provisionado na Plataforma do uCloud, logo após o item grupos deste contrato e, depois, provisionar os usuários vinculados a cada grupo. Somente um usuário com perfil de Administrador da Plataforma tem permissão de provisionar um novo contrato. Veja o documento Manual do Administrador da Plataforma do uCloud para entender como provisionar um contrato.

Este documento não cobre o procedimento do processo de provisionar um novo contrato.

Somente usuários com perfil de Administrador de Contrato têm a permissão de visualizar esta lista de contratos da empresa. Este usuário terá acesso apenas aos contratos os quais o seu login de usuário está vinculado no campo de Administrador de Contrato:

.. figure:: /figuras/ucloud_menu_contrato_001.png
   :alt: menu de contrato
   :align: center

----

Abaixo seguem descritas as colunas apresentadas nesta tabela:

* **Nome**: Esta coluna apresenta o nome do contrato da forma como está provisionado na Plataforma do uCloud.

* **Admin**: Esta coluna apresenta as credenciais do usuário como está associado ao campo: Administrador do Contrato. Qualquer usuário (simples) pode ser associado a este campo, após esta ação o usuário fica associado ao perfil de Administrador de Contrato.

* **CPF/CNPJ**: Esta coluna apresenta o conteúdo da identificação fiscal brasileira que pode corresponder a uma identificação de pessoa física (CPF) ou identificação fiscal de pessoa jurídica (CNPJ).

* **Estado**: Esta coluna apresenta o estado deste contrato na Plataforma do uCloud, onde a situação do contrato pode ser uma das três opções abaixo:

  * **Em Produção**: Indica que o contrato está ativo e todos os recursos computacionais estão ativos e funcionais no provedor de serviço de nuvem; o campo Experimental (no formulário do Contrato) o seu estado está indicado como “Desabilitado”.
  * **Expirado**: Esta opção determina que os recursos computacionais devem continuar existindo no provedor de serviço de nuvem (incorrendo o custo, mesmo sem uso). Esta opção depende da data informada no campo Prazo do Contrato.
  * **Cleaned/Limpo**: Esta opção determina que no caso do contrato se encontrar encerrado, por atingir/ultrapassar a data definida no Prazo do Contrato. Todos os seus recursos de nuvem serão expurgados (removidos) automaticamente dos ambientes dos provedores de serviço.
  * **Manual**: Esta opção determina que no caso do contrato se encontrar encerrado, ultrapassou a data definida no Prazo do Contrato, todos seus recursos de nuvem deverão ser expurgados (removidos) manualmente dos ambientes dos provedores de serviço.

Governança Financeira via Contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Através do uso inteligente da associação dos Grupos e Usuários de Grupos, a Plataforma do uCloud possibilita algumas formas de permitir (ou limitar) o isolamento financeiro e lógico dos recursos computacionais do provedor, utilizados em diferentes projetos, de modo a não haver interferência entre projetos, centros de custos, filiais, iniciativas ou departamentos.

Abaixo estão descritas as duas formas simples de isolamento financeiro que advém do correto provisionamento de Contrato e a vinculação de Grupos e de Usuários ao contrato.

Isolamento Financeiro de Recursos Computacionais
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A Plataforma uCloud estabelece o conceito de Grupo que permite a alocação de uma determinada quantidade de recursos computacionais, ou valores financeiros, os quais podem ser consumidos por todos os usuários que estão vinculados ao Grupo, assim é criada uma pequena ‘célula’ de governança financeira. A Plataforma do uCloud pode conter diversos Grupos, deste modo, a governança financeira fica mais próxima do cenário real da organização.

Importante ressaltar que o conceito de ''Grupos" permanece somente para a Plataforma do uCloud e nada similar existe nos provedores de serviço de nuvem pública ou privada.

Um Grupo que contém usuários, pode ser um Departamento, uma Unidade de Negócio, um Centro de Custos, uma Filial. Quando se define um limite de quantidade de recursos computacionais ou um limite financeiro a um grupo, significa que a Plataforma do uCloud nega (bloqueia) a criação ou alteração de um recurso computacional, se este ultrapassar os limites estabelecidos para o grupo, por qualquer usuário vinculado a este grupo - Uma vez definido o limite de recurso do grupo, este novo recurso computacional não pode ultrapassar estes limites.

Estes limites podem ser ajustados a qualquer momento (aumento ou redução) e apenas os usuários com perfil de Administrador de Grupo ou Administrador de Contrato estão habilitados para alterar estes valores limites (cotas) estabelecidos no grupo. A funcionalidade de Cotas de Grupo é uma forma de se configurar um isolamento lógico financeiro.

Isolamento Lógico de Recursos Computacionais
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A Plataforma do uCloud implementa um conceito de Virtual Data Center (VDC), que permite à organização definir um conjunto lógico que seja apenas uma pequena parte (subgrupo) da ampla quantidade dos recursos computacionais de um provedor de nuvem. O conceito de um Virtual Data Center é exclusivo do ambiente da Plataforma do uCloud, não existe nenhum conceito similar (ou próximo) nos ambientes dos provedores de serviço de nuvem.

Quando a organização define um VDC, este fica vinculado a um Contrato, logo somente os recursos do provedor de serviços de nuvem deste contrato serão disponibilizados para sua correta personalização. 

Como mencionado acima, um Grupo de Usuários faz parte de um contrato, e o grupo de usuários pode ser vinculado no mínimo a um (01) único VDC. Desta forma, os usuários do grupo serão apresentados somente ao subconjunto de recursos computacionais específicos do VDC vinculado ao seu grupo.

O que significa um subgrupo de recursos computacionais. Se, por exemplo, um provedor de serviço de nuvem possui um total de sessenta (60) tipos de configuração de hardware (flavor), a organização seleciona deste total apenas doze (12).

O usuário pode restringir, para a configuração lógica o VDC, selecionar os componentes do ambiente do provedor de nuvem, apenas os itens do provedor que sejam importantes e relevantes para o Grupo de Usuários ao qual o VCD está vinculado. Desta forma, será provisionado um Agrupamento Lógico de recursos computacionais.

No menu Financeiro, quando o usuário com perfil de Administrador de Grupo tem acesso ao resumo financeiro do Grupo de Usuários, este Administrador pode visualizar o consumo dos recursos computacionais, e seus respectivos valores, totalizados unicamente para o Grupo de Usuários, portanto, esta forma de visualização de custos de recursos computacionais de um Grupo de Usuários, permite estabelecer um Agrupamento Lógico de recursos computacionais com seus custos associados ao Grupo de Usuários específico.

Um usuário, sem perfil de Administrador  de Contrato ou Grupo, pode visualizar a relação completa de recursos computacionais em nuvem de toda a organização, entretanto, um usuário de outro grupo não tem como operar (start, stop, reboot, delete, outros) um recurso computacional associado a outro usuário vinculado a um Grupo de Usuários diferente ao qual está originalmente associado.


Visualizando Contrato
---------------------

A Tela de visualização de contrato é a uma das mais extensas telas da Plataforma uCloud e com a quantidade de dezesseis (16) seções (cards). Para simplificar a descrição, cada seção será apresentada de forma individualizada. Abaixo segue um exemplo da tela inicial e descrição de cada seção (card) em separado.

.. figure:: /figuras/ucloud_menu_contrato_002.png
   :alt: menu de contrato
   :align: center

----

Seção Geral
-----------

Quando um contrato é provisionado no sistema, o usuário com perfil de Administrador informa os dados cadastrais básicos da organização, informações gerais para um contrato, tais como Identificação do contrato, nome da empresa, o código CNPJ para empresas (ou CPF no caso de pessoa física), a forma padrão de faturamento das máquinas deste contrato (este padrão de faturamento fica válido somente no caso de não existir regras de bilhetagem no restante do contrato).

.. figure:: /figuras/ucloud_menu_contrato_003.png
   :alt: menu de contrato
   :align: center

----

Deve ser informadas as credenciais de login de um usuário no campo Administrador, neste momento este usuário (simples) fica associado ao perfil de Administrador do Contrato. Veja a seção (card) abaixo:

Abaixo detalhamento dos campos não mencionados;

* **Public Gateway**: Este botão é válido apenas para ambientes em que o contrato está associado a um ambiente de um Data Center privado, no qual o ambiente de virtualização (hypervisor) é de controle da organização (on-premises). Para que este botão seja válido é necessário ao usuário, com perfil de Administrador da Plataforma uCloud, ter provisionado um Gateway SDN (Software Defined Network). Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração de um Gateway SDN.
* **Experimental**: Durante o provisionamento do contrato o Administrador do Contrato informa os limites (cotas) financeiros e/ou dos recursos computacionais. Em seguida, pode-se acessar a configuração de contrato Experimental. 

Através desta configuração é possível estabelecer a data de validade (expiração) do contrato, bem como um limite percentual, que ao ser atingido envia uma mensagem de ‘alerta’ de custo do contrato ou de consumo dos recursos computacionais. Adicionalmente, o usuário pode definir para quem o e-mail de alerta deve ser enviado (Administrador da Plataforma, Administrador do Contrato ou todos os usuários vinculados ao contrato). Veja o exemplo na tela abaixo;

.. figure:: /figuras/ucloud_menu_contrato_004.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração do campo Experimental.

Seção Regras de Faturamento
---------------------------

Nesta seção o Administrador do Contrato pode personalizar as regras de como os valores dos custos do contrato podem ser convertidos para moeda local, também personaliza, se para o cálculo de conversão de moeda aplicará no fator de conversão: um valor fixo ou um valor variável. Para o valor variável, a Plataforma do uCloud está configurada para obter a taxa do valor de conversão diretamente do site do Banco Central do Brasil, local onde pode extrair a taxa PTAX do último dia útil do mês. 

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração do campo Experimental.

.. figure:: /figuras/ucloud_menu_contrato_005.png
   :alt: menu de contrato
   :align: center

----

#. Quantidade de Casas Decimais: Este campo define a quantidade de casas decimais e é muito útil quando o Contrato possui valor em moeda estrangeira.
#. Perfil de Tagueamento: Ver opção de Menu Configurações / Tagueamento de Recursos USN.

Seção Categorias de Preço
-------------------------

Nesta seção é possível provisionar as categorias de preço utilizadas para agrupar os preços do contrato, quando este contrato está associado a uma empresa do Governo municipal, estadual ou federal em que os valores a serem apresentados referente ao consumo dos recursos computacionais de nuvem deverão ser convertidos para a métrica de Unidade de Serviço de Nuvem (USN).

A Unidade de Serviço de Nuvem (USN) é um modelo de precificação dos serviços, divididos em categorias: os serviços de IaaS, PaaS e serviços técnicos. Visa estabelecer-se como método previsível, linear e flexível para obtenção de uma quantidade objetivamente definida a ser cobrada pelos serviços de computação em nuvem. A métrica de USN consiste no estabelecimento de um valor de referência específico para cada tipo de serviço de nuvem, conforme métrica individual associada ao consumo dos recursos.

.. figure:: /figuras/ucloud_menu_contrato_021.png
   :alt: menu de contrato
   :align: center

----

Conforme mencionado, o Administrador do Contrato, deverá efetuar o provisionamento de Categorias de Preço somente no caso deste contrato controlar algum órgão do Governo Brasileiro no âmbito municipal, estadual ou federal, única e somente este deve ser regido pela métrica de USN.
Importante ressaltar que se deve ignorar provisionar qualquer Categorias de Preço quando o seu contrato for controlar os recursos computacionais de nuvem de uma organização privada.


Seção Políticas de Alertas
--------------------------

A Plataforma do uCloud possibilita, ao usuário com perfil de Administrador do Contrato, definir Políticas de Alertas de consumo individual de recursos computacionais de nuvem. Quando a condição da regra for atingida a Plataforma do uCloud envia um e-mail para o Administrador de Contrato. Veja o exemplo da tela abaixo:

.. figure:: /figuras/ucloud_menu_contrato_006.png
   :alt: menu de contrato
   :align: center

----

Abaixo descrevemos as colunas desta seção da tela de contratos:

* **Nome**: Esta coluna apresenta o nome de identificação da política de alerta definido durante seu provisionamento.

* **Recurso**: Essa coluna apresenta o tipo de recurso definido para que a Plataforma do uCloud monitore o consumo.

* **Política**: Essa coluna apresenta a forma definida que estabelece o limite do alerta.

* **Valor**: Essa coluna apresenta o valor de limite superior definido para que a Plataforma do uCloud possa comparar e enviar o alerta para o usuário Administrador do Contrato.

* **Ações**: Esta coluna apresenta dois ícones para que o usuário possa interagir com a política definida:

* **Botão Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud remova esta Política de Alarme de forma imediata e definitiva.

* **Botão Habilitar/Desabilitar** |icone_habil_verde|/|icone_desb_verm|: Este botão é um tipo “checkbox” que o usuário pode atuar para alternar o seu modo atual. A cor verde indica que a política está HABILITADA. A cor vermelha indica que a política está DESABILITADA.

Para alternar entre os estados basta clicar com o cursor do mouse e o campo será ativado, apresentando a cor verde. Se estiver na cor verde, basta clicar com o mouse e o campo será desativado, apresentando a cor vermelha.

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração de uma Política de Alerta.

Seção Preço dos Recursos - Contrato
-----------------------------------

Esta seção permite que o Administrador do Contrato possa redefinir os valores dos recursos que estão sendo consumidos dentro deste contrato. Através desta tela é possível definir preços diferentes para os recursos cobrados pelo provedor de serviço de nuvem. Estes novos valores devem ser informados manual e individualmente, não sendo necessário que todos sejam informados.
Apenas os valores dos recursos que foram informados serão recalculados pela Plataforma do uCloud, apresentados nos relatórios do menu Financeiro.
Os recursos com valor igual a zero (0), terão o seu valor original cobrado pelo provedor de serviço de nuvem sem ser recalculado.

.. figure:: /figuras/ucloud_menu_contrato_007.png
   :alt: figura da interface
   :align: center

----

Recomendamos fortemente que, qualquer alteração nos Valores dos Recursos altere os valores originalmente cobrados pelo provedor de serviços de nuvem.

..  attention::
	*Lembramos ao usuário: ao informar qualquer novo valor, este ‘novo valor’ altera o valor da fatura mensal a ser cobrada pelo provedor, e qualquer diferença, multa ou penalidade contratual advindas destas alterações não são responsabilidade da Ustore ou da Plataforma do uCloud, pois a plataforma está desempenhando o função pela qual foi desenhada a efetuar.*
	
Seção Cota do Contrato
----------------------

A tela abaixo apresenta um exemplo da seção (card) de um contrato, o contrato apresenta os limites financeiros e os limites definidos para a quantidade dos recursos definidos para o contrato, pela organização.

.. figure:: /figuras/ucloud_menu_contrato_007.png
   :alt: figura da interface
   :align: center

----

Abaixo segue o detalhamento dos valores da tela acima:
* **Cota de Faturamento / Alocada**: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite financeiro (cota) do contrato. O primeiro número é a definição do limite superior do contrato, e o segundo número, representa o valor que já foi “alocado” para um (ou vários) grupo(s) que estão vinculados a este contrato. Neste exemplo: o contrato tem um limite de cem mil reais (R$100.000,00) e foi alocado para um (ou mais) grupo(s) um montante de três mil reais (R$3.000,00). O valor informado aqui é uma referência, não impede qualquer usuário na criação de novos recursos computacionais ultrapassar este valor *quando esta criação seja efetuada diretamente via console do provedor de nuvem pública/privada*. O número informado aqui, será utilizado como base de referência para a definição de “Alerta de Consumo” conforme descrito na seção acima.

.. important:: |importante| *Outros grupos que venham a ser criados não podem ter locado valor acima deste limite financeiro.*

* **Cota de IPs Públicos / Alocada**: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite numérico (cota) da quantidade de recurso de Endereços TCP-IP do contrato. O primeiro número é a definição do limite superior do contrato, e o segundo número, representa o valor que já foi “alocado” para um (ou vários) grupo(s) que estão vinculados a este contrato. Neste exemplo: o contrato tem um limite de duzentos (200) recursos e já foi alocado para um (ou mais) grupo(s) um total de dez (10) Endereços TCP-IP.

* **Cota de CPU / Alocada**: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite numérico (cota) da quantidade de recurso de CPUs do contrato. Neste exemplo: o contrato tem um limite de trezentos e sessenta (360) CPUs e já foram alocadas para um (ou mais) grupo(s) um total de duzentas (200) CPUs.

* **Cota de Memória / Alocada**: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite numérico (cota) da quantidade de recurso de Memória do contrato. Neste exemplo: o contrato tem um limite de seiscentos e dez Gigabytes (610GB) e já foram alocadas para um (ou mais) grupo(s) um total de quinhentos Gigabytes (500GB).

* **Cota do Disco / Alocada**: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite numérico (cota) da quantidade de recurso de espaço em disco para armazenamento do contrato. Neste exemplo: o contrato tem um limite de cinquenta (50) Terabytes e já foram alocadas para um (ou mais) grupo(s) um total de trinta e nove (39) Terabytes.

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração de Cotas do Contrato.

Seção Contato Primário
----------------------

Esta seção possibilita ao Administrador do Contrato informar os dados de contato de um responsável Financeiro, Fiscal ou Contábil referente a este contrato.

.. figure:: /figuras/ucloud_menu_contrato_009.png
   :alt: menu de contrato
   :align: center

----

Esta seção não é obrigatória, e o não preenchimento desta seção não impede, ou bloqueia, nenhuma funcionalidade do perfeito uso da Plataforma do uCloud. 
Recomendamos o preenchimento destas informações para que a Plataforma do uCloud possa enviar informações automaticamente para o gestor do contrato.


Seção Administradores
---------------------

Esta seção apresenta a relação de usuários (e/ou Grupos de Usuários), que possuem permissão de alterar qualquer um dos dados que compõem um contrato.

.. figure:: /figuras/ucloud_menu_contrato_010.png
   :alt: menu de contrato
   :align: center

----

Seção Dados da Empresa
----------------------

Esta seção possibilita ao Administrador do Contrato informar os dados genéricos da empresa associada a este contrato.

.. figure:: /figuras/ucloud_menu_contrato_009.png
   :alt: menu de contrato
   :align: center

----

Esta seção não é obrigatória. No caso desta seção deixar de ser preenchida, isto não impede ou bloqueia as funcionalidades e o perfeito uso da Plataforma do uCloud.

Seção Virtual Datacenters Concedidos
------------------------------------

Nesta seção o usuário Administrador do Contrato vincula o Virtual Data Center (VDC) ao contrato. Esta é uma das alternativas de Governança de Custos permitida pela Plataforma do uCloud – veja mais informações acima no item Administração de Contrato na página 58.
Quando ocorre a vinculação de um VDC a um contrato, significa que o usuário administrador do contrato estabelece para a Plataforma do uCloud a concessão deste VDC ao contrato. Assim, para o usuário - com permissão de administrador do contrato - serão listados apenas os VDCs deste contrato. Em outras palavras, todas as telas da Plataforma do uCloud onde um VDC pode ser ofertado (solicitado) ao usuário selecionar, o usuário pode visualizar/solicitar apenas os VDCs listados nesta seção.

.. figure:: /figuras/ucloud_menu_contrato_011.png
   :alt: menu de contrato
   :align: center

----

Favor consultar *uCloud - Manual do Administrador*, para conhecer os procedimentos de como vincular um VDC a um contrato.

Seção Usuários
--------------

Nesta seção (card) estão listados todos os usuários que estão vinculados, indiretamente, ao contrato. A associação do usuário ao contrato é estabelecida, pela inclusão do usuário a um Grupo e a vinculação do Grupo ao Contrato. Desta forma, o usuário fica vinculado a um contrato, ele compartilha e consome os limites financeiros e os limites (cotas) dos recursos computacionais de nuvem.
Nesta seção é possível verificar as cotas de cada usuário e o consumo dos recursos até o presente momento.

.. figure:: /figuras/ucloud_menu_contrato_012.png
   :alt: menu de contrato
   :align: center

----

Seção Grupos
------------

Esta seção apresenta todos os Grupos vinculados ao Contrato. A Plataforma do uCloud mostra ou lista as cotas que foram alocadas para cada Grupo vinculado ao Contrato. É possível verificar as cotas de cada grupo e o consumo dos recursos, dentro do grupo, até o momento da pesquisa.

.. figure:: /figuras/ucloud_menu_contrato_013.png
   :alt: menu de contrato
   :align: center

----

* **Botão “+Adicionar Grupo Existente”** |botao_adiciona_grp|: Através deste botão, o usuário com perfil de Administrador de Grupo, poderá vincular um grupo - previamente provisionado na Plataforma do uCloud - ao contrato que se está visualizando. Quando o usuário clicar com o cursor do mouse sobre este botão, será apresentada a seguinte tela;

.. figure:: /figuras/ucloud_menu_contrato_014.png
   :alt: menu de contrato
   :align: center

----

* **Grupo**: Neste campo o usuário precisa informar parte do nome de um grupo existente, como resultado a Plataforma do uCloud apresenta uma lista de todos os grupos que possuem parte dos caracteres informados. Basta o usuário selecionar o grupo desejado, o resultado é apresentado da seguinte forma;

.. figure:: /figuras/ucloud_menu_contrato_015.png
   :alt: menu de contrato
   :align: center

----

   * **Botão Adicionar Grupo** |botao_adiciona|: Neste momento, o usuário deve clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud efetive a vinculação do grupo selecionado ao contrato que se está visualizando.
   * **Botão Ok**: Ao clicar com o cursor do mouse sobre este botão, a Plataforma do uCloud encerra esta tela e retorna à visualização do Contrato, e a relação de grupos vinculados ao contrato, atualizada com o novo grupo.
   * **Botão “+Criar Grupo”** |botao_adiciona_grp|: Através deste botão o usuário, com perfil de Administrador de Grupo, poderá provisionar um novo grupo na Plataforma do uCloud. Mediante este botão, o novo grupo ficará obrigatoriamente vinculado ao contrato que se está visualizando. Veja a descrição de todo o processo de provisionamento de um grupo na Plataforma do uCloud no item Criando Novo Grupo na página 55 .

Seção Dados de Faturamento
--------------------------

Nesta seção são apresentadas as informações de Faturamento de um Contrato. Estas informações, geralmente, são necessárias para integrações automatizadas com sistemas de CRM, showback e chargeback.

.. figure:: /figuras/ucloud_menu_contrato_016.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos para informar os dados de Faturamento do Contrato.

Seção Perfis de Permissionamento
--------------------------------

Esta seção (card) se aplica ao usuário Administrador da Plataforma uCloud (perfil diferente do Administrador do Contrato), que tiver provisionado antecipadamente Perfis de Permissões através do menu Configurações / Perfis de Permissionamento. Somente um usuário com o perfil Administrador da Plataforma é responsável pela gerência de todos e dos demais grupos e permissões.
Quando um Perfil de Permissionamento é vinculado ao Contrato, isto implica que todos seus Grupos e Usuários recebem as mesmas permissões para acessar os menus da plataforma definidas neste perfil, de forma a permitir aos usuários vinculados a este contrato acesso às funcionalidades da Plataforma do uCloud definidas neste perfil de permissionamento.

.. figure:: /figuras/ucloud_menu_contrato_017.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como provisionar um Perfil de Permissionamento e vincular um VDC a um contrato.

Seção Produtos
--------------
Um produto pode ser visto como recurso, um software, o valor de uma licença específica, um serviço recorrente ou qualquer coisa que se seja necessário incluir em um Contrato. Importante ressaltar que o produto sempre será algo que não existe ou que não pode ser criado e gerenciado pela Plataforma do uCloud, diretamente no console dos provedores de nuvem pública e/ou privada. É indicado configurar um Produto quando a oferta é o Virtual Data Center como um todo, no caso de serviços, ofertas específicas para máquinas virtuais, é recomendado optar pelas assinaturas.

.. figure:: /figuras/ucloud_menu_contrato_018.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como adicionar um Produto a um contrato.

Seção Permissões Concedidas
---------------------------

Esta seção (card) permite personalizar as permissões concedidas aos usuários com acesso às funcionalidades na Plataforma do uCloud, de forma global. Estas permissões básicas, definidas e vinculadas ao Contrato, implicam que todos seus Grupos e Usuários recebam as mesmas permissões de acesso às funcionalidades definidas nesta seção. Diferente do Perfil de Permissionamento, esta configuração permite que o usuário com perfil de Administrador de Contrato adicione ou remova, permissões não previstas no Perfil de Permissionamento. Permite também, remover/excluir permissões do Contrato.

.. figure:: /figuras/ucloud_menu_contrato_019.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como provisionar ou excluir Permissões vinculadas a um contrato.

Seção Perfil de Faturamento de Container
----------------------------------------

Esta seção apresenta todos os dados relacionados ao perfil de faturamento de um contrato por tipo de container a ser utilizado. A Plataforma do uCloud permite vincular um Contrato a um Container. O termo container representa um hypervisor ou conexão com uma nuvem pública, sendo assim é possível que existam perfis de preços distintos de acordo com o container que um usuário possa vincular a um contrato. 
Através desta configuração é possível que sejam definidos preços distintos por perfil de faturamento (preço fixo, recurso alocado ou recurso efetivamente utilizado) por tipo de container.

.. figure:: /figuras/ucloud_menu_contrato_020.png
   :alt: menu de contrato
   :align: center

----

Favor consultar uCloud - Manual do Administrador, para conhecer os procedimentos de como provisionar um contrato.

Provisionando Contrato
----------------------

É relevante ressaltar que não é objetivo deste documento descrever o processo de provisionamento de um contrato, pois apenas os usuários com perfil de Administrador da Plataforma uCloud têm permissão para isto. Veja o documento Manual do Administrador da Plataforma do uCloud onde descrevemos o processo como provisionar um contrato.

Menu Configuração
=================

O menu configuração permite que o usuário com perfil de Administrador da Plataforma defina os parâmetros básicos do sistema. Estes parâmetros serão utilizados em várias áreas e outros menus da Plataforma do uCloud de forma global.
A Plataforma do uCloud é um ambiente, por definição, multi-empresas (multi tenant). Portanto, todos os parâmetros definidos impactam todas as empresas, seus contratos e todos os usuários de forma global. Este impacto é de responsabilidade do usuário com o perfil de Administrador da Plataforma, que possui o perfeito conhecimento e compreensão de todas as implicações destas configurações globais.
Os submenus descritos a seguir permitem configurações que terão impacto em muitas atividades e rotinas de todos os usuários e empresas provisionados.


Configuração / Geral
--------------------

Esta tela está dividida em seções, por meio destas seções (card) o Administrador da Plataforma, pode definir as cotas (limites) padronizados para serem aplicados a qualquer novo usuário a ser adicionado na plataforma quando consumir/criar recursos computacionais em nuvem (público e/ou privado).

Seção Geral:
~~~~~~~~~~~~

Na seção Geral, os usuários definem as opções de quotas padrão por usuário do sistema, ou seja, ao criar um usuário se ele não tiver sua quota informada o sistema usará as cotas constantes na tela de aplicação.

Abaixo esclarecemos os campos desta seção. Importante ressaltar que somente usuários com perfil de Administrador de Plataforma podem alterar os valores armazenados nestes campos.

* **Botão “Sincronizar Active Directory”**: Este botão permite configurar a integração de um servidor de Active Directory para o ambiente de forma que possa validar, duplamente, as credenciais de usuários provisionados no ambiente de forma global. Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos corretos para configurar a sincronização com um servidor de Active Directory.

* **Botão Ativação Automática “On/Off”**: Este botão tem função de permitir que todos os novos usuários provisionados via o processo descrito no item Criando Novo Usuário na página 41 sejam ativados de forma automática para se registrarem na Plataforma do uCloud.

* **Cota Padrão de CPU**: O conteúdo informado neste campo será utilizado, de forma global, como o padrão de cota de quantidade de recurso computacional CPU. Será válido para todos os usuários. Deve-se informar um número inteiro.

* **Cota Padrão da Memória**: O conteúdo informado neste campo será utilizado, de forma global, como o padrão de cota de quantidade de recurso computacional Memória. Será válido para todos os usuários. Deve-se informar um número inteiro no campo ao lado o Administrador da Plataforma pode selecionar se o limite será em Gigabytes ou em Megabytes.

* **Cota Padrão do Disco**: O conteúdo informado neste campo será utilizado, de forma global, como o padrão de cota de quantidade de recurso computacional no Espaço de Armazenamento de Disco. Será válido para todos os usuários. Deve-se informar um número inteiro no campo ao lado, o Administrador da Plataforma pode selecionar se o limite será em Gigabytes, Megabytes ou em Terabytes.

* **E-mail Administrador**: Neste campo deve constar o endereço do correio eletrônico (e-mail) do Administrador da Plataforma, para que este possa receber mensagens de alerta da Plataforma do uCloud, nas opções em que possuem esta funcionalidade.

* **Valor do Dólar**: Este campo não é obrigatório (pode estar ‘em branco’) e deve constar o valor padrão geral (global) para a conversão da moeda de Dólares Americanos para Reais. Este valor será a referência padrão, caso não exista nenhuma configuração no contrato provisionado. Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos corretos e provisionar um contrato.

* **Valor dos Impostos**: Este campo não é obrigatório (pode estar ‘em branco’) nele deve constar o valor padrão geral (global) referente a Taxa de Impostos a ser aplicada sobre os valores das Faturas no menu Financeiro. Este valor será a referência padrão, caso não exista nenhuma configuração no contrato provisionado. Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos corretos para provisionar um contrato.

* **Valor da meta mensal**: Este campo não é obrigatório (pode estar ‘em branco’) e deve constar o valor padrão geral (global) da meta mensal de consumo de recursos financeiros. Este valor será a referência padrão, caso não exista nenhuma configuração no contrato provisionado.

.. important:: |importante| Importante ressaltar que no caso deste valor ser informado, poderão ser enviadas mensagens de alerta para o Administrador da Plataforma, porque houve um consumo financeiro mensal global acima deste valor estabelecido. Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos corretos para provisionar um contrato.

Solicite acesso ao documento Manual do Administrador da Plataforma do uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma do uCloud.


Seção Preço dos Recursos
~~~~~~~~~~~~~~~~~~~~~~~~

A seção Preço dos Recursos permite definir os preços por hora de consumo para CPU, Memória e Disco, os valores cobrados por taxa de transferência e por recursos de rede.

Solicite acesso ao documento Manual do Administrador da Plataforma do uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma do uCloud.

Seção Configurações de Usuários LDAP Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta seção permite que o Administrador da Plataforma selecione quais usuários provisionados na Plataforma do uCloud devem ter suas credenciais sincronizadas com o servidor de LDAP/AD configurado no botão “Sincronizar Active Directory” da seção Geral.

Solicite acesso ao documento Manual do Administrador da Plataforma do uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma do uCloud.

Menu Configuração / Rede
========================

A seção Configuração da Rede, indica a listagem do controlador SDN e as opções de configuração do uCloud. O qual permite o uso de vários controladores SDN transferindo assim mais escalabilidade para o sistema.

* O que é SDN?

  * A **SDN** (Rede Definida por Software – *Software Defined Network*) é uma abordagem de arquitetura de rede que permite controlar ou "programar" a rede de maneira central e inteligente usando aplicativos de software. Ela ajuda as empresas a gerenciar toda a rede de modo consistente e holístico, seja qual for o fornecedor de equipamentos de rede.

* Para acompanhar o ritmo, o mundo está adotando a tecnologia de SDN para revolucionar o design e as operações de rede.
* A SDN permite o gerenciamento consistente da rede, que pode ser constituída por peças de tecnologia complexas.

A Ustore possui em seu portfólio o produto uSDN para complementar ambientes de data center privado (on-premises) para transformar o ambiente privado de forma a simplificar a configuração de parâmetros de rede de dados através da interface da Plataforma do uCloud.

.. important:: |importante| Importante ressaltar que a configuração das telas abaixo somente será necessária quando a Plataforma do uCloud estiver configurada para o controle e o gerenciamento dos recursos computacionais em um data center privado. Para o gerenciamento e controle dos recursos computacionais de nuvem pública, as telas abaixo não demandam configuração e podem ser ignoradas.

A Ustore possui em seu portfólio o produto uSDN para complementar ambientes de data center privado (on-premises) para transformar o ambiente privado de forma a simplificar a configuração de parâmetros de rede de dados através da interface da Plataforma do uCloud.
Importante ressaltar que a configuração das telas abaixo somente será necessária quando a Plataforma do uCloud estiver configurada para o controle e o gerenciamento dos recursos computacionais em um data center privado. Para o gerenciamento e controle dos recursos computacionais de nuvem pública, as telas abaixo não demandam configuração e podem ser ignoradas.

Seção Configurações de Rede
---------------------------

Nesta tela são provisionadas as configurações de rede (de forma geral) que serão enviadas para o controlador SDN do ambiente do data center privado (on-premises).

* **Range de VLAN Global**: Neste campo deve ser configurada a faixa (range) de endereços TCP-IP da rede privada.

* **CIDR Global**: Neste campo deve ser informado o CIDR, ou endereçamento IP sem classes. Esta configuração de CIDR Global otimiza a distribuição dos endereços IP de 32 bits, permitindo máscaras de rede de qualquer tamanho.

* **Prefixo CIDR do Usuário**: Neste campo devem ser informados os prefixos de endereços TCP-IP específicos da rede corporativa privada da empresa. Podem ser informados CIDRs de todas as classes de endereçamento TCP-IP, por exemplo: 255.0.0.0 (classe A); ou 255.255.0.0 (classe B) ou 255.255.255.0 (classe C), de acordo com a configuração do ambiente de rede da empresa que está sendo configurada na Plataforma do uCloud.

* **Botão Network Sharing**: Este botão permite configurar a opção de que a rede que se está provisionando a configuração seja compartilhada (shared) ou não. Se este botão estiver com a opção “ON” ativa, significa que a configuração de rede será de uma rede que pode ser compartilhada. Se o botão estiver com a opção “OFF” ativa, significa que a configuração de rede será privada e os seus endereços TCP-IP serão privados.

Solicite acesso ao documento Manual do Administrador da Plataforma do uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma do uCloud.

Seção Controlador SDN
---------------------

Quando conectamos um data center privado (on-premises) é necessário instalar uma solução de SDN previamente. Uma vez que o ambiente do servidor de SDN, do cliente, esteja configurado e disponível, o usuário deve selecionar o container no qual ele está associado. O controlador SDN já prevê a existência de dois nós de gerenciamento em alta disponibilidade indicados nos campos primário e secundário. Um controlador não deve estar vinculado a mais de um container.
Importante mencionar que para a instalação do controlador de SDN é necessário consultar a equipe da Ustore, para auxiliar a empresa na correta instalação e configuração do servidor que executará a aplicação uSDN (Controlador SDN).
  
* **IP**: Este campo apresenta o endereço TCP-IP onde está instalado o Controlador SDN, este endereço será utilizado pela API do uCloud que se conecta a este servidor.

* **Porta**: Este campo apresenta a porta TCP-IP na qual a API do uCloud se conecta a este servidor.

* **Interface VLAN**: Este campo apresenta o endereço da interface VLAN, que foi configurado no controlador SDN.

* **Container Virtualizado**: Este campo apresenta o nome do Container (hypervisor) primário, existente no data center privado, que foi configurado para estar vinculado ao Controlador SDN.

* **Container Controlador**: Este campo apresenta o nome do Container (hypervisor) primário, existente no data center privado, que foi configurado para estar vinculado ao Controlador SDN.

* **Ações**: Esta coluna apresenta dois ícones para que o usuário possa interagir com a política definida:

* **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud remova este Controlador SDN de forma imediata e definitiva.

* **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone e a Plataforma do uCloud apresenta uma tela que permite editar as configurações do Servidor de SDN respectivo. Importante mencionar que apenas o usuário com perfil de Administrador de Plataforma, poderá editar os valores informados nesta tela.

Solicite acesso ao documento Manual do Administrador da Plataforma do uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma do uCloud.

Menu Configuração / Sub-Redes Públicas
======================================

Quando a empresa configura um servidor de SDN para controlar as configurações de sua rede privada, são controlados e gerenciados apenas endereços restritos (privados). Estes endereços não podem ser acessados de máquinas que estejam em outras redes.
Para que o controlador SDN possa gerenciar os endereços que poderão ser acessados de forma externa (pública) é fundamental que a equipe de segurança e redes, estabeleça a faixa (range) de endereços que serão públicos e a informação destes endereços seja repassada para o Controlador SDN.
Esta opção de menu permite que sejam criadas faixas (ranges) de endereços TCP-IP que sejam públicos, para quando um recurso computacional da nuvem privada (máquina virtual) necessitar de um endereço público, a Plataforma do uCloud possa interagir com o Gerenciador SDN e vincular um endereço TCP-IP Público para este recurso computacional (máquina virtual). 

* **Nome**: Este campo apresenta o nome da rede que foi escolhido no momento do provisionamento da configuração da rede.

* **CIDR**: Este campo apresenta o CIDR, ou endereçamento IP sem classes, acrescentado com a respectiva definição de bloco de endereços (“/xx”). Esta configuração de CIDR e a quantidade de blocos de endereços, deve ser definida pela equipe de engenharia de redes de dados da empresa.

* **Range start**: Este campo apresenta o endereço TCP-IP inicial da faixa que se deseja disponibilizar.

* **Range end**: Este campo apresenta o endereço TCP-IP final da faixa que se deseja disponibilizar.

* **Gateway**: Este campo apresenta o endereço TCP-IP do Gateway de rede que transfere o tráfego de pacotes da rede local para a outras redes, neste caso a rede externa/pública.

* **Container**: Este campo apresenta o nome do container o qual este Controlador SDN está conectado, para controlar e gerenciar as atribuições de endereçamentos TCP-IP.

* **Ignored Address**: Este campo apresenta a lista de endereços TCP-IP, definidos pela equipe de rede da empresa, a ser ignorado e evitado, para serem assinalados a recursos computacionais. Os endereços apresentados nesta lista estão separados por vírgula.

* **Ações**: Esta coluna apresenta apenas o Ícone Lata de Lixo |icone_lixo|. Basta clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud remova a configuração de Sub-Rede Pública de forma imediata e definitiva. Importante ressaltar que a Plataforma do uCloud não solicita confirmação desta remoção para o usuário, a ação de remoção é imediata e irreversível. Se a ação não foi intencional, o usuário deverá iniciar o processo de configuração da Sub-Rede Pública novamente desde seu início.

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como provisionar corretamente o Controlador SDN dentro do ambiente de rede privada.

Solicite acesso ao documento Manual do Administrador da Plataforma do uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma do uCloud.

Menu Configuração / Assinaturas
===============================

Assinaturas são serviços vinculados a uma máquina virtual. As assinaturas têm que conter apenas as ofertas de serviços que devem ser cobrados mensalmente ou mês específico. No caso da remoção de uma assinatura vinculada a uma máquina virtual, o valor será cobrado integralmente pelo agente de bilhetagem.
São exemplos de assinaturas: gerenciamento, licenças de sistema operacional e monitoramento, entre outros. A figura abaixo apresenta exemplos de modalidades de assinaturas que uma máquina virtual pode possuir:

* **Nome**: Este campo apresenta o nome informado no momento da sua configuração.

* **Preço**: Este campo apresenta o valor mensal referente ao custo da assinatura, informado no momento de criar a assinatura.

* **Descrição**: Este campo apresenta a descrição estendida da assinatura, que foi informado no momento da sua criação.

* **Ações**: Esta coluna apresenta apenas o Ícone Lata de Lixo. Basta clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud remova a assinatura de forma imediata e definitiva. Importante ressaltar que a Plataforma do uCloud não solicita confirmação desta remoção para o usuário, a ação de remoção é imediata e irreversível.

Criando Assinatura
------------------

O processo de criação de assinatura é muito simples, importante mencionar que as assinaturas devem conter apenas as ofertas de serviços, ou qualquer custo adicional, que serão cobrados mensalmente.

Abaixo a descrição dos campos para o provisionamento de uma nova assinatura:

* **Nome**: Neste campo deve ser informado o nome desejado para identificar a assinatura. Não existe limite máximo para o nome desejado. O limite mínimo de caracteres para informar neste campo é um (01) caractere. Sugerimos utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido).

* **Preço**: Neste campo deve ser informado o valor mensal (número) referente ao custo da assinatura. Se o usuário informar um número inteiro (sem zeros), a Plataforma do uCloud assume somente o valor inteiro, seguido de zeros após a vírgula. Para valores com casas decimais, o usuário deve usar a "vírgula" seguido do valor referente decimal do valor mensal (por ex.: “123,90”).

* **Descrição**: Neste campo o usuário informa uma descrição estendida que pode esclarecer a que se refere esta assinatura, este campo pode contar até duzentos e cinquenta e cinco caracteres (255). O limite mínimo de caracteres a informar neste campo é um (01) caractere. Sugerimos utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido).

* **Botão Criar**: Neste ponto, após preencher e finalizar todos os campos para provisionar uma assinatura, o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma do uCloud provisione a nova assinatura em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório precisa ser preenchido.

Após confirmar a criação da nova assinatura, a Plataforma do uCloud encerra a tela de nova assinatura e retorna a lista atualizada de assinaturas existentes, com a nova assinatura apresentada na relação da tela. Eventualmente, pode existir um atraso para que a Plataforma do uCloud atualize a lista de assinaturas.

Menu Configuração / Flavor Billing Profile
==========================================

Esta opção permite definir o preço padrão por tipo de *flavor* a ser utilizado por qualquer usuário na Plataforma do uCloud, definindo seu custo de CPU, custo de memória e custo do disco.

*Flavor*, é o termo genérico que todos os provedores de serviço de nuvem utilizam para identificar uma combinação de configuração de hardware (CPU, memória e disco). Podemos traduzir o termo *flavor* para **tipos de instâncias**. Cada tipo de *flavor* (instância) inclui um ou mais tamanhos de configurações de hardware e, desta forma, cada *flavor* possui um valor de custo referente ao conjunto dos seus recursos.

Cada provedor tem um custo para cada tipo de *flavor* em sua lista de preços de recursos computacionais, portanto os valores já existem.

A configuração de um *Flavor Billing Profile* é muito útil para os containers de ambientes de data center privado (*hypervisor on-premises*) desta forma é possível aplicar conceitos de custo de recursos computacionais de nuvem pública (*flavors*) para os ambientes de nuvem privada.

Caso seja utilizado um flavor atual (existente) de um provedor de serviço de nuvem pública, o novo valor pode substituir o valor do provedor por um valor provisionado na Plataforma do uCloud definido pelo usuário. Importante ressaltar que esta ação pode criar diversos desdobramentos financeiros na fatura mensal do provedor de serviço de nuvem.

.. image:: /figuras/ucloud_flavor_billing_profile.png
   :alt: Billing Profile
   :align: center

----

* **Botão “Criar Flavor Billing Profile”**: Quando o usuário clicar com o cursor do mouse sobre este botão, a Plataforma do uCloud apresenta a tela para configuração de um novo Flavor Billing Profile. O processo de configuração está descrito abaixo no item: Criando um Flavor Billing Profile na página 89.

* **Nome**: Esta coluna apresenta o nome do Flavor Billing Profile, anteriormente informado no processo de criação.

* **Custo de CPU**: Esta coluna apresenta o valor deste recurso computacional CPU. Este campo pode apresentar um valor igual a “0” (zero), caso este recurso seja controlado por seu valor fixo mensal.

* **Custo de Memória**: Esta coluna apresenta o valor deste recurso computacional Memória. Este campo pode apresentar um valor igual a “0” (zero), caso este recurso seja controlado por seu valor fixo mensal.

* **Custo de Disco**: Esta coluna apresenta o valor deste recurso computacional Disco. Este campo pode apresentar um valor igual a “0” (zero), caso este recurso seja controlado por seu valor fixo mensal.

* **Preço Mensal Fixo**: Esta coluna apresenta o valor definido como um valor total fixo por mês. Este campo pode apresentar um valor igual a “0” (zero), caso este recurso seja definido pela somatória dos custos de CPU, memória e disco.

* **Ações**: Esta coluna apresenta dois ícones para que o usuário possa interagir com a política definida:

* **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud remova o Flavor Billing Profile de forma imediata e definitiva. Importante ressaltar que esta ação não terá solicitação de nenhuma confirmação por parte do usuário, portanto será definitiva.

* **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone e a Plataforma do uCloud apresenta uma tela que permite editar as configurações do respectivo Flavor Billing Profile. Importante mencionar que apenas o usuário com perfil de Administrador de Plataforma, poderá editar os valores informados nesta tela.

Criando um Flavor Billing Profile
---------------------------------

Nesta etapa, será descrito o processo de como definir o valor padrão para um Flavor. Os valores de CPU, Memória e Disco apenas serão aplicados ao alterar a configuração padrão do flavor, principalmente nos casos de adição de discos extras.
Caso seja mais prático é possível configurar um valor de referência que pode ser preenchido no campo “Valor Fixo Mensal”.

Quando o usuário clica com o cursor do mouse no botão “Criar Flavor Billing Profile” a Plataforma do uCloud apresenta a seguinte tela;

.. image:: /figuras/ucloud_criar_billing_profile_001.png
   :alt: Billing Profile
   :align: center

----

* **Flavor**: Este campo é um campo do tipo “Dropdown” e quando o usuário clica com o cursor do mouse a Plataforma do uCloud lista todos os flavors que existem na plataforma:

  * Todos os flavors do provedor de serviço de nuvem pública (importado após a configuração das credenciais de acesso a este provedor),
  * Todos os flavors provisionados para serem utilizados no container do data center privado.

.. image:: /figuras/ucloud_criar_billing_profile_002.png
   :alt: Billing Profile
   :align: center

----

Após o usuário selecionar o flavor desejado, a Plataforma do uCloud altera e retorna a tela conforme o exemplo abaixo:

Para compreensão da imagem acima, segue abaixo a descrição dos campos da tela:

.. image:: /figuras/ucloud_criar_billing_profile_003.png
   :alt: Billing Profile
   :align: center

----

* **Custo de CPU**: Este campo é obrigatório, o usuário deve informar o custo referente a quantidade de recursos de CPU do flavor selecionado no campo inicial. Por ser um campo obrigatório, o usuário deve informar um número inteiro correspondente para o valor mensal deste recurso, ou preencher com “zero (0)”, para os casos em que o flavor tenha um valor fixo mensal.

* **Custo de Disco**: Este campo é obrigatório, o usuário deve informar o custo referente ao recurso de Disco do flavor selecionado no campo inicial. Por ser um campo obrigatório, o usuário deve informar um número inteiro correspondente para o valor mensal deste recurso, ou preencher com “zero (0)”, para os casos em que o flavor tenha um valor fixo mensal.

* **Custo de Memória**: Este campo é obrigatório, o usuário deve informar o custo referente ao recurso de Memória do flavor selecionado no campo inicial. Por ser um campo obrigatório, o usuário deve informar um número inteiro correspondente para o valor mensal deste recurso, ou preencher com “zero (0)”, para os casos em que o flavor tenha um valor fixo mensal.

* **Custo Fixo Mensal**: Este campo é obrigatório, o usuário deve informar o custo referente ao valor mensal do flavor selecionado no campo inicial. Por ser um campo obrigatório, o usuário deve informar um número inteiro correspondente para o valor mensal deste recurso, ou preencher com “zero (0)”, para os casos em que o flavor tenha custos específicos para os recursos de CPU, Memória e Disco.

* **Botão Criar**: Após todos os campos para provisionar Flavor Billing Profile estarem preenchidos o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma do uCloud possa provisionar o Flavor Billing Profile em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório precisa ser preenchido.

Menu Configuração / Perfis de Permissionamento
==============================================

A Plataforma do uCloud possui uma grande diversidade de permissões, precisamente são 154 (cento e cinquenta e quatro) permissões que podem ser associadas a um usuário. Esta tarefa pode ser complexa e talvez consumir uma grande quantidade de tempo do usuário, ao considerar a associação de permissões para cada usuário provisionado na Plataforma do uCloud ou para os novos usuários, no futuro.
Desta forma, para facilitar a associação de permissões existe a facilidade de provisionar perfil que possua um grupo específico de permissões, para acesso às facilidades da Plataforma do uCloud, e assim, vincular o(s) usuário(s) a este determinado perfil.
O Perfil de Permissionamento habilita ou bloqueia o usuário a executar uma determinada funcionalidade da Plataforma do uCloud, através do Menu de Usuário e os Submenus. As funcionalidades podem ser visualizadas ou acessadas, mas, de acordo com o perfil selecionado, o usuário terá permissão ou não de executar tal funcionalidade.
A seguir, um exemplo da tela com a lista de Perfis de Permissionamento:

.. image:: /figuras/ucloud_perfil_permissionamento_001.png
   :alt: Billing Profile
   :align: center

----

Para compreensão da imagem acima, segue abaixo a descrição das colunas:

* **Botão Criar Perfil**: Quando o usuário clicar com o cursor do mouse sobre este botão, a Plataforma do uCloud apresenta a tela para configuração de um novo Perfil de Permissionamento. O processo de configuração está descrito abaixo no item Criar um Perfil, página 95.

* **Nome do Perfil**: Esta coluna apresenta o nome do Perfil de Permissionamento que foi informado no momento da sua criação. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de perfis de permissionamento de forma alfabética crescente (a – z) ou decrescente (z – a) com base no nome do perfil.

* **Descrição**: Esta coluna apresenta a descrição estendida do Perfil de Permissionamento informado no momento da sua criação. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de perfis de permissionamento de forma alfabética crescente (a – z) ou decrescente (z – a) com base na descrição do perfil.

* **Criado Por**: Esta coluna apresenta a identificação da credencial de login do usuário responsável pela criação do Perfil de Permissionamento. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de perfis de permissionamento de forma alfabética crescente (a – z) ou decrescente (z – a) com base nas credenciais de login de usuário.

Visualizar e Editar um Perfil de Permissionamento
-------------------------------------------------
Quando o usuário clica com o cursor do mouse em qualquer linha da tabela a Plataforma do uCloud apresenta a tela de visualização do Perfil de Permissionamento, conforme o exemplo da tela abaixo:

.. image:: /figuras/ucloud_perfil_permissionamento_002.png
   :alt: Billing Profile
   :align: center

----

Esta tela possui um botão de ação e duas seções (cards), descritos a seguir:

* **Botão Excluir** |botao_excluir|: O usuário deve clicar com o cursor do mouse sobre este botão quando for necessário remover um Perfil de Permissionamento previamente provisionado. Ao clicar neste botão, a Plataforma do uCloud apresenta o  seguinte pop-up (imagem abaixo), o usuário responde “sim, pode excluir” e assim confirma a remoção ou “não, cancelar” e desiste de excluir o perfil:

  * **Botão “Não Cancele”**: Basta o usuário clicar sobre este botão (ou teclar “Esc”) para cancelar a ação, na situação de que tenha acidentalmente clicado sobre o botão de exclusão. Quando o usuário cancela a ação de exclusão a Plataforma do uCloud apresenta a seguinte tela:
  * **Botão “Sim Pode Excluir”**: Quando o usuário está seguro da ação de exclusão, basta clicar com o cursor do mouse sobre este botão e a Plataforma do uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que o Perfil de Permissionamento foi excluído da Plataforma do uCloud;

.. image:: /figuras/ucloud_perfil_permissionamento_003.png
   :alt: Billing Profile
   :align: center

----

* **Seção Geral**: Nesta seção são apresentadas informações básicas em relação ao perfil de permissionamento:

  * **Nome**: Neste campo é apresentado o nome (curto) do Perfil de Permissionamento, informado pelo usuário no momento do seu provisionamento. Caso o perfil do usuário, que está acessando esta tela, tenha a permissão de alteração de perfis de permissionamento, o ícone de edição estará ativo.

    * **Ícone de Edição Ativo** |icone_edita_on|: Todos os campos que possuem o ícone de edição ativo são passíveis de alteração do seu conteúdo.
    * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma do uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma do uCloud.
    * **Ícone de Cancelamento** |icone_cancela_vermelho|: No caso do usuário clicar sobre o ícone de edição por engano, ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente. Basta o usuário clicar com o cursor do mouse sobre o ícone vermelho, e assim, cancelar a alteração. O conteúdo do campo retorna aos valores iniciais, antes de qualquer preenchimento ou alteração.

  * **Descrição**: Neste campo é apresentada a descrição (extensa) do Perfil de Permissionamento, informado pelo usuário no momento do provisionamento.

    * **Ícone de Edição Ativo** |icone_edita_on|: Todos os campos que possuem o ícone de edição ativo são passíveis de ter seu conteúdo alterado.
    * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma do uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma do uCloud.
    * **Ícone de Cancelamento** |icone_cancela_vermelho|: Caso o usuário tenha clicado sobre o ícone de edição, por engano, ou no caso de não desejar gravar a alteração permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. A alteração será cancelada e o conteúdo do campo retorna aos valores iniciais, ou seja, antes de qualquer preenchimento ou alteração.

* **Seção Permissões**: Nesta seção da tela são listadas as primeiras vinte e cinco (25) permissões vinculadas a este perfil de permissionamento. Importante relembrar que a Plataforma do uCloud possui mais de cento e cinquenta permissões, as quais são apresentadas com as iniciais de cada permissão.

  * **Mudar a Classificação**: Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica e lista os nomes das permissões em ordem alfabética crescente (a – z) ou decrescente (z – a).
  * **Busca Rápida**: O usuário observa que logo abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista com os nomes das permissões. Basta preencher o campo em branco, com uma sequência de caracteres percebidos como relevantes e a Plataforma do uCloud atualiza a tela de forma a representar este padrão de busca.

    * **Botão Editar** |botao_editar|: Este botão destina-se ao usuário que possuir a permissão de alteração de Perfil de Permissionamento, se ele desejar alterar o conjunto de permissões vinculadas a este perfil, basta clicar com o cursor do mouse sobre este botão e a Plataforma do uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_perfil_permissionamento_005.png
   :alt: perfil de permissionamento
   :align: center

----

      * Esta tela possui duas colunas distintas, à esquerda são as permissões previamente adicionadas ao perfil. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, pode excluir (revogar) a respectiva permissão deste usuário.
      * À direita estão as permissões disponíveis na Plataforma do uCloud que podem ser adicionadas ao perfil. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, adiciona a respectiva permissão deste usuário.
      * “Checkbox” no título da coluna: Ao selecionar este campo “checkbox”, que está presente no título da coluna, ele informa a Plataforma do uCloud a ação de selecionar todas as permissões ainda não vinculadas ao perfil de permissionamento. Desta forma, uma única ação seleciona todas as permissões de uma única vez.
      * **Botão Aplicar**: Após o usuário certificar-se de que todas as alterações necessárias foram configuradas (inclusões ou exclusões), ele deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação a Plataforma do uCloud fecha esta tela e recupera a tela anterior com seu conteúdo atualizado que apresenta a nova relação de permissões deste usuário que se está visualizando ou alterando o perfil.

Criando um Perfil de Permissionamento
-------------------------------------

Ao criar um Perfil de Permissionamento é necessário seguir o processo descrito, importa mencionar que apenas um usuário com permissão de criar perfil é que pode realizar esta ação e executar com êxito.
Para isto, o usuário deve clicar com o cursor do mouse no botão “Criar Perfil” assim a Plataforma do uCloud exibe a tela abaixo;

.. image:: /figuras/ucloud_perfil_permissionamento_007.png
   :alt: perfil de permissionamento
   :align: center

----

* **Nome**: *Este campo é obrigatório*, o usuário deve inserir o nome do Perfil de Permissionamento. O nome do perfil deve ter, no mínimo, três (03) caracteres e o limite máximo de setenta (70) caracteres.

* **Descrição**: *Este campo é obrigatório*, o usuário deve inserir uma descrição estendida do Perfil de Permissionamento. A descrição do perfil deve ter, no mínimo, três (03) caracteres e no máximo cento e vinte (120) caracteres.

* **Permissões**: Nesta coluna são apresentadas todas as permissões disponíveis na Plataforma do uCloud, as quais podem ser vinculadas ao Perfil de Permissionamento que se está a provisionar.

* **Mudar a Classificação**: Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de nomes de permissões de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Busca Rápida**: O usuário pode observar que abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de nomes de permissões. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma do uCloud atualiza a tela de forma a representar este padrão de busca.

* **“Checkbox” no título da coluna**: Ao selecionar este campo “checkbox”, presente no título da coluna, a Plataforma do uCloud atende a ação de selecionar todas as permissões ainda não vinculadas ao perfil de permissionamento. Desta forma, uma única ação seleciona todas as permissões de uma única vez.

* **“Checkbox” de cada Permissão**: Esta coluna apresenta a lista de permissões disponíveis na Plataforma do uCloud. Ao lado de cada permissão existe um campo do tipo “checkbox”, ao ser selecionado, significa que a permissão será vinculada (habilitada) ao Perfil de Permissionamento.

* **Botão Criar**: Após checar se todas as permissões desejadas foram configuradas, o usuário deve clicar com o botão do mouse no botão Criar para configurar as alterações, de forma definitiva e imediata. A Plataforma do uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que o novo Perfil de Permissionamento está cadastrado.

Após esta ação a Plataforma do uCloud fecha a tela e retorna à tela anterior, sendo que o seu conteúdo atualizado apresenta o novo Perfil de Permissionamento, recém provisionado.

Menu Configuração / Perfis de visualização
==========================================

O Perfil de Visualização permite ao usuário *visualizar* as opções do menu de usuário. De certa forma, pode ser complementar ao Perfil de Permissionamento (descrito acima) para criar um controle bem granular do que um usuário pode ou não pode visualizar, das opções da barra de menu apresentadas à esquerda.

.. image:: /figuras/ucloud_perfil_visualizacao_001.png
   :alt: perfil de permissionamento
   :align: center

----

Esta tela possui dois botões em sua parte superior, suas funções, são descritas a seguir.

Criando Perfil de Visualização
------------------------------

Para provisionar um novo perfil de visualização, o usuário deve clicar com o cursor do mouse sobre este botão, assim a Plataforma do uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_perfil_visualizacao_002.png
   :alt: perfil de permissionamento
   :align: center

----

* **Nome**: *Este campo é obrigatório*, o usuário deve inserir o nome do Perfil de Visualização. O nome do perfil deve ter, no mínimo, três (03) caracteres e o limite máximo de setenta (70) caracteres. Importante ressaltar que é recomendado utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido).
* **Descrição**: *Este campo é obrigatório*, o usuário deve inserir uma descrição estendida do Perfil de Visualização. A descrição do perfil deve ter, no mínimo, três (03) caracteres e no máximo, cento e vinte (120) caracteres.
* **Permissões**: Nesta coluna são apresentadas todas as opções de menu disponíveis na Plataforma do uCloud que podem ser vinculadas ao Perfil de Visualização que se está provisionando.
* **Mudar a Classificação**: Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de nomes de opções de menu, de forma alfabética crescente (a – z) ou decrescente (z – a).

  * **Busca Rápida**: O usuário pode observar o campo abaixo do nome da coluna, existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências, nesta lista de nomes de opções de menu. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma do uCloud atualiza a tela e representa este padrão de busca.
  * **“Checkbox” no título da coluna**: Ao selecionar este campo “checkbox” presente no título da coluna, o usuário informa à Plataforma do uCloud a ação de selecionar todas as opções de menu ainda não vinculadas ao perfil de visualização. Desta forma, uma única ação seleciona todas as opções de menu de uma única vez.
  * **“Checkbox” de cada Opção de Menu**: Esta coluna apresenta a lista das opções de menu disponíveis na Plataforma do uCloud. Ao lado de cada opção de menu existe um campo do tipo “checkbox”, selecioná-lo significa que a opção de menu será vinculada (habilitada) ao Perfil de Visualização.
  * **Botão Criar**: Após certificar que todas as opções de menu desejadas foram configuradas, o usuário deve clicar com o botão do mouse no botão Criar para configurar as alterações, de forma definitiva e imediata. A Plataforma do uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que o novo Perfil de Visualização está cadastrado.

Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo atualizado e apresenta o novo Perfil de Visualização recém provisionado.


Editando Perfil de Visualização
-------------------------------

O usuário pode verificar que ao visualizar a lista de perfis existem dois ícones na coluna Ações:

* Ações: Esta coluna apresenta dois ícones para que o usuário possa interagir com o perfil de visualização desejado:

  * **Ícone Lata de Lixo |icone_lixo|**: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud possa remover (excluir) este Perfil de Visualização, de forma imediata e definitiva.
  * **Ícone Edição |icone_edita_on|**: Basta o usuário clicar sobre este ícone para que a Plataforma do uCloud possa apresentar uma tela que permite editar Perfil de Visualização respectivo. Importante mencionar que apenas o usuário com a permissão correta poderá editar as opções de menu de um Perfil de Visualização.

.. image:: /figuras/ucloud_perfil_visualizacao_003.png
   :alt: perfil de permissionamento
   :align: center

----

* **Nome**: O usuário pode alterar o nome do Perfil de Visualização. O nome do perfil deve ter, no mínimo, três (03) caracteres, e no máximo setenta (70) caracteres. Importante recomendar a utilização apenas dos caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido).
* **Descrição**: Este campo é obrigatório, o usuário deve inserir uma descrição estendida do Perfil de Visualização. A descrição do perfil deve ter, no mínimo, três (03) caracteres, e no máximo, cento e vinte (120) caracteres.
* **Permissões**: Nesta coluna são apresentadas todas as opções de menu disponíveis na Plataforma do uCloud, elas podem ser vinculadas ao Perfil de Visualização que se está a provisionar.

  * **Mudar a Classificação**: Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de nomes de opções de menu de forma alfabética,  crescente (a – z) ou decrescente (z – a).
  * **Busca Rápida**: O usuário observa que abaixo do nome da coluna existe um campo em ‘branco’, este campo permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista, nomes de opções de menu. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma do uCloud atualiza a tela, e representa a informação neste padrão de busca.
  * **“Checkbox” no título da coluna**: Ao selecionar este campo “checkbox”, presente no título da coluna, o clique informa à Plataforma do uCloud a ação de selecionar todas as opções do menu, ainda não vinculadas ao perfil de visualização. Desta forma, uma única ação seleciona todas as opções de menu de uma vez.
  * **“Checkbox” de cada Opção de Menu**: Esta coluna apresenta a lista das opções de menu disponíveis na Plataforma do uCloud. Ao lado de cada opção de menu existe um campo do tipo “checkbox”, ao ser selecionado, isto significa que a opção de menu será vinculada (habilitada) ao Perfil de Visualização.
  * **Botão Criar**: Após certificar que todas as opções desejadas no menu foram configuradas, o usuário pode clicar com o botão do mouse no botão Criar e configurar as alterações, de forma definitiva e imediata. A Plataforma do uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que o novo Perfil de Visualização está cadastrado.

Após esta ação a Plataforma do uCloud fecha a tela e retorna à tela anterior, com o conteúdo atualizado que apresenta o novo Perfil de Visualização recém provisionado.

Menu Configuração / Billing Admin
=================================

A configuração de Billing Admin é a forma como a Plataforma do uCloud identifica o arquivo da fatura (cobrança) dos valores, referentes aos custos dos recursos computacionais de nuvem, nas credenciais do cliente.
Normalmente, os provedores de nuvem calculam os custos dos recursos computacionais num período de seis ou oito horas. Após este período de contabilização, um arquivo texto não formatado (Comma Separated Values – .CSV) é atualizado com todos os valores de todo o período de vigência da relação do cliente com o provedor.
A configuração de Billing Admin, na Plataforma do uCloud, estabelece uma identificação e o agendamento de um processo de sincronização (download) do conteúdo do arquivo texto não formatado (.CSV), do provedor para dentro das bases de dados do uCloud. Esta sincronização é planejada para que a apresentação dos valores na tela do uCloud seja rápida, uma vez que todos os valores já estão atualizados e prontos para o usuário consultar - valores dos recursos computacionais do provedor de serviço de nuvem.
A Plataforma do uCloud não cria valores - o ator responsável por gerar e adicionar um valor aos recursos computacionais consumidos no período, são os provedores de serviço de nuvem pública.
Qualquer discrepância de valores, consultados na console do provedor pelo usuário e na interface da Plataforma do uCloud pode estar associada a alguma condição específica estabelecida no Contrato. Veja acima no item Administração de Contrato na página 58.
Nesta tela, são listados apenas os provedores provisionados para esta empresa. Importante ressaltar que a Plataforma do uCloud é um ambiente multi-nuvem (multi-cloud), desta forma, pode ser listada mais de uma configuração de Billing Admin para cada empresa.
Na tela a seguir, é apresentado um exemplo de Billing Profile para dois provedores diferentes de serviço de nuvem (AWS e Azure). É possível haver apenas um ou mais provedores configurados.
  
.. inserir tela (remover este comentario)

.. important:: |importante| *Importante mencionar que não é objetivo deste documento descrever o processo de configuração de Billing Admin, pois apenas usuários com perfil de Administrador da Plataforma uCloud têm permissão para isto. Veja o documento Manual do Administrador da Plataforma do uCloud onde está descrito o processo correto de provisionar um Billing Admin.*

Segue a descrição dos botões desta tela:

* **Botão Lançar Accountant** |botao_lanca_acct| : Este botão apresenta a tela para provisionar um novo Billing Profile na Plataforma do uCloud. Importa ressaltar que apenas o usuário com perfil de Administrador de Plataforma pode provisionar um novo Billing Profile. Veja o documento Manual do Administrador da Plataforma do uCloud onde está descrito o processo correto de provisionar um Billing Admin.

* **Botão Limpar Histórico** |botao_limpa_acct| : *ATENÇÃO, é relevante ressaltar que este botão efetua o expurgo (apaga) completo de todos os registros de valores de bilhetagem das bases de dados da Plataforma do uCloud, de forma definitiva e irreversível. Serão removidos todos os valores desde a data  inicial até o dia da ação.*

* **Botão Refresh** |botao_refresh| : A Plataforma do uCloud se comunica com o console dos provedores através da API Rest, assim, toda ação executada ou configurada nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes, então, executem a ação desejada. Para atualizar apenas o conteúdo das seções de tela (as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, o qual aciona a execução e atualiza as informações contidas na base de dados da plataforma.

Informações de Registro (LOG) do Billing Admin
----------------------------------------------

A configuração de Billing Admin é a forma como a Plataforma do uCloud identifica o arquivo da fatura (cobrança) dos valores, referentes aos custos dos recursos computacionais de nuvem, nas credenciais do cliente.
Normalmente, os provedores de nuvem calculam os custos dos recursos computacionais num período de seis ou oito horas. Após este período de contabilização, um arquivo texto não formatado (Comma Separated Values – .CSV) é atualizado com todos os valores de todo o período de vigência da relação do cliente com o provedor.
A configuração de Billing Admin, na Plataforma do uCloud, estabelece uma identificação e o agendamento de um processo de sincronização (download) do conteúdo do arquivo texto não formatado (.CSV), do provedor para dentro das bases de dados do uCloud. Esta sincronização é planejada para que a apresentação dos valores na tela do uCloud seja rápida, uma vez que todos os valores já estão atualizados e prontos para o usuário consultar - valores dos recursos computacionais do provedor de serviço de nuvem.
A Plataforma do uCloud não cria valores - o ator responsável por gerar e adicionar um valor aos recursos computacionais consumidos no período, são os provedores de serviço de nuvem pública.
Qualquer discrepância de valores, consultados na console do provedor pelo usuário e na interface da Plataforma do uCloud pode estar associada a alguma condição específica estabelecida no Contrato. Veja acima no item Administração de Contrato na página 58.
Nesta tela, são listados apenas os provedores provisionados para esta empresa. Importante ressaltar que a Plataforma do uCloud é um ambiente multi-nuvem (multi-cloud), desta forma, pode ser listada mais de uma configuração de Billing Admin para cada empresa.
Na tela a seguir, é apresentado um exemplo de Billing Profile para dois provedores diferentes de serviço de nuvem (AWS e Azure). É possível haver apenas um ou mais provedores configurados.

.. image:: /figuras/ucloud_billing_admin_001.png
   :alt: perfil de permissionamento
   :align: center

----

Importante mencionar que não é objetivo deste documento descrever o processo de configuração de Billing Admin, pois apenas usuários com perfil de Administrador da Plataforma uCloud têm permissão para isto. Veja o documento Manual do Administrador da Plataforma do uCloud onde está descrito o processo correto de provisionar um Billing Admin.
Segue a descrição dos botões desta tela;

* **Botão Lançar Accountant** |botao_lanca_acct|: Este botão apresenta a tela para provisionar um novo Billing Profile na Plataforma do uCloud. Importa ressaltar que apenas o usuário com perfil de Administrador de Plataforma pode provisionar um novo Billing Profile. Veja o documento Manual do Administrador da Plataforma do uCloud onde está descrito o processo correto de provisionar um Billing Admin.
* **Botão Limpar Histórico** |botao_limpa_acct|: *ATENÇÃO, é relevante ressaltar que este botão efetua o expurgo (apaga) completo de todos os registros de valores de bilhetagem das bases de dados da Plataforma do uCloud, de forma definitiva e irreversível. Serão removidos todos os valores desde a data  inicial até o dia da ação*.
* **Botão Refresh** |botao_refresh|: A Plataforma do uCloud se comunica com o console dos provedores através da API Rest, assim, toda ação executada ou configurada nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes, então, executem a ação desejada. Para atualizar apenas o conteúdo das seções de tela (as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, o qual aciona a execução e atualiza as informações contidas na base de dados da plataforma.

Registro (LOG) do Billing Admin
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

É permitido ao usuário com o perfil de Administrador do Contrato identificar potenciais discrepâncias de valores, que porventura sejam apresentadas no menu Financeiro, este usuário pode verificar se há algum problema na comunicação entre a Plataforma do uCloud e a console do provedor, através do botão “Log”.
Ao visualizar todos os Billing Admin, o usuário pode identificar alguns ícones a cada configuração provisionada;

.. image:: /figuras/ucloud_billing_admin_002.png
   :alt: perfil de permissionamento
   :align: center

----

* **Nome**: Esta etiqueta identifica o nome do Billing Profile que foi informado no momento de sua configuração inicial.
* **Indicador do Tipo de Execução**: Esta etiqueta identifica (“ASYNC”) o tipo de execução do processo de sincronização, selecionado no momento da sua configuração inicial.
* **Ícone de Status de Execução**: Esta etiqueta apresenta o status do processo de sincronização da Plataforma do uCloud com a console do provedor de serviço de nuvem pública.
* **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para informar a Plataforma do uCloud que remova (exclua) esta configuração de Billing Admin de forma imediata e definitiva. 
* **Ícone LOG**: Basta o usuário clicar neste ícone que a Plataforma do uCloud apresenta uma tela que permite visualizar o registro de atividade (log) referente às tarefas de sincronização do Billing Profile com as bases de dados do uCloud. Este recurso é fundamental para identificar qualquer problema de comunicação da Plataforma do uCloud com o ambiente do provedor de serviço de nuvem pública, para obtenção do arquivo texto não formatado (.CSV).

.. image:: /figuras/ucloud_billing_admin_003.png
   :alt: perfil de permissionamento
   :align: center

----

Menu Configuração / Tagueamento de Recursos USN
===============================================

Esta opção, do menu de funcionalidades, somente deve ser acessada quando o modelo Financeiro do contrato for vinculado a um Ministério, Órgão ou Agência do Governo Brasileiro. E que os valores dos recursos computacionais de nuvem pública, sejam convertidos para Unidade de Serviço de Nuvem (USN).

.. note:: |atencao| *Importante mencionar empresas privadas não necessitam nenhuma das facilidades de USN descritos neste menu*.

No modelo de cobrança do recurso computacional de nuvem pública, todo recurso deve ter uma etiqueta (tag) na qual é aplicado um valor, em USN, a ser tarifado (billing) no ambiente da Plataforma do uCloud. Os recursos importados do arquivo de billing das nuvens públicas que não possuam nenhuma etiqueta (tag) no provedor de serviço de nuvens, no processo de importação, estes recursos recebem uma etiqueta (tag) na plataforma do uCloud, baseado no perfil de tagueamento adicionado ao contrato ao qual este recurso pertence.

Uma etiqueta (tag) é um rótulo no qual o usuário atribui um valor a um recurso computacional de nuvem pública. As etiquetas (tags) permitem categorizar seus recursos nas nuvens. Por exemplo, o usuário ou a organização, podem definir um conjunto de etiquetas (tag), para as instâncias do Amazon EC2, na sua conta que auxilie rastrear o nível do agrupamento (empilhamento de valores - stack) de cada recurso computacional de nuvem pública consumido.

A seguir, será descrito o processo de criação de um perfil de etiquetamento de recursos computacionais de nuvem pública (tag profile) em USN.

Criação de um Tagueamento de Recurso USN
----------------------------------------

O usuário deve acessar o Menu Configuração / Tagueamento de Recurso USN para a Plataforma do uCloud apresentar a tela abaixo:

.. image:: /figuras/ucloud_criar_recurso_usn_001.png
   :alt: perfil de permissionamento
   :align: center

----

* **Selecione um Contrato**: Este campo é do tipo “dropdown”, quando o usuário clicar com o cursor do mouse sobre ele, a Plataforma do uCloud listará todos os contratos existentes no ambiente do uCloud, o usuário deve selecionar o contrato da empresa onde o recurso será convertido para USN.

* **Botão Criar Perfil de Tags**: O usuário deve clicar com o cursor do mouse sobre este botão para visualizar a tela abaixo:


.. image:: /figuras/ucloud_criar_recurso_usn_002.png
   :alt: perfil de permissionamento
   :align: center

----

* **Contrato**: Este campo se apresenta preenchido com o contrato selecionado na etapa anterior.

* **Nome**: Neste campo, o usuário deve informar o nome desejado para identificar o arquivo do perfil de tagueamento em USN, para o contrato.

* **Botão Upload Arquivo JSON**: Este botão deve ser utilizado pelo usuário, para facilitar a localização e seleção do arquivo JSON em um diretório/folder desejado. Este arquivo texto deve estar formatado com a sintaxe JSON, conforme o exemplo abaixo:

.. image:: /figuras/ucloud_criar_recurso_usn_003.png
   :alt: perfil de permissionamento
   :align: center

----

* **Botão Importar**: Este botão fica ativo (verde) após preencher todos os campos descritos anteriormente. Assim, o usuário deve clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud possa iniciar o processo de importação do arquivo de Tagueamento de USN. O usuário visualiza a tela a seguir.

Após criado o perfil é possível editar

.. image:: /figuras/ucloud_criar_recurso_usn_004.png
   :alt: perfil de permissionamento
   :align: center

----

1. Troca o perfil do contrato 
2. Edita o perfil

.. image:: /figuras/ucloud_criar_recurso_usn_005.png
   :alt: perfil de permissionamento
   :align: center

----

É possível editar os valores e a descrição de cada etiqueta (*tag*) ao perfil de tagueamento deste contrato, através do processo abaixo:

.. image:: /figuras/ucloud_criar_recurso_usn_006.png
   :alt: perfil de permissionamento
   :align: center

----

1. **Botão Criar Tag**: Adicionar uma nova tag ao perfil.
2. **Botão Importar Tags**: Importar as etiquetas presentes no arquivo JSON e tags já mapeadas no perfil atual. Elas serão sobrescritas no perfil criado para o contrato selecionado da Plataforma uCloud.
3. Visualizar o estado atual da tag
4. Remover a tag do perfil
5. Listagem dos recursos no contrato que não possuem tags para bilhetagem USN

Neste ponto também será possívelalterar as configurações provisionadas ao Perfil de Tagueamento deste contrato, através do processo abaixo:

.. image:: /figuras/ucloud_criar_recurso_usn_007.png
   :alt: perfil de permissionamento
   :align: center

----

1. Selecionar o contrato.
2. Editar o conteúdo do perfil.
3. Buscar os recursos sem tag no contrato, por período selecionado.
4. Criar um novo perfil.
5. Exportar em xlsx a listagem de recursos no contrato que não tem tag.
6. Adicionar ao perfil os recursos. 

Após completar os passos acima descritos, para configurar o Perfil de Tagueamento, será necessário iniciar o processo de aplicação das etiquetas (tags) aos dados do billing. Ao final do processo, todos os valores referentes às novas etiquetas haverão sido aplicadas às etiquetas (tags) configuradas no perfil do usuário e aos dados de billing do contrato selecionado.

Máquinas Virtuais
=================

Como mencionado anteriormente, o uCloud está posicionado como uma plataforma de *Cloud Service Broker* (broker de serviços em nuvem) que permite gerenciar múltiplos provedores de serviços de nuvem, tanto privados quanto provedores de nuvem pública.

Quando configurada a comunicação entre a Plataforma do uCloud e a console do provedor de serviço de nuvem pública, como a Plataforma do uCloud, dois dos cinco pontos de uma plataforma de **CSB**, permitem às empresas atuar em cinco pontos fundamentais para o gerenciamento de ambientes híbridos multi-nuvem. Na apresentação do menu de Máquinas Virtuais, serão focados apenas dois destes cinco pontos fundamentais:

1. **Governança Financeira**
2. **Billing** (Faturamento dos Serviços)
3. **Monitoração da Infraestrutura**
4. **Inventário** (Assessment)

   A Plataforma do uCloud se conecta aos provedores de nuvem através do cadastramento de credenciais de acesso específicas para cada provedor de serviço de nuvem (público e/ou privado).
   Uma vez que as credenciais estão configuradas na Plataforma do uCloud, a primeira atividade é sincronizar as configurações e o inventário dos recursos computacionais existentes no provedor (máquinas virtuais – workloads). Este inventário de máquinas virtuais é extraído e adicionado nas bases de dados da plataforma do uCloud, de forma que é apresentado rapidamente, na tela do usuário.

5. **Operação da Infraestrutura**

  Com o inventário disponível diretamente dentro da Plataforma do uCloud, o usuário pode operar cada uma das máquinas virtuais, independente de em qual provedor de nuvem este recurso está provisionado. Será descrito, a seguir, as possíveis operações a serem aplicadas aos recursos computacionais existentes nos provedores de nuvem (público e/ou privado).

  A menção *operar* significa o leitor que é a capacidade do usuário comandar certas ações diretamente nestas máquinas virtuais, como ações de: parar (*shutdown*), reiniciar (*restart*), suspender (*suspend*), remover (*delete*), para citar algumas operações básicas.
  
  Através da interface da Plataforma do uCloud o usuário pode enviar comandos para os consoles de cada provedor de nuvem, além das ações acima listadas. Este também pode visualizar as informações das configurações específicas da máquina virtual, bem como alterar ou adicionar algum recurso extra a esta máquina virtual (por exemplo: placa de rede, disco, grupo de segurança, snapshot, entre outros).

Menu Máquinas Virtuais
======================

Quando o usuário acessa esta opção de menu, a Plataforma do uCloud apresenta uma tela com o inventário completo de todas as máquinas virtuais (instâncias, workloads) que podem ser acessadas com as credenciais da empresa.
Esta tela pode se apresentar muito extensa por listar todas as máquinas virtuais encontradas. No exemplo abaixo, estão listadas apenas três máquinas virtuais:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_001.png
   :alt: perfil de permissionamento
   :align: center

----

As colunas da tela listada anteriormente, está descrita abaixo:
* **Botão “Criar Máquina Virtual** (|botao_criar_VM|): Este botão permite provisionar (criar) uma máquina virtual no(s) ambiente(s) do(s) provedor de serviço de nuvem (público e/ou privado). Os detalhes estão descritos no item Criando uma Máquina Virtual.

* **Botão Refresh** (|botao_refresh|): A Plataforma do uCloud se comunica com a console dos provedores através da API Rest, assim toda ação executada ou configurada, nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada. Para atualizar apenas o conteúdo das seções de tela (ou as informações contidas nestas seções) é mandatório que o usuário clique com o mouse sobre o botão Refresh, ele executa apenas a atualização das informações contidas nas bases de dados da plataforma.

* **Coluna Acionável**: Esta coluna apresenta uma forma alternativa de interagir com várias máquinas virtuais com um único comando. Cada linha está representada por um ícone selecionável (“  ”). Quando o usuário seleciona uma linha ou várias, a Plataforma do uCloud apresenta ícone(s) acima desta coluna, eles representam ações ao usuário que podem ser executadas de uma única vez, para todas as linhas selecionadas. A seguir, são apresentados os seis ícones, suas ações são distintas:
  * **Ícone de Iniciar** (|icone_vm_start|): Este ícone permite ao usuário iniciar (Start – Boot) toda(s) máquina(s) virtual(is) que estiver com o status de “Stopped”. Este ícone ficará inativo se alguma máquina virtual selecionada permanecer com um status diferente de “Stopped”.
  * **Ícone de Parar** (|icone_vm_stop|): Este ícone permite ao usuário parar (Stop – Shutdown) toda(s) máquina(s) virtual(is) que estiver com o status de “Running”. Este ícone ficará inativo se alguma máquina virtual selecionada permanecer com um status diferente de “Running”.
  * **Ícone de Reiniciar** (|icone_vm_reboot|): Este ícone permite ao usuário reiniciar (Restart – Reboot) toda(s) máquina(s) virtual(is) que estiver com o status de “Running”.
  * **Ícone de Suspender** (|icone_vm_suspend|): Este ícone permite ao usuário suspender (Suspend) toda(s) máquina(s) virtual(is) que estiver com o status de “Running”.
  * **Ícone de Retomar** (|icone_vm_resume|): Este ícone permite ao usuário retomar (Resume) toda(s) máquina(s) virtual(is) que estiver com o status de “Suspended”.
  * **Ícone de Lata do Lixo** (|icone_lixo|): Este ícone permite ao usuário excluir (Remove – Delete) toda(s) máquina(s) virtual(is) que estiver selecionada com o ícone selecionável (“  ” – check mark). Este ícone somente ficará ativo para excluir as máquinas virtuais que foram criadas pelo próprio usuário que está registrado na plataforma. Este ícone ficará inativo, se o usuário registrado, selecionar máquinas virtuais criadas por outros usuários.
  * **Ícone de Desconectar** (|icone_desconecta|): Este ícone permite ao usuário desconectar (unplug) as máquinas virtuais da Plataforma do uCloud. Importante ressaltar que esta ação não remove (delete) a máquina virtual do ambiente do provedor de serviço de nuvem. Esta ação removerá a máquina virtual do inventário da base de dados da Plataforma do uCloud, portanto, a máquina não mais será listada nesta tela.

* **Busca Rápida**: O usuário pode observar que logo abaixo do nome da coluna existe um campo em *branco* que permite efetuar uma busca rápida no conteúdo recuperado para reduzir e estreitar a quantidade de incidências desta lista de nomes de opções de menu. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma do uCloud atualiza a tela de forma a representar este padrão de busca refletida na relação de máquinas virtuais na lista.

  * **Nome**: Esta coluna apresenta o nome da máquina virtual informado no momento da sua criação, no console do provedor de serviço de nuvem, configurado através do uCloud. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de nomes de máquinas virtuais de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **Usuário**: Esta coluna apresenta o login de usuário que estava com uma sessão ativa no momento do provisionamento desta máquina virtual, este á o usuário que está vinculado para efeito da totalização de todos os custos relativos à existência desta máquina virtual. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma do uCloud atualiza a tela de forma a representar este padrão de busca refletida na relação de máquinas virtuais na lista.
  * **IP Privado**: Esta coluna apresenta o endereço TCP-IP vinculado a esta máquina virtual no momento de sua criação. Importante ressaltar que este endereçamento TCP-IP pertence ao ambiente de rede privada do provedor de serviço de nuvem (recebe do servidor DHCP interno do provedor). Este endereço poderá mudar quando a máquina virtual for reiniciada (reboot). Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **IP Público**: Esta coluna pode estar em *branco*, pois nesta coluna será apresentado o endereço TCP-IP Público que foi vinculado a esta máquina virtual em um momento posterior ao provisionamento da máquina virtual. O Endereço TCP-IP Público, é um endereço fixo e pode incorrer em custos mensais para sua manutenção e vinculação a uma máquina virtual provisionada. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **Memória**: Nesta coluna será apresentado um número que é a quantidade de memória RAM configurada nesta máquina virtual, expressa em Gigabytes. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de máquinas virtuais com base no tamanho da memória, de forma crescente ou decrescente.
  * **CPUs**: Nesta coluna será apresentado um número que é a quantidade de CPU(s) configurada nesta máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de máquinas virtuais com base na quantidade de CPU(s), de forma crescente ou decrescente.
  * **Status**: Nesta coluna será apresentado o status corrente da máquina virtual. Importante ressaltar que o status é obtido do provedor de serviço de nuvem, pois a máquina virtual está instalada e sendo executada na infraestrutura do provedor de serviço de nuvem. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica o status da lista de máquinas virtuais, de forma alfabética crescente (a – z) ou decrescente (z – a). A Plataforma do uCloud apresenta os seguintes status:

    * **Running**: Status que indica que a máquina virtual está em funcionamento normal.
    * **Stopped**: Status que indica que a máquina virtual está parada.
    * **Suspended**: Este status indica que a máquina virtual está em um estado suspenso, possibilitando um tempo de inicialização (boot) mais rápido que o estado parado (stopped).
    * **Unrecognized**: Este status pode ser apresentado, pois se refere a um estado, temporário, onde momentaneamente não foi possível distinguir se a máquina está parada ou ‘rodando’ (falha de comunicação entre a Plataforma do uCloud e o console do provedor de serviço de nuvem pública).
    * **Deallocated**: Este status é particular da nuvem Azure e se refere a uma máquina virtual que se encontra parada, não está sendo cobrada, este estado faz a liberação de alguns recursos e seu tempo para inicialização (boot) será maior. Para maiores detalhes, consultar material de documentação do Azure.
    * **Orphan**: Este status somente será apresentado quando uma máquina não é encontrada no provedor de serviço de nuvem ou no ambiente de virtualização do datacenter privado (hypervisor).
  
  * **TAGs (Etiquetas)**: Esta coluna apresenta as TAGs (etiquetas) que foram provisionadas diretamente através da console do provedor de serviço de nuvem pública, quanto através da Plataforma do uCloud (Menu Inventário de Recursos).

Gerenciando uma Máquina Virtual
-------------------------------

Para gerenciar uma máquina virtual é necessário listar o relatório das máquinas, o usuário deve clicar com o cursor do mouse sobre qualquer uma das máquinas virtuais listadas para que a Plataforma do uCloud possa apresentar a tela que permite o gerenciamento e operacionalização da máquina virtual selecionada.
Esta tela possui diversas seções (cards) ela é bem ampla e completa, por isto, será apresentada a figura do início da tela e, a seguir a descrição de cada seção em detalhe e de forma individualizada.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_022.png
   :alt: perfil de permissionamento
   :align: center

----

A Plataforma do uCloud apresenta alguns ícones de botões, logo acima das seções (cards) para gerenciar a máquina virtual.

* **Ícone de Iniciar** (|icone_vm_start|): Este ícone permite ao usuário iniciar (Start – Boot) a máquina virtual que estiver com o status de “Stopped”. Este ícone permanece inativo se alguma máquina virtual selecionada estiver com um status diferente de “Stopped”.
* **Ícone de Parar** (|icone_vm_stop|): Este ícone permite ao usuário parar (Stop – Shutdown) toda(s) máquina(s) virtual(is) que estiver(em) com o status de “Running”. Este ícone permanece inativo se alguma máquina virtual selecionada estiver com um status diferente de “Running”.
* **Ícone de Reiniciar** (|icone_vm_reboot|): Este ícone permite ao usuário reiniciar (Restart – Reboot) toda(s) a(s) máquina(s) virtual(is) que estiver(em) com o status de “Running”.
* **Ícone de Suspender** (|icone_vm_suspend|): Este ícone permite ao usuário suspender (Suspend) toda(s) a(s) máquina(s) virtual(is) que estiver(em) com o status de “Running”.
* **Ícone de Retomar** (|icone_vm_resume|): Este ícone permite ao usuário retomar (Resume) toda(s) a(s) máquina(s) virtual(is) que estiver(em) com o status de “Suspended”.

.. comentado Ícone de Remote Desktop |icone_vm_rdp|: Este ícone permite efetuar o download do arquivo com as configurações para efetuar uma Conexão de Área de Trabalho Remota (Remote Desktop) nesta máquina virtual. Detalhe relevante: Somente para a(s) máquina(s) virtual(is) com o sistema operacional Microsoft Windows Server. Ao clicar com o cursor do mouse sobre este ícone a Plataforma do uCloud apresenta a tela para efetuar o download do arquivo de configuração:

.. comentado .. image:: /figuras/ucloud_menu_maquinas_virtuais_023.png
   :alt: perfil de permissionamento
   :align: center

..  comentado ----

* **Ícone Remote Console** (|icone_vm_ssh|): Este ícone permite ao usuário iniciar uma sessão de console do sistema operacional diretamente através da interface web da Plataforma do uCloud. Basta o usuário clicar com o cursor do mouse sobre este ícone, que a Plataforma do uCloud irá apresentar a tela abaixo:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_024.png
   :alt: perfil de permissionamento
   :align: center

----

  * **Nome**: Este campo apresenta o nome  da máquina virtual a qual o usuário deseja iniciar uma sessão de console.
  * **Versão**: Este campo apresenta o nome estendido do sistema operacional (template) que foi selecionado durante o provisionamento desta máquina virtual.
  * **Tipo**: Este campo apresenta o nome tipo do sistema operacional que foi selecionado durante o provisionamento desta máquina virtual.
  * **Protocolo**: Este campo é do tipo “dropdown”, quando o usuário clicar com o cursor do mouse sobre este campo, serão listadas os tipos de protocolos de console disponíveis na versão corrente da Plataforma do uCloud. O usuário deve selecionar o protocolo ideal (o adequado) para iniciar uma sessão de console no sistema operacional da máquina virtual.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_024b.png
   :alt: perfil de permissionamento
   :align: center

----

  * **Porta**: Neste campo o usuário deverá informar o número da Porta TCP-IP através da qual será iniciada a sessão de console. Este campo será preenchido automaticamente com as portas padrões, no momento que o usuário selecionar a opção do campo Protocolo. O usuário é livre para informar o número de Porta TCP-IP diferente, de acordo com a configuração adotada durante a criação da máquina virtual.
  * **Endereço**: Este campo é do tipo “dropdown”, quando o usuário clicar com o cursor do mouse sobre este campo, serão listados todos os endereços TCP-IP em que a máquina virtual está vinculada. O usuário deverá selecionar o endereço TCP-IP que é possível alcançar na máquina virtual.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_024c.png
   :alt: perfil de permissionamento
   :align: center

----

  * **Botão Conectar**: Basta o usuário clicar com o cursor do mouse sobre este botão e a Plataforma do uCloud irá apresentar uma janela pop-up com a sessão de console conforme o exemplo da tela abaixo:

.. comentario incluir tela de SSH do uCloud

.. attention:: |atencao| Importante ressaltar que a porta informada deve estar aberta para a rede pública Internet na configuração de Grupo de Segurança (Security Group) vinculada a esta máquina virtual. Caso o Grupo de Segurança vinculado a esta máquina não esteja configurado com a referida porta do protocolo, a Plataforma do uCloud não será capaz de iniciar uma sessão de console.
 
.. note:: |nota| Importante ressaltar que cada sistema operacional somente permite iniciar sessões do console através de um protocolo específico, consulte a documentação técnica do sistema operacional em questão para selecionar o protocolo correto.

.. important:: |importante| **ATENÇÃO**: caso o usuário selecione a opção VNC (Virtual Network Computing) é importante mencionar que esta modalidade necessita de um software adicional que funciona em um modelo cliente / servidor. Caso este componente server não esteja instalado, ou seu serviço não estiver ativo, na máquina virtual desejada, a Plataforma do uCloud não será capaz de iniciar uma sessão de console através desta opção.

Adicionalmente, é necessário que a senha de usuário de conexão seja conhecida, sem a informação da senha correta, a Plataforma do uCloud não será capaz de iniciar a sessão de console.

* **Botão Excluir** |botao_excluir|: Este botão efetua a exclusão da máquina virtual do ambiente do provedor de serviço de nuvem. Esta ação é irreversível e definitiva, por isto, a Plataforma do uCloud apresenta uma tela para confirmação desta ação.

  * **Botão Não Cancelar**: Este botão permite ao usuário cancelar a ação e manter a máquina virtual tanto no provedor de serviço de nuvem quanto na interface da Plataforma do uCloud. Será apresentada uma tela informando, ao usuário, informando que a máquina virtual não será excluída.
  * **Botão Sim Pode Excluir**: Ao clicar com o cursor do mouse neste botão, a Plataforma do uCloud envia a solicitação de exclusão para o provedor de serviço de nuvem (público e/ou privado) no qual esta máquina virtual está sendo executada, e em seguida, remove a mesma das bases de dados do uCloud. Importante mencionar, que quaisquer recursos computacionais adicionais (disco adicional, IP Públicos, snapshot) associados a esta máquina virtual, não serão excluídos.

A seguir descrição de cada seção (*card*) de forma individual:

Seção Geral - VMs
~~~~~~~~~~~~~~~~~

Esta seção permite visualizar as informações fundamentais e básicas da máquina virtual. 

.. image:: /figuras/ucloud_menu_maquinas_virtuais_025.png
   :alt: altera Usuario
   :align: center

----

* **Status**: Este campo apresenta o status corrente da máquina virtual. Importante ressaltar que status é obtido do provedor de serviço de nuvem, pois a máquina virtual está instalada e sendo executada na Infraestrutura do provedor de serviço de nuvem. A Plataforma do uCloud pode apresentar neste campo, o seguinte:

  * **Running**: Indica que a máquina virtual está em funcionamento normal.
  * **Stopped**: Indica no status que a máquina virtual está parada.
  * **Suspended**: Indica que a máquina virtual está em um estado suspenso, possibilitando um tempo de inicialização (boot) mais rápido que o estado parado (stopped).
  * **Unrecognized**: Este status pode ser apresentado, pois se refere a um estado, temporário, onde momentaneamente não foi possível distinguir se a máquina está parada ou rolando (falha de comunicação entre a Plataforma do uCloud e o console do provedor de serviço de nuvem pública).
  * **Deallocated**: Este status é particular da nuvem Azure, refere-se a uma máquina virtual que se encontra parada, e não está sendo cobrada, este estado faz a liberação de alguns recursos e seu tempo para inicialização (boot) será maior. Para maiores detalhes, consultar material de documentação do Azure.
  * **Orphan**: Este status somente será apresentado quando uma máquina não é encontrada no provedor de serviço de nuvem ou no ambiente de virtualização do datacenter privado (hypervisor).

* **Nome**: Este campo apresenta o nome da máquina virtual que foi informado no momento da sua criação, no console do provedor de serviço de nuvem ou no momento que foi configurado através do uCloud.

* **Criada em**: Este campo apresenta a data e a hora do provisionamento da máquina virtual (no formato DD/MM/AAAA HH:MM:SS). Adicionalmente é apresentada a informação do tempo total que esta máquina virtual está ativa (no formato dias, horas, minutos e segundos – XXd NNh YYm ZZs).

* **Região**: Neste campo será apresentado o código (ou o nome) da região onde a máquina virtual foi vinculada, no momento do seu provisionamento, tanto no console do provedor de serviço de nuvem quanto através da interface da Plataforma do uCloud. Importante mencionar que cada provedor possui identificação de regiões específicas, este campo reflete suas especificidades.

* **Zona de Disponibilidade**: *Este campo é opcional*, pois nem todos os provedores de serviço de nuvem possuem zonas de disponibilidade (zonas dentro de uma região). Este campo é apresentado nos casos em que o provedor possui esta informação.

* **IPs Públicos**: Este campo apresenta o endereço TCP-IP Público Dinâmico (obtido do servidor DHCP interno do provedor de serviço de nuvem), o qual foi vinculado a esta máquina no momento do provisionamento da máquina virtual. Importante ressaltar que o Endereço TCP-IP Público Dinâmico, não é um endereço fixo. Este endereço pode ser alterado quando esta máquina virtual for reiniciada (reboot). Caso o usuário veja um Endereço TCP-IP, mas sem a indicação "Dinâmico", isto significa que esta máquina virtual possui um Endereço TCP-IP fixo, e este não será alterado mesmo após a máquina virtual ter sido reiniciada.

* **IPs Privados**: Neste campo será apresentado o endereço TCP-IP vinculado a esta máquina virtual, no momento da sua criação. Importante ressaltar que este endereçamento TCP-IP pertence ao ambiente de rede privada do provedor de serviço de nuvem (obtido do servidor DHCP interno do provedor de serviço de nuvem) este endereço poderá ser alterado quando esta máquina virtual for reiniciada (reboot).

* **Par de Chave**: Este campo apresenta o nome da chave criptográfica, informada durante o processo de provisionamento desta máquina virtual. No caso do uso de autenticação de chave pública SSH, é bastante típico o usuário criar (ou seja, provisionar) o par de chaves para si próprio. Cada par de chaves SSH inclui duas chaves:

  * Uma chave pública que é copiada para o (s) servidor (es) SSH. Qualquer pessoa com uma cópia da chave pública pode criptografar dados que só podem ser lidos pela pessoa que possui a chave privada correspondente. Depois que um servidor SSH recebe uma chave pública de um usuário e a considera confiável, o servidor marca a chave como autorizada em seu arquivo authorized_keys. Essas chaves são chamadas de chaves autorizadas.

  * Uma chave privada que permanece (apenas) com o usuário. A posse dessa chave é a prova da identidade do usuário. Apenas um usuário de posse de uma chave privada que corresponda à chave pública no servidor será capaz de se autenticar com sucesso. As chaves privadas precisam ser armazenadas e manuseadas com cuidado, nenhuma cópia da chave privada deve ser distribuída. As chaves privadas usadas para autenticação do usuário são chamadas de chaves de identidade.

* **Grupo de Segurança**: Neste campo será apresentado o nome do Grupo de Segurança (Security Group) vinculado à máquina virtual, que controla as portas TCP-IP as quais podem ser utilizadas para acesso a esta máquina virtual. Um grupo de segurança atua como firewall virtual para as máquinas virtuais. O usuário pode criar diversos grupos de segurança e personalizar cada um com as regras que permitem tráfego de entrada ou de saída nas instâncias associadas.
  
  * **Botão de Alteração de Grupo de Segurança** |icone_edita_on|: Este botão permite ao usuário alterar a vinculação da máquina virtual ao Grupo de Segurança que está sendo apresentado na interface. Durante o provisionamento da máquina virtual, o usuário selecionou um Grupo de Segurança para controlar as portas TCP-IP desta máquina virtual. Para alterar o Grupo de Segurança que está vinculado a esta máquina virtual, basta clicar com o cursor do mouse sobre este botão e a interface da Plataforma do uCloud alterna para o modo de edição do conteúdo deste campo. Neste momento, a Plataforma do uCloud apresenta uma lista “drop-box” com uma lista de todos os Grupos de Segurança que este usuário tem autorização de ver. Basta o usuário clicar com o botão do mouse sobre o Grupo de Segurança desejado.

  * **Ícone de Confirmação** |icone_conf_verde|: Após selecionar o Grupo de Segurança desejado, será  permitido confirmar a intenção de alterar o conteúdo no campo desejado, em seguida, a Plataforma do uCloud apresenta um ícone de confirmação. Após finalizar a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Concluída esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma do uCloud e na configuração da máquina virtual no ambiente do provedor de serviço de nuvem pública.

  * **Ícone de Cancelamento** |icone_cancela_vermelho|: Para o caso do usuário clicar sobre o ícone de edição por engano ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna aos valores iniciais, antes de qualquer preenchimento ou alteração.
 
* **Flavor**: Este campo apresenta o nome do flavor selecionado como a definição do tipo de hardware da máquina virtual. Um flavor define o tamanho dos recursos de computação (número de CPUs virtuais, memória e capacidade de armazenamento) que podem ser atribuídos automaticamente a instâncias da máquina virtual, em uma configuração de nuvem. Cada provedor de serviço de nuvem possui uma denominação específica para o ambiente do provedor. Importante mencionar que a configuração dos recursos (CPU, memória e disco) podem ser similares em diferentes provedores, mas sua nomenclatura é particular.

* **Template**: Este campo apresenta o sistema operacional (template) selecionado no momento do provisionamento da máquina virtual.

* **Virtual Datacenter**: Este campo apresenta o nome do Virtual Datacenter (VDC) ao qual esta máquina virtual está vinculada. Veja no item Virtual Datacenters: da página 184 a 195, para entender o conceito e saber como provisionar um Virtual Datacenter.

  * **Botão para Mover para outro Virtual Datacenter** |icone_edita_vdc|: Este botão permite ao usuário alterar a vinculação da máquina virtual ao Virtual Datacenter que está sendo apresentado na interface. Durante o provisionamento da máquina virtual, a Plataforma do uCloud, vincula esta máquina virtual ao Virtual Datacenter que o usuário selecionou. Para mover a máquina virtual para outro Virtual Datacenter, basta clicar com o cursor do mouse sobre este botão e a interface da Plataforma do uCloud alterna para o modo de edição do conteúdo deste campo. Para mover esta máquina virtual para outro Virtual Datacenter, basta clicar com o cursor do mouse sobre este botão e a interface da Plataforma do uCloud habilita editar o conteúdo do campo. Assim o usuário pode digitar uma parte da sequência de caracteres do novo Virtual Datacenter, para que a Plataforma do uCloud apresenta uma lista que combina com a sequência de caracteres desejada:
  
.. image:: /figuras/ucloud_botao_edita_vdc.png
   :alt: altera Usuario
   :align: center

----

  * **Ícone de Confirmação** |icone_conf_verde|: Após selecionar o novo Virtual Datacenter, será  permitido confirmar a intenção de mover a máquina virtual para outro Virtual Datacenter, e a Plataforma do uCloud apresenta um ícone de confirmação. Após finalizar a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Concluída esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma do uCloud de forma permanente e imediata.
  * **Ícone de Cancelamento** |icone_cancela_vermelho|: Para o caso do usuário clicar sobre o ícone de edição por engano ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna aos valores iniciais, antes de qualquer preenchimento ou alteração.[e]

* **Usuário**: Este campo apresenta a credencial do usuário que estava conectado na Plataforma do uCloud, o qual foi o responsável pelo aprovisionamento da máquina virtual no provedor de serviço de nuvem. Esta informação pode ser alterada com os botões que se apresentam ao lado da tela:

  * **Botão de Edição de Usuário** |icone_edita_user|: Este botão permite ao usuário alterar o nome do usuário que está vinculado a esta máquina virtual, basta clicar com o cursor do mouse sobre este botão e a interface da Plataforma do uCloud habilita editar o conteúdo do campo. Assim o usuário pode digitar uma parte da sequência de caracteres do novo usuário, para que a Plataforma do uCloud recupere a lista de usuários com a informação que combina com a palavra digitada.

.. image:: /figuras/ucloud_botao_change_user_vm.png
   :alt: altera Usuario
   :align: center

----

    * **Ícone de Confirmação** |icone_conf_verde|: Após selecionar o usuário desejado, é permitido confirmar a intenção de alterar o conteúdo no campo desejado, em seguida, a Plataforma do uCloud apresenta um ícone de confirmação. Após finalizar a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Concluída esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma do uCloud.
    * **Ícone de Cancelamento** |icone_cancela_vermelho|: Para o caso do usuário clicar sobre o ícone de edição por engano ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna aos valores iniciais, antes de qualquer preenchimento ou alteração.

* **Proteção Exclusão Acidental**: Este ícone indica se esta máquina virtual está com o parâmetro de exclusão acidental configurado, como: Desabilitado (vermelho) ou Habilitado (verde).
  
  * **Ícone Disable** |icone_desb_verm|: Este ícone indica que a proteção acidental está desabilitada. Isto significa que esta máquina pode ser excluída (apagada) sem restrição, apenas com a confirmação desta ação por parte do usuário que a está removendo (excluindo).

  * **Ícone Enable** |icone_habil_verde|: Este ícone indica que a proteção acidental está habilitada. Isto significa que esta máquina não pode ser excluída (apagada). Para efetuar a remoção desta máquina virtual, é necessário que o usuário que provisionou a máquina virtual e a habilitou neste parâmetro, realize a alteração do parâmetro para: Desabilitado. Posteriormente, deve efetuar o procedimento de exclusão da máquina virtual, ao clicar no botão, que deve estar ativo.
  
* **Template Privado (opcional/variável)**: Este ícone |icone_private_net| permite ao usuário criar um tipo de hardware (“flavor”) personalizado. Este novo “flavor” pode ter um nome personalizado (diferente do nome no provedor de serviço de nuvem). Sua configuração é baseada nas configurações do hardware configurado na máquina virtual. Este recurso pode ser útil para personalizar opções de “flavors” específicos para o cenário da empresa.

* **Identificador de Provedor**: Este campo apresenta a identificação da máquina virtual como nomenclatura baseada em recursos (RBN - Resource-based Naming) que é gerada automaticamente pelo próprio provedor de serviço de nuvem pública. A Plataforma do uCloud, não possui mecanismos para criar, ou alterar, o conteúdo desta informação. Consulte a documentação técnica online de cada provedor para mais informações.

* **ID de Rede**: Este campo apresenta a identificação da interface de rede elástica é um componente de rede lógico de cada provedor de serviço de nuvem pública e que representa uma placa de rede virtual.

* **Network ID do Provedor**: Este campo apresenta a identificação da Rede é um componente de rede lógico de cada provedor de serviço de nuvem pública e que representa uma placa de rede virtual.

Seção Performance Instantânea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Seção Metrics (exclusivo AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Seção Interfaces de Rede
~~~~~~~~~~~~~~~~~~~~~~~~

Seção Disco
~~~~~~~~~~~

Seção Snapshots
~~~~~~~~~~~~~~~

Seção Signatures (Exclusivo Azure e Google Cloud Platform)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Seção Histórico de Performance (Azure e GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Criando uma Máquina Virtual
---------------------------

Wizard Etapa 1 (Seleção da Nuvem)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Etapa 2 (informações básicas da máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Etapa 3 (informações básicas da máquina virtual – cont.)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Etapa 4a (informações de segurança da máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Etapa 4b (informações de segurança – Exclusivo Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Etapa 5a (User data)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Etapa 5b (User data VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Wizard Etapa 6 (visualizar as configurações da máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Menu Scaling Groups
===================
Criando um Scaling Group AWS
----------------------------
Problemas Conhecidos com Grupo de Escalabilidade AWS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criado um Scaling Group Azure
-----------------------------

Menu Banco de Dados
===================
Gerenciando um Banco de Dados
-----------------------------

Seção Geral - Grupo Segurança
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Seção Grupos de Segurança
~~~~~~~~~~~~~~~~~~~~~~~~~
Provisionando um Banco de Dados
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criação de Banco de Dados (MySQL & AWS)
---------------------------------------
Etapa 1 Seleção do Provedor de Serviço de Nuvem (AWS)  [4 nivel]
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 2 Seleção do Banco de Dados (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 3 Especificações do Banco de Dados (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 4 Configurações de acesso ao Banco de Dados (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 5 Especificações de Rede e Segurança (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 6 Parâmetro de Cópia de Segurança (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criação de Banco de Dados (MySQL & Azure)
-----------------------------------------
Etapa 1 Seleção do Provedor de Serviço de Nuvem (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 2 Seleção do Banco de Dados (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 3 Especificações do Banco de Dados (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 4 Configurações de acesso ao Banco de Dados (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 5 Especificações de Rede e Segurança (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 6 Parâmetro de Cópia de Segurança (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criação de Banco de Dados (MySQL & GCP)
---------------------------------------
Etapa 1 Seleção do Provedor de Serviço de Nuvem (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 2 Seleção do Banco de Dados (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 3 Especificações do Banco de Dados (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 4 Configurações de acesso ao Banco de Dados (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 5 Especificações de Rede e Segurança (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Etapa 6 Parâmetro de Cópia de Segurança (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Menu Virtual Datacenters
========================
Gerenciando Virtual Datacenters
-------------------------------
Editando um Virtual Datacenter
------------------------------
Criando um Virtual Datacenter
-----------------------------

Menu Financeiro
===============
Empresas Privadas
-----------------
Empresas Públicas (USN)
-----------------------

Menu Financeiro (Ambiente Corporativo)
======================================
Seção Minha Fatura
------------------
Seção X Contratos
-------------------
Fatura do Grupo no Contrato
---------------------------
Faturamento do Usuário
----------------------
Menu Financeiro (USN)
---------------------
Ambiente Governo Brasileiro
---------------------------

Menu Financeiro / USN Billing
=============================
Menu Financeiro / Relatório Consolidado de Faturamento
------------------------------------------------------

Menu Ordem de Serviço
=====================
Gerenciando a Ordem de Serviço
------------------------------
Seção Geral - Ordem de Serviço
------------------------------

Seção Estimativa de Custo (USN)
-------------------------------
Configuração de Estimativa de Custo (UST)
-----------------------------------------
De Acordo
---------

Menu Containers
===============
Gerenciando um Container
------------------------
Criando Novo Container
----------------------

Menu Hosts
==========

Visualizando um Host
--------------------

Menu Redes
==========

Redes
-----

Adicionar “Sub-Rede” no ambiente AWS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Adicionar “Sub-Rede” no ambiente Azure
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Adicionar “Sub-Rede” no ambiente GCP
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Adicionar “Sub-Rede” no ambiente Privado (ex.: VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Rede em Provedores de Serviço de Nuvem Pública
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Rede em Ambiente Privado (On-Premisses)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Rede em Provedores de Serviço de Nuvem Público (AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Rede em Provedores de Serviço de Nuvem Público (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Rede em Provedores de Serviço de Nuvem Público (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Rede em Ambiente Privado (ex: VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
IPs Públicos
------------
Solicitando um IP -Público (AWS e GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Solicitando um IP Público (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Solicitando um IP Público (ambiente privado VMware vCenter)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Grupos de Segurança e ACLs
--------------------------
Gerenciar Grupo de segurança
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Grupo de Segurança
~~~~~~~~~~~~~~~~~~~~~~~~
Par de Chaves
-------------
Gerenciar um Par de Chaves
~~~~~~~~~~~~~~~~~~~~~~~~~~
Criando um Par de Chaves
~~~~~~~~~~~~~~~~~~~~~~~~
Importando um Par de Chaves
~~~~~~~~~~~~~~~~~~~~~~~~~~~
Balanceadores
-------------
Gerenciando Balanceador
~~~~~~~~~~~~~~~~~~~~~~~
Criando Balanceador (Ambientes AWS e GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criando Balanceador (Ambiente Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Zonas DNS
---------
Gerenciar Zona DNS Pública
~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Zona DNS Pública (AWS e GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Zona DNS Pública (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Criar Zona DNS Privada - Observação
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
VPN
---
Criar a VPN em 3 Passos
~~~~~~~~~~~~~~~~~~~~~~~
Criar Customer Gateway
~~~~~~~~~~~~~~~~~~~~~~
Criar Private Gateway
~~~~~~~~~~~~~~~~~~~~~
Criar Túnel VPN
~~~~~~~~~~~~~~~

Menu Storage
============
Visualizando um Storage
-----------------------
Seção Templates
---------------

Menu Flavors
============
Visualizando um Flavor
----------------------

Menu Workflows
==============
Editando Workflow
-----------------
Criando Workflow
----------------
Criando Tarefas Associadas
--------------------------
Tarefa de Iniciar e Parar Máquina Virtual
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Tarefa de Criar Imagem de Disco (Snapshot)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Tarefa de Script
~~~~~~~~~~~~~~~~

Menu Tarefas
============
Aba Tarefas
-----------
Aba Aprovações Pendentes
------------------------
Aba Tarefas Agendadas
---------------------

Menu Inventário de Recursos
===========================
Editor de Etiquetas (tags) Nativo
---------------------------------

.. |atencao| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/hand-stop-o.png?raw=true

.. |nota| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/hand-pointer-o.png?raw=true

.. |importante| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/warning.png?raw=true

.. |dica| image:: https://github.com/Rush/Font-Awesome-SVG-PNG/blob/master/black/png/22/asterisk.png?raw=true

.. |botao_adiciona| image:: /figuras/uCloud_botao_adicionar.png

.. |botao_adiciona_user| image:: /figuras/uCloud_botao_adicionar_usuario_exist.png

.. |botao_adiciona_grp| image:: /figuras/uCloud_botao_criar_grupo.png

.. |botao_cria_user| image:: /figuras/uCloud_botao_criar_usuario.png

.. |botao_editar| image:: /figuras/uCloud_botao_editar.png

.. |botao_exclui_grp| image:: /figuras/uCloud_botao_excluir_grupo.png

.. |botao_adiciona_aogrupo| image:: /figuras/uCloud_botao_adicionar_aogrupo.png

.. |botao_adiciona_verde| image:: /figuras/uCloud_botao_adiciona_verde.png

.. |botao_conecta_container| image:: /figuras/uCloud_botao_conecta_container.png

.. |botao_criar_VM| image:: /figuras/uCloud_botao_criar_VM.png

.. |botao_desabilita| image:: /figuras/uCloud_botao_disable.png

.. |botao_download| image:: /figuras/uCloud_botao_download.png

.. |botao_enable| image:: /figuras/uCloud_botao_enable.png

.. |botao_excluir| image:: /figuras/uCloud_botao_excluir.png

.. |botao_exclui_VDC| image:: /figuras/uCloud_botao_excluir_VDC.png

.. |botao_exclui_user| image:: /figuras/uCloud_botao_exclui_usuario.png

.. |botao_exportar| image:: /figuras/uCloud_botao_exportar.png

.. |botao_filtrar| image:: /figuras/uCloud_botao_filtrar.png

.. |botao_lanca_acct| image:: /figuras/uCloud_botao_lancar_acct.png

.. |botao_limpa_acct| image:: /figuras/uCloud_botao_limpar_acct.png

.. |botao_pesquisar| image:: /figuras/uCloud_botao_pesquisar.png

.. |botao_refresh| image:: /figuras/uCloud_botao_refresh.png

.. |botao_seleciona_azul| image:: /figuras/uCloud_botao_seleciona_azul.png

.. |icone_conf_verde| image:: /figuras/uCloud_icone_confirma_verde.png

.. |icone_cancela_vermelho| image:: /figuras/uCloud_icone_cancela_vermelho.png

.. |icone_cota_grp| image:: /figuras/ucloud_icone_cota_grupo.png

.. |icone_cota_indv| image:: /figuras/ucloud_icone_cota_individual.png

.. |icone_desb_verm| image:: /figuras/uCloud_icone_desabilita_vermelho.png

.. |icone_edita_on| image:: /figuras/uCloud_icone_editar_on.png

.. |icone_habil_verde| image:: /figuras/uCloud_icone_habilita_verde.png

.. |icone_lixo| image:: /figuras/uCloud_icone_lixo.png

.. |icone_abre_fatura| image:: /figuras/uCloud_icone_abrir_fatura.png

.. |icone_agenda| image:: /figuras/uCloud_icone_agendar.png

.. |icone_anexa_branco| image:: /figuras/uCloud_icone_anexar_branco.png

.. |icone_conecta_rede| image:: /figuras/uCloud_icone_conecta_rede.png

.. |icone_desconecta| image:: /figuras/uCloud_icone_desconectar.png

.. |icone_download| image:: /figuras/uCloud_icone_download.png

.. |icone_edita_user| image:: /figuras/uCloud_icone_edita_user.png

.. |icone_private_net| image:: /figuras/uCloud_icone_private_template.png

.. |icone_remove_user| image:: /figuras/uCloud_icone_remove_user.png

.. |icone_visualiza| image:: /figuras/uCloud_icone_visualiza.png

.. |icone_vm_start| image:: /figuras/ucloud_icone_vm_start.png

.. |icone_vm_stop| image:: /figuras/ucloud_icone_vm_stop.png

.. |icone_vm_reboot| image:: /figuras/ucloud_icone_vm_reboot.png

.. |icone_vm_suspend| image:: /figuras/ucloud_icone_vm_suspend.png

.. |icone_vm_desconecta| image:: /figuras/ucloud_icone_vm_desconecta.png

.. |icone_vm_ssh| image:: /figuras/ucloud_icone_vm_ssh.png

.. |icone_vm_rdp| image:: /figuras/ucloud_icone_vm_rdp.png

.. |icone_vm_clone| image:: /figuras/ucloud_icone_vm_clone.png

.. |icone_vm_resume| image:: /figuras/ucloud_icone_vm_resume.png

.. |icone_edita_vdc| image:: /figuras/ucloud_icone_edita_vdc.png