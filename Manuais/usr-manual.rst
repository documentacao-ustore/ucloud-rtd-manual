uCloud - Manual de Usuário
++++++++++++++++++++++++++

.. figure:: /figuras/ucloud_logo_peq.png
   :alt: Logo uCLoud
   :align: center

----

Introdução Visão Geral
======================

As organizações empresariais adotaram a nuvem como solução para gerenciar seus ambientes e adotam uma combinação de nuvens privadas e públicas, o grande desafio atual é o gerenciamento destes ambientes híbridos de diversas nuvens (hybrid multi-cloud).

Para alcançar uma visão unificada, bem como obter um controle dos custos financeiros de forma centralizada, uma vez que cada organização empresarial tem uma necessidade e enfrenta diferentes desafios.

A Plataforma uCloud foi desenvolvida para estes cenários, independente de quantos provedores (públicos e/ou privados) existam, o usuário poderá interagir com suas plataformas de Infraestrutura como Serviço (Infrastructure as a Service – IaaS), Plataforma como Serviço (Platform as a Service – PaaS).

Como mencionado anteriormente, o uCloud está posicionado como uma plataforma de Cloud Service Broker – CSB (broker de serviços em nuvem) que permite gerenciar múltiplos provedores de serviços de nuvem, tanto privados quanto provedores de nuvem pública.

Uma plataforma de CSB como a Plataforma uCloud permite às organizações atuar em cinco pontos fundamentais para o gerenciamento de ambientes híbridos multi-nuvem, são eles:

Governança Financeira
---------------------

Além do controle da infraestrutura, a Plataforma uCloud permite que empresas usuárias desta plataforma possam estabelecer limites, tanto financeiros quanto quantitativos de recursos (cotas). Estes limites financeiros ou de infraestrutura, podem ser aplicados em três níveis:

* Para um provedor público em geral (ver o ítem Contratos, no Menu Administração)
* Para um grupo de usuários (ver o item Grupos, no Menu Administração)
* Para um usuário/indivíduo (ver o item Usuários, no Menu Administração)

Desta forma, a organização aplicará critérios de governança financeira e controle de custos, como também poderá acompanhar os custos do seu ambiente híbrido de multi-nuvem através de uma única interface.

A adoção da aplicação de limites (cotas) financeiros e/ou recursos computacionais em diversos níveis alcança o nível de usuário, assim o controle de custos será efetivo e permitirá evitar que o orçamento da organização seja surpreendida em situações que o custo da infraestrutura computacional seja exorbitante ou acima dos valores pré-estabelecidos.

Outro aspecto da Plataforma uCloud é a redução de custo de certificação e treinamento dos especialistas, em cada uma das interfaces de cada provedor (público e/ou privado), visto que o emprego de uma interface de uso e gerenciamento único e simples, permite extrair mais produtividade do ambiente do provedor de nuvem. Mesmo que o usuário não tenha treinamento ou certificação no console específico do provedor (público e/ou privado), a Plataforma uCloud possibilitará ao usuário provisionar um recurso computacional no ambiente desejado de forma simples e fácil.

Billing (Faturamento dos Serviços)
----------------------------------

A Plataforma uCloud viabiliza às organizações empresariais a informação dos custos recorrentes referente ao uso dos recursos computacionais na(s) operação(ões) em um ambiente híbrido multi-nuvem. Este é apenas um dos pontos que faz parte da prática de Cloud Financial Management - FinOps (Gestão financeira da nuvem).

Importante ressaltar que, individualmente, a Plataforma uCloud não atende a todos os três pilares da prática de FinOps por default. A Ustore possui outros produtos que podem ser complementares e o conjunto de produtos tem potencial para atuar como um ambiente capaz de englobar e atender a prática de FinOps.

O quesito suportado pelo uCloud é o ponto de Informação (Inform), os outros pontos desta melhor prática de FinOps: a Otimização e a Operação pertencem aos outros produtos do portfólio da Ustore que complementa a Plataforma uCloud.

Deve-se esclarecer que a Plataforma uCloud não cria ou gera valores de recursos computacionais, estes valores são gerados nos provedores de nuvem pública dos quais a Plataforma uCloud extrai (download) o arquivo de billing (faturamento) destes provedores e adiciona estas informações em suas bases de dados internas. Para que, posteriormente, de acordo com os critérios comerciais do contrato possam ser aplicados e estes custos calculados e convertidos para a moeda corrente no Brasil.

Desta forma, o usuário permanece informado da evolução dos custos e poderá acompanhar se estes custos encontram-se dentro dos critérios da governança financeira da organização.

Geralmente estes custos são apresentados em arquivos de texto não estruturados (Comma-separated Values – CSV) gerados a cada período (média de 8 horas) e a Plataforma uCloud adiciona a informação deste arquivo CSV para a sua base de dados interna de forma a agilizar e simplificar a apresentação destes valores na tela do usuário.

Exclusivamente, os usuários com um perfil específico podem ‘visualizar custos’ e permanecer informados dos valores de consumo dos seus recursos computacionais totais em cada provedor de nuvem (pública e/ou privada). Isto permite que o usuário possa acompanhar os custos acumulados dos recursos computacionais ativos nos provedores de serviços de nuvem.

Monitoração da Infraestrutura
-----------------------------

Uma funcionalidade importante da Plataforma uCloud é a recente implementação do módulo de gerência de eventos (monitoração) que permite coletar eventos e alarmes que foram gerados nos ambientes de nuvem (público e/ou privado), ativar notificações e criar relatórios customizados.

Todas essas facilidades reduzem os custos para as organizações, uma vez que elimina a necessidade de contratação de serviços de monitoração dos provedores, pois tal serviço pode representar altos custos os quais podem impactar de forma negativa no orçamento (ultrapassar o limite) destinado para infraestrutura de nuvem pública.

Esta funcionalidade permite integrar a um ambiente de gerenciamento de Service Desk para controle IT Service Management (gerenciamento de serviços de TI).

Inventário (Assessment)
-----------------------

A Plataforma uCloud se conecta aos provedores de nuvem através do cadastramento de credenciais de acesso específicas de cada provedor de serviço de nuvem (público e/ou privado). Para esta finalidade as empresas devem providenciar credenciais de modo “operativo”.

Esta credencial operativa é fornecida pelo administrador do serviço de nuvem e são credenciais que são geradas nas contas dos provedores que somente tem permissão de interagirem com a console do provedor público de nuvem através de uma API, não são credenciais normais com informações padrão de login e senha. Desta forma, a segurança e as regras de regulamentação de segurança da informação estão previstas e atendidas em sua totalidade.

Uma vez que as credenciais operativas são configuradas na Plataforma uCloud, a primeira atividade é sincronizar as configurações e o inventário de recursos computacionais existentes no provedor (máquinas virtuais – workloads). Este inventário de máquinas virtuais é extraído e adicionado nas bases de dados do uCloud, de forma que a apresentação na tela do usuário seja rápida.

Com este inventário disponível diretamente dentro da Plataforma uCloud, o usuário poderá operar cada uma das máquinas virtuais, independente de qual é o provedor de nuvem que este recurso está provisionado. Veja a seguir as possíveis operações a serem aplicadas aos recursos computacionais existentes nos provedores de nuvem (público e/ou privado).

Importante mencionar que a Plataforma uCloud não possui nenhum recurso computacional, estes recursos existem nas nuvens dos provedores de serviço de nuvem pública ou nos ambientes de virtualização (hypervisors) instalados em seu Data Center privado. Através da API Rest a Plataforma uCloud, envia ações (tarefas) para o gerenciador de ambiente de nuvem específico (público e/ou privado) para que estes então executem a ação desejada.

O usuário poderá acompanhar o resultado de qualquer uma das ações de operação nos recursos computacionais de forma quase que imediata, vale lembrar que não é a Plataforma uCloud que executa as ações, e sim, o ambiente onde a máquina virtual existe (seja ele público e/ou privado). Este é o encarregado de executar a tarefa enviada através da API Rest.

Caso o resultado não seja refletido na interface da tela do usuário, o console destino pode levar um certo tempo para executar esta tarefa e somente após o término da execução da tarefa o resultado será apresentado na interface do uCloud.

Existe uma opção de menu onde o usuário poderá acompanhar o percentual de andamento destas tarefas, seu resultado de sucesso ou a mensagem de erro referente a alguma restrição do ambiente destino.

Importante ressaltar que podem existir restrições aplicadas ao usuário provisionado na Plataforma uCloud, restrições ao usuário porque ele pode haver exaurido seu limite, sua cota financeira ou de recursos computacionais, desta forma a Plataforma uCloud gerar um aviso de erro: “limite de cota excedido” por exemplo. Estes cenários serão descritos no menu Tarefas.

Operação da Infraestrutura
--------------------------

A menção operar significa ao leitor que é a capacidade do usuário comandar certas ações diretamente nestas máquinas virtuais, como ações de: parar (shutdown), reiniciar (restart), suspender (suspend), remover (delete), para citar algumas operações básicas.

Através da interface da Plataforma uCloud, o usuário pode enviar comandos para os consoles de cada provedor de nuvem, além das ações acima listadas. Este também pode visualizar as informações das configurações específicas da máquina virtual, bem como alterar ou adicionar algum recurso extra a esta máquina virtual (por exemplo: placa de rede, disco, grupo de segurança, snapshot, entre outros).

Em relação aos provedores de serviço de nuvem pública, a Plataforma uCloud está preparada para se conectar com as seguintes plataformas de nuvem pública:

* Amazon Web Services (**AWS**)
* Google Cloud Plataform (**GCP**)
* Microsoft **Azure**
* IBM Cloud
* Huawei Cloud
* Oracle Cloud Infrastructure (**OCI** - *Roadmap*)

Atualmente, a Plataforma uCloud está preparada para se conectar com as seguintes plataformas (hypervisors) de gerenciamento de ambiente de nuvem privada:

* **VMware** (vCenter Versões 5.0, 5.1, 5.5, 6.0, 6.5, 6.7, 7.x ou superior);
* **vCloud**
* **Hyper-v** (Windows 2008R2, Windows 2012, Windows 2012R2 e Windows 2016, ou superior)
* **Openstack**
* **Xen Server**
* **XCP-NG**
* **KVM**

A Plataforma uCloud, além das funções de CSB (*Cloud Service Broker*), também é um agregador de funcionalidades que permite aos usuários, de forma simples e centralizada, o controle de diversos consoles de gerenciadores de ambientes virtualizados (*hypervisors*) seja do ambiente privado on-premises quanto do ambiente de fornecedores de nuvem pública. Agrega as funcionalidades de monitoração, fluxo de trabalho na nuvem (*Cloud Workflow*) e possibilita implementar um repositório biblioteca centralizado de arquivos (playbooks) de referência para uso de ferramentas de infraestrutura como código (*Infrastructure as a Code*).

Integração e Interoperabilidade entre Plataformas (*API Ucloud*)
----------------------------------------------------------------

Interoperabilidade é a habilidade de dois ou mais sistemas (computadores, meios de comunicação, redes, software e outros componentes de tecnologia da informação) de interagir e de intercambiar dados de acordo com um método definido, de forma a obter os resultados esperados. Interoperabilidade define se dois componentes de um sistema, desenvolvidos com ferramentas diferentes, de fornecedores diferentes, podem ou não atuar em conjunto.

A comunicação entre estes "sistemas" se baseia no consumo de uma interface de programação de aplicação (API) que possibilita o envio e recebimento de chamadas para execução de alguma atividade ou extrair de algum tipo de informação armazenada. A sigla API deriva da expressão inglesa Application Programming Interface que, traduzida para o português, pode ser compreendida como uma interface de programação de aplicação. Ou seja, API é um conjunto de normas que possibilita a comunicação entre plataformas através de uma série de padrões e protocolos.

Por meio de APIs, desenvolvedores podem estabelecer comunicação (interoperabilidade) entre softwares e aplicativos capazes de se comunicar com outras plataformas.

O principal exemplo é a integração nativa e direta da Plataforma uCloud com a console dos provedores de nuvem pública, toda esta é executada através da interoperabilidade via API dos  consoles dos provedores.

Outro exemplo bastante comum do uso da plataforma uCloud é a emissão de invoices de bilhetagem para sistemas de showback e chargeback, bem como o envio de informações e alertas sobre recursos gerenciados.

Nossos clientes (e/ou integradores) podem utilizar a documentação da API da Plataforma uCloud com suas plataformas internas, de forma a complementar ou automatizar certas atividades ou ações que estão além das capacidades nativas da Plataforma uCloud. Por exemplo: consultar e extrair da Plataforma uCloud o custo da fatura dos valores de um provedor de nuvem pública através de uma aplicação financeira/contábil para a emissão da Nota Fiscal.

A Plataforma uCloud possui uma documentação da sua API, mas o acesso a documentação completa deve ser solicitada à Equipe de Atendimento ao Cliente (contato@usto.re) para que seja criada e enviada uma credencial de acesso à documentação da Plataforma uCloud.
A Equipe Ustore está preparada para auxiliar e avaliar as demandas de interoperabilidade e integração entre a Plataforma uCloud e as plataformas que possuem e permitem o uso de API’s para a interoperabilidade.

Arquitetura da Plataforma uCloud
-----------------------------------

Abaixo apresentamos uma arquitetura de referência para a Plataforma uCloud com os seus componentes, os provedores e as integrações nativas.

.. figure:: /figuras/uCloud_future_vision-small.jpg
   :alt: Arquitetura de Referência da Plataforma uCloud
   :align: center

----

A Plataforma uCloud se comunica com o console dos provedores através da API Rest, assim toda ação executada ou configurada nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada. A Ustore tem o compromisso de manter o desenvolvimento constante das suas Plataformas de Software e aplicar as melhores práticas (best practices) de DevOps vigentes no mercado de TI, na atualidade. Nosso compromisso versa na manutenção da compatibilidade de integração para que as mais recentes mudanças e implementações no console dos provedores, e de todos os softwares com os quais mantemos interoperabilidade, de forma que as novas funcionalidades estejam sempre disponíveis através da interface da Plataforma uCloud. Utiliza-se um conjunto de práticas e ferramentas projetadas para aumentar a capacidade de uma organização fornecer aplicativos e serviços mais rapidamente do que os processos tradicionais de desenvolvimento de software.

Acesso a Plataforma uCloud
==========================

O acesso à plataforma é feito através de um endereço de Internet, o usuário deve utilizar um navegador de Internet (Internet browser) e inserir o endereço da URL/link, assim o usuário visualiza a tela inicial de apresentação. Os navegadores de Internet compatíveis com a Plataforma uCloud são: Microsoft Edge versão 86.x, Google Chrome versão 85.x, Firefox verão 80.x ou Opera versão 71.x.

A Plataforma uCloud está adaptada para que sua interface seja apresentada nos idiomas **Português (nativo), Espanhol e Inglês**. Esta configuração é executada pelo próprio usuário. Em seu perfil é possível selecionar o idioma de apresentação da interface, sem a necessidade de alterar a configuração de idioma de sua sessão do navegador de internt (browser).

.. figure:: /figuras/ucloud_idioma_plataforma.png
   :alt: Idioma da Plataforma uCloud
   :scale: 50 %
   :align: center

----

.. attention::
    *Importante ressaltar que a Plataforma uCloud não é compatível com o Microsoft Internet Explorer (IE) em qualquer versão, pois as tecnologias deste navegador se encontram desatualizadas e não suportam a evolução das atuais páginas HTML.*

Após iniciar uma sessão de Internet browser, o endereço/caminho para o acesso a aplicação deve ser preenchido conforme exemplo abaixo, da seguinte forma:

- Link de exemplo com Endereço IP: ``http://<ucloudserverTCP_IP_Address>:80``

- Link de exemplo com Nome de Servidor: ``http://ucloud_Server_Name.com/``

Após entrar com o endereço corretamente, a tela do usuário será similar a figura abaixo:

.. figure:: /figuras/uCloud_acesso_platafform_001.png
   :alt: Tela de Login da Plataforma uCloud
   :align: center

----

As credenciais para o login e senha devem ter sido provisionadas previamente na Plataforma uCloud, por um usuário com perfil de Administrador (ou outro usuário com esta permissão).

O usuário deverá informar nos campos os seus dados de login e senha e clicar com o cursor do mouse sobre o botão Entrar.

Caso as credenciais de acesso não tenham sido provisionadas, não existam ou em último caso, o usuário não se recorde das corretas informações das suas credenciais, não terá acesso a plataforma. Ver o item Solicitação de Nova Senha, no caso de o usuário esquecer algum tipo de informação para proceder com o login de acesso à Plataforma uCloud.

Após inserir suas credenciais de acesso (nome do usuário e senha), efetuar o procedimento de login, ao usuário será apresentada a tela inicial da Plataforma uCloud.

.. figure:: /figuras/uCloud_acesso_platafform_002.png
   :alt: Dashboard uCloud
   :align: center

----

Siga para o próximo tópico para a descrição detalhada das características da tela inicial (Dashboard) da Plataforma uCloud.

Menu de Usuário
===============

A barra de menu do usuário fica localizada à esquerda da tela e, inicialmente, é apresentada no modo expandido, como na figura abaixo:
  
.. figure:: /figuras/uCloud_menu_usuario_001.png
   :align: center


Algumas opções de menu possuem um submenu, as quais são apresentadas quando o usuário posiciona o mouse sobre a indicação (sinal de menor “<”). Ao clicar sobre este ícone, a interface apresenta o submenu desta opção ao usuário, ver o exemplo na figura abaixo:

.. figure:: /figuras/uCloud_menu_usuario_002.png
   :align: center

----

É possível ao usuário optar pela redução da apresentação da barra de Menu do Usuário para o modo de Somente Ícones, para ter uma maior área de apresentação. Para alternar entre o Menu do Usuário Modo Expandido e o Menu do Usuário Modo Ícones, existe um elemento gráfico verde com três barras, de fácil identificação para o usuário. Este elemento estará presente em qualquer tela da Plataforma uCloud.
Quando o usuário clica sobre este elemento, a barra do Menu de Usuário será alternada para o Modo Ícones, conforme o exemplo na figura abaixo:

.. figure:: /figuras/uCloud_menu_usuario_003.png
   :align: center

----

Quando a barra de Menu do Usuário está em modo ícone, os submenus serão apresentados conforme a figura abaixo:

.. figure:: /figuras/uCloud_menu_usuario_004.png
   :align: center

----

O conteúdo abaixo detalha cada uma das opções do menu de usuário e suas respectivas funcionalidades.

Menu Administração 
==================

Ao apresentar alguns conceitos sobre o ambiente de administração do uCloud, é importante esclarecer alguns pontos sobre a Plataforma uCloud, nos conceitos existem três termos que serão amplamente utilizados no ambiente do uCloud.

* **Contrato**: é a forma com o qual se define a relação *comercial* entre o provedor e a empresa que o contratou. No contrato são definidos os custos, a margem financeira, taxa de conversão de moeda, custos de recursos (opcional) e a cota (limite) global que pode ser uma cota financeira ou uma cota de recursos computacionais.

* **Grupo**: é uma forma lógica definida unicamente dentro da Plataforma uCloud que pode definir um grupo de usuários (ex.: DevOps), um departamento (ex.: vendas), uma iniciativa (ex.: VDI), ao qual vários usuários estão associados sendo parte integrante deste grupo. Estes ‘grupos’ não existem nos provedores de nuvem (público e/ou privado) existem somente dentro da Plataforma uCloud.

* **Usuário**: Um usuário é a entidade que possui acesso identificado à Plataforma uCloud para efetuar ações nos recursos computacionais dos provedores (público e/ou privado).

A figura abaixo exemplifica, em uma imagem, a relação entre estes três termos e é primordial que o usuário utilize esta figura como referência para entender as relações.

.. figure:: /figuras/ucloud_arquitetura_conceitual001.png
   :align: center

----

É importante entender que um **Contrato** pode possuir vários grupos e cada *Grupo* pode conter vários *Usuários*. Entretanto, a Plataforma uCloud permite somente que um Usuário faça parte de apenas um grupo e um único Grupo esteja vinculado a exclusivamente um contrato.

A seguir, neste documento, será descrito que ao configurar as cotas (limites financeiros ou de recursos) do contrato, estes limites serão compartilhados/divididos por cada um dos grupos existentes e, por consequência, os usuários estão limitados às cotas do grupo ao qual estão incluídos.

É possível notar, na figura anterior, o termo Virtual Data Center (VDC) este termo é uma alocação lógica de máquinas virtuais que permite às organizações definir um (ou mais) grupo(s) de servidor(es) que faz(em) parte de uma nuvem. Um VDC pode representar um departamento, uma subsidiária ou um grupo de usuários. Veja mais informações no item Virtual Data Center.

A opção Administração apresenta campos que variam de acordo com o perfil do usuário que está acessando o sistema naquele momento. O uCloud possui cinco perfis diferentes.

#. **Usuários do sistema**: são os usuários regulares que acessam o sistema para consumir os recursos. Existe a possibilidade de *Usuários com perfil apenas de leitura*, que podem designar usuários regulares mas limitados em somente para acessar a Plataforma uCloud para visualizar as informações. 

#. **Usuários Administradores de Contrato**: são os usuários que estão associados a um contrato e sobre este contrato podem definir regras de bilhetagem, provisionar e alterar outros usuários na plataforma.

#. **Usuários Administradores de Grupo**: são usuários que estão associados a um grupo de usuários, eles podem provisionar e alterar outros usuários na plataforma.

#. **Usuários Gestores Financeiros**: usuários com perfil para acessar as informações financeiras do uCloud.

#. **Usuários Administradores**: São usuários com perfil de acesso total e podem efetuar intervenções globais nas configurações da plataforma. Este perfil de usuário é exclusivo da Ustore ou de um único perfil de usuário da organização que efetuou a aquisição das licenças da Plataforma uCloud. Este usuário administrador possui permissão para gerenciar todas as funcionalidades e recursos globais ofertados pela plataforma.

.. note::
  |atencao| *O Perfil Administrador não será coberto neste documento. Entre em contato com seu ponto focal na Ustore para obter o documento específico: Manual do Administrador da Plataforma uCloud. Por segurança, melhores práticas e por padrão, existe apenas um (01) usuário provisionado com este tipo de perfil*.

Switch Roles
------------

Quando um usuário de infraestrutura multi-nuvem precisa alternar entre diversos consoles de provedores de nuvem, o processo de login com diversas credenciais em diversos consoles gera um gasto de tempo e pode incorrer em erros de digitação de logins e senhas.

A plataforma do uCloud por ser um ambiente multi-nuvem permite que o usuário possa interagir com os recursos computacionais existentes em diversos provedores de nuvem diferentes de forma simultânea.

Ao iniciar uma sessão na Plataforma uCloud (login) o usuário obtém um conjunto específico de permissões para executar ações que pertencem ao contrato ao qual o usuário está vinculado. O(s) usuário(s) pertencem a um Grupo, e os Grupos pertencem a um contrato. Portanto, as credenciais de acesso do usuário estão vinculadas a um, ou mais, contratos, Este contrato pode estar provisionado para ter acesso a um (ou mais) credenciais de acesso aos ambientes dos provedores de nuvem pública e/ou privada.

Veja a figura abaixo, que demonstra a vinculação do usuário a um, ou mais, contratos:

.. figure:: /figuras/ucloud_arquitetura_conceitual001.png
   :align: center

----

O primeiro aspecto da figura acima é que podemos verificar que este cliente possui dois contratos diferentes. O **Contrato A** está associado a somente um provedor de nuvem pública (ex: **AWS**) e o **Contrato B** está associado a dois provedores de nuvem pública diferentes (ex: **AWS** e **Azure**).

Switch Roles - Cenário Exemplo
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Na figura acima podemos visualizar que os usuários Mariah, João e Carlos pertencem a somente um único contrato e este contrato possui somente um único provedor (ex: AWS).

O usuário **Josué** está associado a dois contratos diferentes e para evitar que este usuário tenha de alternar entre sessões de registro diferentes (encerrar uma sessão e iniciar outra com outra credencial), a Ustore desenvolveu e implementou a funcionalidade de **Switch Roles**.

Desta forma **apenas** o usuário Josué, através da funcionalidade de Switch Roles pode alternar entre os contratos aos quais ele está vinculado, simplesmente alternando entre os contratos aos quais ele está vinculado.

O usuário Josué é responsável pela total gestão da infraestrutura do ambiente Azure, porém, no ambiente da AWS, ele pode somente visualizar os recursos computacionais, pois não possui a permissão de operar estes recursos computacionais (ex: Read Only).

Através da funcionalidade Switch Roles será possível aplicar esta mudança de papel sem a necessidade de troca do usuário, isso será feito com um através da seleção de contrato e/ou container que este usuário deseja acessar.

Ainda para ilustrar este exemplo, com a nova implementação de Perfil de Permissionamento, seria possível criar diferentes conjuntos de permissões e vincular cada conjunto (Perfil de Permissionamento) a cada usuário e provisionar um nível de granularidade bem específico.

Cenário exemplo (AWS):
~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+---------+--------------------+-----------+
| Perfil de Permissionamento | Usuário | Virtual Datacenter | Permissão |
+============================+=========+====================+===========+
| AWS DevOps Full            | Maria   | DevOps             | Full      |
+----------------------------+---------+--------------------+-----------+
| AWS DevOps *Read Only*     | João    | DevOps             | Read Only |
| AWS Homolog Full           |         | Homolog            | Full      |
+----------------------------+---------+--------------------+-----------+
| AWS Homolog Full           | Carlos  |  Homolog           | Full      |
+----------------------------+---------+--------------------+-----------+
| AWS Infra Full             | Josué   | Infra              | Full      |
+----------------------------+---------+--------------------+-----------+

Atualmente é possível provisionar quatro (04) Perfis de Permissionamento diferentes e vincular cada perfil a um usuário específico.

No exemplo da tabela acima, é possível visualizar que o usuário João possui dois conjuntos de permissões diferentes que são específicas para cada conjunto de infraestruturas virtuais (Virtual Datacenter - VDC) que este usuário pode acessar. Vemos que o usuário João tem acesso irrestrito ao VDC Homolog, e somente visualização ao VDC DevOps.

Vejamos o exemplo do usuário Josué que possui características diferentes para cada contrato.

Cenário Exemplo (AZURE e AWS):
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

+----------------------------+---------+--------------------+-----------+
| Perfil de Permissionamento | Usuário | Virtual Datacenter | Permissão |
+============================+=========+====================+===========+
| Azure Infra RO             | Josué   | Infra Azure        | Read Only |
| AWS Infra Full             |         | Infra AWS          | Full      |
+----------------------------+---------+--------------------+-----------+

Este é um exemplo da simplicidade e da transparência que advém da ampliação e alteração do novo Perfil de Permissionamento, que permite vincular conjuntos de permissões diferentes ao mesmo usuário, que estão vinculados a contratos diferentes. Podemos verificar que o usuário *Josué* possui acesso irrestrito (*full*) para a infraestrutura do VDC Infra AWS (Contrato AWS) e acesso apenas leitura (*read only*) para o VDC Infra AZURE (Contrato Azure).

Anteriormente o usuário teria de ter duas credenciais diferentes (ex: `josue.aws/senhaABC` e `josue.azure/senha123`) e efetuar diversas sessões de login diferentes na Plataforma uCloud.

Com a combinação do novo Perfil de Permissionamento em conjunto da funcionalidade Switch Roles será possível aplicar esta mudança de tipos de permissões sem a necessidade de troca do usuário, isso será feito com um através da seleção de contrato e/ou container que este usuário deseja acessar.

Switch Roles - Utilizando
~~~~~~~~~~~~~~~~~~~~~~~~~

A funcionalidade de Switch Roles fica posicionada no canto superior direito da área de tela da Plataforma uCloud (ao lado do nome do usuário) - veja a tela abaixo:

.. figure:: /figuras/ucloud_dashboard_switch_roles001.png
   :align: center

----

Basta o usuário clicar com o cursor do mouse sobre o nome do contrato e a Plataforma uCloud apresenta uma janela pop-up que apresenta ao usuário a lista de contratos aos quais este está vinculado para que ele selecione o contrato desejado.

.. figure:: /figuras/ucloud_dashboard_switch_roles002.png
   :scale: 60 %
   :align: center

----

Ao selecionar o contrato desejado a Plataforma uCloud irá atualizar a informação apresentada no canto superior direito da sessão do usuário.
Importante ressaltar que essa janela pop-up lista somente os contratos aos quais o usuário está vinculado. Caso existam outros contratos provisionados na Plataforma uCloud, o usuário não terá acesso a nenhum destes outros contratos.

.. figure:: /figuras/ucloud_dashboard_switch_roles003.png
   :align: center

----

A funcionalidade Switch Roles possibilita a um usuário alternar tanto seu nível de acesso bem como obter acesso a diferentes contratos com diferentes regras de permissões para cada contrato sem ter de encerrar a sua sessão na Plataforma uCloud.
Com esta nova funcionalidade um único usuário poderá acessar, por exemplo, a nuvem Azure e a nuvem AWS com a possibilidade de ter responsabilidades, permissões e níveis de acesso completamente diferentes e específicos para cada um dos ambientes dos provedores de nuvem pública.
A personalização das permissões de atividades que o usuário poderá possuir será esclarecido no tópico Perfil de Permissionamento, neste documento.

Menu Administração / Usuários
-----------------------------

A Plataforma uCloud possui bancos de dados próprios que armazenam as informações dos usuários como login e senha de forma segura e criptografada. A tela inicial do Menu Administração apresenta a lista de usuários provisionados, a informação de login de um usuário, o grupo ao qual o usuário está associado e o tipo do seu perfil deste login.

De acordo com o tipo de perfil do usuário que está acessando o sistema, a Plataforma uCloud apresentará somente a relação de usuários que o perfil que está registrado e ativo pode gerenciar ou administrar.

.. figure:: /figuras/uCloud_menu_administracao_usuario_001.png
   :scale: 80 %
   :align: center

----

Para proceder com o acesso à Plataforma uCloud deve-se provisionar (cadastrar) um usuário com seu respectivo login e senha de acesso.

Abaixo estão descritas as colunas apresentadas nesta lista de usuários:

* **Botão Criar Usuário**: Quando selecionado este botão, o processo está descrito no item Criando Novo Usuário.

* **Login**: Esta coluna apresenta as credenciais de login do usuário. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de login de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Nome**: Esta coluna apresenta o nome do usuário que foi informado durante o processo do seu provisionamento na Plataforma uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Grupo**: Esta coluna apresenta o grupo principal do usuário que foi informado durante o processo do seu provisionamento na Plataforma uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Perfil**: Esta coluna apresenta o perfil do usuário que foi informado durante o processo do seu provisionamento na Plataforma uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de perfis de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Busca Rápida**: O usuário poderá observar que logo abaixo do nome de cada coluna existe um campo em ‘branco’, este campo permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de eventos de login. Basta preencher o campo em ‘branco’ com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualizará a tela de forma a representar este padrão de busca.

* **Coluna Perfil**: O campo de busca rápida, na coluna Perfil, possui um controle avançado em forma de um "*dropdownlist*" que permite aplicar um **filtro** de ‘tipo perfil’ para que a lista apresentada fique restrita somente à opção que foi selecionada. Para isto, basta clicar com o cursor do mouse neste campo, a Plataforma uCloud apresenta as opções de filtragem.

.. figure:: /figuras/uCloud_menu_administracao_usuario_002.png
   :align: center

----

Um usuário, provisionado, deve estar vinculado a apenas um dos seis **Tipos de Perfil** disponíveis, e esta definição decorre de qual função este usuário pode estar associado. Destes seis tipos, apenas *dois (02)* perfis (perfil *Usuário* e *Auditor*) são utilizados no dia a dia das operações na Plataforma uCloud.

O perfil **Auditor** tem uma função muito restrita, mas muito importante no controle e gerenciamento de custos do ambiente de recursos computacionais em nuvem (público e/ou privado).

O perfil **Usuário** é o mais fundamental e mais flexível, pois este pode assumir diferentes níveis de permissões e funções de operação, gerenciamento e administração do ambiente empresarial no uCloud.

Abaixo descrevemos os quatro tipos básicos de perfil de usuários na Plataforma uCloud:

* **Usuário**: é o perfil universal e todo outro perfil tem como premissa ser provisionado como um usuário da Plataforma uCloud e que deve estar vinculado a um grupo e está limitado as permissões (acesso a menus) e cotas (limites financeiros ou de recursos) que podem ser individuais ou compartilhadas do grupo. Importante ressaltar que qualquer outro perfil descrito abaixo, são variações deste perfil inicial.

  * Este usuário não possui permissão de alterar nenhuma das suas permissões, as quais foram estabelecidas durante o seu provisionamento. Apenas um usuário com perfil de Administrador de Grupo e/ou de Contrato, poderá redefinir os limites (cotas) e permissões deste perfil de usuário.

  * Este usuário está identificado na listagem com a marca (flag) gráfica: ``user``

* **Usuário Administrador de Contrato**: é um usuário, anteriormente provisionado, que está cadastrado no campo Administrador na tela de Contratos. Este perfil de usuário tem permissão de provisionar novos usuários bem como alterar alguns campos da tela de Contrato.

  * Este usuário possui permissão de alterar algumas das suas permissões estabelecidas durante o seu provisionamento, bem como alterar algumas das suas próprias permissões bem como as permissões de outros usuários. Apenas um usuário com perfil de Administrador de Grupo e/ou de Contrato, poderá redefinir os limites (cotas) e permissões deste perfil de usuário.

  * Este usuário está identificado na listagem com a marca (flag) gráfica: ``user`` - o termo User + uma estrela parcialmente preenchida - indica que este usuário é um Administrador de Contrato.

* **Usuário Administrador de Grupo**: é um usuário, anteriormente provisionado, que está cadastrado no campo Administrador do Grupo na tela de Grupos. Este usuário possui permissão de alterar algumas de suas permissões estabelecidas durante o seu provisionamento, bem como alterar algumas das suas próprias permissões bem como as permissões de outros usuários. Apenas um usuário com perfil de Administrador de Grupo e/ou de Contrato, poderá redefinir os limites (cotas) e permissões deste perfil de usuário.

  * Este usuário está identificado na listagem com a marca (flag) gráfica: ``user`` - o termo User + uma estrela não preenchida - indica que este usuário é um Administrador de Grupo.

* **Usuário Administrador de Contrato e Administrador de Grupo**: A Plataforma uCloud permite que um usuário possa estar associado como Administrador de um Grupo e, simultaneamente, Administrador de um Contrato este usuário está identificado na listagem com a marca (flag) gráfica: ``user``, e uma estrela estará completamente preenchida indicando que este usuário é um Administrador de Grupo e de Contrato.

  * Esta dupla associação de perfil, permite a este usuário um alto nível de controle e administração do ambiente da empresa 

* **Auditor**: é um usuário que tem acesso ao menu da Gestão Financeira e realiza o acompanhamento do faturamento do portal, bem como define as regras de precificação do contrato.

  * Este usuário, por premissa básica, não está associado a nenhuma permissão para operação e alteração de qualquer que sejam os recursos computacionais em qualquer provedor de serviço de nuvem (público e/ou privado). Este perfil tem acesso unicamente a análise financeira e de custos do contrato ao qual este usuário está vinculado, por intermédio de um grupo.
  * Este usuário está identificado na listagem com a marca (flag) gráfica: ``Auditor``, o termo indica que este usuário é um Auditor do Contrato.

Os outros quatro perfis (Administrator, Service, VDI User, VDI Administrator) são perfis internos da Plataforma uCloud, não serão cobertos neste documento. Entre em contato com seu ponto focal na Ustore para obter os documentos específicos: Manual do Administrador da Plataforma uCloud e Manual do Ambiente VDI Ustore.

Visualizando um Usuário
-----------------------
Na listagem de usuários é possível visualizar as informações de um usuário,  basta clicar com o mouse sobre a linha na qual o usuário se apresenta, a Plataforma uCloud exibirá a tela com todas as informações do usuário provisionado na plataforma. Nesta tela é possível adicionar novas configurações ao perfil de um usuário. A tela de visualização de detalhes de um usuário está dividida em seções e será descrita abaixo:

.. figure:: /figuras/uCloud_menu_administracao_usuario_003.png
   :scale: 60 %
   :align: center

----

* **Seção Geral**: A primeira seção desta tela apresenta os dados gerais do perfil do usuário provisionado na Plataforma uCloud. Por meio desta tela será possível alterar alguns campos referentes ao usuário.

  * **Botão de Excluir Usuário**: Este botão pode ser usado para remover o usuário provisionado na Plataforma uCloud de forma definitiva e irreversível. Basta o usuário clicar com o cursor do mouse sobre o botão, e será apresentada a tela solicitando a confirmação da ação, conforme a tela abaixo:

.. figure:: /figuras/uCloud_menu_administracao_usuario_004.png
   :align: center

----

Após a confirmação da Exclusão do usuário, este usuário e suas credenciais de acesso ficam indisponíveis imediatamente de forma irreversível, não sendo possível recuperar as informações deste usuário. Se a exclusão for acidental, este usuário deverá ser provisionado novamente.

  * **Ícone de Edição Ativo** |icone_edita_on|: Todos os campos que possuem o ícone de edição ativo são passíveis de terem seu conteúdo altera.

  * **Ícone de Edição Inativo** |icone_edita_on|: Todos os campos que possuem o ícone de edição inativo ou não são passíveis de terem seu conteúdo alterado através desta tela (ex.: valores das cotas de grupo) ou o perfil do usuário que está registrado e acessando esta tela, não possui permissão para alterar o conteúdo do(s) campo(s).

  * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma uCloud.

  * **Ícone de Cancelamento** |icone_cancela_vermelho|: Caso o usuário tenha clicado sobre o ícone de edição por engano ou não deseja que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna para os valores iniciais, antes de proceder qualquer preenchimento ou alteração.

  * **Barra de Rolagem**: Esta seção possui um grande conjunto de campos, para a completa visualização de todos o usuário deve utilizar a barra de rolagem ao lado direito desta seção. Se o usuário rolar o mouse, a tela desce e apresenta os campos que não estavam sendo visualizados, conforme a tela abaixo:

  * **Login**: Este campo apresenta a forma como a credencial do usuário foi provisionada na Plataforma uCloud. Importante ressaltar que o conteúdo deste campo **não é passível de alteração**. Será necessário remover (apagar) este usuário e em seguida efetuar um novo provisionamento com a informação de identificação de credencial preenchida da forma desejada.

  * **Nome**: Este campo apresenta a nome completo do usuário que corresponde a credencial apresentada acima, conforme foi informado no momento de seu provisionamento.

  * **Senha**: Este campo é obrigatório e deve ser preenchido com a sequência de caracteres da senha do usuário. Importante ressaltar que esta sequência deve ser maior do que oito (08) caracteres alfanuméricos. Deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”, conforme a documentação encontrada no site da Azure. A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres e deve conter caracteres de três das seguintes categorias:

    * Letras maiúsculas e minúsculas (A a Z)
    * Números de base 10 (de 0 a 9)
    * Caracteres não alfanuméricos (caracteres especiais): ~ ! @ # $ % ^ & * - + = ' | \ \ () {} \ [ ] : ; " ' < > , . ? /

.. note:: Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são válidos como caracteres especiais para essa configuração de política.

    Por padrão, somente o próprio usuário pode alterar sua própria senhas. Estando em uma sessão ativa o usuário pode alterar sua própria senha, clicando com o cursor do mouse sobre a identificação de seu usuário, no canto superior direito da tela da Plataforma uCloud e logo em seguida clicar com o cursor do moue sobre o texto **Configurações da Conta**, conforme a tela abaixo:

.. figure:: /figuras/ucloud_menu_administracao_usuario_004b.png
   :align: center

----

  Para os casos que o usuário não recorde de sua senha de acesso, o usuário deverá clicar com o cursor do mouse sobre a opção **Esqueceu sua Senha?** e seguir o processo de Solicitação de Nova Senha descrito acima.

.. figure:: /figuras/uCloud_acesso_platafform_001.png
   :alt: Tela de Login da Plataforma uCloud
   :align: center

----

  * **Idioma**: Este campo é do tipo "dropdown" e permite ao usuário trocar o idioma da interface da Plataforma uCloud. Basta clicar com o cursos do moue sobre este campo (em modo edição ativa) para apresentar as opções de idiomas **Português (nativo), Espanhol e Inglês**. Basta selecionar o idioma desejado que a Plataforma uCloud altera a interface de forma imediata.

.. figure:: /figuras/ucloud_idioma_plataforma.png
   :alt: Idioma da Plataforma uCloud
   :scale: 50 %
   :align: center

----

  * **Telefone**: Este campo não é obrigatório, e pode ser utilizado para armazenar o número de telefone (fixo ou móvel) do usuário. Este é uma informação apenas para consulta, a Plataforma uCloud não possui qualquer integração com plataformas de telefonia pública, privada ou móvel e deve ser preenchido com um número de telefone fixo ou do serviço móvel celular, utilizando o seguinte formato:

    * **dois (02)** números que identificam o código de área do número de telefone fixo ou de serviço móvel celular (XX). Não é necessário informar o número "zero (0)" que antecede ao código de área no padrão brasileiro.
    * **oito (08)/nove (09)** números que identificam o número de telefone fixo ou do serviço móvel celular do usuário. Não é necessário informar qualquer outro caractere para separação dos grupos de números de telefone serviço móvel celular.
    * Exemplo de preenchimento: ´´11999991234´´

  * **Correio Eletrônico**: Este campo é obrigatório, nele deve ser informado um endereço de correio eletrônico (e-mail) válido. Este endereço de correio eletrônico será fundamental durante o processo de redefinição de senha pelo usuário, pois a Plataforma uCloud utiliza este e-mail para o envio de uma mensagem que permite ao usuário criar uma senha, para ele, de forma automática. Adicionalmente a plataforma uCloud para o referido correio eletrônico uma mensagem para o processo de validação de **DUPLO FATOR DE AUTENTICAÇÃO**.

  * **Cargo**: Este campo não é obrigatório, seu conteúdo é meramente informativo para identificar o cargo do usuário que se deseja provisionar.

  * **Apenas Leitura** : Este campo configura um usuário que não tem permissão de efetuar nenhuma ação através da Plataforma uCloud, mas seu login está ativo e ele possui a capacidade de visualizar todas as telas, as quais ele tenha permissão.

    * Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o seu perfil permita proceder a alteração. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.
  
  * **Autenticação Multifator**: Este campo indica se este usuário terá seu processo de autenticação na plataforma (login) sendo verificado duplamente, antes de aprovar que este usuário tenha acesso a Plataforma uCloud. Para isto ocorrer, será enviada uma mensagem para o endereço de correio eletrônico do usuário.

    * Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o seu perfil permita proceder a alteração. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.
  
  * **Ativar Cota de Faturamento**: Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o perfil permita alterar. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.

  * **Aprovação do Administrador**: Este campo configura que todas as ações e solicitações efetuadas na interface da Plataforma uCloud, deste usuário, deverão ser aprovadas por um usuário Administrador do Grupo. Esta é uma funcionalidade para aumentar o controle de governança de custos e operações.

    * Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o perfil permita alterar. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.


.. note:: Importante ressaltar que a Plataforma uCloud não efetua qualquer validação prévia referente a existência do e-mail informado ou seu efetivo funcionamento. No caso de inexistência do e-mail destino, ou erro em sua digitação, o usuário ficará impossibilitado de executar a redefinição da sua senha de acesso. Neste caso deverá contactar o administrador do seu grupo/contrato.


* **Seção Permissões do Usuário**: Quando o usuário é criado ele herda/recebe todas as permissões definidas no Grupo ao qual ele pertence (ver próxima seção), bem como as permissões estabelecidas no Contrato. Esta tabela é opcional, mas permite adicionar, ou revogar, as permissões que este usuário possui para efetuar ações, ou acessar menus, na Plataforma uCloud.

  * **Botão Editar** : Para acrescentar ou revogar permissões para o usuário, o Administrador (ou usuário com autorização) deve clicar neste botão para que a Plataforma uCloud possa apresentar a tela que seja possível realizar o procedimento de adicionar ou excluir permissões específicas para este usuário. Veja exemplo abaixo:
  Esta tela possui duas colunas distintas;

  À esquerda são as permissões previamente adicionadas ao usuário. Ao lado de cada permissão existe um campo do tipo “check box” que ao ser selecionado exclui (revoga) a respectiva permissão deste usuário.

  À direita estão as permissões disponíveis na Plataforma uCloud que podem ser adicionadas ao perfil individual deste usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, adiciona a respectiva permissão deste usuário.

    * **Utilizar as permissões padrões**: Ao selecionar este campo “check box”, e confirmar a ação, o usuário receberá todas as permissões de usuário disponíveis na Plataforma uCloud.

    * **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o mouse no botão Aplicar para confirmar as alterações - de forma definitiva e imediata - para o usuário que está visualizando/alterando. Terminada esta ação a Plataforma uCloud fechará esta tela e retorna à tela anterior, com seu conteúdo atualizado, apresentando a nova relação de permissões do usuário.

* **Seção Políticas de Permissionamento do Usuário (eventual)**: Esta seção somente será apresentada para usuários que foram provisionados na Plataforma uCloud com o "checkbox" Criar Usuário na Nuvem habilitado. Esta seção apresenta todas as políticas de permissionamento únicas e específicas do ambiente do provedor de serviço de nuvem pública. Estas políticas são ‘importadas’ durante o processo de sincronização do container, e permitem um alto nível de controle granular das capacidades (permissões) que o usuário pode efetuar dentro do ambiente do provedor de serviço de nuvem. Quando o usuário é recém provisionado, este pode estar associado a nenhuma política de permissionamento, será necessário configurar manualmente as permissões.

  * **Botão Editar**: Este botão permite ao usuário Administrador (ou usuário com autorização) acrescentar ou revogar políticas de permissionamento do ambiente do provedor de serviço de nuvem. Para isto, ele deve clicar no botão ‘Editar’ a partir daí será permitido ao usuário administrador adicionar ou excluir permissões específicas para o usuário desejado. Veja exemplo abaixo:

  * À esquerda são as políticas de permissionamento previamente adicionadas ao usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, exclui (revoga) a respectiva permissão deste usuário.

  * À direita estão as políticas de permissionamento disponíveis do ambiente do provedor de serviço de nuvem pública que podem ser adicionadas ao perfil individual deste usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, adiciona a respectiva permissão deste usuário.
  
  * **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação, a Plataforma uCloud fechará esta tela e retornará à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.
   
* **Seção Permissões do Grupo**: Esta seção somente apresenta as permissões que foram definidas nas configurações do Grupo ao qual este usuário está vinculado. A Plataforma uCloud não permite que as permissões listadas aqui possam ser alteradas através desta tela. Para ter contato e conhecer as permissões definidas no grupo, veja o item Administração / Grupos. Se forem necessárias alterações de qualquer permissão listadas aqui, estas alterações devem ser efetuadas nas configurações do Grupo.

* **Seção Grupos Secundários**: Nesta seção é possível associar um usuário a mais de um grupo na Plataforma uCloud. Na seção Geral, é possível verificar o Grupo principal ao qual o usuário está vinculado.

   * **Botão Editar**: Para vincular este usuário a um grupo secundário, ou desvincular este usuário de um grupo secundário, o Administrador (ou usuário com autorização) deve clicar neste botão Editar para que a Plataforma uCloud possa apresentar a tela que permite desvincular o usuário de grupos secundários. Veja exemplo abaixo:

   * À direita estão listados os grupos que estão vinculados ao contrato do grupo principal ao qual este usuário foi provisionado originalmente. A Plataforma uCloud lista somente os grupos que estão vinculados ao contrato vigente. Ao lado de cada grupo existe um campo do tipo “check box” que, quando selecionado, vincula o grupo selecionado a este usuário.

   * À esquerda estão listados os grupos secundários que este usuário está vinculado. Ao lado de cada grupo existe um campo do tipo “check box” que, quando selecionado, desvincula o grupo selecionado deste usuário.

   * **Botão Aplicar**: Após certificar que todas as vinculações, ou remoção, foram configuradas, o usuário deve clicar no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação a Plataforma uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

* **Seção Perfis de Visualização**: Esta seção permite que o administrador do contrato possa selecionar quais opções do Menu do Usuário, este usuário poderá visualizar. Através desta funcionalidade, o administrador pode personalizar como este usuário interage com a Plataforma uCloud. É possível acompanhar o processo de definição destes perfis no item Configurações / Perfis de Visualização. Esta configuração retira ou adiciona as opções da barra de Menu de Usuário, de forma que para o usuário não há como saber que tal função existe. A possibilidade de saber, seria acompanhar outro usuário utilizando a plataforma com outras opções de Menu de Usuário visíveis.

* **Botão Adicionar**: Para adicionar este usuário a um perfil de visualização, ou desvincular este usuário de um grupo secundário, o Administrador (ou usuário com autorização) deve clicar neste botão Adicionar para que a Plataforma uCloud possa apresentar a tela que possibilita associar o usuário a um dos perfis de visualização configurados na plataforma. Veja exemplo abaixo:

  * Pode-se informar parte do nome de um grupo e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma uCloud apresente uma lista com todos os grupos que possuem a mesma sequência de caracteres informados. Este campo é sensível a maiúsculas e/ou minúsculas, somente irá listar os Perfis de Visualização que combinam exatamente com a parte do texto que foi digitado (se nada for listado, digitar o texto com outra combinação de maiúsculas e ou minúsculas.

  * **Botão Salvar**: Após certificar que vinculou o usuário ao Perfil de Visualização correto, o usuário deve clicar com o botão do mouse no botão Salvar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação a Plataforma uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

.. note:: |atencao| *Importante ressaltar que os perfis listados na tela exemplo não existem e foram criados apenas para fins ilustrativos.*

* **Seção Últimos Logins**: Nesta seção serão listados todos os eventos em que este usuário se conectou (login) na Plataforma uCloud. Veja a tela exemplo abaixo:

   * **Data do Login**: Este campo apresenta a data e a hora em que o usuário inicia uma sessão na Plataforma uCloud, utilizando o seu login. A informação está apresentada no formato de data no padrão brasileiro (Dia/Mês/Ano Hora:Minuto:segundo).

   * **Data de Logout**: Este campo apresenta a data e a hora em que o usuário encerra uma sessão na Plataforma uCloud, utilizando o seu login. A informação está apresentada no formato de data no padrão brasileiro (Dia/Mês/Ano Hora:Minuto:segundo).

   * **Tempo da Sessão**: Este campo apresenta o total de tempo que este login de usuário permanecer conectado a Plataforma uCloud, no formato de horas, minutos e segundos (ex.: 6h 18m 33s).

   * **IP Remoto**: Este campo apresenta o número do endereço TCP-IP o qual o usuário estava associado, quando iniciou a sessão com a Plataforma uCloud.

   * **Busca Rápida**: O usuário pode notar que logo abaixo do nome de cada coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de eventos de login. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualizará a tela de forma a representar este padrão de busca.

* **Seção Máquinas Virtuais**: Esta seção apresenta uma lista das máquinas virtuais (VMs) ou cargas de trabalho (workloads) que foram criadas por este usuário, durante uma sessão ativa na Plataforma uCloud.

   * **Busca Rápida**: O usuário pode notar que logo abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de máquinas virtuais (VMs) deste usuário. Basta preencher o campo em branco com uma sequência de caracteres que possa ser relevante e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca.

Criando Novo Usuário
--------------------

Antes de tratar da criação de um usuário é importante estabelecer que para a Plataforma uCloud um Usuário está vinculado a um Grupo e um Grupo está vinculado a um Contrato [Usuário<Grupo<Contrato].

Desta forma, antes de iniciar a criação de um novo usuário, é importante verificar a existência do grupo ao qual este usuário será associado. Para criar um usuário é necessário selecionar a opção **Criar Usuário** conforme indicado abaixo.

.. figure:: /figuras/uCloud_menu_usuario_022.png
   :align: center

----

A seguir a descrição do correto preenchimento dos campos desta tela, para provisionar um usuário na Plataforma uCloud, são eles:

* **Grupo**: Este campo é obrigatório e o usuário deve informar um grupo previamente provisionado na Plataforma uCloud, pois não será possível continuar o cadastramento de um usuário sem vincular este novo usuário a um grupo existente.

.. figure:: /figuras/uCloud_menu_usuario_017.png
   :align: center

----

   * Pode-se informar parte do nome de um grupo e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo:

   * Quando encontrado o Grupo ao qual este novo usuário deverá estar vinculado, basta selecioná-lo e o campo se preencherá com o grupo específico.

   * *Importante ressaltar que será possível associar este usuário a mais de um grupo, caso seja necessário. Mas estes grupos devem estar vinculados a somente um único Contrato.*

* **Nome**: Este campo é obrigatório e deve ser preenchido com o nome do usuário que se está provisionando.

* **Login**: Este campo é obrigatório e deve ser preenchido com a sequência de caracteres que será utilizada para identificar o usuário durante o processo de login no uCloud.

* **Senha**: Este campo é obrigatório e deve ser preenchido com a sequência de caracteres da senha do usuário. Importante ressaltar que esta sequência deve ser maior do que quatro (04) caracteres alfanuméricos. Deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”, conforme a documentação encontrada no site da Azure. A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres e deve conter caracteres de três das seguintes categorias:

   * Letras maiúsculas e minúsculas (A a Z)
   * Números de base 10 (de 0 a 9)
   * Caracteres não alfanuméricos (caracteres especiais): ~ ! @ # $ % ^ & * - + = '| \ \ ( ) { } \ [ ] : ; " ' < > , .? /

.. note:: Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política.

* **Confirmar Senha**: Este campo é obrigatório e deve ser preenchido com a mesma sequência de caracteres informados no campo anterior. Caso a sequência informada neste campo seja diferente da anterior, será apresentado um pop-up com uma mensagem de erro na tela.

.. figure:: /figuras/uCloud_menu_usuario_018.png
   :alt: Menu de Usuário
   :align: center

----

.. attention:: A Plataforma uCloud **não efetua** qualquer validação prévia referente a existência do e-mail informado ou seu efetivo funcionamento. No caso de inexistência do e-mail destino, ou erro em sua digitação, o usuário ficará impossibilitado de executar a redefinição da sua senha de acesso. Neste caso deverá contactar o administrador do seu grupo/contrato.

* **Email**: Este campo é obrigatório, nele deve ser informado um endereço de correio eletrônico (e-mail) válido. Este endereço de correio eletrônico será fundamental durante o processo de redefinição de senha pelo usuário, pois a Plataforma uCloud utiliza este e-mail para o envio de uma mensagem que permite ao usuário criar uma senha, para ele, de forma automática.

* **Telefone**: Este campo é obrigatório, e deve ser preenchido com um número de telefone fixo ou de serviço móvel celular, utilizar o seguinte formato:

   * **Dois (02)** números que identificam o código de área do número de telefone fixo ou de serviço móvel celular (XX). Não é necessário informar o número ‘zero (0)’ que antecede ao código de área no padrão brasileiro.
   * **oito(08/)nove (09)** números que identificam o número de telefone fixo ou do serviço móvel celular do usuário. Não é necessário informar qualquer outro caractere para separação dos grupos de números de telefone serviço móvel celular.
   * Exemplo de preenchimento: `(11)999991234`

* **Cargo**: Este campo é obrigatório, mas é meramente informativo para identificar o cargo do usuário que se deseja provisionar.

* **Empresa**: Este campo é obrigatório, mas é meramente informativo para identificar a organização a qual este usuário está associado.

* **Tipo de Cota**: Este campo é obrigatório, trata-se de um campo do tipo “drop down list”, quando o usuário clicar sobre este será apresentada a lista das opções de tipos de cota disponíveis para provisionar um usuário, veja as opções abaixo:

.. figure:: /figuras/uCloud_menu_usuario_019.png
   :alt: Tipo de Cota de Usuário
   :align: center

----

* **Cota de Grupo**: Quando selecionada esta opção o usuário compartilha dos limites (cotas) financeiros ou de recursos computacionais que estão definidos nas configurações do Grupo. Usuários com cota de grupo devem ficar atentos nas informações apresentadas na tela inicial (dashboard – veja item Dashboard) uma vez que a Plataforma uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites disponíveis no grupo ao qual o usuário está vinculado.

* **Cota de Usuário**: Quando selecionada esta opção pelo usuário, a Plataforma uCloud solicita que sejam informados os limites (cotas) financeiros ou de recursos computacionais específicos e individuais para este usuário, conforme a tela abaixo;
 
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

* Quando um usuário se registra, ele deve observar as informações apresentadas na tela inicial (dashboard – veja item Dashboard) pois a Plataforma uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites definidos para este usuário.

.. note:: |atencao| *Usuários com cotas individuais: esta cota individual será subtraída (retirada) da cota do Grupo ao qual este usuário está vinculado*.

* **Habilitar Primeiro Acesso**: Este campo é um campo opcional do tipo de seleção  “check box”, que permite que o usuário possa alterar sua senha de acesso no primeiro acesso deste usuário a Plataforma uCloud. Quando selecionado, a Plataforma uCloud irá apresentar um ‘pop-up’ solicitando ao usuário informar uma nova senha, para substituir a senha inicialmente provisionada para este usuário,

----
.. warning:: A Plataforma uCloud não irá permitir que o usuário inicie uma sessão ativa sem antes o usuário substituir a senha originalmente informada. Após o usuário informar a nova senha, será armazenada de forma encriptada nas bases de dados internas, neste momento a sessão do usuário se torna ativa para iniciar a o uso da Plataforma uCloud normalmente.
----

* **Ativar Autenticação Multifator**: Este campo é um campo de seleção “check box” que indica se este usuário terá seu processo de autenticação na plataforma (login) sendo verificado duplamente antes de aprovar que este usuário tenha acesso a Plataforma uCloud. Será enviada uma mensagem para o correio eletrônico informado no campo **e-mail** com um link/url para o usuário confirmar a segunda etapa de autenticação.

* **Ativar cota de Faturamento**: Este campo é um campo de seleção “check box” que indica se este usuário terá seu faturamento computado constantemente na relação de consumo de Faturamento (ver item Financeiro).

* **Administrador precisa aprovar a realização de atividades**: Este campo é um campo de seleção "checkbox" que indica todas as ações e solicitações efetuadas na interface da Plataforma uCloud, elas devem ser aprovadas por um usuário Administrador do Grupo. Esta é uma funcionalidade destinada a aumentar o controle de governança de custos e operações.

  * Na prática, qualquer novo recurso computacional (uma nova máquina virtual) que este usuário solicitar através da interface do uCloud: a solicitação não será enviada para o provedor de serviço de nuvem (público e/ou privado) de forma imediata, a solicitação ocorrerá em 2 tempos. No primeiro momento, ela aguarda a aprovação do Administrador do Grupo. No segundo tempo, após a aprovação do administrador do grupo (se aprovada) a solicitação segue no processo de criação/alteração solicitada por este usuário.

* **Criar Usuário na Nuvem**: Este campo é um campo de seleção "checkbox" que indica as credenciais de login e senha deste usuário (informadas acima), elas serão enviadas ao provedor de serviço de nuvem pública para que seja provisionado um usuário com as mesmas credenciais de acesso no provedor de serviço de nuvem pública selecionado abaixo.

   * **Containers**: Este campo é obrigatório e do tipo “Dropdown” quando o usuário clica com o cursor do mouse, a Plataforma uCloud lista todos os containers configurados na Plataforma uCloud. O usuário deve selecionar um provedor da lista.

.. figure:: /figuras/uCloud_menu_usuario_021.png
   :alt: Menu de Usuario
   :align: center

----

* **Permissões**: O usuário recebe/herda todas as permissões definidas no Grupo ao qual ele pertence, bem como as permissões estabelecidas no Contrato e por último as permissões específicas deste usuário. Esta tabela é opcional, ela permite adicionar ou revogar as permissões que este usuário recebe, o que permite efetuar ações ou acessar menus na Plataforma uCloud. São cento e trinta e duas (132) permissões disponíveis que podem ser associadas ao usuário (todas ou apenas uma parte). Qualquer alteração efetuada nas permissões disponíveis (inclusão ou revogação) será aplicada de forma imediata no login deste usuário após a confirmação. Veja o item Configurações / Perfis de Permissionamento para uma forma alternativa de criar grupos de permissões customizados para sua empresa.

   * **Botão Criar**: Após todos os campos obrigatórios e opcionais para provisionar o novo usuário estarem preenchidos o usuário pode clicar com o cursor do mouse no botão verde Criar, assim a Plataforma uCloud provisiona o novo usuário em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, significa que algum campo obrigatório permanece sem preenchimento (o usuário deve checar e corrigir) ou a sequência de caracteres da senha do login deve ser inferior a quatro (04) caracteres.

Administração / Grupos
----------------------

Na Plataforma uCloud, o termo Grupo estabelece um conceito que permite alocar uma determinada quantidade de recursos computacionais, ou recursos financeiros, que poderão ser consumidos por todos os usuários que estão vinculados ao grupo, criando assim uma pequena ‘célula’ de governança financeira. A Plataforma uCloud pode conter diversos Grupos para que a governança financeira fique mais próxima do cenário real da organização.

Importante ressaltar que o conceito de ""Grupos" existe somente para a Plataforma uCloud e não existe nada similar nos provedores de serviço de nuvem pública ou privada.

Um Grupo de usuários pode ser um Departamento, uma Unidade de Negócio, um Centro de Custos, uma Filial. Quando se define um limite de quantidade de recursos computacionais ou um limite financeiro para um grupo, significa que a Plataforma uCloud registra este limite.

Se este recurso ultrapassar os limites estabelecidos para o grupo, da parte de qualquer usuário vinculado a este grupo, a Plataforma uCloud nega (bloqueia) a criação ou alteração de determinada quantidade de recurso computacional, uma vez que este novo recurso computacional não poderá ultrapassar estes limites.

Estes limites podem ser ajustados a qualquer momento (aumento ou redução) da parte dos usuários com perfil de Administrador de Grupo ou Administrador de Contrato, apenas eles estão habilitados para alterar os valores limites (cotas) estabelecidos no grupo.

.. figure:: /figuras/uCloud_menu_grupo_001.png
   :alt: Menu de Usuario
   :align: center

----

A seguir a descrição das colunas apresentadas nesta lista de grupos:

* **Botão Criar Grupo**; Quando selecionado este botão o processo está descrito no item.

* **Nome**: Esta coluna apresenta o nome do Grupo. Como forma de simplificar a visualização, é possível clicar com o botão do mouse no título desta coluna, o resultado apresentado na Plataforma uCloud apresenta a classificação da lista de grupos de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Contrato**: Esta coluna apresenta o nome do Contrato ao qual este grupo está associado. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no nome do contrato de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Admin**: Esta coluna apresenta o nome do login de usuário que foi associado no campo de Administrador do Grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no nome do login de usuário de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Cota de CPU**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de CPU que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no valor da quantidade de CPU de forma crescente ou decrescente.

* **Cota de Memória**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Memória que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no valor da quantidade de memória de forma crescente ou decrescente.

* **Cota de Disco**: Esta coluna apresenta o número inteiro que representa o limite (cota) valor total de Disco de Armazenamento que foi definido para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no valor total do Disco de Armazenamento de forma crescente ou decrescente.

Visualizando Grupo
------------------

Estando na listagem de grupos é possível visualizar algumas informações de um grupo, para isto, basta clicar com o mouse sobre a linha à qual um grupo faz parte e a Plataforma uCloud apresentará a tela com todas as informações de um grupo provisionado na plataforma. Através desta tela é possível adicionar novas configurações ao perfil de um usuário.

A tela de visualização de detalhes de um usuário está dividida em seções, descrita abaixo;

.. figure:: /figuras/uCloud_menu_grupo_002.png
   :alt: menu de usuário
   :align: center

----

* **Botão de Excluir Grupo** Este botão pode ser usado para remover o grupo provisionado na Plataforma uCloud de forma definitiva e irreversível. Basta o usuário clicar com o cursor do mouse sobre o botão, e será apresentada uma tela solicitando a confirmação da ação, conforme a tela abaixo;

.. figure:: /figuras/uCloud_menu_grupo_003.png
   :alt: menu de usuário
   :align: center

----

* Após a confirmação da Exclusão do grupo, este grupo e as configurações associadas a este estarão indisponíveis imediatamente de forma irreversível, não sendo possível recuperar as informações deste grupo. Se a exclusão for acidental, este usuário deverá ser provisionado novamente.

.. warning:: A Plataforma uCloud não permite remover um grupo quando existem ainda usuários vinculados ao grupo. Antes de excluir um grupo da plataforma certifique que todos seus usuários foram desvinculados do referido grupo para que seja possível a remoção do grupo seja definitiva.
	
* **Seção Geral**: Esta seção da tela apresenta as informações sobre o grupo que está provisionado e os campos apresentados nesta seção podem ter seu conteúdo alterado através desta tela. O que define a condição de alteração está relacionado com o ícone de edição a seguir;

   * **Ícone de Edição Ativo**: Todos os campos que possuem o ícone de edição ativo são passíveis de ter seu conteúdo alterado.

   * **Ícone de Edição Inativo**: Todos os campos que possuem o ícone de edição inativo ou não são passíveis de terem seu conteúdo alterado através desta tela (ex.: valores das cotas de grupo) ou o perfil do usuário que está registrado e acessando esta tela, não possui permissão para alterar o conteúdo do(s) campo(s).

   * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma uCloud.

   * **Ícone de Cancelamento** |icone_cancela_vermelho|: Caso o usuário tenha clicado sobre o ícone de edição por engano, ou não deseja que as alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho, para cancelar as alterações e o conteúdo do campo irá retornar para os valores iniciais, antes de qualquer preenchimento ou alteração.

* **Seção Permissões**: O Grupo recebe (herda) todas as permissões definidas no Contrato ao qual este grupo está vinculado. Esta tabela é opcional, mas permite adicionar ou revogar as permissões que este grupo possui para efetuar ações ou acessar menus na Plataforma uCloud.

.. figure:: /figuras/uCloud_menu_grupo_004.png
   :alt: menu de usuário
   :align: center

----

   * **Botão Editar**; Para acrescentar ou revogar permissões para o usuário Administrador do Grupo (ou usuário autorizado com perfil semelhante ao administrador), basta clicar neste botão para que a Plataforma uCloud apresente a tela para adicionar ou excluir permissões específicas para este grupo.

.. figure:: /figuras/uCloud_menu_grupo_005.png
   :alt: menu de usuário
   :align: center

----

Abaixo descreveos os campos desta tela:

* Esta tela possui duas colunas distintas, à esquerda são as permissões definidas no Contrato que são repassadas para o Grupo vinculado ao contrato. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, exclui (revoga) a respectiva permissão deste usuário.

* À direita estão as permissões disponíveis na Plataforma uCloud que podem ser adicionadas ao grupo. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, adiciona a respectiva permissão deste usuário.

* **Utilizar as permissões padrões**: Ao selecionar este campo “checkbox”, e confirmar a ação, o Grupo receberá todas as permissões disponíveis na Plataforma uCloud.

* **Botão Aplicar**: Após o usuário certificar-se de que todas as alterações necessárias foram configuradas (inclusões ou exclusões),ele deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o grupo que se está alterando. Após esta ação a Plataforma uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

* **Seção Virtual Data Center**: Nesta seção são listados todos os Virtual Data Centers (VDC) associados a este grupo. Um Virtual Data Center é um agrupamento ‘lógico’ de determinados recursos computacionais de nuvem (templates, flavors, redes, regiões globais, storage e máquinas virtuais) que possibilita um controle de governança financeira para a empresa. O usuário vinculado a este grupo, que possui um (ou mais) Virtual Data Center, somente poderá consumir os recursos computacionais disponíveis neste Virtual Data Center. Para mais informações veja no item Menu Virtual Data Center.

.. figure:: /figuras/uCloud_menu_grupo_006.png
   :alt: menu de usuário
   :align: center

----

* **Botão Editar** |botao_editar|; Para vincular um Grupo a um Virtual Data Center, o usuário Administrador do Grupo (ou usuário com autorização) deve clicar neste botão para que a Plataforma uCloud possa apresentar a tela para adicionar ou excluir um Virtual Data Center vinculado a este grupo.

.. figure:: /figuras/uCloud_menu_grupo_007.png
   :alt: menu de usuário
   :align: center

----

* Esta tela possui duas colunas distintas, à esquerda estão apresentados os Virtual Data Centers (VDCs) que foram vinculados a este Grupo (no momento do seu provisionamento). Ao lado de cada VDC existe um campo do tipo “checkbox” , ao selecioná-lo a Plataforma uCloud exclui (desvincula) o VDC deste grupo.

* À direita estão apresentados os Virtual Data Centers (VDCs) que estão vinculados ao contrato deste, ao qual este grupo pertence e que permite ser vinculado a este Grupo. Ao lado de cada VDC existe um campo do tipo “checkbox” , quando selecionado, vincula o VDC ao Grupo.

* **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o grupo que se está alterando. Após esta ação a Plataforma uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

* **Coluna Ações / Botão Kick-Off** ; Este botão permite desvincular o Virtual Data Center do Grupo em uma ação. Basta o usuário clicar com o mouse no botão Kick-Off para que o VDC seja desvinculado do Grupo, de forma definitiva e imediata, para o grupo que se está alterando. Importante ressaltar que esta ação não solicita validação para o usuário.

* **Seção Usuários**: Esta seção da tela apresenta a lista de todos os usuários que estão vinculados ao grupo e o respectivo consumo individual de recursos computacionais. Através desta tela o usuário com perfil de Administrador do Grupo, pode acompanhar qual(is) usuário(s) consome(m) mais recursos computacionais nos provedores de nuvem (público e/ou privado);

.. figure:: /figuras/uCloud_menu_grupo_008.png
   :alt: menu de usuário
   :align: center

----

* **Botão Criar Usuário**; Este botão permite provisionar um novo usuário na Plataforma uCloud já vinculando este novo usuário ao grupo que se está visualizando. Esta é a metodologia recomendada pela Ustore para provisionar novos usuários para acessar o ambiente. Quando clicar com o botão do Mouse sobre este botão, a Plataforma uCloud apresenta a tela de Criando Novo Usuário.

* **Botão Adicionar Usuário Existente**; Este botão permite vincular um usuário existente a este grupo. Quando o usuário clicar com o cursor do mouse neste botão será apresentada uma tela;

.. figure:: /figuras/uCloud_menu_grupo_009.png
   :alt: menu de usuário
   :align: center

----

* É necessário preencher o campo desta tela com alguns caracteres do login do usuário que se deseja associar e a Plataforma uCloud apresenta uma lista com os logins de usuário que possuam os caracteres informados em sua identificação de login. Selecionar o usuário desejado com o botão do mouse e depois confirmar a ação através do botão verde OK. Esta tela será encerrada e a lista de usuários do grupo será atualizada - como resultado apresenta este usuário, neste grupo.

Esta seção da tela possui uma lista com colunas, descritas a seguir;

* **Login** : Esta coluna apresenta as credenciais de login do usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de login de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Cota de CPU** : Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de CPU que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no valor da quantidade de CPU de forma crescente ou decrescente.

  * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
  * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de Faturamento** : Esta coluna apresenta o número que representa o limite (cota) do valor financeiro que foi definido para o usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de usuários com base no valor financeiro de forma crescente ou decrescente.

   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de Memória** : Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Memória que for definida para este usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de usuários com base no valor da quantidade de memória de forma crescente ou decrescente.

   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de Disco** : Esta coluna apresenta o número inteiro que representa o limite (cota) valor total de Disco de Armazenamento que for definido para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no valor total do Disco de Armazenamento de forma crescente ou decrescente.

   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de IPs Públicos** : Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Endereços TCP-IP Públicos que foram definidos para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no valor da quantidade de IPs Públicos de forma crescente ou decrescente.

   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Uso da CPU**: Esta coluna apresenta a quantidade consumida do recurso computacional CPU por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de usuários com base no valor total de consumo do recurso CPU de forma crescente ou decrescente.

* **Uso da Memória**: Esta coluna apresenta a quantidade consumida do recurso computacional de Memória por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de usuários com base no valor total de consumo do recurso Memória de forma crescente ou decrescente.

* **Uso do Disco**: Esta coluna apresenta a quantidade consumida do recurso computacional Disco de Armazenamento por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista dos usuários com base no valor total de consumo do recurso Disco de Armazenamento, de forma crescente ou decrescente.

* **Uso de IP**: Esta coluna apresenta a quantidade consumida do recurso computacional Endereços TCP-IP Público por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de usuários com base no valor total de consumo do recurso Endereço IP, de forma crescente ou decrescente.

* **Ações**: Esta coluna apresenta ícones que demonstram se o usuário está provisionado consumindo as cotas do Grupo ou possui cota individual. Para usuários com cotas individuais, existe um botão para editar os limites (cotas) dos recursos computacionais ou financeiros de um usuário com cotas individuais.

   * **Ícone de Cota de Grupo** |icone_cota_grp|; Este ícone será apresentado nas linhas de usuários que estão associados a cota de grupo.
   * **Ícone de Cota de Usuário** |icone_cota_indv|; Este ícone será apresentado nas linhas de usuários que estão associados a cota individual.
   * **Botão Editar Cotas** |botao_editar|; Este botão é apresentado somente nas linhas de usuários que estão associados às cotas individuais. Exclusivamente estará ativo se o perfil do usuário que está registrado e acessando esta tela for um administrador de grupo ou de contrato e possuir a permissão para alterar o conteúdo do(s) campo(s). Quando for pressionado o botão "Editar Cotas" a Plataforma uCloud apresenta a tela abaixo:

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

Após esta ação a Plataforma uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando as novas cotas do usuário.

Criando Novo Grupo
------------------

O conceito de Grupos criado unicamente para a Plataforma uCloud,  não existe nada semelhante em qualquer provedor de recursos computacionais de nuvem (público e/ou privado).
Para a Plataforma uCloud um “Grupo” tem duas atribuições básicas que são:

#. Permite organizar usuários de forma a identificar um departamento, um centro de custo, uma iniciativa, apenas para citar alguns pontos.
#. Pode estabelecer um limite (cotas de recursos ou financeiro) para os usuários vinculados ao grupo, de como será possível consumir os recursos computacionais de nuvem (público e/ou privado).

Para criar um grupo é preciso provisionar, previamente, um Contrato na Plataforma uCloud, e vincular o grupo a um contrato existente.
Importante ressaltar que somente os usuários com perfil de Administrador de Contrato, ou Administrador de Grupo estão habilitados para provisionar um grupo na Plataforma uCloud.
Abaixo se apresenta a tela para provisionar um grupo na Plataforma uCloud;

.. figure:: /figuras/uCloud_menu_grupo_011.png
   :alt: menu de grupo
   :align: center

----

* **Nome**: *Este campo é obrigatório* e deve ser preenchido com o nome do grupo.

* **Contrato**: *Este campo é obrigatório* e deve ser informado o nome do contrato, ao qual o grupo está vinculado. Pode-se informar parte do nome de um contrato e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo.

.. figure:: /figuras/uCloud_menu_grupo_012.png
   :alt: menu de grupo
   :align: center

----

Serão listados apenas os contratos aos quais o perfil do usuário tem a permissão de visualizar. Assim que selecionado o grupo ficará vinculado ao contrato.

Assim que um contrato é selecionado, a Plataforma uCloud apresenta, na coluna à direita desta tela, o grupo de Permissões que foram definidas no Contrato.

.. figure:: /figuras/uCloud_menu_grupo_013.png
   :alt: menu de grupo
   :align: center

----

Todos os usuários que pertencem ao grupo recebem as mesmas permissões. Existem duas formas diferentes que podem ser utilizadas neste momento para repassar as permissões do contrato para o grupo.

  * **Utilizar as permissões padrões**: Esta opção engloba um conjunto padrão de permissões para o grupo, assim todos os usuários herdam este grupo de permissões padrão.

  * **Definir manualmente as permissões**: Ao lado de cada linha de permissão existe um campo do tipo “check box”, ao ser selecionado, adiciona a respectiva permissão ao grupo e aos usuários pertencentes a este grupo. Este processo é detalhado, pois existem mais de cento e sessenta permissões na Plataforma uCloud. Se o “check box” existente no topo da tabela for selecionado, significa marcar todas as permissões de uma única vez.

  * **Apenas permissões de leitura**: Este campo é do tipo “radio button” ao ser selecionado configura que este grupo (e os usuários que o compõem) estão restritos a visualizar as informações do ambiente de nuvem. Os usuários vinculados a este grupo não possuem permissão de criação e/ou modificação de qualquer recurso computacional nos provedores de nuvem (público e/ou privado).

* **Cota de IPs Públicos**: Este campo é obrigatório e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo de Endereços TCP-IP Públicos que poderão ser consumidos por todos os usuários do grupo.

* **Cota de CPU**: Este campo é obrigatório e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais das CPUs que poderão ser consumidos por todos os usuários do grupo.

* **Cota de Memória**: Este campo é obrigatório e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais de Memória que poderão ser consumidos por todos os usuários do grupo. Pode ser selecionado o limite em Megabytes ou em Gigabytes.

* **Cota do Disco**: Este campo é obrigatório e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais de Disco de Armazenamento que poderá ser consumido por todos os usuários do grupo. Pode ser selecionado o limite em Gigabytes, Megabytes ou em Terabytes.

* **Botão Criar**: Após preencher todos os campos obrigatórios e opcionais para provisionar o novo grupo, o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma uCloud provisione o novo grupo em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório foi deixado sem preenchimento.

Após o usuário confirmar a ação de criar um grupo, a Plataforma uCloud encerra a tela anterior e retorna para a tela com a lista de grupos e o grupo recém criado se apresenta nesta lista.

Administração / Contrato
------------------------

Uma grande vantagem para as empresas quando adotam a Plataforma uCloud é o controle e monitoração da Governança de Custos e de Recursos Computacionais.

Permitir a governança de custos em ambientes híbridos de multi-nuvem (público e/ou privado) facilita as empresas a manterem os limites definidos dos seus investimentos (orçamento) dentro dos objetivos de negócio das organizações usuárias da Plataforma uCloud.

O Contrato é o ponto principal onde a organização usuária do uCloud estabelece a forma como gerencia os aspectos comerciais, os limites financeiros (ou dos recursos computacionais), define seus valores para recursos computacionais de forma individualizada (válido somente para uma nuvem privada), vincula os grupos e os usuários.

Quando os valores dos recursos computacionais de nuvens públicas são totalizados em outras moedas, no contrato se estabelece a forma da conversão da moeda estrangeira para a moeda local (e o valor de conversão é fixo ou variável) e as taxas de impostos aplicadas aos custos do contrato.

No contrato, a organização pode estabelecer a data inicial e sua expiração (prazo do contrato). Ao estabelecer a data do prazo do contrato, a organização poderá definir se os recursos computacionais existentes no provedor de nuvem pública, deverão ser removidos definitivamente de forma manual (um a um) ou de forma automática (remoção de todos os recursos automaticamente).

A maneira de configurar um contrato pode variar de organização para organização, por isso, abaixo estão listados alguns exemplos de configuração:

#. Um contrato pode abranger mais de um provedor de nuvem: desta forma todos os provedores serão controlados dentro dos mesmos padrões do contrato. Esta modalidade é muito útil quando os custos são fixos e não existe negociação dos valores de recursos computacionais. Desta forma, os custos estão centralizados em um único ponto.

#. Um contrato pode estar vinculado a apenas um provedor de nuvem: desta forma o contrato limita os custos de forma mais granular e permite criar grupos que consumam apenas recursos computacionais deste provedor. Desta forma, todos os custos de um único provedor estão centralizados em um único ponto.

#. Dois contratos podem estar vinculados a um mesmo provedor de nuvem: esta forma é a mais indicada quando a organização e o provedor de nuvem renegociam os custos dos recursos computacionais. Como existem dois momentos diferentes (custos anteriores à renegociação e custos após a renegociação) e cada contrato reflete as margens e valores dos diferentes períodos de cada negociação. Desta forma, os custos de cada momento da negociação estão centralizados em um único ponto.

#. Um contrato para cada filial fiscal (CNPJ) da empresa: desta forma é possível efetuar a governança de custos de cada unidade fiscal da organização, caso cada uma destas filiais tenham liberdade de contratação de provedores de nuvem de forma individual. Desta forma, os custos de cada filial terá a sua própria governança de custos de serviços de computação em nuvem (público e/ou privado).

O contrato é o primeiro item a ser provisionado na Plataforma uCloud, logo após o item grupos deste contrato e, depois, provisionar os usuários vinculados a cada grupo. Somente um usuário com perfil de Administrador da Plataforma tem permissão de provisionar um novo contrato. Veja o documento Manual do Administrador da Plataforma uCloud para entender como provisionar um contrato.

Este documento não cobre o procedimento do processo de provisionar um novo contrato.

Somente usuários com perfil de Administrador de Contrato têm a permissão de visualizar esta lista de contratos da empresa. Este usuário terá acesso apenas aos contratos os quais o seu login de usuário está vinculado no campo de Administrador de Contrato:

.. figure:: /figuras/ucloud_menu_contrato_001.png
   :alt: menu de contrato
   :align: center

----

Abaixo seguem descritas as colunas apresentadas nesta tabela:

* **Nome**: Esta coluna apresenta o nome do contrato da forma como está provisionado na Plataforma uCloud.
* **Admin**: Esta coluna apresenta as credenciais do usuário como está associado ao campo: Administrador do Contrato. Qualquer usuário (simples) pode ser associado a este campo, após esta ação o usuário fica associado ao perfil de Administrador de Contrato.
* **CPF/CNPJ**: Esta coluna apresenta o conteúdo da identificação fiscal brasileira que pode corresponder a uma identificação de pessoa física (CPF) ou identificação fiscal de pessoa jurídica (CNPJ).
* **Estado**: Esta coluna apresenta o estado deste contrato na Plataforma uCloud, onde a situação do contrato pode ser uma das três opções abaixo:

  * **Em Produção**: Indica que o contrato está ativo e todos os recursos computacionais estão ativos e funcionais no provedor de serviço de nuvem; o campo Experimental (no formulário do Contrato) o seu estado está indicado como “Desabilitado”.
  * **Expirado**: Esta opção determina que os recursos computacionais devem continuar existindo no provedor de serviço de nuvem (incorrendo o custo, mesmo sem uso). Esta opção depende da data informada no campo Prazo do Contrato.
  * **Cleaned/Limpo**: Esta opção determina que no caso do contrato se encontrar encerrado, por atingir/ultrapassar a data definida no Prazo do Contrato. Todos os seus recursos de nuvem serão expurgados (removidos) automaticamente dos ambientes dos provedores de serviço.
  * **Manual**: Esta opção determina que no caso do contrato se encontrar encerrado, ultrapassou a data definida no Prazo do Contrato, todos seus recursos de nuvem deverão ser expurgados (removidos) manualmente dos ambientes dos provedores de serviço.

Governança Financeira via Contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Através do uso inteligente da associação dos Grupos e Usuários de Grupos, a Plataforma uCloud possibilita algumas formas de permitir (ou limitar) o isolamento financeiro e lógico dos recursos computacionais do provedor, utilizados em diferentes projetos, de modo a não haver interferência entre projetos, centros de custos, filiais, iniciativas ou departamentos.

Abaixo estão descritas as duas formas simples de isolamento financeiro que advém do correto provisionamento de Contrato e a vinculação de Grupos e de Usuários ao contrato.

Isolamento Financeiro de Recursos Computacionais
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A Plataforma uCloud estabelece o conceito de Grupo que permite a alocação de uma determinada quantidade de recursos computacionais, ou valores financeiros, os quais podem ser consumidos por todos os usuários que estão vinculados ao Grupo, assim é criada uma pequena ‘célula’ de governança financeira. A Plataforma uCloud pode conter diversos Grupos, deste modo, a governança financeira fica mais próxima do cenário real da organização.

Importante ressaltar que o conceito de ""Grupos" permanece somente para a Plataforma uCloud e nada similar existe nos provedores de serviço de nuvem pública ou privada.

Um Grupo que contém usuários, pode ser um Departamento, uma Unidade de Negócio, um Centro de Custos, uma Filial. Quando se define um limite de quantidade de recursos computacionais ou um limite financeiro a um grupo, significa que a Plataforma uCloud nega (bloqueia) a criação ou alteração de um recurso computacional, se este ultrapassar os limites estabelecidos para o grupo, por qualquer usuário vinculado a este grupo - Uma vez definido o limite de recurso do grupo, este novo recurso computacional não pode ultrapassar estes limites.

Estes limites podem ser ajustados a qualquer momento (aumento ou redução) e apenas os usuários com perfil de Administrador de Grupo ou Administrador de Contrato estão habilitados para alterar estes valores limites (cotas) estabelecidos no grupo. A funcionalidade de Cotas de Grupo é uma forma de se configurar um isolamento lógico financeiro.

Isolamento Lógico de Recursos Computacionais
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A Plataforma uCloud implementa um conceito de Virtual Data Center (VDC), que permite à organização definir um conjunto lógico que seja apenas uma pequena parte (subgrupo) da ampla quantidade dos recursos computacionais de um provedor de nuvem. O conceito de um Virtual Data Center é exclusivo do ambiente da Plataforma uCloud, não existe nenhum conceito similar (ou próximo) nos ambientes dos provedores de serviço de nuvem.

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

* **Public Gateway**: Este botão é válido apenas para ambientes em que o contrato está associado a um ambiente de um Data Center privado, no qual o ambiente de virtualização (hypervisor) é de controle da organização (on-premises). Para que este botão seja válido é necessário ao usuário, com perfil de Administrador da Plataforma uCloud, ter provisionado um Gateway SDN (Software Defined Network). Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de configuração de um Gateway SDN.
* **Experimental**: Durante o provisionamento do contrato o Administrador do Contrato informa os limites (cotas) financeiros e/ou dos recursos computacionais. Em seguida, pode-se acessar a configuração de contrato Experimental.

Através desta configuração é possível estabelecer a data de validade (expiração) do contrato, bem como um limite percentual, que ao ser atingido envia uma mensagem de ‘alerta’ de custo do contrato ou de consumo dos recursos computacionais. Adicionalmente, o usuário pode definir para quem o e-mail de alerta deve ser enviado (Administrador da Plataforma, Administrador do Contrato ou todos os usuários vinculados ao contrato). Veja o exemplo na tela abaixo.

.. figure:: /figuras/ucloud_menu_contrato_004.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de configuração do campo Experimental.

Seção Regras de Faturamento
---------------------------

Nesta seção o Administrador do Contrato pode personalizar as regras de como os valores dos custos do contrato podem ser convertidos para moeda local, também personaliza, se para o cálculo de conversão de moeda aplicará no fator de conversão: um valor fixo ou um valor variável. Para o valor variável, a Plataforma uCloud está configurada para obter a taxa do valor de conversão diretamente do site do Banco Central do Brasil, local onde pode extrair a taxa PTAX do último dia útil do mês.

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de configuração do campo Experimental.

.. figure:: /figuras/ucloud_menu_contrato_005.png
   :alt: menu de contrato
   :align: center

----

Podem ser:
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

A Plataforma uCloud possibilita, ao usuário com perfil de Administrador do Contrato, definir Políticas de Alertas de consumo individual de recursos computacionais de nuvem. Quando a condição da regra for atingida a Plataforma uCloud envia um e-mail para o Administrador de Contrato. Veja o exemplo da tela abaixo:

.. figure:: /figuras/ucloud_menu_contrato_006.png
   :alt: menu de contrato
   :align: center

----

Abaixo descrevemos as colunas desta seção da tela de contratos:

* **Nome**: Esta coluna apresenta o nome de identificação da política de alerta definido durante seu provisionamento.
* **Recurso**: Essa coluna apresenta o tipo de recurso definido para que a Plataforma uCloud monitore o consumo.
* **Política**: Essa coluna apresenta a forma definida que estabelece o limite do alerta.
* **Valor**: Essa coluna apresenta o valor de limite superior definido para que a Plataforma uCloud possa comparar e enviar o alerta para o usuário Administrador do Contrato.
* **Ações**: Esta coluna apresenta dois ícones para que o usuário possa interagir com a política definida:
* **Botão Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova esta Política de Alarme de forma imediata e definitiva.
* **Botão Habilitar/Desabilitar** |icone_habil_verde|/|icone_desb_verm|: Este botão é um tipo “checkbox” que o usuário pode atuar para alternar o seu modo atual. A cor verde indica que a política está HABILITADA. A cor vermelha indica que a política está DESABILITADA.

Para alternar entre os estados basta clicar com o cursor do mouse e o campo será ativado, apresentando a cor verde. Se estiver na cor verde, basta clicar com o mouse e o campo será desativado, apresentando a cor vermelha.

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de configuração de uma Política de Alerta.

Seção Preço dos Recursos - Contrato
-----------------------------------

Esta seção permite que o Administrador do Contrato possa redefinir os valores dos recursos que estão sendo consumidos dentro deste contrato. Através desta tela é possível definir preços diferentes para os recursos cobrados pelo provedor de serviço de nuvem. Estes novos valores devem ser informados manual e individualmente, não sendo necessário que todos sejam informados.

Apenas os valores dos recursos que foram informados serão recalculados pela Plataforma uCloud, apresentados nos relatórios do menu Financeiro.

Os recursos com valor igual a zero (0), terão o seu valor original cobrado pelo provedor de serviço de nuvem sem ser recalculado.

.. figure:: /figuras/ucloud_menu_contrato_007.png
   :alt: figura da interface
   :align: center

----

Recomendamos fortemente que, qualquer alteração nos Valores dos Recursos altere os valores originalmente cobrados pelo provedor de serviços de nuvem.

..  attention:: *Lembramos ao usuário: ao informar qualquer novo valor, este ‘novo valor’ altera o valor da fatura mensal a ser cobrada pelo provedor, e qualquer diferença, multa ou penalidade contratual advindas destas alterações não são responsabilidade da Ustore ou da Plataforma uCloud, pois a plataforma está desempenhando o função pela qual foi desenhada a efetuar.*

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

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de configuração de Cotas do Contrato.

Seção Contato Primário
----------------------

Esta seção possibilita ao Administrador do Contrato informar os dados de contato de um responsável Financeiro, Fiscal ou Contábil referente a este contrato.

.. figure:: /figuras/ucloud_menu_contrato_009.png
   :alt: menu de contrato
   :align: center

----

Esta seção não é obrigatória, e o não preenchimento desta seção não impede, ou bloqueia, nenhuma funcionalidade do perfeito uso da Plataforma uCloud.

Recomendamos o preenchimento destas informações para que a Plataforma uCloud possa enviar informações automaticamente para o gestor do contrato.


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

Esta seção não é obrigatória. No caso desta seção deixar de ser preenchida, isto não impede ou bloqueia as funcionalidades e o perfeito uso da Plataforma uCloud.

Seção Virtual Datacenters Concedidos
------------------------------------

Nesta seção o usuário Administrador do Contrato vincula o Virtual Data Center (VDC) ao contrato. Esta é uma das alternativas de Governança de Custos permitida pela Plataforma uCloud – veja mais informações acima no item Administração de Contrato.

Quando ocorre a vinculação de um VDC a um contrato, significa que o usuário administrador do contrato estabelece para a Plataforma uCloud a concessão deste VDC ao contrato. Assim, para o usuário - com permissão de administrador do contrato - serão listados apenas os VDCs deste contrato. Em outras palavras, todas as telas da Plataforma uCloud onde um VDC pode ser ofertado (solicitado) ao usuário selecionar, o usuário pode visualizar/solicitar apenas os VDCs listados nesta seção.

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

Esta seção apresenta todos os Grupos vinculados ao Contrato. A Plataforma uCloud mostra ou lista as cotas que foram alocadas para cada Grupo vinculado ao Contrato. É possível verificar as cotas de cada grupo e o consumo dos recursos, dentro do grupo, até o momento da pesquisa.

.. figure:: /figuras/ucloud_menu_contrato_013.png
   :alt: menu de contrato
   :align: center

----

* **Botão “+Adicionar Grupo Existente”** |botao_adiciona_grp|: Através deste botão, o usuário com perfil de Administrador de Grupo, poderá vincular um grupo - previamente provisionado na Plataforma uCloud - ao contrato que se está visualizando. Quando o usuário clicar com o cursor do mouse sobre este botão, será apresentada a seguinte tela;

.. figure:: /figuras/ucloud_menu_contrato_014.png
   :alt: menu de contrato
   :align: center

----

* **Grupo**: Neste campo o usuário precisa informar parte do nome de um grupo existente, como resultado a Plataforma uCloud apresenta uma lista de todos os grupos que possuem parte dos caracteres informados. Basta o usuário selecionar o grupo desejado, o resultado é apresentado da seguinte forma;

.. figure:: /figuras/ucloud_menu_contrato_015.png
   :alt: menu de contrato
   :align: center

----

   * **Botão Adicionar Grupo** |botao_adiciona|: Neste momento, o usuário deve clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud efetive a vinculação do grupo selecionado ao contrato que se está visualizando.
   * **Botão Ok**: Ao clicar com o cursor do mouse sobre este botão, a Plataforma uCloud encerra esta tela e retorna à visualização do Contrato, e a relação de grupos vinculados ao contrato, atualizada com o novo grupo.
   * **Botão “+Criar Grupo”** |botao_adiciona_grp|: Através deste botão o usuário, com perfil de Administrador de Grupo, poderá provisionar um novo grupo na Plataforma uCloud. Mediante este botão, o novo grupo ficará obrigatoriamente vinculado ao contrato que se está visualizando. Veja a descrição de todo o processo de provisionamento de um grupo na Plataforma uCloud no item Criando Novo Grupo.

Seção Dados de Faturamento
--------------------------

Nesta seção são apresentadas as informações de Faturamento de um Contrato. Estas informações, geralmente, são necessárias para integrações automatizadas com sistemas de CRM, showback e chargeback.

.. figure:: /figuras/ucloud_menu_contrato_016.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos para informar os dados de Faturamento do Contrato.

Seção Perfis de Permissionamento
--------------------------------

Esta seção (card) se aplica ao usuário Administrador da Plataforma uCloud (perfil diferente do Administrador do Contrato), que tiver provisionado antecipadamente Perfis de Permissões através do menu Configurações / Perfis de Permissionamento. Somente um usuário com o perfil Administrador da Plataforma é responsável pela gerência de todos e dos demais grupos e permissões.
Quando um Perfil de Permissionamento é vinculado ao Contrato, isto implica que todos seus Grupos e Usuários recebem as mesmas permissões para acessar os menus da plataforma definidas neste perfil, de forma a permitir aos usuários vinculados a este contrato acesso às funcionalidades da Plataforma uCloud definidas neste perfil de permissionamento.

.. figure:: /figuras/ucloud_menu_contrato_017.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de como provisionar um Perfil de Permissionamento e vincular um VDC a um contrato.

Seção Produtos
--------------

Um produto pode ser visto como recurso, um software, o valor de uma licença específica, um serviço recorrente ou qualquer coisa que se seja necessário incluir em um Contrato. Importante ressaltar que o produto sempre será algo que não existe ou que não pode ser criado e gerenciado pela Plataforma uCloud, diretamente no console dos provedores de nuvem pública e/ou privada. É indicado configurar um Produto quando a oferta é o Virtual Data Center como um todo, no caso de serviços, ofertas específicas para máquinas virtuais, é recomendado optar pelas assinaturas.

.. figure:: /figuras/ucloud_menu_contrato_018.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de como adicionar um Produto a um contrato.

Seção Permissões Concedidas
---------------------------

Esta seção (card) permite personalizar as permissões concedidas aos usuários com acesso às funcionalidades na Plataforma uCloud, de forma global. Estas permissões básicas, definidas e vinculadas ao Contrato, implicam que todos seus Grupos e Usuários recebam as mesmas permissões de acesso às funcionalidades definidas nesta seção. Diferente do Perfil de Permissionamento, esta configuração permite que o usuário com perfil de Administrador de Contrato adicione ou remova, permissões não previstas no Perfil de Permissionamento. Permite também, remover/excluir permissões do Contrato.

.. figure:: /figuras/ucloud_menu_contrato_019.png
   :alt: menu de contrato
   :align: center

----

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de como provisionar ou excluir Permissões vinculadas a um contrato.

Seção Perfil de Faturamento de Container
----------------------------------------

Esta seção apresenta todos os dados relacionados ao perfil de faturamento de um contrato por tipo de container a ser utilizado. A Plataforma uCloud permite vincular um Contrato a um Container. O termo container representa um hypervisor ou conexão com uma nuvem pública, sendo assim é possível que existam perfis de preços distintos de acordo com o container que um usuário possa vincular a um contrato.
Através desta configuração é possível que sejam definidos preços distintos por perfil de faturamento (preço fixo, recurso alocado ou recurso efetivamente utilizado) por tipo de container.

.. figure:: /figuras/ucloud_menu_contrato_020.png
   :alt: menu de contrato
   :align: center

----

Favor consultar uCloud - Manual do Administrador, para conhecer os procedimentos de como provisionar um contrato.

Provisionando Contrato
----------------------

Importante ressaltar que não é objetivo deste documento descrever o processo de provisionamento de um contrato, pois apenas os usuários com perfil de Administrador da Plataforma uCloud têm permissão para isto. Veja o documento Manual do Administrador da Plataforma uCloud onde descrevemos o processo como provisionar um contrato.

Menu Configuração
=================

O menu configuração permite que o usuário com perfil de Administrador da Plataforma defina os parâmetros básicos do sistema. Estes parâmetros serão utilizados em várias áreas e outros menus da Plataforma uCloud de forma global.
A Plataforma uCloud é um ambiente, por definição, multi-empresas (multi tenant). Portanto, todos os parâmetros definidos impactam todas as empresas, seus contratos e todos os usuários de forma global. Este impacto é de responsabilidade do usuário com o perfil de Administrador da Plataforma, que possui o perfeito conhecimento e compreensão de todas as implicações destas configurações globais.
Os submenus descritos a seguir permitem configurações que terão impacto em muitas atividades e rotinas de todos os usuários e empresas provisionados.


Configuração / Geral
--------------------

Esta tela está dividida em seções, por meio destas seções (card) o Administrador da Plataforma, pode definir as cotas (limites) padronizados para serem aplicados a qualquer novo usuário a ser adicionado na plataforma quando consumir/criar recursos computacionais em nuvem (público e/ou privado).

Seção Geral:
~~~~~~~~~~~~

Na seção Geral, os usuários definem as opções de quotas padrão por usuário do sistema, ou seja, ao criar um usuário se ele não tiver sua quota informada o sistema usará as cotas constantes na tela de aplicação.
Abaixo esclarecemos os campos desta seção. Importante ressaltar que somente usuários com perfil de Administrador de Plataforma podem alterar os valores armazenados nestes campos.

* **Botão “Sincronizar Active Directory”**: Este botão permite configurar a integração de um servidor de Active Directory para o ambiente de forma que possa validar, duplamente, as credenciais de usuários provisionados no ambiente de forma global. Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos corretos para configurar a sincronização com um servidor de Active Directory.

* **Botão Ativação Automática “On/Off”**: Este botão tem função de permitir que todos os novos usuários provisionados via o processo descrito no item Criando Novo Usuário sejam ativados de forma automática para se registrarem na Plataforma uCloud.
* **Cota Padrão de CPU**: O conteúdo informado neste campo será utilizado, de forma global, como o padrão de cota de quantidade de recurso computacional CPU. Será válido para todos os usuários. Deve-se informar um número inteiro.
* **Cota Padrão da Memória**: O conteúdo informado neste campo será utilizado, de forma global, como o padrão de cota de quantidade de recurso computacional Memória. Será válido para todos os usuários. Deve-se informar um número inteiro no campo ao lado o Administrador da Plataforma pode selecionar se o limite será em Gigabytes ou em Megabytes.
* **Cota Padrão do Disco**: O conteúdo informado neste campo será utilizado, de forma global, como o padrão de cota de quantidade de recurso computacional no Espaço de Armazenamento de Disco. Será válido para todos os usuários. Deve-se informar um número inteiro no campo ao lado, o Administrador da Plataforma pode selecionar se o limite será em Gigabytes, Megabytes ou em Terabytes.
* **E-mail Administrador**: Neste campo deve constar o endereço do correio eletrônico (e-mail) do Administrador da Plataforma, para que este possa receber mensagens de alerta da Plataforma uCloud, nas opções em que possuem esta funcionalidade.
* **Valor do Dólar**: Este campo não é obrigatório (pode estar ‘em branco’) e deve constar o valor padrão geral (global) para a conversão da moeda de Dólares Americanos para Reais. Este valor será a referência padrão, caso não exista nenhuma configuração no contrato provisionado. Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos corretos e provisionar um contrato.
* **Valor dos Impostos**: Este campo não é obrigatório (pode estar ‘em branco’) nele deve constar o valor padrão geral (global) referente a Taxa de Impostos a ser aplicada sobre os valores das Faturas no menu Financeiro. Este valor será a referência padrão, caso não exista nenhuma configuração no contrato provisionado. Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos corretos para provisionar um contrato.
* **Valor da meta mensal**: Este campo não é obrigatório (pode estar ‘em branco’) e deve constar o valor padrão geral (global) da meta mensal de consumo de recursos financeiros. Este valor será a referência padrão, caso não exista nenhuma configuração no contrato provisionado.

.. important:: |importante| Importante ressaltar que no caso deste valor ser informado, poderão ser enviadas mensagens de alerta para o Administrador da Plataforma, porque houve um consumo financeiro mensal global acima deste valor estabelecido. Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos corretos para provisionar um contrato.

Solicite acesso ao documento Manual do Administrador da Plataforma uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma uCloud.


Seção Preço dos Recursos
~~~~~~~~~~~~~~~~~~~~~~~~

A seção Preço dos Recursos permite definir os preços por hora de consumo para CPU, Memória e Disco, os valores cobrados por taxa de transferência e por recursos de rede.
Solicite acesso ao documento Manual do Administrador da Plataforma uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma uCloud.

Seção Configurações de Usuários LDAP Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta seção permite que o Administrador da Plataforma selecione quais usuários provisionados na Plataforma uCloud devem ter suas credenciais sincronizadas com o servidor de LDAP/AD configurado no botão “Sincronizar Active Directory” da seção Geral.

Solicite acesso ao documento Manual do Administrador da Plataforma uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma uCloud.

Menu Configuração / Rede
========================

A seção Configuração da Rede, indica a listagem do controlador SDN e as opções de configuração do uCloud. O qual permite o uso de vários controladores SDN transferindo assim mais escalabilidade para o sistema.

* O que é SDN?

  * A **SDN** (Rede Definida por Software – *Software Defined Network*) é uma abordagem de arquitetura de rede que permite controlar ou "programar" a rede de maneira central e inteligente usando aplicativos de software. Ela ajuda as empresas a gerenciar toda a rede de modo consistente e holístico, seja qual for o fornecedor de equipamentos de rede.

Para acompanhar o ritmo, o mundo está adotando a tecnologia de SDN para revolucionar o design e as operações de rede.

A SDN permite o gerenciamento consistente da rede, que pode ser constituída por peças de tecnologia complexas.

A Ustore possui em seu portfólio o produto uSDN para complementar ambientes de data center privado (on-premises) para transformar o ambiente privado de forma a simplificar a configuração de parâmetros de rede de dados através da interface da Plataforma uCloud.

.. important:: |importante| Importante ressaltar que a configuração das telas abaixo somente será necessária quando a Plataforma uCloud estiver configurada para o controle e o gerenciamento dos recursos computacionais em um data center privado. Para o gerenciamento e controle dos recursos computacionais de nuvem pública, as telas abaixo não demandam configuração e podem ser ignoradas.

A Ustore possui em seu portfólio o produto uSDN para complementar ambientes de data center privado (on-premises) para transformar o ambiente privado de forma a simplificar a configuração de parâmetros de rede de dados através da interface da Plataforma uCloud.

Importante ressaltar que a configuração das telas abaixo somente será necessária quando a Plataforma uCloud estiver configurada para o controle e o gerenciamento dos recursos computacionais em um data center privado. Para o gerenciamento e controle dos recursos computacionais de nuvem pública, as telas abaixo não demandam configuração e podem ser ignoradas.

Seção Configurações de Rede
---------------------------

Nesta tela são provisionadas as configurações de rede (de forma geral) que serão enviadas para o controlador SDN do ambiente do data center privado (on-premises).

* **Range de VLAN Global**: Neste campo deve ser configurada a faixa (range) de endereços TCP-IP da rede privada.
* **CIDR Global**: Neste campo deve ser informado o CIDR, ou endereçamento IP sem classes. Esta configuração de CIDR Global otimiza a distribuição dos endereços IP de 32 bits, permitindo máscaras de rede de qualquer tamanho.
* **Prefixo CIDR do Usuário**: Neste campo devem ser informados os prefixos de endereços TCP-IP específicos da rede corporativa privada da empresa. Podem ser informados CIDRs de todas as classes de endereçamento TCP-IP, por exemplo: 255.0.0.0 (classe A); ou 255.255.0.0 (classe B) ou 255.255.255.0 (classe C), de acordo com a configuração do ambiente de rede da empresa que está sendo configurada na Plataforma uCloud.
* **Botão Network Sharing**: Este botão permite configurar a opção de que a rede que se está provisionando a configuração seja compartilhada (shared) ou não. Se este botão estiver com a opção “ON” ativa, significa que a configuração de rede será de uma rede que pode ser compartilhada. Se o botão estiver com a opção “OFF” ativa, significa que a configuração de rede será privada e os seus endereços TCP-IP serão privados.

Solicite acesso ao documento Manual do Administrador da Plataforma uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma uCloud.

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
* **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova este Controlador SDN de forma imediata e definitiva.
* **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela que permite editar as configurações do Servidor de SDN respectivo. Importante mencionar que apenas o usuário com perfil de Administrador de Plataforma, poderá editar os valores informados nesta tela.

Solicite acesso ao documento Manual do Administrador da Plataforma uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma uCloud.

Menu Configuração / Sub-Redes Públicas
======================================

Quando a empresa configura um servidor de SDN para controlar as configurações de sua rede privada, são controlados e gerenciados apenas endereços restritos (privados). Estes endereços não podem ser acessados de máquinas que estejam em outras redes.

Para que o controlador SDN possa gerenciar os endereços que poderão ser acessados de forma externa (pública) é fundamental que a equipe de segurança e redes, estabeleça a faixa (range) de endereços que serão públicos e a informação destes endereços seja repassada para o Controlador SDN.

Esta opção de menu permite que sejam criadas faixas (ranges) de endereços TCP-IP que sejam públicos, para quando um recurso computacional da nuvem privada (máquina virtual) necessitar de um endereço público, a Plataforma uCloud possa interagir com o Gerenciador SDN e vincular um endereço TCP-IP Público para este recurso computacional (máquina virtual).

* **Nome**: Este campo apresenta o nome da rede que foi escolhido no momento do provisionamento da configuração da rede.
* **CIDR**: Este campo apresenta o CIDR, ou endereçamento IP sem classes, acrescentado com a respectiva definição de bloco de endereços (“/xx”). Esta configuração de CIDR e a quantidade de blocos de endereços, deve ser definida pela equipe de engenharia de redes de dados da empresa.
* **Range start**: Este campo apresenta o endereço TCP-IP inicial da faixa que se deseja disponibilizar.
* **Range end**: Este campo apresenta o endereço TCP-IP final da faixa que se deseja disponibilizar.
* **Gateway**: Este campo apresenta o endereço TCP-IP do Gateway de rede que transfere o tráfego de pacotes da rede local para a outras redes, neste caso a rede externa/pública.
* **Container**: Este campo apresenta o nome do container o qual este Controlador SDN está conectado, para controlar e gerenciar as atribuições de endereçamentos TCP-IP.
* **Ignored Address**: Este campo apresenta a lista de endereços TCP-IP, definidos pela equipe de rede da empresa, a ser ignorado e evitado, para serem assinalados a recursos computacionais. Os endereços apresentados nesta lista estão separados por vírgula.
* **Ações**: Esta coluna apresenta apenas o Ícone Lata de Lixo |icone_lixo|. Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova a configuração de Sub-Rede Pública de forma imediata e definitiva. Importante ressaltar que a Plataforma uCloud não solicita confirmação desta remoção para o usuário, a ação de remoção é imediata e irreversível. Se a ação não foi intencional, o usuário deverá iniciar o processo de configuração da Sub-Rede Pública novamente desde seu início.

Favor consultar o documento: Manual do Administrador da Plataforma uCloud, para conhecer os procedimentos de como provisionar corretamente o Controlador SDN dentro do ambiente de rede privada.

Solicite acesso ao documento Manual do Administrador da Plataforma uCloud, e você irá encontrar os procedimentos de configuração dos parâmetros gerais da Plataforma uCloud.

Menu Configuração / Assinaturas
===============================

Assinaturas são serviços vinculados a uma máquina virtual. As assinaturas têm que conter apenas as ofertas de serviços que devem ser cobrados mensalmente ou mês específico. No caso da remoção de uma assinatura vinculada a uma máquina virtual, o valor será cobrado integralmente pelo agente de bilhetagem.

São exemplos de assinaturas: gerenciamento, licenças de sistema operacional e monitoramento, entre outros. A figura abaixo apresenta exemplos de modalidades de assinaturas que uma máquina virtual pode possuir:

* **Nome**: Este campo apresenta o nome informado no momento da sua configuração.

* **Preço**: Este campo apresenta o valor mensal referente ao custo da assinatura, informado no momento de criar a assinatura.

* **Descrição**: Este campo apresenta a descrição estendida da assinatura, que foi informado no momento da sua criação.

* **Ações**: Esta coluna apresenta apenas o Ícone Lata de Lixo. Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova a assinatura de forma imediata e definitiva. Importante ressaltar que a Plataforma uCloud não solicita confirmação desta remoção para o usuário, a ação de remoção é imediata e irreversível.

Criando Assinatura
------------------

O processo de criação de assinatura é muito simples, importante mencionar que as assinaturas devem conter apenas as ofertas de serviços, ou qualquer custo adicional, que serão cobrados mensalmente.

Abaixo a descrição dos campos para o provisionamento de uma nova assinatura:

* **Nome**: Neste campo deve ser informado o nome desejado para identificar a assinatura. Não existe limite máximo para o nome desejado. O limite mínimo de caracteres para informar neste campo é um (01) caractere. Sugerimos utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido).

* **Preço**: Neste campo deve ser informado o valor mensal (número) referente ao custo da assinatura. Se o usuário informar um número inteiro (sem zeros), a Plataforma uCloud assume somente o valor inteiro, seguido de zeros após a vírgula. Para valores com casas decimais, o usuário deve usar a "vírgula" seguido do valor referente decimal do valor mensal (por ex.: “123,90”).

* **Descrição**: Neste campo o usuário informa uma descrição estendida que pode esclarecer a que se refere esta assinatura, este campo pode contar até duzentos e cinquenta e cinco caracteres (255). O limite mínimo de caracteres a informar neste campo é um (01) caractere. Sugerimos utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido).

* **Botão Criar**: Neste ponto, após preencher e finalizar todos os campos para provisionar uma assinatura, o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma uCloud provisione a nova assinatura em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório precisa ser preenchido.

Após confirmar a criação da nova assinatura, a Plataforma uCloud encerra a tela de nova assinatura e retorna a lista atualizada de assinaturas existentes, com a nova assinatura apresentada na relação da tela. Eventualmente, pode existir um atraso para que a Plataforma uCloud atualize a lista de assinaturas.

Menu Configuração / Flavor Billing Profile
==========================================

Esta opção permite definir o preço padrão por tipo de *flavor* a ser utilizado por qualquer usuário na Plataforma uCloud, definindo seu custo de CPU, custo de memória e custo do disco.

*Flavor*, é o termo genérico que todos os provedores de serviço de nuvem utilizam para identificar uma combinação de configuração de hardware (CPU, memória e disco). Podemos traduzir o termo *flavor* para **tipos de instâncias**. Cada tipo de *flavor* (instância) inclui um ou mais tamanhos de configurações de hardware e, desta forma, cada *flavor* possui um valor de custo referente ao conjunto dos seus recursos.

Cada provedor tem um custo para cada tipo de *flavor* em sua lista de preços de recursos computacionais, portanto os valores já existem.

A configuração de um *Flavor Billing Profile* é muito útil para os containers de ambientes de data center privado (*hypervisor on-premises*) desta forma é possível aplicar conceitos de custo de recursos computacionais de nuvem pública (*flavors*) para os ambientes de nuvem privada.

Caso seja utilizado um flavor atual (existente) de um provedor de serviço de nuvem pública, o novo valor pode substituir o valor do provedor por um valor provisionado na Plataforma uCloud definido pelo usuário. Importante ressaltar que esta ação pode criar diversos desdobramentos financeiros na fatura mensal do provedor de serviço de nuvem.

.. image:: /figuras/ucloud_flavor_billing_profile.png
   :alt: Billing Profile
   :align: center

----

* **Botão “Criar Flavor Billing Profile”**: Quando o usuário clicar com o cursor do mouse sobre este botão, a Plataforma uCloud apresenta a tela para configuração de um novo Flavor Billing Profile. O processo de configuração está descrito abaixo no item: Criando um Flavor Billing Profile.

* **Nome**: Esta coluna apresenta o nome do Flavor Billing Profile, anteriormente informado no processo de criação.

* **Custo de CPU**: Esta coluna apresenta o valor deste recurso computacional CPU. Este campo pode apresentar um valor igual a “0” (zero), caso este recurso seja controlado por seu valor fixo mensal.

* **Custo de Memória**: Esta coluna apresenta o valor deste recurso computacional Memória. Este campo pode apresentar um valor igual a “0” (zero), caso este recurso seja controlado por seu valor fixo mensal.

* **Custo de Disco**: Esta coluna apresenta o valor deste recurso computacional Disco. Este campo pode apresentar um valor igual a “0” (zero), caso este recurso seja controlado por seu valor fixo mensal.

* **Preço Mensal Fixo**: Esta coluna apresenta o valor definido como um valor total fixo por mês. Este campo pode apresentar um valor igual a “0” (zero), caso este recurso seja definido pela somatória dos custos de CPU, memória e disco.

* **Ações**: Esta coluna apresenta dois ícones para que o usuário possa interagir com a política definida:

* **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova o Flavor Billing Profile de forma imediata e definitiva. Importante ressaltar que esta ação não terá solicitação de nenhuma confirmação por parte do usuário, portanto será definitiva.

* **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela que permite editar as configurações do respectivo Flavor Billing Profile. Importante mencionar que apenas o usuário com perfil de Administrador de Plataforma, poderá editar os valores informados nesta tela.

Criando um Flavor Billing Profile
---------------------------------

Nesta etapa, será descrito o processo de como definir o valor padrão para um Flavor. Os valores de CPU, Memória e Disco apenas serão aplicados ao alterar a configuração padrão do flavor, principalmente nos casos de adição de discos extras.
Caso seja mais prático é possível configurar um valor de referência que pode ser preenchido no campo “Valor Fixo Mensal”.

Quando o usuário clica com o cursor do mouse no botão “Criar Flavor Billing Profile” a Plataforma uCloud apresenta a seguinte tela;

.. image:: /figuras/ucloud_criar_billing_profile_001.png
   :alt: Billing Profile
   :align: center

----

* **Flavor**: Este campo é um campo do tipo “Dropdown” e quando o usuário clica com o cursor do mouse a Plataforma uCloud lista todos os flavors que existem na plataforma:

  * Todos os flavors do provedor de serviço de nuvem pública (importado após a configuração das credenciais de acesso a este provedor),
  * Todos os flavors provisionados para serem utilizados no container do data center privado.

.. image:: /figuras/ucloud_criar_billing_profile_002.png
   :alt: Billing Profile
   :align: center

----

Após o usuário selecionar o flavor desejado, a Plataforma uCloud altera e retorna a tela conforme o exemplo abaixo:

Para compreensão da imagem acima, segue abaixo a descrição dos campos da tela:

.. image:: /figuras/ucloud_criar_billing_profile_003.png
   :alt: Billing Profile
   :align: center

----

* **Custo de CPU**: Este campo é obrigatório, o usuário deve informar o custo referente a quantidade de recursos de CPU do flavor selecionado no campo inicial. Por ser um campo obrigatório, o usuário deve informar um número inteiro correspondente para o valor mensal deste recurso, ou preencher com “zero (0)”, para os casos em que o flavor tenha um valor fixo mensal.

* **Custo de Disco**: Este campo é obrigatório, o usuário deve informar o custo referente ao recurso de Disco do flavor selecionado no campo inicial. Por ser um campo obrigatório, o usuário deve informar um número inteiro correspondente para o valor mensal deste recurso, ou preencher com “zero (0)”, para os casos em que o flavor tenha um valor fixo mensal.

* **Custo de Memória**: Este campo é obrigatório, o usuário deve informar o custo referente ao recurso de Memória do flavor selecionado no campo inicial. Por ser um campo obrigatório, o usuário deve informar um número inteiro correspondente para o valor mensal deste recurso, ou preencher com “zero (0)”, para os casos em que o flavor tenha um valor fixo mensal.

* **Custo Fixo Mensal**: Este campo é obrigatório, o usuário deve informar o custo referente ao valor mensal do flavor selecionado no campo inicial. Por ser um campo obrigatório, o usuário deve informar um número inteiro correspondente para o valor mensal deste recurso, ou preencher com “zero (0)”, para os casos em que o flavor tenha custos específicos para os recursos de CPU, Memória e Disco.

* **Botão Criar**: Após todos os campos para provisionar Flavor Billing Profile estarem preenchidos o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma uCloud possa provisionar o Flavor Billing Profile em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório precisa ser preenchido.

Menu Configuração / Perfis de Permissionamento
==============================================

A Plataforma uCloud possui uma grande diversidade de permissões, precisamente são 154 (cento e cinquenta e quatro) permissões que podem ser associadas a um usuário. Esta tarefa pode ser complexa e talvez consumir uma grande quantidade de tempo do usuário, ao considerar a associação de permissões para cada usuário provisionado na Plataforma uCloud ou para os novos usuários, no futuro.

Desta forma, para facilitar a associação de permissões existe a facilidade de provisionar perfil que possua um grupo específico de permissões, para acesso às facilidades da Plataforma uCloud, e assim, vincular o(s) usuário(s) a este determinado perfil.

O Perfil de Permissionamento habilita ou bloqueia o usuário a executar uma determinada funcionalidade da Plataforma uCloud, através do Menu de Usuário e os Submenus. As funcionalidades podem ser visualizadas ou acessadas, mas, de acordo com o perfil selecionado, o usuário terá permissão ou não de executar tal funcionalidade.

A seguir, um exemplo da tela com a lista de Perfis de Permissionamento:

.. image:: /figuras/ucloud_perfil_permissionamento_001.png
   :alt: Billing Profile
   :align: center

----

Para compreensão da imagem acima, segue abaixo a descrição das colunas:

* **Botão Criar Perfil**: Quando o usuário clicar com o cursor do mouse sobre este botão, a Plataforma uCloud apresenta a tela para configuração de um novo Perfil de Permissionamento. O processo de configuração está descrito abaixo no item Criar um Perfil.

* **Nome do Perfil**: Esta coluna apresenta o nome do Perfil de Permissionamento que foi informado no momento da sua criação. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de perfis de permissionamento de forma alfabética crescente (a – z) ou decrescente (z – a) com base no nome do perfil.

* **Descrição**: Esta coluna apresenta a descrição estendida do Perfil de Permissionamento informado no momento da sua criação. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de perfis de permissionamento de forma alfabética crescente (a – z) ou decrescente (z – a) com base na descrição do perfil.

* **Criado Por**: Esta coluna apresenta a identificação da credencial de login do usuário responsável pela criação do Perfil de Permissionamento. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de perfis de permissionamento de forma alfabética crescente (a – z) ou decrescente (z – a) com base nas credenciais de login de usuário.

Visualizar e Editar um Perfil de Permissionamento
-------------------------------------------------
Quando o usuário clica com o cursor do mouse em qualquer linha da tabela a Plataforma uCloud apresenta a tela de visualização do Perfil de Permissionamento, conforme o exemplo da tela abaixo:

.. image:: /figuras/ucloud_perfil_permissionamento_002.png
   :alt: Billing Profile
   :align: center

----

Esta tela possui um botão de ação e duas seções (cards), descritos a seguir:

* **Botão Excluir** |botao_excluir|: O usuário deve clicar com o cursor do mouse sobre este botão quando for necessário remover um Perfil de Permissionamento previamente provisionado. Ao clicar neste botão, a Plataforma uCloud apresenta o  seguinte pop-up (imagem abaixo), o usuário responde “sim, pode excluir” e assim confirma a remoção ou “não, cancelar” e desiste de excluir o perfil:

  * **Botão “Não Cancele”**: Basta o usuário clicar sobre este botão (ou teclar “Esc”) para cancelar a ação, na situação de que tenha acidentalmente clicado sobre o botão de exclusão. Quando o usuário cancela a ação de exclusão a Plataforma uCloud apresenta a seguinte tela:
  * **Botão “Sim Pode Excluir”**: Quando o usuário está seguro da ação de exclusão, basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que o Perfil de Permissionamento foi excluído da Plataforma uCloud;

.. image:: /figuras/ucloud_perfil_permissionamento_003.png
   :alt: Billing Profile
   :align: center

----

* **Seção Geral**: Nesta seção são apresentadas informações básicas em relação ao perfil de permissionamento:

  * **Nome**: Neste campo é apresentado o nome (curto) do Perfil de Permissionamento, informado pelo usuário no momento do seu provisionamento. Caso o perfil do usuário, que está acessando esta tela, tenha a permissão de alteração de perfis de permissionamento, o ícone de edição estará ativo.

    * **Ícone de Edição Ativo** |icone_edita_on|: Todos os campos que possuem o ícone de edição ativo são passíveis de alteração do seu conteúdo.
    * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma uCloud.
    * **Ícone de Cancelamento** |icone_cancela_vermelho|: No caso do usuário clicar sobre o ícone de edição por engano, ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente. Basta o usuário clicar com o cursor do mouse sobre o ícone vermelho, e assim, cancelar a alteração. O conteúdo do campo retorna aos valores iniciais, antes de qualquer preenchimento ou alteração.

  * **Descrição**: Neste campo é apresentada a descrição (extensa) do Perfil de Permissionamento, informado pelo usuário no momento do provisionamento.

    * **Ícone de Edição Ativo** |icone_edita_on|: Todos os campos que possuem o ícone de edição ativo são passíveis de ter seu conteúdo alterado.
    * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma uCloud.
    * **Ícone de Cancelamento** |icone_cancela_vermelho|: Caso o usuário tenha clicado sobre o ícone de edição, por engano, ou no caso de não desejar gravar a alteração permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. A alteração será cancelada e o conteúdo do campo retorna aos valores iniciais, ou seja, antes de qualquer preenchimento ou alteração.

* **Seção Permissões**: Nesta seção da tela são listadas as primeiras vinte e cinco (25) permissões vinculadas a este perfil de permissionamento. Importante relembrar que a Plataforma uCloud possui mais de cento e cinquenta permissões, as quais são apresentadas com as iniciais de cada permissão.

  * **Mudar a Classificação**: Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica e lista os nomes das permissões em ordem alfabética crescente (a – z) ou decrescente (z – a).
  * **Busca Rápida**: O usuário observa que logo abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista com os nomes das permissões. Basta preencher o campo em branco, com uma sequência de caracteres percebidos como relevantes e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca.

    * **Botão Editar** |botao_editar|: Este botão destina-se ao usuário que possuir a permissão de alteração de Perfil de Permissionamento, se ele desejar alterar o conjunto de permissões vinculadas a este perfil, basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_perfil_permissionamento_005.png
   :alt: perfil de permissionamento
   :align: center

----

      * Esta tela possui duas colunas distintas, à esquerda são as permissões previamente adicionadas ao perfil. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, pode excluir (revogar) a respectiva permissão deste usuário.
      * À direita estão as permissões disponíveis na Plataforma uCloud que podem ser adicionadas ao perfil. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, adiciona a respectiva permissão deste usuário.
      * “Checkbox” no título da coluna: Ao selecionar este campo “checkbox”, que está presente no título da coluna, ele informa a Plataforma uCloud a ação de selecionar todas as permissões ainda não vinculadas ao perfil de permissionamento. Desta forma, uma única ação seleciona todas as permissões de uma única vez.
      * **Botão Aplicar**: Após o usuário certificar-se de que todas as alterações necessárias foram configuradas (inclusões ou exclusões), ele deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação a Plataforma uCloud fecha esta tela e recupera a tela anterior com seu conteúdo atualizado que apresenta a nova relação de permissões deste usuário que se está visualizando ou alterando o perfil.

Criando um Perfil de Permissionamento
-------------------------------------

Ao criar um Perfil de Permissionamento é necessário seguir o processo descrito, importa mencionar que apenas um usuário com permissão de criar perfil é que pode realizar esta ação e executar com êxito.
Para isto, o usuário deve clicar com o cursor do mouse no botão “Criar Perfil” assim a Plataforma uCloud exibe a tela abaixo;

.. image:: /figuras/ucloud_perfil_permissionamento_007.png
   :alt: perfil de permissionamento
   :align: center

----

* **Nome**: *Este campo é obrigatório*, o usuário deve inserir o nome do Perfil de Permissionamento. O nome do perfil deve ter, no mínimo, três (03) caracteres e o limite máximo de setenta (70) caracteres.

* **Descrição**: *Este campo é obrigatório*, o usuário deve inserir uma descrição estendida do Perfil de Permissionamento. A descrição do perfil deve ter, no mínimo, três (03) caracteres e no máximo cento e vinte (120) caracteres.

* **Permissões**: Nesta coluna são apresentadas todas as permissões disponíveis na Plataforma uCloud, as quais podem ser vinculadas ao Perfil de Permissionamento que se está a provisionar.

* **Mudar a Classificação**: Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de permissões de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Busca Rápida**: O usuário pode observar que abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de nomes de permissões. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca.

* **“Checkbox” no título da coluna**: Ao selecionar este campo “checkbox”, presente no título da coluna, a Plataforma uCloud atende a ação de selecionar todas as permissões ainda não vinculadas ao perfil de permissionamento. Desta forma, uma única ação seleciona todas as permissões de uma única vez.

* **“Checkbox” de cada Permissão**: Esta coluna apresenta a lista de permissões disponíveis na Plataforma uCloud. Ao lado de cada permissão existe um campo do tipo “checkbox”, ao ser selecionado, significa que a permissão será vinculada (habilitada) ao Perfil de Permissionamento.

* **Botão Criar**: Após checar se todas as permissões desejadas foram configuradas, o usuário deve clicar com o botão do mouse no botão Criar para configurar as alterações, de forma definitiva e imediata. A Plataforma uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que o novo Perfil de Permissionamento está cadastrado.

Após esta ação a Plataforma uCloud fecha a tela e retorna à tela anterior, sendo que o seu conteúdo atualizado apresenta o novo Perfil de Permissionamento, recém provisionado.

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

Para provisionar um novo perfil de visualização, o usuário deve clicar com o cursor do mouse sobre este botão, assim a Plataforma uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_perfil_visualizacao_002.png
   :alt: perfil de permissionamento
   :align: center

----

* **Nome**: *Este campo é obrigatório*, o usuário deve inserir o nome do Perfil de Visualização. O nome do perfil deve ter, no mínimo, três (03) caracteres e o limite máximo de setenta (70) caracteres. Importante ressaltar que é recomendado utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido).
* **Descrição**: *Este campo é obrigatório*, o usuário deve inserir uma descrição estendida do Perfil de Visualização. A descrição do perfil deve ter, no mínimo, três (03) caracteres e no máximo, cento e vinte (120) caracteres.
* **Permissões**: Nesta coluna são apresentadas todas as opções de menu disponíveis na Plataforma uCloud que podem ser vinculadas ao Perfil de Visualização que se está provisionando.
* **Mudar a Classificação**: Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de opções de menu, de forma alfabética crescente (a – z) ou decrescente (z – a).

  * **Busca Rápida**: O usuário pode observar o campo abaixo do nome da coluna, existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências, nesta lista de nomes de opções de menu. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualiza a tela e representa este padrão de busca.
  * **“Checkbox” no título da coluna**: Ao selecionar este campo “checkbox” presente no título da coluna, o usuário informa à Plataforma uCloud a ação de selecionar todas as opções de menu ainda não vinculadas ao perfil de visualização. Desta forma, uma única ação seleciona todas as opções de menu de uma única vez.
  * **“Checkbox” de cada Opção de Menu**: Esta coluna apresenta a lista das opções de menu disponíveis na Plataforma uCloud. Ao lado de cada opção de menu existe um campo do tipo “checkbox”, selecioná-lo significa que a opção de menu será vinculada (habilitada) ao Perfil de Visualização.
  * **Botão Criar**: Após certificar que todas as opções de menu desejadas foram configuradas, o usuário deve clicar com o botão do mouse no botão Criar para configurar as alterações, de forma definitiva e imediata. A Plataforma uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que o novo Perfil de Visualização está cadastrado.

Após esta ação a Plataforma uCloud fecha esta tela e retorna à tela anterior com seu conteúdo atualizado e apresenta o novo Perfil de Visualização recém provisionado.


Editando Perfil de Visualização
-------------------------------

O usuário pode verificar que ao visualizar a lista de perfis existem dois ícones na coluna Ações:

* Ações: Esta coluna apresenta dois ícones para que o usuário possa interagir com o perfil de visualização desejado:

  * **Ícone Lata de Lixo |icone_lixo|**: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud possa remover (excluir) este Perfil de Visualização, de forma imediata e definitiva.
  * **Ícone Edição |icone_edita_on|**: Basta o usuário clicar sobre este ícone para que a Plataforma uCloud possa apresentar uma tela que permite editar Perfil de Visualização respectivo. Importante mencionar que apenas o usuário com a permissão correta poderá editar as opções de menu de um Perfil de Visualização.

.. image:: /figuras/ucloud_perfil_visualizacao_003.png
   :alt: perfil de permissionamento
   :align: center

----

* **Nome**: O usuário pode alterar o nome do Perfil de Visualização. O nome do perfil deve ter, no mínimo, três (03) caracteres, e no máximo setenta (70) caracteres. Importante recomendar a utilização apenas dos caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido).
* **Descrição**: Este campo é obrigatório, o usuário deve inserir uma descrição estendida do Perfil de Visualização. A descrição do perfil deve ter, no mínimo, três (03) caracteres, e no máximo, cento e vinte (120) caracteres.
* **Permissões**: Nesta coluna são apresentadas todas as opções de menu disponíveis na Plataforma uCloud, elas podem ser vinculadas ao Perfil de Visualização que se está a provisionar.

  * **Mudar a Classificação**: Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de opções de menu de forma alfabética,  crescente (a – z) ou decrescente (z – a).
  * **Busca Rápida**: O usuário observa que abaixo do nome da coluna existe um campo em ‘branco’, este campo permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista, nomes de opções de menu. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualiza a tela, e representa a informação neste padrão de busca.
  * **“Checkbox” no título da coluna**: Ao selecionar este campo “checkbox”, presente no título da coluna, o clique informa à Plataforma uCloud a ação de selecionar todas as opções do menu, ainda não vinculadas ao perfil de visualização. Desta forma, uma única ação seleciona todas as opções de menu de uma vez.
  * **“Checkbox” de cada Opção de Menu**: Esta coluna apresenta a lista das opções de menu disponíveis na Plataforma uCloud. Ao lado de cada opção de menu existe um campo do tipo “checkbox”, ao ser selecionado, isto significa que a opção de menu será vinculada (habilitada) ao Perfil de Visualização.
  * **Botão Criar**: Após certificar que todas as opções desejadas no menu foram configuradas, o usuário pode clicar com o botão do mouse no botão Criar e configurar as alterações, de forma definitiva e imediata. A Plataforma uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que o novo Perfil de Visualização está cadastrado.

Após esta ação a Plataforma uCloud fecha a tela e retorna à tela anterior, com o conteúdo atualizado que apresenta o novo Perfil de Visualização recém provisionado.

Menu Configuração / Billing Admin
=================================

A configuração de Billing Admin é a forma como a Plataforma uCloud identifica o arquivo da fatura (cobrança) dos valores, referentes aos custos dos recursos computacionais de nuvem, nas credenciais do cliente.
Normalmente, os provedores de nuvem calculam os custos dos recursos computacionais num período de seis ou oito horas. Após este período de contabilização, um arquivo texto não formatado (Comma Separated Values – .CSV) é atualizado com todos os valores de todo o período de vigência da relação do cliente com o provedor.
A configuração de Billing Admin, na Plataforma uCloud, estabelece uma identificação e o agendamento de um processo de sincronização (download) do conteúdo do arquivo texto não formatado (.CSV), do provedor para dentro das bases de dados do uCloud. Esta sincronização é planejada para que a apresentação dos valores na tela do uCloud seja rápida, uma vez que todos os valores já estão atualizados e prontos para o usuário consultar - valores dos recursos computacionais do provedor de serviço de nuvem.
A Plataforma uCloud não cria valores - o ator responsável por gerar e adicionar um valor aos recursos computacionais consumidos no período, são os provedores de serviço de nuvem pública.
Qualquer discrepância de valores, consultados na console do provedor pelo usuário e na interface da Plataforma uCloud pode estar associada a alguma condição específica estabelecida no Contrato. Veja acima no item Administração de Contrato.
Nesta tela, são listados apenas os provedores provisionados para esta empresa. Importante ressaltar que a Plataforma uCloud é um ambiente multi-nuvem (multi-cloud), desta forma, pode ser listada mais de uma configuração de Billing Admin para cada empresa.
Na tela a seguir, é apresentado um exemplo de Billing Profile para dois provedores diferentes de serviço de nuvem (AWS e Azure). É possível haver apenas um ou mais provedores configurados.

.. inserir tela (remover este comentario)

.. important:: |importante| *Importante mencionar que não é objetivo deste documento descrever o processo de configuração de Billing Admin, pois apenas usuários com perfil de Administrador da Plataforma uCloud têm permissão para isto. Veja o documento Manual do Administrador da Plataforma uCloud onde está descrito o processo correto de provisionar um Billing Admin.*

Segue a descrição dos botões desta tela:

* **Botão Lançar Accountant** |botao_lanca_acct| : Este botão apresenta a tela para provisionar um novo Billing Profile na Plataforma uCloud. Importa ressaltar que apenas o usuário com perfil de Administrador de Plataforma pode provisionar um novo Billing Profile. Veja o documento Manual do Administrador da Plataforma uCloud onde está descrito o processo correto de provisionar um Billing Admin.

* **Botão Limpar Histórico** |botao_limpa_acct| : *ATENÇÃO, é relevante ressaltar que este botão efetua o expurgo (apaga) completo de todos os registros de valores de bilhetagem das bases de dados da Plataforma uCloud, de forma definitiva e irreversível. Serão removidos todos os valores desde a data  inicial até o dia da ação.*

* **Botão Refresh** |botao_refresh| : A Plataforma uCloud se comunica com o console dos provedores através da API Rest, assim, toda ação executada ou configurada nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes, então, executem a ação desejada. Para atualizar apenas o conteúdo das seções de tela (as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, o qual aciona a execução e atualiza as informações contidas na base de dados da plataforma.

Informações de Registro (LOG) do Billing Admin
----------------------------------------------

A configuração de Billing Admin é a forma como a Plataforma uCloud identifica o arquivo da fatura (cobrança) dos valores, referentes aos custos dos recursos computacionais de nuvem, nas credenciais do cliente.
Normalmente, os provedores de nuvem calculam os custos dos recursos computacionais num período de seis ou oito horas. Após este período de contabilização, um arquivo texto não formatado (Comma Separated Values – .CSV) é atualizado com todos os valores de todo o período de vigência da relação do cliente com o provedor.
A configuração de Billing Admin, na Plataforma uCloud, estabelece uma identificação e o agendamento de um processo de sincronização (download) do conteúdo do arquivo texto não formatado (.CSV), do provedor para dentro das bases de dados do uCloud. Esta sincronização é planejada para que a apresentação dos valores na tela do uCloud seja rápida, uma vez que todos os valores já estão atualizados e prontos para o usuário consultar - valores dos recursos computacionais do provedor de serviço de nuvem.
A Plataforma uCloud não cria valores - o ator responsável por gerar e adicionar um valor aos recursos computacionais consumidos no período, são os provedores de serviço de nuvem pública.
Qualquer discrepância de valores, consultados na console do provedor pelo usuário e na interface da Plataforma uCloud pode estar associada a alguma condição específica estabelecida no Contrato. Veja acima no item Administração de Contrato.
Nesta tela, são listados apenas os provedores provisionados para esta empresa. Importante ressaltar que a Plataforma uCloud é um ambiente multi-nuvem (multi-cloud), desta forma, pode ser listada mais de uma configuração de Billing Admin para cada empresa.
Na tela a seguir, é apresentado um exemplo de Billing Profile para dois provedores diferentes de serviço de nuvem (AWS e Azure). É possível haver apenas um ou mais provedores configurados.

.. image:: /figuras/ucloud_billing_admin_001.png
   :alt: perfil de permissionamento
   :align: center

----

Importante mencionar que não é objetivo deste documento descrever o processo de configuração de Billing Admin, pois apenas usuários com perfil de Administrador da Plataforma uCloud têm permissão para isto. Veja o documento Manual do Administrador da Plataforma uCloud onde está descrito o processo correto de provisionar um Billing Admin.
Segue a descrição dos botões desta tela;

* **Botão Lançar Accountant** |botao_lanca_acct|: Este botão apresenta a tela para provisionar um novo Billing Profile na Plataforma uCloud. Importa ressaltar que apenas o usuário com perfil de Administrador de Plataforma pode provisionar um novo Billing Profile. Veja o documento Manual do Administrador da Plataforma uCloud onde está descrito o processo correto de provisionar um Billing Admin.
* **Botão Limpar Histórico** |botao_limpa_acct|: *ATENÇÃO, é relevante ressaltar que este botão efetua o expurgo (apaga) completo de todos os registros de valores de bilhetagem das bases de dados da Plataforma uCloud, de forma definitiva e irreversível. Serão removidos todos os valores desde a data  inicial até o dia da ação*.
* **Botão Refresh** |botao_refresh|: A Plataforma uCloud se comunica com o console dos provedores através da API Rest, assim, toda ação executada ou configurada nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes, então, executem a ação desejada. Para atualizar apenas o conteúdo das seções de tela (as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, o qual aciona a execução e atualiza as informações contidas na base de dados da plataforma.

Registro (LOG) do Billing Admin
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

É permitido ao usuário com o perfil de Administrador do Contrato identificar potenciais discrepâncias de valores, que porventura sejam apresentadas no menu Financeiro, este usuário pode verificar se há algum problema na comunicação entre a Plataforma uCloud e a console do provedor, através do botão “Log”.
Ao visualizar todos os Billing Admin, o usuário pode identificar alguns ícones a cada configuração provisionada;

.. image:: /figuras/ucloud_billing_admin_002.png
   :alt: perfil de permissionamento
   :align: center

----

* **Nome**: Esta etiqueta identifica o nome do Billing Profile que foi informado no momento de sua configuração inicial.
* **Indicador do Tipo de Execução**: Esta etiqueta identifica (“ASYNC”) o tipo de execução do processo de sincronização, selecionado no momento da sua configuração inicial.
* **Ícone de Status de Execução**: Esta etiqueta apresenta o status do processo de sincronização da Plataforma uCloud com a console do provedor de serviço de nuvem pública.
* **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para informar a Plataforma uCloud que remova (exclua) esta configuração de Billing Admin de forma imediata e definitiva.
* **Ícone LOG**: Basta o usuário clicar neste ícone que a Plataforma uCloud apresenta uma tela que permite visualizar o registro de atividade (log) referente às tarefas de sincronização do Billing Profile com as bases de dados do uCloud. Este recurso é fundamental para identificar qualquer problema de comunicação da Plataforma uCloud com o ambiente do provedor de serviço de nuvem pública, para obtenção do arquivo texto não formatado (.CSV).

.. image:: /figuras/ucloud_billing_admin_003.png
   :alt: perfil de permissionamento
   :align: center

----

Menu Configuração / Tagueamento de Recursos USN
===============================================

Esta opção, do menu de funcionalidades, somente deve ser acessada quando o modelo Financeiro do contrato for vinculado a um Ministério, Órgão ou Agência do Governo Brasileiro. E que os valores dos recursos computacionais de nuvem pública, sejam convertidos para Unidade de Serviço de Nuvem (USN).

.. note:: |atencao| *Importante mencionar empresas privadas não necessitam nenhuma das facilidades de USN descritos neste menu*.

No modelo de cobrança do recurso computacional de nuvem pública, todo recurso deve ter uma etiqueta (tag) na qual é aplicado um valor, em USN, a ser tarifado (billing) no ambiente da Plataforma uCloud. Os recursos importados do arquivo de billing das nuvens públicas que não possuam nenhuma etiqueta (tag) no provedor de serviço de nuvens, no processo de importação, estes recursos recebem uma etiqueta (tag) na plataforma do uCloud, baseado no perfil de tagueamento adicionado ao contrato ao qual este recurso pertence.

Uma etiqueta (tag) é um rótulo no qual o usuário atribui um valor a um recurso computacional de nuvem pública. As etiquetas (tags) permitem categorizar seus recursos nas nuvens. Por exemplo, o usuário ou a organização, podem definir um conjunto de etiquetas (tag), para as instâncias do Amazon EC2, na sua conta que auxilie rastrear o nível do agrupamento (empilhamento de valores - stack) de cada recurso computacional de nuvem pública consumido.

A seguir, será descrito o processo de criação de um perfil de etiquetamento de recursos computacionais de nuvem pública (tag profile) em USN.

Criação de um Tagueamento de Recurso USN
----------------------------------------

O usuário deve acessar o Menu Configuração / Tagueamento de Recurso USN para a Plataforma uCloud apresentar a tela abaixo:

.. image:: /figuras/ucloud_criar_recurso_usn_001.png
   :alt: perfil de permissionamento
   :align: center

----

* **Selecione um Contrato**: Este campo é do tipo “dropdown”, quando o usuário clicar com o cursor do mouse sobre ele, a Plataforma uCloud listará todos os contratos existentes no ambiente do uCloud, o usuário deve selecionar o contrato da empresa onde o recurso será convertido para USN.

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

* **Botão Importar**: Este botão fica ativo (verde) após preencher todos os campos descritos anteriormente. Assim, o usuário deve clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud possa iniciar o processo de importação do arquivo de Tagueamento de USN. O usuário visualiza a tela a seguir.

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

Quando configurada a comunicação entre a Plataforma uCloud e a console do provedor de serviço de nuvem pública, como a Plataforma uCloud, dois dos cinco pontos de uma plataforma de **CSB**, permitem às empresas atuar em cinco pontos fundamentais para o gerenciamento de ambientes híbridos multi-nuvem. Na apresentação do menu de Máquinas Virtuais, serão focados apenas dois destes cinco pontos fundamentais:

1. **Governança Financeira**
2. **Billing** (Faturamento dos Serviços)
3. **Monitoração da Infraestrutura**
4. **Inventário** (Assessment)

   A Plataforma uCloud se conecta aos provedores de nuvem através do cadastramento de credenciais de acesso específicas para cada provedor de serviço de nuvem (público e/ou privado).
   Uma vez que as credenciais estão configuradas na Plataforma uCloud, a primeira atividade é sincronizar as configurações e o inventário dos recursos computacionais existentes no provedor (máquinas virtuais – workloads). Este inventário de máquinas virtuais é extraído e adicionado nas bases de dados da plataforma do uCloud, de forma que é apresentado rapidamente, na tela do usuário.

5. **Operação da Infraestrutura**

  Com o inventário disponível diretamente dentro da Plataforma uCloud, o usuário pode operar cada uma das máquinas virtuais, independente de em qual provedor de nuvem este recurso está provisionado. Será descrito, a seguir, as possíveis operações a serem aplicadas aos recursos computacionais existentes nos provedores de nuvem (público e/ou privado).

  A menção *operar* significa o leitor que é a capacidade do usuário comandar certas ações diretamente nestas máquinas virtuais, como ações de: parar (*shutdown*), reiniciar (*restart*), suspender (*suspend*), remover (*delete*), para citar algumas operações básicas.

  Através da interface da Plataforma uCloud o usuário pode enviar comandos para os consoles de cada provedor de nuvem, além das ações acima listadas. Este também pode visualizar as informações das configurações específicas da máquina virtual, bem como alterar ou adicionar algum recurso extra a esta máquina virtual (por exemplo: placa de rede, disco, grupo de segurança, snapshot, entre outros).

Menu Máquinas Virtuais
======================

Quando o usuário acessa esta opção de menu, a Plataforma uCloud apresenta uma tela com o inventário completo de todas as máquinas virtuais (instâncias, workloads) que podem ser acessadas com as credenciais da empresa.
Esta tela pode se apresentar muito extensa por listar todas as máquinas virtuais encontradas. No exemplo abaixo, estão listadas apenas três máquinas virtuais:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_001.png
   :alt: perfil de permissionamento
   :align: center

----

As colunas da tela listada anteriormente, está descrita abaixo:
* **Botão “Criar Máquina Virtual** (|botao_criar_VM|): Este botão permite provisionar (criar) uma máquina virtual no(s) ambiente(s) do(s) provedor de serviço de nuvem (público e/ou privado). Os detalhes estão descritos no item Criando uma Máquina Virtual.

* **Botão Refresh** (|botao_refresh|): A Plataforma uCloud se comunica com a console dos provedores através da API Rest, assim toda ação executada ou configurada, nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada. Para atualizar apenas o conteúdo das seções de tela (ou as informações contidas nestas seções) é mandatório que o usuário clique com o mouse sobre o botão Refresh, ele executa apenas a atualização das informações contidas nas bases de dados da plataforma.

* **Coluna Acionável**: Esta coluna apresenta uma forma alternativa de interagir com várias máquinas virtuais com um único comando. Cada linha está representada por um ícone selecionável (“  ”). Quando o usuário seleciona uma linha ou várias, a Plataforma uCloud apresenta ícone(s) acima desta coluna, eles representam ações ao usuário que podem ser executadas de uma única vez, para todas as linhas selecionadas. A seguir, são apresentados os seis ícones, suas ações são distintas:

  * **Ícone de Iniciar** (|icone_vm_start|): Este ícone permite ao usuário iniciar (Start – Boot) toda(s) máquina(s) virtual(is) que estiver com o status de “Stopped”. Este ícone ficará inativo se alguma máquina virtual selecionada permanecer com um status diferente de “Stopped”.
  * **Ícone de Parar** (|icone_vm_stop|): Este ícone permite ao usuário parar (Stop – Shutdown) toda(s) máquina(s) virtual(is) que estiver com o status de “Running”. Este ícone ficará inativo se alguma máquina virtual selecionada permanecer com um status diferente de “Running”.
  * **Ícone de Reiniciar** (|icone_vm_reboot|): Este ícone permite ao usuário reiniciar (Restart – Reboot) toda(s) máquina(s) virtual(is) que estiver com o status de “Running”.
  * **Ícone de Suspender** (|icone_vm_suspend|): Este ícone permite ao usuário suspender (Suspend) toda(s) máquina(s) virtual(is) que estiver com o status de “Running”.
  * **Ícone de Retomar** (|icone_vm_resume|): Este ícone permite ao usuário retomar (Resume) toda(s) máquina(s) virtual(is) que estiver com o status de “Suspended”.
  * **Ícone de Lata do Lixo** (|icone_lixo|): Este ícone permite ao usuário excluir (Remove – Delete) toda(s) máquina(s) virtual(is) que estiver selecionada com o ícone selecionável (“  ” – check mark). Este ícone somente ficará ativo para excluir as máquinas virtuais que foram criadas pelo próprio usuário que está registrado na plataforma. Este ícone ficará inativo, se o usuário registrado, selecionar máquinas virtuais criadas por outros usuários.
  * **Ícone de Desconectar** (|icone_desconecta|): Este ícone permite ao usuário desconectar (unplug) as máquinas virtuais da Plataforma uCloud. Importante ressaltar que esta ação não remove (delete) a máquina virtual do ambiente do provedor de serviço de nuvem. Esta ação removerá a máquina virtual do inventário da base de dados da Plataforma uCloud, portanto, a máquina não mais será listada nesta tela.

* **Busca Rápida**: O usuário pode observar que logo abaixo do nome da coluna existe um campo em *branco* que permite efetuar uma busca rápida no conteúdo recuperado para reduzir e estreitar a quantidade de incidências desta lista de nomes de opções de menu. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca refletida na relação de máquinas virtuais na lista.

  * **Nome**: Esta coluna apresenta o nome da máquina virtual informado no momento da sua criação, no console do provedor de serviço de nuvem, configurado através do uCloud. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de máquinas virtuais de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **Usuário**: Esta coluna apresenta o login de usuário que estava com uma sessão ativa no momento do provisionamento desta máquina virtual, este á o usuário que está vinculado para efeito da totalização de todos os custos relativos à existência desta máquina virtual. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca refletida na relação de máquinas virtuais na lista.
  * **IP Privado**: Esta coluna apresenta o endereço TCP-IP vinculado a esta máquina virtual no momento de sua criação. Importante ressaltar que este endereçamento TCP-IP pertence ao ambiente de rede privada do provedor de serviço de nuvem (recebe do servidor DHCP interno do provedor). Este endereço poderá mudar quando a máquina virtual for reiniciada (reboot). Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **IP Público**: Esta coluna pode estar em *branco*, pois nesta coluna será apresentado o endereço TCP-IP Público que foi vinculado a esta máquina virtual em um momento posterior ao provisionamento da máquina virtual. O Endereço TCP-IP Público, é um endereço fixo e pode incorrer em custos mensais para sua manutenção e vinculação a uma máquina virtual provisionada. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **Memória**: Nesta coluna será apresentado um número que é a quantidade de memória RAM configurada nesta máquina virtual, expressa em Gigabytes. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de máquinas virtuais com base no tamanho da memória, de forma crescente ou decrescente.
  * **CPUs**: Nesta coluna será apresentado um número que é a quantidade de CPU(s) configurada nesta máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de máquinas virtuais com base na quantidade de CPU(s), de forma crescente ou decrescente.
  * **Status**: Nesta coluna será apresentado o status corrente da máquina virtual. Importante ressaltar que o status é obtido do provedor de serviço de nuvem, pois a máquina virtual está instalada e sendo executada na infraestrutura do provedor de serviço de nuvem. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica o status da lista de máquinas virtuais, de forma alfabética crescente (a – z) ou decrescente (z – a). A Plataforma uCloud apresenta os seguintes status:

    * **Running**: Status que indica que a máquina virtual está em funcionamento normal.
    * **Stopped**: Status que indica que a máquina virtual está parada.
    * **Suspended**: Este status indica que a máquina virtual está em um estado suspenso, possibilitando um tempo de inicialização (boot) mais rápido que o estado parado (stopped).
    * **Unrecognized**: Este status pode ser apresentado, pois se refere a um estado, temporário, onde momentaneamente não foi possível distinguir se a máquina está parada ou ‘rodando’ (falha de comunicação entre a Plataforma uCloud e o console do provedor de serviço de nuvem pública).
    * **Deallocated**: Este status é particular da nuvem Azure e se refere a uma máquina virtual que se encontra parada, não está sendo cobrada, este estado faz a liberação de alguns recursos e seu tempo para inicialização (boot) será maior. Para maiores detalhes, consultar material de documentação do Azure.
    * **Orphan**: Este status somente será apresentado quando uma máquina não é encontrada no provedor de serviço de nuvem ou no ambiente de virtualização do datacenter privado (hypervisor).

  * **TAGs (Etiquetas)**: Esta coluna apresenta as TAGs (etiquetas) que foram provisionadas diretamente através da console do provedor de serviço de nuvem pública, quanto através da Plataforma uCloud (Menu Inventário de Recursos).

Gerenciando uma Máquina Virtual
-------------------------------

Para gerenciar uma máquina virtual é necessário listar o relatório das máquinas, o usuário deve clicar com o cursor do mouse sobre qualquer uma das máquinas virtuais listadas para que a Plataforma uCloud possa apresentar a tela que permite o gerenciamento e operacionalização da máquina virtual selecionada.
Esta tela possui diversas seções (cards) ela é bem ampla e completa, por isto, será apresentada a figura do início da tela e, a seguir a descrição de cada seção em detalhe e de forma individualizada.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_022.png
   :alt: perfil de permissionamento
   :align: center

----

A Plataforma uCloud apresenta alguns ícones de botões, logo acima das seções (cards) para gerenciar a máquina virtual.

* **Ícone de Iniciar** (|icone_vm_start|): Este ícone permite ao usuário iniciar (Start – Boot) a máquina virtual que estiver com o status de “Stopped”. Este ícone permanece inativo se alguma máquina virtual selecionada estiver com um status diferente de “Stopped”.

* **Ícone de Parar** (|icone_vm_stop|): Este ícone permite ao usuário parar (Stop – Shutdown) toda(s) máquina(s) virtual(is) que estiver(em) com o status de “Running”. Este ícone permanece inativo se alguma máquina virtual selecionada estiver com um status diferente de “Running”.

* **Ícone de Reiniciar** (|icone_vm_reboot|): Este ícone permite ao usuário reiniciar (Restart – Reboot) toda(s) a(s) máquina(s) virtual(is) que estiver(em) com o status de “Running”.

* **Ícone de Suspender** (|icone_vm_suspend|): Este ícone permite ao usuário suspender (Suspend) toda(s) a(s) máquina(s) virtual(is) que estiver(em) com o status de “Running”.

* **Ícone de Retomar** (|icone_vm_resume|): Este ícone permite ao usuário retomar (Resume) toda(s) a(s) máquina(s) virtual(is) que estiver(em) com o status de “Suspended”.

* **Ícone Remote Console** (|icone_vm_ssh|): Este ícone permite ao usuário iniciar uma sessão de console do sistema operacional diretamente através da interface web da Plataforma uCloud. Basta o usuário clicar com o cursor do mouse sobre este ícone, que a Plataforma uCloud irá apresentar a tela abaixo:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_024.png
   :alt: perfil de permissionamento
   :align: center

----

  * **Nome**: Este campo apresenta o nome  da máquina virtual a qual o usuário deseja iniciar uma sessão de console.
  * **Versão**: Este campo apresenta o nome estendido do sistema operacional (template) que foi selecionado durante o provisionamento desta máquina virtual.
  * **Tipo**: Este campo apresenta o nome tipo do sistema operacional que foi selecionado durante o provisionamento desta máquina virtual.
  * **Protocolo**: Este campo é do tipo “dropdown”, quando o usuário clicar com o cursor do mouse sobre este campo, serão listadas os tipos de protocolos de console disponíveis na versão corrente da Plataforma uCloud. O usuário deve selecionar o protocolo ideal (o adequado) para iniciar uma sessão de console no sistema operacional da máquina virtual.

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

  * **Botão Conectar**: Basta o usuário clicar com o cursor do mouse sobre este botão e a Plataforma uCloud irá apresentar uma janela pop-up com a sessão de console conforme o exemplo da tela abaixo:

.. comentario incluir tela de SSH do uCloud

.. attention:: |atencao| Importante ressaltar que a porta informada deve estar aberta para a rede pública Internet na configuração de Grupo de Segurança (Security Group) vinculada a esta máquina virtual. Caso o Grupo de Segurança vinculado a esta máquina não esteja configurado com a referida porta do protocolo, a Plataforma uCloud não será capaz de iniciar uma sessão de console.

.. note:: |nota| Importante ressaltar que cada sistema operacional somente permite iniciar sessões do console através de um protocolo específico, consulte a documentação técnica do sistema operacional em questão para selecionar o protocolo correto.

.. important:: |importante| **ATENÇÃO**: caso o usuário selecione a opção VNC (Virtual Network Computing) é importante mencionar que esta modalidade necessita de um software adicional que funciona em um modelo cliente / servidor. Caso este componente server não esteja instalado, ou seu serviço não estiver ativo, na máquina virtual desejada, a Plataforma uCloud não será capaz de iniciar uma sessão de console através desta opção.

Adicionalmente, é necessário que a senha de usuário de conexão seja conhecida, sem a informação da senha correta, a Plataforma uCloud não será capaz de iniciar a sessão de console.

* **Botão Excluir** |botao_excluir|: Este botão efetua a exclusão da máquina virtual do ambiente do provedor de serviço de nuvem. Esta ação é irreversível e definitiva, por isto, a Plataforma uCloud apresenta uma tela para confirmação desta ação.

  * **Botão Não Cancelar**: Este botão permite ao usuário cancelar a ação e manter a máquina virtual tanto no provedor de serviço de nuvem quanto na interface da Plataforma uCloud. Será apresentada uma tela informando, ao usuário, informando que a máquina virtual não será excluída.
  * **Botão Sim Pode Excluir**: Ao clicar com o cursor do mouse neste botão, a Plataforma uCloud envia a solicitação de exclusão para o provedor de serviço de nuvem (público e/ou privado) no qual esta máquina virtual está sendo executada, e em seguida, remove a mesma das bases de dados do uCloud. Importante mencionar, que quaisquer recursos computacionais adicionais (disco adicional, IP Públicos, snapshot) associados a esta máquina virtual, não serão excluídos.

----

A seguir descrição de cada seção (*card*) de forma individual:

Seção Geral - VMs
~~~~~~~~~~~~~~~~~

Esta seção permite visualizar as informações fundamentais e básicas da máquina virtual.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_025.png
   :alt: altera Usuario
   :align: center

----

* **Status**: Este campo apresenta o status corrente da máquina virtual. Importante ressaltar que status é obtido do provedor de serviço de nuvem, pois a máquina virtual está instalada e sendo executada na Infraestrutura do provedor de serviço de nuvem. A Plataforma uCloud pode apresentar neste campo, o seguinte:

  * **Running**: Indica que a máquina virtual está em funcionamento normal.
  * **Stopped**: Indica no status que a máquina virtual está parada.
  * **Suspended**: Indica que a máquina virtual está em um estado suspenso, possibilitando um tempo de inicialização (boot) mais rápido que o estado parado (stopped).
  * **Unrecognized**: Este status pode ser apresentado, pois se refere a um estado, temporário, onde momentaneamente não foi possível distinguir se a máquina está parada ou rolando (falha de comunicação entre a Plataforma uCloud e o console do provedor de serviço de nuvem pública).
  * **Deallocated**: Este status é particular da nuvem Azure, refere-se a uma máquina virtual que se encontra parada, e não está sendo cobrada, este estado faz a liberação de alguns recursos e seu tempo para inicialização (boot) será maior. Para maiores detalhes, consultar material de documentação do Azure.
  * **Orphan**: Este status somente será apresentado quando uma máquina não é encontrada no provedor de serviço de nuvem ou no ambiente de virtualização do datacenter privado (hypervisor).

* **Nome**: Este campo apresenta o nome da máquina virtual que foi informado no momento da sua criação, no console do provedor de serviço de nuvem ou no momento que foi configurado através do uCloud.

* **Criada em**: Este campo apresenta a data e a hora do provisionamento da máquina virtual (no formato DD/MM/AAAA HH:MM:SS). Adicionalmente é apresentada a informação do tempo total que esta máquina virtual está ativa (no formato dias, horas, minutos e segundos – XXd NNh YYm ZZs).

* **Região**: Neste campo será apresentado o código (ou o nome) da região onde a máquina virtual foi vinculada, no momento do seu provisionamento, tanto no console do provedor de serviço de nuvem quanto através da interface da Plataforma uCloud. Importante mencionar que cada provedor possui identificação de regiões específicas, este campo reflete suas especificidades.

* **Zona de Disponibilidade**: *Este campo é opcional*, pois nem todos os provedores de serviço de nuvem possuem zonas de disponibilidade (zonas dentro de uma região). Este campo é apresentado nos casos em que o provedor possui esta informação.

* **IPs Públicos**: Este campo apresenta o endereço TCP-IP Público Dinâmico (obtido do servidor DHCP interno do provedor de serviço de nuvem), o qual foi vinculado a esta máquina no momento do provisionamento da máquina virtual. Importante ressaltar que o Endereço TCP-IP Público Dinâmico, não é um endereço fixo. Este endereço pode ser alterado quando esta máquina virtual for reiniciada (reboot). Caso o usuário veja um Endereço TCP-IP, mas sem a indicação "Dinâmico", isto significa que esta máquina virtual possui um Endereço TCP-IP fixo, e este não será alterado mesmo após a máquina virtual ter sido reiniciada.

* **IPs Privados**: Neste campo será apresentado o endereço TCP-IP vinculado a esta máquina virtual, no momento da sua criação. Importante ressaltar que este endereçamento TCP-IP pertence ao ambiente de rede privada do provedor de serviço de nuvem (obtido do servidor DHCP interno do provedor de serviço de nuvem) este endereço poderá ser alterado quando esta máquina virtual for reiniciada (reboot).

* **Par de Chave**: Este campo apresenta o nome da chave criptográfica, informada durante o processo de provisionamento desta máquina virtual. No caso do uso de autenticação de chave pública SSH, é bastante típico o usuário criar (ou seja, provisionar) o par de chaves para si próprio. Cada par de chaves SSH inclui duas chaves:

  * Uma chave pública que é copiada para o (s) servidor (es) SSH. Qualquer pessoa com uma cópia da chave pública pode criptografar dados que só podem ser lidos pela pessoa que possui a chave privada correspondente. Depois que um servidor SSH recebe uma chave pública de um usuário e a considera confiável, o servidor marca a chave como autorizada em seu arquivo authorized_keys. Essas chaves são chamadas de chaves autorizadas.

  * Uma chave privada que permanece (apenas) com o usuário. A posse dessa chave é a prova da identidade do usuário. Apenas um usuário de posse de uma chave privada que corresponda à chave pública no servidor será capaz de se autenticar com sucesso. As chaves privadas precisam ser armazenadas e manuseadas com cuidado, nenhuma cópia da chave privada deve ser distribuída. As chaves privadas usadas para autenticação do usuário são chamadas de chaves de identidade.

* **Grupo de Segurança**: Neste campo será apresentado o nome do Grupo de Segurança (Security Group) vinculado à máquina virtual, que controla as portas TCP-IP as quais podem ser utilizadas para acesso a esta máquina virtual. Um grupo de segurança atua como firewall virtual para as máquinas virtuais. O usuário pode criar diversos grupos de segurança e personalizar cada um com as regras que permitem tráfego de entrada ou de saída nas instâncias associadas.

  * **Botão de Alteração de Grupo de Segurança** |icone_edita_on|: Este botão permite ao usuário alterar a vinculação da máquina virtual ao Grupo de Segurança que está sendo apresentado na interface. Durante o provisionamento da máquina virtual, o usuário selecionou um Grupo de Segurança para controlar as portas TCP-IP desta máquina virtual. Para alterar o Grupo de Segurança que está vinculado a esta máquina virtual, basta clicar com o cursor do mouse sobre este botão e a interface da Plataforma uCloud alterna para o modo de edição do conteúdo deste campo. Neste momento, a Plataforma uCloud apresenta uma lista “drop-box” com uma lista de todos os Grupos de Segurança que este usuário tem autorização de ver. Basta o usuário clicar com o botão do mouse sobre o Grupo de Segurança desejado.

  * **Ícone de Confirmação** |icone_conf_verde|: Após selecionar o Grupo de Segurança desejado, será  permitido confirmar a intenção de alterar o conteúdo no campo desejado, em seguida, a Plataforma uCloud apresenta um ícone de confirmação. Após finalizar a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Concluída esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma uCloud e na configuração da máquina virtual no ambiente do provedor de serviço de nuvem pública.

  * **Ícone de Cancelamento** |icone_cancela_vermelho|: Para o caso do usuário clicar sobre o ícone de edição por engano ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna aos valores iniciais, antes de qualquer preenchimento ou alteração.

* **Flavor**: Este campo apresenta o nome do flavor selecionado como a definição do tipo de hardware da máquina virtual. Um flavor define o tamanho dos recursos de computação (número de CPUs virtuais, memória e capacidade de armazenamento) que podem ser atribuídos automaticamente a instâncias da máquina virtual, em uma configuração de nuvem. Cada provedor de serviço de nuvem possui uma denominação específica para o ambiente do provedor. Importante mencionar que a configuração dos recursos (CPU, memória e disco) podem ser similares em diferentes provedores, mas sua nomenclatura é particular.

* **Template**: Este campo apresenta o sistema operacional (template) selecionado no momento do provisionamento da máquina virtual.

* **Virtual Datacenter**: Este campo apresenta o nome do Virtual Datacenter (VDC) ao qual esta máquina virtual está vinculada. Veja no item Virtual Datacenters, para entender o conceito e saber como provisionar um Virtual Datacenter.

  * **Botão para Mover para outro Virtual Datacenter** |icone_edita_vdc|: Este botão permite ao usuário alterar a vinculação da máquina virtual ao Virtual Datacenter que está sendo apresentado na interface. Durante o provisionamento da máquina virtual, a Plataforma uCloud, vincula esta máquina virtual ao Virtual Datacenter que o usuário selecionou. Para mover a máquina virtual para outro Virtual Datacenter, basta clicar com o cursor do mouse sobre este botão e a interface da Plataforma uCloud alterna para o modo de edição do conteúdo deste campo. Para mover esta máquina virtual para outro Virtual Datacenter, basta clicar com o cursor do mouse sobre este botão e a interface da Plataforma uCloud habilita editar o conteúdo do campo. Assim o usuário pode digitar uma parte da sequência de caracteres do novo Virtual Datacenter, para que a Plataforma uCloud apresenta uma lista que combina com a sequência de caracteres desejada:

.. image:: /figuras/ucloud_botao_edita_vdc.png
   :alt: altera Usuario
   :align: center

----

  * **Ícone de Confirmação** |icone_conf_verde|: Após selecionar o novo Virtual Datacenter, será  permitido confirmar a intenção de mover a máquina virtual para outro Virtual Datacenter, e a Plataforma uCloud apresenta um ícone de confirmação. Após finalizar a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Concluída esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma uCloud de forma permanente e imediata.
  * **Ícone de Cancelamento** |icone_cancela_vermelho|: Para o caso do usuário clicar sobre o ícone de edição por engano ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna aos valores iniciais, antes de qualquer preenchimento ou alteração.[e]

* **Usuário**: Este campo apresenta a credencial do usuário que estava conectado na Plataforma uCloud, o qual foi o responsável pelo aprovisionamento da máquina virtual no provedor de serviço de nuvem. Esta informação pode ser alterada com os botões que se apresentam ao lado da tela:

  * **Botão de Edição de Usuário** |icone_edita_user|: Este botão permite ao usuário alterar o nome do usuário que está vinculado a esta máquina virtual, basta clicar com o cursor do mouse sobre este botão e a interface da Plataforma uCloud habilita editar o conteúdo do campo. Assim o usuário pode digitar uma parte da sequência de caracteres do novo usuário, para que a Plataforma uCloud recupere a lista de usuários com a informação que combina com a palavra digitada.

.. image:: /figuras/ucloud_botao_change_user_vm.png
   :alt: altera Usuario
   :align: center

----

    * **Ícone de Confirmação** |icone_conf_verde|: Após selecionar o usuário desejado, é permitido confirmar a intenção de alterar o conteúdo no campo desejado, em seguida, a Plataforma uCloud apresenta um ícone de confirmação. Após finalizar a alteração do conteúdo do campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Concluída esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma uCloud.
    * **Ícone de Cancelamento** |icone_cancela_vermelho|: Para o caso do usuário clicar sobre o ícone de edição por engano ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna aos valores iniciais, antes de qualquer preenchimento ou alteração.

* **Proteção Exclusão Acidental**: Este ícone indica se esta máquina virtual está com o parâmetro de exclusão acidental configurado, como: Desabilitado (vermelho) ou Habilitado (verde).

  * **Ícone Disable** |icone_desb_verm|: Este ícone indica que a proteção acidental está desabilitada. Isto significa que esta máquina pode ser excluída (apagada) sem restrição, apenas com a confirmação desta ação por parte do usuário que a está removendo (excluindo).

  * **Ícone Enable** |icone_habil_verde|: Este ícone indica que a proteção acidental está habilitada. Isto significa que esta máquina não pode ser excluída (apagada). Para efetuar a remoção desta máquina virtual, é necessário que o usuário que provisionou a máquina virtual e a habilitou neste parâmetro, realize a alteração do parâmetro para: Desabilitado. Posteriormente, deve efetuar o procedimento de exclusão da máquina virtual, ao clicar no botão, que deve estar ativo.

* **Template Privado (opcional/variável)**: Este ícone |icone_private_net| permite ao usuário criar um tipo de hardware (“flavor”) personalizado. Este novo “flavor” pode ter um nome personalizado (diferente do nome no provedor de serviço de nuvem). Sua configuração é baseada nas configurações do hardware configurado na máquina virtual. Este recurso pode ser útil para personalizar opções de “flavors” específicos para o cenário da empresa.

* **Identificador de Provedor**: Este campo apresenta a identificação da máquina virtual como nomenclatura baseada em recursos (RBN - Resource-based Naming) que é gerada automaticamente pelo próprio provedor de serviço de nuvem pública. A Plataforma uCloud, não possui mecanismos para criar, ou alterar, o conteúdo desta informação. Consulte a documentação técnica online de cada provedor para mais informações.

* **ID de Rede**: Este campo apresenta a identificação da interface de rede elástica é um componente de rede lógico de cada provedor de serviço de nuvem pública e que representa uma placa de rede virtual.

* **Network ID do Provedor**: Este campo apresenta a identificação da Rede é um componente de rede lógico de cada provedor de serviço de nuvem pública e que representa uma placa de rede virtual.

Seção Performance Instantânea
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta seção apresenta um gráfico que demonstra a ocupação, na máquina virtual, da CPU e da memória. Importante mencionar que a grande maioria dos sistemas operacionais, aloca 100% da memória disponível na máquina virtual, durante o processo de inicialização. Desta forma, o índice de memória pode ficar fixo no máximo da escala. Em relação ao índice de utilização da CPU, este apresenta a taxa de utilização corrente, e é atualizado constantemente.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_026.png
   :alt: Performance Instantânea de VM
   :align: center

----

.. important:: Importante mencionar que as estatísticas estão disponíveis de forma aberta para todos os provedores de serviço de nuvem. A Plataforma uCloud coleta e armazena estas informações em suas bases de dados internas, para que esta informação possa ser utilizada por outros produtos do portfólio Ustore (por ex.: *uSavings*).

----

Seção Metrics (exclusivo **AWS**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta seção é apresentada, somente, para as máquinas virtuais que são criadas no ambiente da Amazon Web Services (AWS), pois somente este provedor informa estas estatísticas de forma aberta e gratuita.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_027.png
   :alt: Performance Instantânea de VM
   :align: center

----

* **Type**: Esta coluna contém o tipo da informação que está sendo exibida:
* **Network In**: Esta linha representa a quantidade de pacotes TCP-IP que trafegam em sentido entrada (in) para a máquina virtual – da rede externa  para a máquina virtual.
* **Network Out**: Esta linha representa a quantidade de pacotes TCP-IP que trafegam em sentido saída (out) da máquina virtual – da máquina virtual para rede externa.
* **Disk Read Ops**: Esta linha representa a quantidade de operações de acesso de leitura no disco rígido da máquina virtual.
* **Disk Write Ops**: Esta linha representa a quantidade de operações de acesso de escrita no disco rígido da máquina virtual.
* **Instantaneous**: Esta coluna apresenta o valor total instantâneo da métrica (type) da linha em que o valor é apresentado. O valor é instantâneo, ou seja, se refere ao momento em que se observa a máquina virtual.
* **Accumulated**: Esta coluna apresenta o valor total acumulado da métrica (type) da linha em que o valor é apresentado. Este valor se refere ao acumulado nas bases de dados da Plataforma uCloud, desde o momento em que a máquina virtual foi provisionada.

----

Seção Interfaces de Rede
~~~~~~~~~~~~~~~~~~~~~~~~

Esta seção apresenta as informações da interface de rede (interface Ethernet) vinculada a esta máquina virtual. Caso seja necessário, através desta seção é possível remover a interface de rede ou adicionar uma nova interface de rede Ethernet para esta máquina virtual.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_027.png
   :alt: Performance Instantânea de VM
   :align: center

----

* **Botão Adicionar** |botao_adiciona_verde|: Quando uma máquina virtual é provisionada, sua configuração já possui uma interface de rede Ethernet vinculada a esta máquina. Caso seja necessário que esta máquina possua outra interface de rede Ethernet, o usuário deve clicar no botão Adicionar e a Plataforma uCloud apresenta o campo tipo “dropdown” em que serão listadas todas as subnets configuradas para este Virtual Datacenter:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_028.png
   :alt: Performance Instantânea de VM
   :align: center

----

  * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma uCloud apresenta um ícone de confirmação. Após finalizar a alteração do conteúdo do campo, o usuário clica com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação, a informação do campo é alterada permanentemente nas bases de dados da Plataforma uCloud.
  * **Ícone de Cancelamento** |icone_cancela_vermelho|: No caso de usuário clicar sobre o ícone de edição por engano ou não desejar que a alteração seja armazenada (gravada) permanentemente, deve clicar com o cursor do mouse sobre o ícone vermelho, para cancelar a alteração realizada. O conteúdo do campo retorna para os valores iniciais antes de qualquer preenchimento/alteração.

.. note:: *Caso o usuário não consiga localizar a subnet desejada, ele deve abandonar este procedimento e consultar o item Redes. Efetuar o procedimento descrito como provisionar uma subnet dentro do ambiente do provedor de serviço de nuvem.*

* **Dispositivo**: Esta coluna apresenta o nome do dispositivo vinculado a esta máquina virtual. Por padrão, estes dispositivos são nomeados com o termo inicial “eth0” – este sendo a primeira interface de rede Ethernet.
* **Network**: Esta coluna apresenta a denominação da rede privada virtual encontrada no provedor de serviço de nuvem. Uma nuvem privada virtual (VPC) é um pool configurável sob demanda de recursos de computação compartilhados e alocados em um ambiente de nuvem pública, fornece um certo nível de isolamento entre as diferentes redes provisionadas.
* **Subnet**: Esta coluna apresenta o CIDR ou endereçamento IP, sem classes, da forma como é provisionado na Plataforma uCloud.
* **IP**: Esta coluna apresenta o Endereço TCP-IP vinculado para esta máquina, pelo usuário, no momento de sua inicialização. Este endereço é gerenciado pelo servidor DHCP do provedor de serviço de nuvem, seguindo a máscara CIDR definida pela sua subnet.
* **MAC**: Este campo apresenta o endereço físico da interface Ethernet.
* **Ações**: Esta coluna apresenta dois ícones que permitem a interação do usuário com a interface de rede Ethernet definida:

  * **Ícone de Edição Inativo** |icone_edita_on|: Importante ressaltar que em uma máquina virtual com apenas uma interface de rede Ethernet, este ícone estará sempre em modo ‘inativo’. Caso seja necessário alterar qualquer um dos parâmetros desta interface, o usuário deve excluir a interface e adicionar outra com as configurações desejadas.
  * **Ícone de Edição Ativo** |icone_edita_on|: No caso desta máquina virtual possuir mais de uma interface de rede, este ícone permanece ativo, apenas para os dispositivos nos quais a edição é possível.
  * **Ícone Lata de Lixo** |icone_lixo|: Ao clicar com o cursor do mouse sobre este botão esta interface de rede Ethernet é removida (excluída) da máquina virtual. A Plataforma uCloud apresenta uma tela que solicita a confirmação da operação ao usuário.

----

Seção Disco
~~~~~~~~~~~

Esta seção apresenta a lista de todos os recursos do disco de armazenamento vinculados a esta máquina virtual.

**Exemplo em Ambiente Azure**

.. image:: /figuras/ucloud_menu_maquinas_virtuais_030a.png
   :alt: Performance Instantânea de VM
   :align: center

----

**Exemplo em Ambiente Amazon AWS**

.. image:: /figuras/ucloud_menu_maquinas_virtuais_030b.png
   :alt: Performance Instantânea de VM
   :align: center

----

**Exemplo em Ambiente Google Cloud Platform**

.. image:: /figuras/ucloud_menu_maquinas_virtuais_030c.png
   :alt: Performance Instantânea de VM
   :align: center

----

Estas telas apresentam as informaçõs referentes ao disco de armazenamento provisionado para esta máquina virtual, abaixo esclarecemos estas informações:

* **Nome**: Esta coluna apresenta o nome do disco de armazenamento vinculado a máquina virtual. Importante ressaltar que cada provedor de serviço de nuvem utiliza metodologias distintas e próprias para assinalar um nome ao dispositivo em seus ambientes específicos. Alguns nomes podem ser muito extensos, e isto é específico de cada provedor.
* **Tamanho**: Esta coluna apresenta o tamanho do disco de armazenamento e pode estar expresso em Gigabytes ou Terabytes.
* **Tipo (Exclusivo AWS)**: Esta coluna somente é exibida para máquinas virtuais provisionadas no ambiente da AWS, apresenta(m) o(s) tipo(s) de disco(s). Consultar a documentação AWS para outros detalhes.
* **Encrypted (Exclusivo AWS)**: Esta coluna apenas é exibida para máquinas virtuais provisionadas no ambiente da AWS, que apresentam o parâmetro de encriptação do(s) disco(s). Consultar a documentação AWS para outros detalhes.
* **IOPS (Exclusivo AWS)**: Esta coluna somente é exibida para máquinas virtuais provisionadas no ambiente da AWS, apresenta o parâmetro da sigla para Input/Output Operations Per Second, ou Operações de Entrada e Saída por Segundo. É um índice de desempenho utilizado nas unidades de armazenamento de dados de encriptação do(s) disco(s). Consultar a documentação AWS para outros detalhes.
* **Dispositivo**: Esta coluna apresenta a identificação da unidade lógica (LUN) específica de cada provedor de serviço de nuvem. Consultar a documentação específica de cada provedor para obter informações em relação à identificação e denominação de cada dispositivo.
* **Storage**: Esta coluna apresenta a identificação do armazenamento que pode ser encontrado no menu Storage.
* **Ações**: Esta coluna apresenta a opção de tres ícones, assim o usuário pode interagir com a interface de rede Ethernet definida:

  * **Ícone de Edição Inativo** |icone_edita_on|: Importante ressaltar que uma máquina virtual com apenas um dispositivo de disco de armazenamento, este ícone estará sempre em modo ‘inativo’. Este ícone permite ao usuário alterar apenas o tamanho deste disco de armazenamento, todos os outros parâmetros listados não são passíveis de alteração, através desta tela. Caso seja necessário alterar qualquer um dos parâmetros deste disco de armazenamento, o usuário deve acessar o menu Storage, para efetuar a alteração dos parâmetros e configurações desejadas.
  * **Ícone de Desconectar** |icone_desconecta|: Este ícone permite ao usuário desconectar (unplug) o dispositivo de armazenamento (disco) da máquina virtual. Importante ressaltar que esta ação não removerá (delete) o disco de armazenamento do ambiente do provedor de serviço de nuvem. Esta ação desvincula a unidade de disco de armazenamento da máquina virtual, portanto, o disco de armazenamento deixa de ser listado nesta tela. Ao clicar com o cursor do mouse sobre este ícone, a Plataforma uCloud apresentará uma tela solicitando a confirmação da operação ao usuário:
  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para remover (excluir) esta unidade de disco de armazenamento da interface da máquina virtual. Para executar esta ação é mandatório que a máquina virtual esteja inativa (shutdown), caso contrário a Plataforma uCloud apresentará uma tela informado o erro. Estando a máquina virtual está inativa, e o usuário deseja excluir a unidade de disco de armazenamento, a Plataforma uCloud apresenta uma tela que informa que esta ação possui uma responsabilidade e há impacto futuro, além do que, solicita a confirmação da operação ao usuário.

* **Botão Adicionar** |botao_adiciona_verde|: Cada provedor de serviço de nuvem, provisiona um recurso de disco de armazenamento de tamanhos específicos para cada máquina virtual provisionada em seu ambiente. Caso seja necessário adicionar um novo recurso de disco de armazenamento, basta o usuário clicar sobre o botão Adicionar para a Plataforma uCloud apresentar as telas específicas para cada provedor de serviço de nuvem.

* **Criar Disco no ambiente AWS**

  * Ao configurar um novo disco de armazenamento, no ambiente AWS, a tela a seguir é apresentada:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_031a.png
   :alt: Performance Instantânea de VM
   :align: center

----

  * **Nome**: Este campo é obrigatório e deve ser nomeado com a informação que se deseja identificar o disco.
  * **Tamanho**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Disco de Armazenamento. Pode ser selecionado o limite em Megabytes, Gigabytes ou Terabytes.
  * **Tipo de Disco**: Este campo é obrigatório ao clicá-lo a Plataforma uCloud apresenta uma lista tipo “dropdown” que deve ser selecionada para configurar o tipo desejado de disco. Consultar a documentação da AWS para entender as características de cada tipo do recurso de disco existente na AWS. No momento da seleção são listados os seguintes tipos de disco:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_031b.png
   :alt: Performance Instantânea de VM
   :align: center

----

  * **Ícone Criptografar Disco** (|icone_habil_verde|/|icone_desb_verm|): Este ícone indica se este disco de armazenamento será configurado para ter seu conteúdo encriptado. Este ícone alterna entre conteúdo Desabilitado (vermelho) ou Habilitado (verde). Selecionar a opção desejada.
  * **Botão Criar**: Após preencher todos os campos obrigatórios, o usuário deve clicar com o cursor do mouse no botão verde Criar, a Plataforma uCloud provisiona o novo Disco de Armazenamento e vincula a máquina virtual. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório falta ser preenchido.

* **Para criar disco em ambiente Azure**

  * Ao configurar um novo disco de armazenamento, no ambiente AWS, a tela a seguir é apresentada:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_032a.png
   :alt: Performance Instantânea de VM
   :align: center

----

  * **Nome**: Este campo é obrigatório e deve ser nomeado com a informação que se deseja identificar o disco.
  * **Selecionar Storage**: Este campo é obrigatório ao clicá-lo a Plataforma uCloud apresenta a lista tipo “dropdown” que deve ser selecionada para configurar o tipo desejado de Storage. Consultar a documentação da Azure para entender as características de cada tipo de recurso de Storage existente na Azure. No momento da seleção são listados os seguintes tipos de storage:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_032b.png
   :alt: Performance Instantânea de VM
   :align: center

----

  * **Tamanho**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Disco de Armazenamento. Pode ser selecionado o limite em Megabytes, Gigabytes ou Terabytes.
  * **Botão Criar**: Após preencher todos os campos obrigatórios, o usuário deve clicar com o cu¬rsor do mouse no botão verde Criar, a Plataforma uCloud provisiona o novo Disco de Armazenamento e vincula a máquina virtual. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório falta ser preenchido.

----

Seção Snapshots
~~~~~~~~~~~~~~~

Esta seção apresenta todas as imagens de snapshots que foram criados referente ao(s) disco(s) que está(ão) vinculado(s) a esta máquina virtual.

Um snapshot é uma cópia de segurança incremental de todo o disco de armazenamento (disk backup) vinculado à máquina virtual. O termo ‘incremental’ significa que: somente os blocos no dispositivo que tiverem mudado depois do snapshot mais recente serão salvos. Isso minimiza o tempo necessário para criá-lo e economiza custos de armazenamento, por evitar duplicar os dados. Cada snapshot contém todas as informações necessárias para restaurar seus dados (desde o momento em que o snapshot foi tirado). Importante ressaltar que o conteúdo de snapshot é completo e totalmente diferente de uma cópia de segurança de arquivo (file backup).

Para obter outras informações, basta consultar a documentação com os detalhes e as características de snapshots de cada provedor de serviço de nuvem, para entender o que cada provedor de serviço de nuvem oferece.
Ao excluir um snapshot, somente os dados exclusivos desse snapshot serão removidos.



* **Botão Adicionar** |botao_adiciona_verde|: Caso seja necessário adicionar um novo recurso de snapshot de um disco de armazenamento, basta o usuário clicar sobre o botão Adicionar, a Plataforma uCloud pode apresentar campos para que o usuário possa informar o nome e assinalar qual o disco selecionado é indicado para provisionar o snapshot:
* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 1 caractere) com o qual deseja identificar este snapshot. A sugestão é de utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido). Importante mencionar que este nome pode ser acrescentado com informações específicas do provedor de serviço de nuvem, e a Plataforma uCloud não tem controle (remoção ou alteração) destas adições do(s) provedor(es).
* **Select a Disk**: Este campo é obrigatório, ao ser selecionado a Plataforma uCloud apresenta uma lista tipo “dropdown” que exibe todos os discos de armazenamento vinculados a esta máquina virtual, neste momento, deve ser selecionado o disco de armazenamento desejado:
* **Ícone de Confirmação** |icone_conf_verde|: Após preenchido o campo ‘nome para o snapshot” deve ser selecionado o disco de armazenamento que se deseja criar a imagem da cópia de segurança (backup), em seguida a Plataforma uCloud apresenta um ícone de confirmação. O usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação é enviada uma solicitação de provisionamento de uma imagem de disco (snapshot) para o provedor de serviço de nuvem, e a nova imagem deve aparecer listada nesta seção após algum tempo. Importante ressaltar que o tempo total para provisionar este snapshot é dependente do tamanho do disco e seu tipo (SSD ou HDD) e do ambiente computacional do provedor de serviço de nuvem. O usuário pode acompanhar a evolução desta solicitação através do menu Tarefas.
* **Ícone de Cancelamento** |icone_cancela_vermelho|: Caso o usuário tenha clicado sobre o ícone de edição por engano, ou não deseja provisionar um snapshot para o disco selecionado, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho, para cancelar a ação e retornar ao conteúdo da seção.
* **Nome**: Nesta coluna é apresentado o nome do snapshot informado no momento do seu provisionamento. Importante mencionar que este nome pode ser acrescentado com informações específicas do provedor de serviço de nuvem, a Plataforma uCloud não tem controle (na remoção ou alteração) destas adições do(s) provedor(es).
* **Data**: Nesta coluna é apresentada a data e o horário em que o snapshot foi criado. Esta data é estabelecida pelo provedor de serviço de nuvem, a Plataforma uCloud apenas apresenta esta informação. Este campo está representado no formato padrão brasileiro (DD/MM/AAAA) e o horário no formato 24 horas (HH:MM:ss).
* **Ações**: Esta coluna apresenta dois ícones para que o usuário possa interagir com cada ocorrência de um snapshot.

  * **Ícone de Reverter Snapshot** |icone_revert_snap|: Basta o usuário clicar sobre este ícone e aplicar a reversão do disco da máquina virtual, com base na imagem do dia e a hora do snapshot selecionado. A Plataforma uCloud apresenta uma tela de confirmação ao usuário:
  * **Ambiente Amazon AWS**: Para ambiente Amazon AWS esta ação é iniciada imediatamente - o disco de armazenamento da máquina virtual tem sua imagem revertida para o snapshot selecionado, após o tempo necessário desta atividade ser executada no ambiente Amazon AWS. Importante mencionar que a Plataforma uCloud não tem controle sobre o tempo necessário para esta execução. O usuário pode acompanhar a evolução desta solicitação através do menu Tarefas.
  * **Ambiente Azure**: Para ambiente Azure esta ação necessita de atividade que deve ser executada pelo próprio usuário. O ambiente Azure não permite reverter uma imagem de snapshot de forma automática. A Plataforma uCloud apresenta uma tela que solicita ao Azure gerar um link o qual contém o arquivo da imagem de disco de armazenamento:

Após o ambiente Azure finalizar o processo de criar o arquivo de imagem, a Plataforma uCloud apresenta outra tela que permite o download do arquivo da imagem do disco (snapshot).

Este processo de download está vinculado à sessão do navegador de Internet (browser) e é armazenado no folder padrão, configurado nas preferências do navegador de Internet. Importante ressaltar que, se a sessão do navegador de Internet for encerrada, este processo de download do arquivo é interrompido. O usuário pode acompanhar o tempo para encerrar o processo do arquivo específico através das ferramentas de download do seu navegador de Internet de preferência (segue abaixo, um exemplo do navegador de Internet Ópera).

Após finalizar a transferência do arquivo da imagem de disco de armazenamento (snapshot), o usuário deve seguir as etapas descritas, conforme documentado no site do ambiente Azure - em seguida, aplicar a imagem à máquina virtual desejada.

* **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para remover (excluir) a imagem de disco de armazenamento do ambiente do provedor de serviço de nuvem. Importante mencionar que a imagem de disco (snapshot) ocupa espaço de armazenamento dentro do ambiente do provedor de serviço de nuvem. A Plataforma uCloud apresenta a tela abaixo, com a mensagem de confirmação da operação ao usuário:

.. warning:: |atencao| A ação de remoção da imagem de disco de armazenamento (snapshot) é definitiva e irreversível, pois não existem outras cópias desta imagem específica. Recomendamos ao usuário atenção redobrada ao confirmar esta ação.

----

Seção Signatures (**Exclusivo Azure e Google Cloud Platform**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta seção são listadas todas as assinaturas vinculadas à máquina virtual que se está observando. Assinaturas são serviços vinculados a uma máquina virtual, unicamente disponíveis para os provedores Azure e Google Cloud Platform. As assinaturas podem conter apenas as ofertas de serviços que devem ser cobrados mensalmente ou no mês específico. No caso da remoção de uma assinatura vinculada a uma máquina virtual, o valor será cobrado integralmente pelo agente de bilhetagem.

O usuário pode consultar o menu Configurações / Assinaturas.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_034.png
   :alt: Performance Instantânea de VM
   :align: center

----

* **Botão Adicionar** |botao_adiciona_verde|: Caso seja necessário vincular uma nova assinatura a esta máquina virtual, basta o usuário clicar sobre o botão Adicionar e a Plataforma uCloud apresenta a tela com o exemplo abaixo;

.. image:: /figuras/ucloud_menu_maquinas_virtuais_034b.png
   :alt: Performance Instantânea de VM
   :align: center

----

  * **Selecionar uma Assinatura**: Este campo é obrigatório ao ser selecionado, a Plataforma uCloud apresenta uma lista tipo “dropdown” que exibe todos as assinaturas provisionadas na Plataforma uCloud. O usuário deve selecionar a assinatura desejada:
  * **Botão Adicionar** |botao_adiciona|: Após selecionar a assinatura desejada para vincular a esta máquina virtual, basta o usuário clicar sobre o botão Adicionar. Importante mencionar que o valor desta assinatura é adicionado aos custos mensais desta máquina virtual.
  * **Botão Cancelar** |botao_cencela_verm|: Caso o usuário tenha clicado sobre o botão de adicionar, por engano, ou não deseja acrescentar a assinatura, basta clicar com o cursor do mouse sobre o ícone vermelho, neste momento a ação é cancelada e a tela retorna ao conteúdo da seção.
  * **Nome**: Esta coluna apresenta o nome da assinatura informado no momento do seu provisionamento na Plataforma uCloud.
  * **Quantidade**: Esta coluna apresenta a quantidade de vezes que a assinatura incide sobre a máquina virtual até a data atual requerida.
  * **Preço**: Esta coluna apresenta o valor financeiro da assinatura vinculada na máquina virtual
  * **Data**: Esta coluna exibe a data na qual a assinatura é vinculada à máquina virtual.
  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para remover (excluir) a assinatura da máquina virtual observada. Importante ressaltar, que no caso da remoção de uma assinatura vinculada a uma máquina virtual, o valor é cobrado integralmente pelo agente de bilhetagem.

Seção Histórico de Performance (**Exclusivo Azure e GCP**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta seção permite ao usuário gerar um gráfico de performance da máquina virtual, gráfico que apresenta as informações dos recursos de memória RAM e o uso de ciclos de CPU, durante um período específico que pode ser definido pelo usuário.

.. image:: /figuras/ucloud_menu_maquinas_virtuais_035a.png
   :alt: Performance Instantânea de VM
   :align: center

----

* **Data Inicial**: O período específico pode ser definido pelo usuário, basta informar a data inicial que se deseja avaliar a performance da máquina virtual, o usuário deve clicar sobre o ícone do calendário |icone_agenda| e selecionar a data inicial do período;

.. image:: /figuras/ucloud_menu_maquinas_virtuais_035b.png
   :alt: Performance Instantânea de VM
   :align: center

----

* **Data Final**: Em seguida, o usuário deve informar a data final do período que deseja avaliar a performance da máquina virtual, assim ao clicar sobre o ícone do calendário |icone_agenda| o usuário deve selecionar a data final do período que se quer avaliar;

.. image:: /figuras/ucloud_menu_maquinas_virtuais_035c.png
   :alt: Performance Instantânea de VM
   :align: center

----

* **Botão Pesquisar** |botao_pesquisar|: Para que a Plataforma uCloud possa apresentar as informações referentes ao histórico de performance desta máquina virtual, o usuário deve clicar com o cursor do mouse sobre o botão “pesquisar” e aguardar os valores serem calculados para a montagem e apresentação do gráfico.

----

Criando uma Máquina Virtual
---------------------------

A Plataforma uCloud, está perfeitamente integrada via API Rest as consoles dos provedores de serviço denuvem pública e/ou privada, e possibilita ao usuário enviar comandos para as respectivas consoles de cada provedor de nuvem e provisionar uma máquina virtual em seus ambientes nativos. *Muito importante ressaltar que não existem máquinas virtuais criadas dentro da Plataforma uCloud, estes recursos computacionais (máquinas virtuais) são provisionados através da Plataforma uCloud e, portanto, existem somente no ambiente destino selecionado*.

Antes de iniciar este processo de criação de máquinas virtuais, verificar se a Plataforma uCloud possui os pré-requisitos para completar o processo de ponta-a-ponta, de forma correta. Devem existir os seguintes pré-requisitos para qualquer ambiente de provedor de serviço de nuvem:

A. Provisionar/Existir um Virtual Datacenter (ver item Virtual Datacenter / Criar Virtual Datacenter);
B. Provisionar/Existir uma sub-rede (ver item Rede / Rede / Criar Rede);
C. Provisionar/Existir um Grupo de Segurança (ver item Rede / Grupo de Segurança / Criar Grupo de Segurança).

.. important:: |atencao| *Importante ressaltar que os tópicos acima são fundamentais, caso não sejam previamente provisionados, o usuário será obrigado a interromper o processo de criação da máquina virtual e efetuar o provisionamento criação dos tópicos acima.*

Para uniformizar e simplificar o processo de provisionamento de uma máquina virtual, a Plataforma uCloud foi desenhada para auxiliar e guiar o usuário (iniciante ou expert) nas principais etapas de parâmetros e configurações. Este processo de criação de uma máquina virtual é apoiado por uma “Wizard in” que serve para simplificar e direcionar o usuário, solicitando os parâmetros necessários para provisionar uma máquina virtual em qualquer provedor de serviço de recursos computacionais de nuvem (público e/ou privado).

* **Botão Criar Máquina Virtual** |botao_criar_VM|: Este botão permite ao usuário provisionar (criar) uma máquina virtual no ambiente do provedor de serviço de nuvem desejado (público e/ou privado). Quando o usuário clicar com o cursor do mouse sobre este botão a Plataforma uCloud apresenta a tela inicial do *Wizard*.

.. image:: /figuras/ucloud_criar_maquina_virtual_001.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

Iremos detalhar cada etapa do assistente *Wizard* de forma separada a seguir.

----

Wizard Etapa 1 (Seleção da Nuvem)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa, o usuário deve clicar com o cursor do mouse sobre o ícone do provedor de serviço de nuvem, conforme apresentado nesta tela.

.. image:: /figuras/ucloud_criar_maquina_virtual_002.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

O exemplo da tela acima, reforça a posição de que a Plataforma uCloud é um verdadeiro ambiente multi-cloud, pois são apresentados três provedores diferentes. Neste exemplo, a empresa usuária da Plataforma uCloud possui relação comercial com cada provedor individualmente. Foram provisionados acessos com cada ambiente e neste ponto o usuário pode selecionar o ambiente destino no qual deseja provisionar uma máquina virtual.
Importante ressaltar que apenas são apresentados os ícones dos provedores que a empresa usuária fornece acesso para seu(s) provedor(es) do serviço de nuvem, desta forma, se a empresa usuária fornecer apenas um único provedor, pode existir apenas um único ícone nesta etapa do wizard, conforme o exemplo abaixo:

.. image:: /figuras/ucloud_criar_maquina_virtual_003.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Botão Cancelar** |botao_cencela_verm|: O usuário pode usar este botão para cancelar o processo de criação de uma máquina virtual, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Máquina Virtual. A Plataforma uCloud fecha a tela do wizard e retorna à tela anterior.
* **Botão Voltar** |botao_voltar|: Este botão se encontra inativo, por se tratar da primeira etapa do processo, portanto não existe etapa anterior para retornar.
* **Botão Próximo** |botao_proximo|: O usuário deve clicar com o cursor do mouse sobre o ícone de um dos provedores, em seguida, clicar com o cursor do mouse sobre o botão Próximo, a Plataforma uCloud apresenta a tela do *Wizard Etapa 2* (ver abaixo).
  * *Caso o usuário não tenha selecionado um ícone de provedor, a Plataforma uCloud apresentará a seguinte tela, a qual abre um aviso*:

.. image:: /figuras/ucloud_criar_maquina_virtual_004.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Botão Voltar** |botao_voltar|: Ao clicar com o cursor do mouse sobre este botão, o usuário retorna à etapa anterior, o que permite selecionar o ambiente do provedor de serviço de nuvem desejado.
* **Botão Criar** |botao_criar_off|: Este botão permanece inativo, até que todos os parâmetros necessários sejam preenchidos ou atendidos, para o correto provisionamento da máquina virtual no provedor selecionado.

Wizard Etapa 2 (informações básicas da máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa são solicitados alguns parâmetros básicos para o correto provisionamento da máquina virtual no provedor de serviço de nuvem:

.. image:: /figuras/ucloud_criar_maquina_virtual_005.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Tipo de Faturamento**: Este campo é obrigatório, quando o usuário clica com o cursor do mouse sobre este campo a Plataforma uCloud apresenta uma lista com as opções disponíveis:

  * **Reservado por CPU**: Quando o usuário escolhe este tipo de faturamento, indica selecionar uma máquina virtual de instância reservada paga no primeiro mês, no período de um ano (12 meses) no provedor. A forma de cálculo do uso da máquina é a ocupação do CPU desta.
  * **Reservado por Memória**: No momento que o usuário elege este tipo de faturamento, determina selecionar uma máquina virtual de instância reservada paga no primeiro mês, no período de um ano (12 meses) no provedor. O cálculo do uso da máquina é a ocupação da memória desta.
  * **Sob Demanda por CPU**: Quando o usuário escolhe este tipo de faturamento, indica selecionar uma máquina virtual que será cobrada por uso mês-a-mês no provedor. A forma de cálculo do uso da máquina será a ocupação do CPU desta.
  * **Sob Demanda por Memória**: No momento que o usuário elege este tipo de faturamento, determina selecionar uma máquina virtual que será cobrada por uso mês-a-mês no provedor. A forma de cálculo do uso da máquina é a ocupação da memória desta.

* **Nome**: Este campo é obrigatório o usuário deve nomear (no mínimo 3 caracteres) com o termo que deseja identificar este snapshot. A sugestão é utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido). Importante mencionar que este nome poderá ser acrescido com informações específicas do provedor de serviço de nuvem. A Plataforma uCloud não tem controle (remoção ou alteração) destas adições do(s) provedor(es).

* **Virtual Datacenter**: Este campo é obrigatório do tipo “dropdown” quando o usuário clica com o cursor do mouse a Plataforma uCloud lista todos os Virtual Datacenters que foram provisionados e vinculados ao provedor de serviço de nuvem selecionado na Etapa 1. Importante mencionar que este campo determina o conteúdo de outros campos tanto nesta etapa quanto em outras etapas deste wizard.

.. note:: *Caso não exista nenhum Virtual Datacenter que tenha sido provisionado antecipadamente, é necessário interromper este processo de máquina virtual para provisionar um Virtual Datacenter, é recomendado seguir o processo descrito no item Criação de Virtual DataCenter.*

* **Regiões**: Este campo é obrigatório do tipo “dropdown” , quando o usuário clica com o cursor do mouse a Plataforma uCloud lista todas as regiões globais de presença do provedor de serviço de nuvem - que foram configuradas no Virtual Datacenter, selecionado no campo anterior.

* **Botão Criar** |botao_criar_off|: Este botão permanece inativo, até preencher todos os parâmetros necessários para o correto provisionamento da máquina virtual, no provedor selecionado.

* **Botão Próximo** |botao_proximo|: O usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud apresentar a tela do Wizard Etapa 3 (ver abaixo).

Wizard Etapa 3 (informações básicas da máquina virtual – cont.)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta seção é a continuação da etapa anterior em que são solicitados alguns parâmetros básicos para o correto provisionamento da máquina virtual, no provedor do serviço de nuvem:

.. image:: /figuras/ucloud_criar_maquina_virtual_006.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Conjunto de Disponibilidade (somente Azure)**: Este campo é obrigatório e exclusivo aos provisionamentos na nuvem Azure. Este campo é do tipo “dropdown” por isto, quando o usuário clica com o cursor do mouse, a Plataforma uCloud lista todos os Conjuntos de Disponibilidade, configurados previamente e/ou informados pelo usuário. Um conjunto de disponibilidade garante que as VMs sejam distribuídas entre vários domínios de falha nos datacenters do Azure, além de serem implantadas em hosts com janelas de manutenção diferentes. O usuário possui duas opções controladas por ícones tipo “radio button” que está descrito a seguir:

.. image:: /figuras/ucloud_criar_maquina_virtual_007.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

  * **Selecione**: Este ícone é obrigatório, ao ser selecionado, transforma o campo abaixo em um campo do tipo “dropdown”. Permite ao usuário clicar com o cursor do mouse e recuperar, na Plataforma uCloud, uma lista de todos os Conjuntos de Disponibilidade configurados no provedor de serviço de nuvem. O usuário pode selecionar o Conjunto de Disponibilidade desejado.

  * **Criar**: Este ícone é obrigatório quando selecionado transforma o campo abaixo em um campo do tipo “texto livre”. Esta opção é válida quando o usuário deseja criar um Grupo de Disponibilidade novo no ambiente Azure. O usuário deve informar o novo nome, clicar com o cursor do mouse no campo abaixo ou pressionar a tecla TAB, assim pode seguir ao próximo campo.

* **Templates**: Este campo é obrigatório do tipo “dropdown” ao ser clicado pelo usuário, a Plataforma uCloud lista todos os Templates do provedor de serviço de nuvem, previamente escolhidos no Virtual Datacenter, operação detalhada no Wizard Etapa 2.

* **Flavors**: Este campo é obrigatório do tipo “dropdown” quando o usuário clica com o cursor do mouse, a Plataforma uCloud recupera e lista de todos os flavors do provedor de serviço de nuvem, previamente configuradas no Virtual Datacenter selecionado no Wizard Etapa 2.

.. note:: *A Plataforma uCloud pode apresentar uma mensagem de erro, caso o flavor selecionado não seja compatível com o Tipo de Faturamento, selecionado na etapa anterior.*

.. image:: /figuras/ucloud_criar_maquina_virtual_008.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

  * O usuário pode escolher outro flavor que não apresente esta mensagem de erro ou retornar a Wizard Etapa 2 e efetuar a mudança na seleção de Tipo de Faturamento.

.. important:: Importante ressaltar que o Botão Criar não se torna ativo, no caso de ocorrer qualquer mensagem de erro que tenha sido apresentada em qualquer etapa deste wizard.

* **Sub-redes**: Este campo é obrigatório do tipo “dropdown”  quando o usuário clica com o cursor do mouse a Plataforma uCloud recupera e lista todas as sub-redes (subnets) que foram configuradas anteriormente para este provedor de serviço de nuvem.

  * Caso nenhuma Sub-rede tenha sido provisionada antecipadamente, será necessário interromper este processo de máquina virtual e provisionar uma sub-rede, o usuário deve seguir o processo descrito no item Redes / Redes / Criar Redes.

* Defina o número de máquinas virtuais que serão criadas: Este campo é obrigatório nele o usuário deve informar um número inteiro, tal número representa a quantidade de máquinas virtuais a serem provisionadas no ambiente do provedor de serviço de nuvem (no mínimo 1 máquina virtual). Este campo não pode ser deixado em branco.

* **Botão Criar** |botao_criar_off|: Este botão permanece inativo, até preencher todos os parâmetros necessários para o correto provisionamento da máquina virtual, no provedor selecionado.

* **Botão Próximo** |botao_proximo|: O usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud apresentar a tela do Wizard Etapa 4 (ver abaixo).

Wizard Etapa 4a (informações de segurança da máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa o usuário deve informar os parâmetros de segurança para o correto provisionamento da máquina virtual no provedor de serviço de nuvem:

.. image:: /figuras/ucloud_criar_maquina_virtual_009.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Par de Chaves**: Este campo é obrigatório do tipo “dropdown” quando o usuário clicar com o cursor do mouse, a Plataforma uCloud lista as duas opções disponíveis:

  * **Opção 1**: Escolher Chave Existente: Quando escolhida esta opção, significa que o usuário pode selecionar algum par de chave, previamente configurado na Plataforma uCloud. Ver o item Rede / Par de Chave, para acompanhar o processo “Provisionar um novo par de chave”.
    * Selecionar Par de Chaves: Este campo é obrigatório e do tipo “dropdown” quando o usuário clicar com o cursor do mouse, a Plataforma uCloud lista apenas as chaves que este usuário possui (ou chaves que foram criadas por um usuário com o perfil de acesso superior – no exemplo acima o usuário é ‘root’) e que estão vinculadas ao ambiente do provedor de serviço de nuvem. Para vincular esta chave à máquina virtual que será provisionada, basta o usuário clicar com o mouse em alguma das chaves existentes,

.. image:: /figuras/ucloud_criar_maquina_virtual_010.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

  * **Opção 2**: Criar Novo Par de Chaves: Este campo é obrigatório quando selecionado significa que o usuário deseja criar um arquivo de Par de Chave - online - durante o processo de provisionamento da máquina virtual.

.. image:: /figuras/ucloud_criar_maquina_virtual_011.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

  * **Nome da Chave**: *Este campo é obrigatório* nele o usuário deve informar o nome do Par de Chave que deseja criar. A sugestão é utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
  * **Botão Download** |botao_download|: Este botão é habilitado somente após o usuário informar o nome da chave no campo anterior. O usuário deve clicar com o botão do mouse sobre este botão para que a Plataforma uCloud possa iniciar o download do arquivo texto, com a chave de autenticação SSH para esta máquina virtual. O download do arquivo de texto (.pem) é executado pelo navegador de Internet utilizado pelo usuário, no momento da operação.

.. image:: /figuras/ucloud_criar_maquina_virtual_011b.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

  Este processo de download está vinculado à sessão do navegador de Internet (browser) armazenado no folder padrão configurado nas preferências do navegador de Internet. Importante ressaltar que no caso da sessão do navegador de Internet ser encerrada, este processo de download do arquivo é interrompido. O usuário pode acompanhar o tempo para encerrar o processo do arquivo específico através das ferramentas de download do seu navegador de Internet de preferência (abaixo está um exemplo do navegador de Internet Opera).
  Após finalizar a transferência do arquivo texto com a chave privada de autenticação (.pem) o usuário está apto a efetuar a conexão no console da máquina virtual utilizando qualquer ferramenta de sessão SSH da sua preferência.

.. important:: |atencao| *Importante ressaltar que a etapa de efetuar o download do arquivo texto com a chave de autenticação SSH é de suma importância, este arquivo permite a primeira conexão SSH na máquina virtual. Sem este arquivo é impossível se conectar (pela primeira vez) ao prompt do sistema operacional da máquina virtual.*

* **Grupo de Segurança**: Este campo é obrigatório do tipo *dropdown*  quando o usuário clicar com o cursor do mouse na Plataforma uCloud é recuperada uma lista de todos os grupos de segurança provisionados na Plataforma uCloud. Basta o usuário selecionar o Grupo de Segurança desejado para vincular a máquina virtual.
* **Botão Criar** |botao_criar_off|: Este botão permanece inativo, até preencher todos os parâmetros necessários para o correto provisionamento da máquina virtual, no provedor selecionado.
* **Botão Próximo** |botao_proximo|: O usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud apresentar a tela do Wizard Etapa 4b (ver abaixo).

Wizard Etapa 4b (informações de segurança – Exclusivo Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa o usuário deve informar os parâmetros de segurança para o correto provisionamento das máquinas virtuais no provedor de serviço de nuvem Azure, a etapa quatro possui campos - alguns deles exclusivos. Neste momento, a Plataforma uCloud adapta o wizard de forma a solicitar parâmetros necessários para o ambiente da nuvem.
Para o ambiente Azure, o método de autenticação é unicamente através de uma senha, nesta etapa existe um campo do tipo “texto livre” que possibilita informar a sequência de caracteres da senha.

A seguir é apresentada a tela referente Wizard Etapa 4b, para máquinas virtuais do Azure:

.. image:: /figuras/ucloud_criar_maquina_virtual_012.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Senha**: Este campo é obrigatório, o usuário deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”, conforme a documentação encontrada no site da Azure. A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres, deve conter caracteres de três das seguintes categorias:
  * *Letras maiúsculas e minúsculas (A a Z)*
  * *Números inteiros de base 10 (de 0 a 9)*
  * **Caracteres não alfanuméricos** (caracteres especiais): (~ ! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' <>,.? /).

* **Grupo de Segurança**: Este campo é obrigatório do tipo *dropdown* quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta uma lista de todos os Grupos de Segurança provisionados na Plataforma uCloud. Basta o usuário selecionar o grupo de segurança desejado para vincular à máquina virtual.

.. important:: |atencao| Mesmo que os símbolos de moedas como o euro (€) ou a libra britânica (£) não fazem parte dos caracteres especiais recomendamos FORTEMENTE QUE NUNCA SEJAM UTILIZADOS em senhas de máquinas virtuais.*

* **Botão Criar** |botao_criar_off|: Este botão permanece inativo, até preencher todos os parâmetros necessários para o correto provisionamento da máquina virtual, no provedor selecionado.
* **Botão Próximo** |botao_proximo|: O usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud apresentar a tela do Wizard Etapa 4b (ver abaixo).

Wizard Etapa 5a (User data)
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta etapa permite ao usuário inserir um código script de inicialização para um certo nível de personalização do ambiente operacional da máquina virtual.

.. image:: /figuras/ucloud_criar_maquina_virtual_013.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **User Data**: Este campo não é obrigatório, ele pode ser deixado em branco (sem conteúdo). Caso seja necessário, o usuário pode inserir neste campo o conteúdo de um script de inicialização que pode ser na linguagem Powershell ou YAML para configuração de parâmetros do ambiente do sistema operacional da máquina virtual. Basta o usuário inserir o conteúdo do script neste campo, através do recurso copiar/colar (copy/paste).

* **Botão Criar** |botao_criar_off|: Este botão permanece inativo, até preencher todos os parâmetros necessários para o correto provisionamento da máquina virtual, no provedor selecionado.
* **Botão Próximo** |botao_proximo|: O usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud apresentar a tela do Wizard Etapa 4b (ver abaixo).

.. note:: Importante ressaltar, que esta etapa pode ser executada neste momento, sem que seja obrigatório passar pela última etapa (etapa seis) do wizard.

----

Wizard Etapa 5b (**User data VMware**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para as máquinas virtuais provisionadas no ambiente on-premises VMware, a etapa cinco possui campos, alguns deles exclusivos, desta forma a Plataforma uCloud adapta o wizard e solicita os parâmetros necessários para o ambiente on-premises VMware.
Abaixo é apresentada a tela referente a Etapa 5a, para máquinas virtuais na VMware:

.. image:: /figuras/ucloud_criar_maquina_virtual_014.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Assinaturas**: Este campo é opcional, do tipo “dropdown” . Quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta todas as Assinaturas anteriormente provisionadas no ambiente. Basta o usuário selecionar a(s) assinatura(s) desejada(s) para adicionar ao custo mensal da máquina virtual. Para provisionar novas assinaturas ou editar as existentes basta ler o item Configurações / Assinaturas.
* **Botão Attach**: Depois de selecionar a assinatura desejada, basta o usuário clicar com o cursor do mouse sobre o botão Attach para vincular (adicionar) o valor mensal da assinatura ao custo da máquina virtual que está provisionando.
* **Botão Excluir**: Este botão é necessário quando o usuário vincular uma assinatura a máquina virtual por engano e desejar remover esta assinatura antes de submeter o comando de criar esta máquina virtual. Basta selecionar a assinatura desejada e clicar com o cursor do mouse sobre o botão Excluir. O valor mensal da assinatura é removido do custo da máquina virtual provisionada.
* **Endereço DHCP**: Este ícone permite ao usuário alternar entre duas opções, a opção padrão: Endereço DHCP (dinâmico) - a máquina virtual provisionada no ambiente VMware, recebe seu Endereço TCP-IP de forma dinâmica com base no Servidor DHCP on-premises.
* **Endereço Estático**: Quando o usuário alterna para a 2ª opção: Endereço Estático - a interface da Plataforma uCloud apresenta campos específicos que devem ser preenchidos para o correto provisionamento da máquina virtual.

.. image:: /figuras/ucloud_criar_maquina_virtual_014b.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **IP**: Este campo é obrigatório do tipo “dropdown”. Quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista de todos os endereços TCP-IP disponíveis na rede on-premises. Basta o usuário clicar com o cursor do mouse sobre o endereço desejado para vincular este à máquina virtual que se está provisionando.
* **Netmask**: Este campo é obrigatório, o usuário deve informar a máscara de rede TCP-IP desejada e adequada para receber o Endereço TCP-IP informado no campo anterior.
* **Gateway**: Este campo é obrigatório, o usuário deve informar o Endereço TCP-IP do Gateway da sub-rede (subnet) selecionada nos campos acima.
* **DNS**: Este campo é obrigatório, o usuário deve informar o Endereço TCP-IP do Servidor DNS (Domain Name Server) específico botão criarque resolve o nome da máquina virtual.

* **Botão Próximo** |botao_proximo|: O usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud apresentar a tela do Wizard Etapa 4b (ver abaixo).

* **Botão Criar** |botao_criar_on|: Nesta etapa todos os parâmetros fundamentais para a criação da máquina virtual devem ter sido informados corretamente, o usuário percebe que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão criar para que a Plataforma uCloud envie todos os parâmetros da máquina virtual para o provedor de serviço de nuvem (via API-Rest) selecionado, para o completo provisionamento da máquina virtual.

.. note:: |nota| Importante ressaltar, que o usuário está livre para pressionar o Botão Criar Verde sem que seja obrigatório passar pela última etapa (etapa seis) do wizard. Caso este botão não esteja habilitado |botao_criar_off| significa afirmar que algum parâmetro anterior não foi informado ou foi deixado em branco, por este motivo a Plataforma uCloud impede o provisionamento da máquina virtual.

----

Wizard Etapa 6 (visualizar as configurações da máquina virtual)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta é a etapa final, momento que a Plataforma uCloud apresenta o resumo de todas as informações referentes aos parâmetros e configurações para o provisionamento da máquina virtual no provedor de serviço de nuvem:

.. image:: /figuras/ucloud_criar_maquina_virtual_015.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Sumário**:
  * Máquina Virtual: <nome>
  * Template: <sistema operacional>
  * Virtual Data Center: <nome do Virtual Datacenter>
  * Host:
  * Provedor Cloud: <Identificação do Provedor de serviço de nuvem>
  * Redes: Subnet <CIDR da sub-rede TCP-IP>
  * Flavor: <Identificação do Flavor – configuração do hardware>
  * Vcpus: <Quantidade de CPUs>
  * Memória: <Total de Memória RAM>

* **Ícone Agendar** |icone_habil_verde|/|icone_desb_verm|: Este ícone permite ao usuário agendar o provisionamento da máquina virtual, o valor padrão de apresentação é Desabilitado (cor vermelho).

* **Ícone Calendário** |icone_agenda|: Basta o usuário clicar sobre o ícone do calendário para a Plataforma uCloud apresentar o pop-up na tela e permitir ao usuário selecionar a data desejada, conforme abaixo:

.. image:: /figuras/ucloud_criar_maquina_virtual_015b.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

  * **Ícone setas (🡩/🡫)**: Inicialmente a Plataforma uCloud apresenta o calendário com o dia e horário corrente, em destaque azul. Basta o usuário clicar com o cursor do mouse sobre o dia desejado e/ou nos ícones de setas para selecionar outro mês. Quando selecionado, este será o dia programado para que a Plataforma uCloud possa enviar a tarefa para o provedor de serviço de nuvem para o provisionamento da máquina virtual.
  * **Hora / Minuto**: Este campo é apresentado no padrão 24 horas, basta o usuário selecionar a hora e minuto desejado. Quando selecionado, este será o horário programado para que a Plataforma uCloud possa enviar a tarefa ao provedor de serviço de nuvem para o provisionamento da máquina virtual.

* **Suas cotas**: Os gráficos apresentados representam os limites (cotas) referentes aos recursos computacionais de Disco, CPU e memória. Isto permite ao usuário identificar se o provisionamento desta nova máquina virtual está dentro dos limites definidos para seu usuário ou grupo. Importante ressaltar que no caso do usuário ter consumido toda sua cota, a Plataforma uCloud não procede com o provisionamento desta máquina virtual.

.. image:: /figuras/ucloud_criar_maquina_virtual_015c.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Estimativa de preço**: Esta informação é obtida diretamente dos valores públicos (abertos) de máquinas virtuais do provedor de serviço de nuvem pública selecionado na Wizard Etapa 1. Esta informação é relevante, para o caso do usuário ter consumido todos os seus limites (cotas), esta informação confirma a possibilidade de que esta máquina virtual não seja criada. Caso o ambiente seja multi-nuvem e o usuário tenha a permissão de provisionar máquinas virtuais em mais de um provedor de serviço de nuvem a Plataforma uCloud apresenta um comparativo de preços dos diversos provedores aos quais o usuário está vinculado:

.. image:: /figuras/ucloud_criar_maquina_virtual_015d.png
   :alt: Wizard para criar Maquina Virtual
   :align: center

----

* **Botão Voltar** |botao_voltar|: Este botão pode ser útil por permitir ao usuário retornar a etapa anterior e informar algum parâmetro que tenha sido deixado sem preenchimento.

* **Botão Criar** |botao_criar_on|: Nesta última etapa todos os parâmetros fundamentais para a criação da máquina virtual devem ter sido informados corretamente, o usuário percebe que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão criar para que a Plataforma uCloud envie todos os parâmetros da máquina virtual para o provedor de serviço de nuvem (via API-Rest) selecionado, para o completo provisionamento da máquina virtual.

* Caso este botão não esteja habilitado (cor cinza |botao_criar_off|), significa afirmar que algum parâmetro anterior foi deixado em branco, por este motivo a Plataforma uCloud impede o provisionamento da máquina virtual.

* Após clicar com o cursor do mouse sobre o botão Criar a Plataforma uCloud encerra a tela do wizard, envia a *Tarefa* de provisionamento da máquina virtual para o provedor de serviço de nuvem selecionado na Wizard Etapa 1, em seguida, atualiza a lista do inventário de máquinas virtuais apresentando a nova máquina virtual nesta lista.

.. important:: |atencao| Importante mencionar que após criar uma nova máquina virtual a atualização da relação de máquinas virtuais na interface da Plataforma uCloud pode não ser imediata, o uCloud não tem controle do tempo que o provedor de serviço de nuvem necessita para coletar todos os recursos computacionais necessários (CPU, memória, Disco, outros) para configurar a máquina virtual.

O usuário pode acompanhar a evolução do processamento da sua solicitação no ambiente do provedor de serviço de nuvem através do menu **Tarefas**.

----

Menu Scaling Groups
===================
Este menu apresenta ao usuário os Grupos de Escalabilidade (Scaling Groups) provisionados na Plataforma uCloud. Esta funcionalidade é comum a qualquer provedor de serviço de nuvem. Os nomes desta funcionalidade diferem em cada provedor, mas os conceitos são universais. O Grupo de Escalabilidade possibilita que novas instâncias de uma máquina virtual sejam criadas, tendo como base a máquina inicial (clonagem). Estas novas instâncias serão criadas e iniciadas automaticamente, de forma a suportar a carga de conexão em paralelo (horizontal). O Grupo de Escalabilidade tanto pode iniciar novas máquinas, bem como desligar as máquinas criadas quando a demanda de conexões diminuir - dentro dos parâmetros definidos na criação - se comporta automaticamente, aumentando ou diminuindo a quantidade de instâncias de máquinas virtuais, com base no consumo monitorado e controlado.

Grupo de Escalabilidade é um recurso integrado de serviços em nuvem, serviços móveis, máquinas virtuais e sites que ajuda os aplicativos a ter o melhor desempenho quando há mudanças na demanda. Importante mencionar que ‘desempenho’ pode significar coisas diferentes para aplicativos diferentes. Alguns aplicativos são limitados pela CPU, outros pela memória. Por exemplo, você pode ter um aplicativo da web que lida com milhões de solicitações durante o dia e nenhum à noite. A escala automática pode escalar seu serviço por qualquer um deles - ou por uma métrica personalizada definida pelo usuário.

Antes de iniciar este processo de criação de um Grupo de Escalabilidade, verifique se a Plataforma uCloud possui os pré-requisitos para completar o processo de ponta-a-ponta de forma correta. Devem existir os seguintes pré-requisitos para qualquer ambiente de provedor de serviço de nuvem:

* Ao menos uma máquina virtual ativa (status: *Running*) que será utilizada como referência para clonagem;
* Provisionamento de Balanceador (*Load Balancer*) (ver item Rede / Balanceador);
* Provisionamento de um Grupo de Segurança (ver item Rede / Grupo de Segurança / Criar Grupo de Segurança).

Importante ressaltar que os tópicos acima são fundamentais, caso não tenham sido previamente provisionados, o usuário será obrigado a interromper a criação do Grupo de Escalabilidade e providenciar a criação dos tópicos acima.
Atualmente apenas dois provedores possuem interface via API-Rest, para suportar o processo de provisionamento de um Grupo de Escalabilidade, Amazon AWS e Azure.

Abaixo segue descrição de ambos os processos, pois cada provedor de serviço de nuvem pública possui parâmetros específicos para o correto provisionamento de um Grupo de Escalabilidade em seu ambiente.

Criando um Scaling Group AWS
----------------------------

Um Grupo de Escalabilidade monitora os recursos das máquinas virtuais e ajusta automaticamente a capacidade para manter um desempenho constante e previsível pelo menor custo possível.

Com o Grupo de Escalabilidade, é fácil estabelecer a escalabilidade de aplicativos para vários recursos em diversos serviços em questão de minutos. O serviço oferece uma interface de usuário simples e eficiente que permite criar planos de escalabilidade para recursos. Importante ressaltar que não haverá nenhum impacto, ou perda, de funcionalidade ao provisionar um Grupo de Escalabilidade seja diretamente no console do ambiente da AWS, seja através da interface da Plataforma uCloud.

Antes de iniciar a criação de um Grupo de Escalabilidade, o usuário deve navegar nas opções de menu da Plataforma uCloud, e certificar se o ambiente possui os pré-requisitos listados abaixo:

* Ao menos uma máquina virtual ativa (status: Running) que será utilizada como referência para clonagem;
* Provisionamento de Balanceador (Load Balancer) (ver item Rede / Balanceador);
* Provisionamento de um Grupo de Segurança configurado de acordo com os listeners do balanceador (ver item Rede / Grupo de Segurança / Criar Grupo de Segurança).

A tela apresentada abaixo permite ao usuário provisionar um Grupo de Escalabilidade (Auto Scaling na AWS), importante ressaltar que os parâmetros apresentados nesta interface são os parâmetros disponíveis para integração via API-Rest. Caso o usuário possua experiência de interação direta via o console da AWS, este poderá notar algumas pequenas diferenças.

.. image:: /figuras/ucloud_scaling_group_AWS_001.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

Abaixo segue a descrição do correto preenchimento da tela para provisionar um Grupo de Escalabilidade no ambiente da AWS:

* **Nome**: Este campo é obrigatório o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar este Grupo de Escalabilidade. Sugerimos utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido). Importante mencionar que este nome pode ser acrescentado com as informações específicas do provedor de serviço de nuvem, a Plataforma uCloud não tem controle (remoção ou alteração) destas adições do(s) provedor(es).
* **Balanceador**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud lista todos os Balanceadores que foram provisionados na Plataforma uCloud e estão vinculados ao provedor de serviço de nuvem Amazon AWS.
* **Instância de Lançamento**: Este campo é obrigatório do tipo “dropdown” quando o usuário clicar com o cursor do mouse a Plataforma uCloud lista todas as máquinas virtuais provisionadas no ambiente da Amazon AWS. O usuário deve selecionar a máquina virtual a ser utilizada como ‘o padrão’ para o processo de clonagens e crescimento do Grupo de Escalabilidade. Importante ressaltar que para o perfeito funcionamento do Grupo de Escalabilidade, a máquina virtual selecionada deve estar operacional e ativa (Status:Running), caso contrário o Grupo de Escalabilidade deixa de efetuar a função para a qual foi provisionado.
* **Valor Máximo**: Este campo é obrigatório o usuário deve informar um número inteiro que representa a quantidade máxima de instâncias que podem ser criadas (clonadas) no ambiente da AWS para suportar a performance máxima desejada.
* **Valor Mínimo**: Este campo é obrigatório o usuário deve informar um número inteiro que representa a quantidade mínima de instâncias que devem existir (serão mantidas ativas) no ambiente da AWS para suportar a performance média desejada.
* **Políticas**: Estes campos são obrigatórios o usuário deve informar os parâmetros de performance - mínimo e máximo - ao ser atingido, o mínimo ou máximo, deve ser disparado o evento de aumento ou redução da quantidade de máquinas virtuais:
* **Ação**: Esta coluna apresenta o tipo de política que foi configurada. O usuário pode criar uma ação tanto para o aumento quanto para diminuição do número de máquinas virtuais.
* **Tipo**: Esta coluna apresenta qual o tipo de recurso computacional definido para ser monitorado na máquina virtual, em relação ao critério da ação da coluna anterior. O usuário pode estabelecer que a tomada de decisão para o Grupo de Escalabilidade seja baseada no recurso computacional CPU ou na  Memória.
* **Condição**: Nesta coluna o usuário nota que existe apenas um sinal matemático de maior-ou-igual (“>=”) para a condição de aumento de quantidade de máquinas virtuais, ou um sinal de menor-ou-igual (“<=”) para a condição de diminuição da quantidade de máquinas virtuais. A Plataforma uCloud não permite ao usuário alterar estas condições para uma condição diferente, existem apenas as duas acima citadas.
* **Quantidade %**: Neste campo o usuário pode definir um número inteiro, de duas casas (nn), sem casas decimais, que indica o valor máximo de ocupação do recurso computacional (CPU ou Memória). Este valor será o limite máximo (threshold) de referência que o ambiente de nuvem da AWS utiliza para iniciar a ação (aumento/diminuição) ao qual este percentual está vinculado.
* **Tempo**: Este campo é obrigatório do tipo “dropdown” ,  quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta uma lista de três opções de limite de tempo (1, 3 ou 5 minutos). Este é o limite de tempo no qual o recurso computacional deve se manter no percentual de ocupação informado acima, limite este que o ambiente de nuvem da AWS utiliza para iniciar a ação (aumento/diminuição) ao qual este limite está vinculado.
* **Ações**: Esta coluna apresenta apenas o ícone de Lata de Lixo “  ”, basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova esta Política de Aumento ou Diminuição de forma imediata e definitiva.
* **Botão “+Adicionar Política de Diminuir”**: Este botão pode ser utilizado para adicionar uma nova linha de controle para diminuição de máquinas virtuais, por exemplo, tendo como base em um recurso computacional diferente do pré-existente.
* **Botão “+Adicionar Política de Aumentar”**: Este botão pode ser utilizado para adicionar uma nova linha de controle para aumento de máquinas virtuais, por exemplo, tendo como base em um recurso computacional diferente do pré-existente.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Grupo de Escalabilidade. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação do Grupo de Escalabilidade no ambiente Amazon AWS, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar , logo a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento do Grupo de Escalabilidade.

  Caso este botão **não esteja habilitado (cor cinza)**, significa que algum parâmetro anterior foi deixado em branco, a Plataforma uCloud não permitirá o provisionamento da máquina virtual até que o parâmetro seja preenchido..

Problemas Conhecidos com Grupo de Escalabilidade AWS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Importante ressaltar: Considerar que o gerenciamento das condições de ocupação de CPU e memória - para o aumento ou diminuição da quantidade de máquinas virtuais, é gerenciado unicamente pela AWS - os problemas podem estar nos critérios conflitantes para a criação ou no monitoramento.

* **Erros na criação**:

  * Informações inseridas incorretamente no formulário (como números negativos, por exemplo);
  * Instância de lançamento desligada durante a criação;
  * Recursos (balanceador, por exemplo) existentes no uCloud, mas inexistentes na AWS por terem sido deletados diretamente no console AWS;

* **Erros no monitoramento**:

  * O status das máquinas do Grupo de Escalabilidade são mantidos atualizados pela Plataforma uCloud a cada 30 segundos, problemas de comunicação Internet com o console da AWS podem fazer com que essas máquinas não sejam atualizadas na tela do uCloud.

Criado um Scaling Group Azure
-----------------------------

O ambiente Microsoft Azure possui uma tela/formulário mais extenso e, portanto, uma tela específica para esta finalidade. Abaixo segue descrição do correto preenchimento da tela para provisionar um Grupo de Escalabilidade (Virtual Machine Scale Set) no ambiente da Azure:

.. image:: /figuras/ucloud_scaling_group_AZURE_001.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Nome**: Este campo é obrigatório o usuário deve informar o nome (no mínimo 3 caracteres no máximo 15 caracteres) com o qual deseja identificar este Grupo de Escalabilidade. Sugerimos utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido). Importante mencionar que este nome pode ser acrescido com informações específicas do provedor de serviço de nuvem, a Plataforma uCloud não tem controle (remoção ou alteração) destas adições do(s) provedor(es).
* **Container**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresentará uma lista com o(s) provedore(s) de serviço de nuvem Azure configurados no ambiente da Plataforma uCloud, basta o usuário selecionar o provedor desejado.
* **Virtual DataCenter**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta uma lista de Virtual Datacenter(s) vinculados ao provedor de serviço de nuvem Azure, configurados no ambiente da Plataforma uCloud. Basta o usuário selecionar o provedor desejado. Importante mencionar que este campo determina o conteúdo de outros campos deste formulário de provisionamento de um Grupo de Escalabilidade Azure.
* **Região**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta uma lista com a(s) região(ões) de presença global do provedor de serviço de nuvem Azure. Estas regiões são configuradas e vinculadas ao Virtual Datacenter selecionado anteriormente, basta o usuário selecionar a região desejada.
* **Contagem de instâncias**: Este campo é obrigatório,  o usuário deve informar um número inteiro que representa a quantidade padrão (default) de instâncias de máquinas virtuais que deve existir no ambiente da Azure para suportar a performance média desejada.
* **Template**: Este campo é obrigatório do tipo “dropdown”,  quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com os templates do provedor de serviço de nuvem Azure. Estes templates são configurados e vinculados ao Virtual Datacenter selecionado anteriormente, basta o usuário selecionar o template desejado.
* **Flavor**: Este campo é obrigatório do tipo “dropdown”, ao clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com os flavors do provedor de serviço de nuvem Azure. Estes flavors são configurados e vinculados ao Virtual Datacenter selecionado anteriormente, basta o usuário selecionar o flavor desejado.
* **Usuário**: Este campo é obrigatório, deve ser preenchido com a sequência de caracteres que será utilizada para identificar as credenciais do usuário ‘Administrador’ para o processo de login no sistema operacional da máquina virtual. Sugerimos utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Senha**: Este campo é obrigatório, o usuário deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”, conforme a documentação encontrada no site da Azure. A recomendação é de no mínimo doze (12) caracteres, a sequência deve conter caracteres de três das seguintes categorias:

  * Letras maiúsculas e minúsculas (A a Z)
  * Números de base 10 (de 0 a 9)
  * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' <>,.? /) – Importante ressaltar que símbolos de moeda como o euro ou a libra britânica (€/£) não são contados como caracteres especiais para essa configuração de política.

* **Rótulo do Nome de Domínio**: Este campo é obrigatório, o usuário deve informar o nome do Balanceador de Carga, que foi provisionado para o ambiente Azure.
* **Porta do balanceador**: Este campo é obrigatório, o usuário deve informar o número da Porta TCP-IP configurada no balanceador, previamente provisionado (pré-requisito), uma vez que é esta a Porta TCP-IP a ser utilizada para monitorar o nível de ocupação do recurso computacional que será definido a seguir  na seção Políticas.
* **Valor Máximo**: Este campo é obrigatório, o usuário deve informar um número inteiro que representa a quantidade máxima de instâncias que podem ser criadas (clonadas) no ambiente da Azure para suportar a performance máxima desejada.
* **Valor Mínimo**: Este campo é obrigatório, o usuário deve informar um número inteiro que representa a quantidade mínima de instâncias que devem existir (serão mantidas ativas) no ambiente da Azure para suportar a performance média desejada.
* **Políticas**: Estes campos são obrigatórios, o usuário deve informar os parâmetros de performance, mínimo e máximo, quando estes patamares são atingidos é disparado o evento de aumento ou redução da quantidade de máquinas virtuais:

  * **Ação**: Esta coluna apresenta o tipo de política que foi configurada. O usuário pode criar uma ação tanto para o aumento quanto para diminuição do número de máquinas virtuais.
  * **Tipo**: Esta coluna apresenta qual o tipo de recurso computacional definido a ser monitorado na máquina virtual, em relação ao critério da ação da coluna anterior. O usuário pode estabelecer que a tomada de decisão para o Grupo de Escalabilidade seja baseada no recurso computacional CPU ou Memória.
  * **Condição**: Nesta coluna o usuário nota que existe apenas um sinal matemático de maior-ou-igual (“>=”) para a condição de aumento da quantidade de máquinas virtuais ou um sinal de menor-ou-igual (“<=”) para a condição de diminuição da quantidade de máquinas virtuais. A Plataforma uCloud impede o usuário de alterar estas condições para uma condição diferente, existem apenas as duas acima citadas.
  * **Quantidade %**: Neste campo o usuário pode definir um número inteiro, de duas casas (nn), sem casas decimais, que indica o valor máximo de ocupação do recurso computacional (CPU ou Memória). Este valor será o limite máximo (threshold) de referência que o ambiente de nuvem da AWS utilizará para iniciar a ação (aumento/diminuição) ao qual este percentual está vinculado.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Grupo de Escalabilidade. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação do Grupo de Escalabilidade no ambiente Azure, o usuário verifica que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão criar para que a Plataforma uCloud envie todos os parâmetros para o ambiente da AWS, para o completo provisionamento do Grupo de Escalabilidade.

  Caso este botão **não esteja habilitado (cor cinza)**, significa que algum parâmetro anterior foi deixado em branco, a Plataforma uCloud não permitirá o provisionamento da máquina virtual até que o parâmetro seja preenchido.


Menu Banco de Dados
===================

Uma instância de banco de dados é um ambiente de banco de dados isolado e pode ser provisionado apenas nos provedores de serviço computacional de nuvem pública. Os ambientes de nuvem privada (“on-premises”), não possuem a camada de aplicação (API) que permitem implementar esta funcionalidade da mesma forma como em um provedor de serviço de nuvem pública.

A instância de banco de dados pode conter vários bancos de dados criados pelo usuário. É possível acessar a instância de banco de dados usando as mesmas ferramentas e os mesmos aplicativos usados com uma instância de banco de dados independente.

Cada instância de banco de dados executa um mecanismo (“engine”) de gerenciamento de banco de dados, e o usuário deve ter em mente as particularidades de cada gerenciador de banco de dados antes de iniciar o provisionamento.

Importante ressaltar que cada provedor de serviço computacional de nuvem pública (AWS, Azure e GCP) possui diferentes conjuntos de suporte para mecanismos de gerenciamento de bancos de dados:

+-------------------------+---------+---------+---------+
| Vendor Data Base Engine |   AWS   |  Azure  |   GCP   |
+=========================+=========+=========+=========+
| MySQL                   | **SIM** | **SIM** | **SIM** |
+-------------------------+---------+---------+---------+
| MariaDB                 | **SIM** | *Não*   | *Não*   |
+-------------------------+---------+---------+---------+
| PostgreSQL              | **SIM** | *Não*   | **SIM** |
+-------------------------+---------+---------+---------+
| Microsoft SQL Server    | **SIM** | **SIM** | *Não*   |
+-------------------------+---------+---------+---------+
| Oracle                  | **SIM** | *Não*   | *Não*   |
+-------------------------+---------+---------+---------+

Cada mecanismo de banco de dados tem seus próprios recursos com suporte, cada versão de um mecanismo de banco de dados pode incluir recursos específicos. Além disso, cada mecanismo de banco de dados tem um conjunto de parâmetros em um parameter group de banco de dados que controlam o comportamento dos bancos de dados que ele gerencia.
Para obter mais informações, consulte a documentação online sobre bancos de dados de seu(s) provedor(es) de serviço de nuvem específico.
Quando o usuário acessa esta opção de menu, a Plataforma uCloud apresenta uma tela com o inventário completo de todas as instâncias de Bancos de Dados (RDS) que foram provisionadas por todos os usuários vinculados ao(s) contrato(s) que o usuário está associado.
Esta tela pode ser muito extensa pois apresenta todas as instâncias de Bancos de Dados encontradas. No exemplo abaixo, estão listadas apenas algumas instâncias de Bancos de Dados:

.. image:: /figuras/ucloud_databases_001.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Busca Rápida**: O usuário pode observar que logo abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de nomes de opções de menu. Basta preencher o campo em branco com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca refletida na relação de máquinas virtuais na lista.
* **Nome**: Nesta coluna é apresentado o nome da máquina virtual informado no momento da sua criação no console do provedor de serviço de nuvem, pode também ser informado no momento que foi configurado através do uCloud. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de máquinas virtuais de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Container**: Esta coluna apresenta o nome do Provedor de Serviço de Nuvem (“container”) informado no momento do provisionamento da instância de Banco de Dados. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de containers de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Região**: Esta coluna apresenta o nome da Região do provedor de serviço de nuvem informada no momento do provisionamento da instância de Banco de Dados. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes das regiões de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Usuário**: Nesta coluna é apresentado o nome das credenciais do usuário que está com uma sessão ativa na Plataforma uCloud, no momento do provisionamento da instância de Banco de Dados. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de containers de forma alfabética crescente (a – z) ou decrescente (z – a).
* **CPU**: Esta coluna apresenta a quantidade de CPU que está associada ao hardware (“flavor”) selecionado no momento do provisionamento da instância de Banco de Dados. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de grupos com base no valor da quantidade de CPU, de forma crescente ou decrescente.
* **Memória**: Nesta coluna é apresentado o número da quantidade de memória RAM que está associada ao hardware (“flavor”) selecionado no momento do provisionamento da instância de Banco de Dados, expressa sempre em Gigabytes. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de máquinas virtuais com base no tamanho da memória, de forma crescente ou decrescente.
* **Status**: Esta coluna apresenta o status corrente da instância de Banco de Dados (“RDS”). Importante ressaltar que o status é obtido do provedor de serviço de nuvem, pois a instância de Banco de Dados está instalada e sendo executada nas infraestruturas do provedor de serviço de nuvem. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica o status da lista de máquinas virtuais de forma alfabética crescente (a – z) ou decrescente (z – a). A Plataforma uCloud apresenta os seguintes status:

  * **Available**: Status que indica que a instância de Banco de Dados está em funcionamento normal.
  * **Unknown**: Este status pode ser apresentado, pois se refere a um estado temporário, onde momentaneamente não é possível distinguir se a instância de Banco de Dados está parada ou rodando (falha de comunicação entre a Plataforma uCloud e o console do provedor de serviço de nuvem pública).

* **Ações**: Esta coluna apresenta dois ícones para que o usuário possa interagir com a Instância de Banco de Dados:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova esta instância de Banco de Dados, de forma imediata e definitiva.
  * **Ícone Reiniciar** |icone_vm_reboot|: Basta clicar sobre este ícone quando o usuário necessita reiniciar a instância de Banco de Dados respectiva. Importante mencionar que reiniciar uma instância de banco de dados é necessário, geralmente, por motivos de manutenção. Por exemplo: Se o usuário fizer determinadas modificações ou alterar o parameter group de banco de dados associado à instância de banco de dados, todas as documentações online sugerem que é necessário reiniciar uma instância de Banco de Dados para que as alterações sejam implementadas.


Gerenciando um Banco de Dados
-----------------------------
Quando o usuário clicar com o cursor do mouse em uma das linhas da lista de Bancos de Dados, a Plataforma uCloud apresenta uma tela com algumas seções (cards), a seguir é apresentada a descrição de cada seção:

.. image:: /figuras/ucloud_databases_002.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

Seção Geral - Grupo Segurança
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
* **Status**: Este campo apresenta a situação atual da instância de banco de dados no ambiente do provedor de serviço de nuvem.
* **Container**: Este campo apresenta o nome do provedor de serviço de nuvem pública (“container”), provisionado na Plataforma uCloud, o qual foi selecionado no momento do provisionamento da instância de banco de dados.
* **Região**: Este campo apresenta o nome da região global do provedor de serviço de nuvem pública (“container”) o qual foi selecionado no momento do provisionamento da instância de banco de dados.
* **Nome**: Este campo apresenta o nome da instância de banco de dados, o qual foi selecionado no momento do provisionamento da instância de banco de dados.
* **Engine**: Este campo apresenta o nome do mecanismo (“engine”) de banco de dados e sua versão, o qual foi selecionado no momento do provisionamento da instância de banco de dados.
* **Nome do banco de dados**: Este campo apresenta o nome do arquivo do banco de dados, informado no momento do provisionamento da instância de banco de dados.
* **ARN (exclusivo AWS)**: Este campo apresenta o nome de recurso Amazon (“ARN – Amazon Resource Name”), somente será apresentado para bancos de dados criados no ambiente da Amazon AWS. Consultar a documentação específica do seu provedor de serviço de nuvem pública.
* **Usuário**: Este campo apresenta o nome do usuário master da instância de banco de dados, informado no momento do provisionamento da instância de banco de dados.
* **Identificador (exclusivo AWS)**: Este campo apresenta o identificador do recurso (“Resource ID”), somente é apresentado para bancos de dados criados no ambiente da Amazon AWS. Consultar a documentação específica do seu provedor de serviço de nuvem pública.
* **Flavor**: Este campo apresenta o nome do flavor (configuração do hardware) da máquina virtual que executa a instância de banco de dados, nome informado no momento do provisionamento da instância de banco de dados.
* **Tipo do Storage**: Este campo apresenta o tipo do storage que armazena o arquivo do banco de dados, informado no momento do provisionamento da instância de banco de dados.
* **Tamanho do disco**: Este campo apresenta o tamanho do disco de armazenamento, informado no momento do provisionamento da instância de banco de dados.
* **EndPoint**: Este campo apresenta a identificação que o provedor de serviço de nuvem pública assinalou a esta instância de banco de dados, procedimento realizado para que se possa conectar um servidor HTML (web) a esta instância de banco de dados. Importante ressaltar que alguns provedores de serviço de nuvem pública não geram automaticamente esta informação. Consultar a documentação específica do seu provedor de serviço de nuvem pública.
* **Porta**: Este campo apresenta o número da Porta TCP-IP informado no momento do provisionamento da instância de banco de dados.
* **Rede**: Este campo apresenta o nome da rede TCP-IP que foi provisionada na Plataforma uCloud, selecionada no momento do provisionamento da instância de banco de dados. Importante mencionar que esta rede está vinculada à região global do provedor de serviço de nuvem pública.
* **Publicamente acessível**: Este campo apresenta a seguinte informação: Se esta instância de banco de dados pode ser acessada através de uma rede pública (Internet). Parâmetro informado no momento do provisionamento da instância de banco de dados.
* **Multi AZ**: Este campo apresenta o parâmetro sobre a existência das réplicas da instância de banco de dados em diferentes Zonas de Disponibilidade (“Availability Zone”) da Região Global do provedor de serviço de nuvem pública. Importante ressaltar que alguns provedores de serviço de nuvem pública não possuem suporte para diferentes Zonas de Disponibilidade (“Multi AZ”). Consultar a documentação específica de seu provedor de serviço de nuvem pública sobre o suporte para esta funcionalidade.
* **Backup automático**: Este campo apresenta o parâmetro referente ao número de dias que a cópia de segurança (backup) permanece armazenada no ambiente do provedor de serviço de nuvem, parâmetro informado no momento do provisionamento da instância de banco de dados.
* **Janela de Backup**: Este campo apresenta o parâmetro referente ao agendamento de cópia de segurança (backup) informado no momento do provisionamento da instância de banco de dados.
* Último momento restaurável: Este campo apresenta a data e a hora, da cópia de segurança mais recente do banco de dados.
* **Criado por**: Este campo apresenta uma identificação gerada, internamente, pelo provedor de serviço de nuvem pública. Importante mencionar que esta identificação não é necessariamente a mesma das credenciais do usuário registrado na Plataforma uCloud.

Seção Grupos de Segurança
~~~~~~~~~~~~~~~~~~~~~~~~~
* **Nome**: Esta coluna apresenta o nome do Grupo de Segurança (security group) vinculado ao Banco de Dados, no momento do provisionamento da instância de banco de dados.
* **Criado Por**: Esta coluna apresenta a identificação da credencial de login do usuário responsável pela criação do Grupo de Segurança.
* **Ações**: Esta coluna apresenta dois ícones para que o usuário possa interagir com as configurações do Grupo de Segurança:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova este Grupo de Segurança de forma imediata e definitiva.
  * **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone para que a Plataforma uCloud possa apresentar uma tela que permite editar as configurações do Grupo de Segurança respectivo.

Provisionando um Banco de Dados
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Importante esclarecer os parâmetros que devem ser informados para completar o processo de provisionar uma instância de Banco de Dados solicitados na interface da Plataforma uCloud, são os parâmetros disponíveis para integração via API-Rest. Caso o usuário possua experiência de interação direta via o console do seu provedor, este poderá notar algumas pequenas diferenças.
Para criar um banco de dados o usuário seleciona a nuvem pública e, logo o portal uCloud indica quais as opções de banco de dados disponíveis em cada provedor de serviço de nuvem, pois são estas as opções e suas respectivas edições, elas são diferentes para cada provedor de serviço de nuvem pública (AWS, Azure e GCP). Cada um destes provedores possui diferentes conjuntos de suporte para os mecanismos de gerenciamento de bancos de dados, através da comunicação via API a Plataforma uCloud apresenta estas opções ao usuário.
O processo de criação de uma instância de Banco de Dados (RDS – Relational Database System) é segmentado em várias etapas e cada mecanismo (“engine”) de gerenciamento de banco de dados possui parâmetros diferentes que são solicitados pela Plataforma uCloud.
O usuário deve sempre consultar a documentação online das opções de instâncias de Bancos de Dados do seu provedor(es) de serviço de nuvem da sua preferência para compreender qual o Gerenciador (“engine”) de bancos de dados e seus parâmetros são os mais adequados e atendem às necessidades do usuário.
Devido a uma grande diversidade de opções de criação de bases de dados e seus parâmetros em diferentes provedores de serviço de nuvem, para apresentar as diferenças entre provedores de serviço de nuvem, a seguir é documentado apenas os processos de criação de uma instância de base de dados com o software MySQL em três diferentes provedores.
Desta forma o usuário pode acompanhar as caraterísticas de cada ambiente de nuvem pública e seus parâmetros específicos.

Criação de Banco de Dados (MySQL & AWS)
---------------------------------------
Nas telas a seguir serão utilizadas as telas de exemplo para o provedor AWS, o qual demonstra as características e o suporte a diversos mecanismos de gerenciamento de bases de dados e seus parâmetros.


Etapa 1 Seleção do Provedor de Serviço de Nuvem (AWS) [4 nivel]
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
A seguir são utilizadas as telas de exemplo para o provedor AWS que demonstra o suporte a diversos mecanismos de gerenciamento bases de dados, apenas para apoiar a conectividade da Plataforma uCloud com a API e para apoiar a didática da criação de uma Instância de Banco de Dados em um provedor de nuvem pública.
Importante ressaltar que, para efeito didático e apenas como exemplo, são seguidas as etapas de criação de um Banco de Dados MySQL.
A Plataforma uCloud apresenta a tela abaixo ao usuário, a seleção do provedor determina o conteúdo das telas seguintes.

.. image:: /figuras/ucloud_databases_003.png
   :alt: Scaling Group AWS - Exemplo
   :scale: 60 %
   :align: center

----

Nesta etapa, o usuário deve clicar com o cursor do mouse sobre o ícone do provedor de serviço de nuvem **AWS** apresentado nesta tela.

Etapa 2 Seleção do Banco de Dados (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Esta tela permite ao usuário selecionar qual o mecanismo (“*engine*”) de gerenciamento de bancos de dados. A seguir é apresentada uma tela capturada do ambiente da **AWS**, apenas como um exemplo didático.

.. image:: /figuras/ucloud_databases_013b.png
   :alt: Scaling Group AWS - Exemplo
   :scale: 60 %
   :align: center

----

Nesta etapa, o usuário deve clicar com o cursor do mouse sobre o ícone do MySQL provedor de serviço de nuvem apresentado nesta tela.
* **Botão Selecione**: Após selecionar qualquer uma das opções de bancos de dados, o usuário deve clicar com o cursor do mouse no botão Selecionar para a Plataforma uCloud apresentar a tela da Etapa 3, descrito a seguir.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 3 Especificações do Banco de Dados (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa, o usuário deve informar os parâmetros iniciais do ambiente computacional que dará suporte para a execução da instância de banco de dados.

.. image:: /figuras/ucloud_databases_004.png
   :alt: Scaling Group AWS - Exemplo
   :scale: 60 %
   :align: center

----

* **Região**: Este campo é obrigatório do tipo “dropdown” , quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas as regiões do provedor de serviço de nuvem selecionado na Etapa 1. Importante mencionar que cada provedor possui identificação de regiões específicas, este campo reflete suas especificidades.
* **Zona de Disponibilidade**: Este campo é obrigatório do tipo “dropdown”, ao clicar com o cursor do mouse a Plataforma uCloud apresenta ao  usuário uma lista com todas as regiões do provedor de serviço de nuvem selecionado na Etapa 1. O usuário  deve ter em mente que nem todos os provedores de serviço de nuvem possuem zonas de disponibilidade (zonas dentro de uma região). O campo é apresentado apenas nos casos em que o provedor possui esta informação.
* **Versão**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas as versões do Banco de Dados MySQL disponíveis no ambiente do provedor de serviço de nuvem.
* **Flavor**: Este campo é obrigatório do tipo “dropdown”, ao clicar com o cursor do mouse a Plataforma uCloud apresenta ao  usuário uma lista com todas as configurações de hardware (“flavor”), criadas pelo provedor de serviço de nuvem e dedicadas (especializadas) para executar instâncias de Bancos de Dados.
* **Multi-AZ Deployment**: As implantações Multi-AZ do Amazon RDS proporcionam disponibilidade e durabilidade melhores para instâncias de banco de dados (DB) do RDS, o que as torna a solução ideal para cargas de trabalho de banco de dados de produção. No momento de provisionar uma Instância de DB Multi-AZ, o Amazon RDS cria automaticamente uma Instância de DB principal e replica de forma síncrona os dados para uma instância de espera em uma Zona de Disponibilidade (AZ) diferente.
* **Tipo de Storage**: Este campo é obrigatório do tipo “dropdown”, ao clicar neste campo com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas as opções de tipos de discos de armazenamento (“storage”). Outras informações consultar a documentação online da AWS (usado neste exemplo como forma didática) para entender as diferenças entre as características entre a opção General Purpose SSD e SSD Provisioned IOPS.
* **Tamanho do Disco**: Este campo é obrigatório ele deve ser preenchido com um número inteiro que define o tamanho máximo do recurso computacional de Disco de Armazenamento. Este número deve ser informado em Gigabytes.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 4 Configurações de acesso ao Banco de Dados (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros de acesso à instância de banco de dados.

.. image:: /figuras/ucloud_databases_004.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo um [1] e no máximo oito [8] caracteres) com o qual deseja identificar o Banco de Dados. É indicado utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Nome do Banco de Dados**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo um [1] e no máximo oito [8] caracteres) com o qual deseja nomear o arquivo do Banco de Dados. É indicado utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Usuário**: Este campo é obrigatório ele deve ser preenchido com a sequência de caracteres (no mínimo um [1] e no máximo quinze [15] caracteres) a ser utilizada para identificar as credenciais do usuário “Master” no processo de login no Gerenciador Banco de Dados. É indicado utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Senha**: Este campo é obrigatório ele deve ser preenchido com a sequência de caracteres da senha do usuário. Importante ressaltar que esta sequência deve ser maior que quatro [4] caracteres alfanuméricos. O preenchimento deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”. A recomendação é utilizar no mínimo oito [8] e no máximo setenta e dois [72] caracteres e deve conter caracteres de três [3] das seguintes categorias:

  * Letras maiúsculas e minúsculas (A a Z)
  * Números de base 10 (de 0 a 9)
  * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' <>,.? /) – Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política.

* **Confirmar Senha**: Este campo é obrigatório ele deve ser preenchido com a mesma sequência de caracteres informados no campo anterior. Caso a sequência informada neste campo seja diferente da anterior, o botão Próximo permanece inativo.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse, por engano, sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 5 Especificações de Rede e Segurança (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros de Rede e de Grupo de Segurança para o acesso à infraestrutura que executa a instância de banco de dados (máquina virtual).

.. image:: /figuras/ucloud_databases_005.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Rede**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista somente com as redes provisionadas na Região selecionadas na Etapa 3.
* **Publicamente Acessível**: Este campo é obrigatório do tipo “dropdown”, no caso do usuário clicar com o cursor do mouse sobre ele, a Plataforma uCloud apresenta uma lista com apenas duas opções SIM ou NÃO. Quando o usuário seleciona a opção SIM, o provedor de serviço de nuvem vincula um Endereço TCP-IP Público a esta instância de Banco de Dados, com a finalidade de ser acessível através da Internet.
* **Zona de Disponibilidade**: Este campo é obrigatório do tipo “dropdown”, ao clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas
* **Grupo de Segurança**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta uma lista com todos os Grupos de Segurança (Security Group) que foram provisionados para a mesma Região e Rede informados nas etapas anteriores.
* **Porta do Banco de Dados**: Este campo é obrigatório, deve ser preenchido com a Porta TCP-IP específica para o acesso ao Bancos de Dados, a Plataforma uCloud apresenta a Porta TCP-IP padrão 3306. A sugestão é manter esta informação.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse, por engano, sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode clicar e retornar a Etapa 1, na seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 6 Parâmetro de Cópia de Segurança (MySQL & AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros que definirão o processo de cópia de segurança (backup) da instância de banco de dados.

.. image:: /figuras/ucloud_databases_003.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Período de Retenção do Backup**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com números que representam o número de dias que a cópia de segurança (backup) permanece armazenada no ambiente do provedor de serviço de nuvem. Um número maior ou igual a um [1] indica que o usuário tem interesse em manter uma cópia de segurança (backup) ativo. Caso o usuário selecione “zero” [0] isto configura que o usuário não manterá nenhuma cópia de segurança (backup) do banco de dados no ambiente.
* **Janela do Backup**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta as duas opções disponíveis:

  * **Sem Preferência**: Esta opção indica que o usuário não deseja programar a cópia de backup em uma janela de tempo específica. Desta forma, a rotina de backup é efetuada na data agendada.
  * **Selecionar Janela**: Esta opção permite ao usuário determinar o horário da programação da cópia de segurança. Esta definição de data e hora, utiliza o agendamento em Tempo Universal Coordenado (UTC – Coordinated Universal Time). Quando selecionada esta opção, a Plataforma uCloud apresenta campos para o usuário definir o horário de início da rotina de backup e o tempo máximo para que este backup ser efetuado
    * *Exemplo*: Início às 2h00 UTC duração 2 horas, significa que a rotina de backup inicia às 2h00 da manhã UTC e encerra às 4h00 manhã UTC (tempo máximo de 2 horas).

* **Ícone Agendar**: Este permite ao usuário agendar o provisionamento do Banco de Dados, o valor padrão é Desabilitado (botão na cor vermelha).

.. image:: /figuras/ucloud_databases_006b.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

  * **Ícone Desabilitado** (|icone_desb_verm|): Este ícone indica que não existe agendamento estabelecido. Isto significa que este Banco de Dados será provisionado imediatamente no ambiente do provedor de serviço de nuvem, basta o usuário clicar com o cursor do mouse no botão Criar (cor verde).
  * **Ícone Habilitado** (|icone_habil_verde|): Este ícone indica que o usuário pretende agendar uma data para que o Banco de Dados seja provisionado no ambiente do provedor de serviço de nuvem. Este processo permite escolher a melhor data para que o recurso computacional de nuvem possa iniciar sua cobrança de valores em datas pré-definidas pela empresa usuária da Plataforma uCloud. Ao alternar o ícone para habilitado (cor verde), a Plataforma uCloud permite que o usuário preencha o campo com a data desejada.
  * **Ícone Calendário** (|icone_agenda|): Basta o usuário clicar sobre o ícone do calendário para a Plataforma uCloud apresentar o pop-up, permitindo ao usuário selecionar a data desejada, conforme a tela abaixo:

.. image:: /figuras/ucloud_databases_006b.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

  * **Ícone setas (🡩/🡫)**: Inicialmente a Plataforma uCloud apresenta o calendário com o dia e horário corrente, em destaque na cor azul. Para acionar o calendário, basta o usuário clicar com o cursor do mouse sobre o dia desejado, e pode clicar nos ícones de setas para selecionar outro mês. Quando selecionado, este será o dia programado para a Plataforma uCloud enviar a tarefa para o provedor de serviço de nuvem no provisionamento da máquina virtual.
  * **Hora / Minuto**: Este campo é apresentado no padrão de 24 horas e basta o usuário selecionar a hora e minuto desejado. Quando selecionado, este será o horário programado para que a Plataforma uCloud possa enviar a tarefa para o provedor de serviço de nuvem para o provisionamento da máquina virtual.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse, por engano, sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da última etapa de seleção do Banco de Dados.
* **Botão Criar**: Nesta etapa, é necessário que todos os parâmetros fundamentais para a criação da instância de Banco de Dados tenham sido informados corretamente, o usuário verifica que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros do Banco de Dados para o provedor de serviço de nuvem (via API-Rest) selecionado.
  Caso este botão não esteja habilitado (cor cinza) significa que algum parâmetro anterior foi deixado em branco, desta forma, a Plataforma uCloud não permite o provisionamento do Banco de Dados.

Criação de Banco de Dados (MySQL & Azure)
-----------------------------------------

Nas telas a seguir na ilustração, será utilizada a tela com o exemplo para o provedor Azure, ele demonstra as pequenas diferenças de suporte a mecanismos de gerenciamento de bases de dados e seus parâmetros.
Na tela a seguir apresentada pela Plataforma uCloud, a seleção do provedor determina o conteúdo das telas seguintes.

Etapa 1 Seleção do Provedor de Serviço de Nuvem (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A seguir são utilizadas as telas de exemplo para o provedor Azure que demonstra o suporte a apenas dois mecanismos de gerenciamento de bases de dados.
*Importante ressaltar que, para efeito didático e apenas como exemplo, seguem as etapas de criação de um Banco de Dados MySQL.*
A Plataforma uCloud apresenta a tela abaixo ao usuário, a seleção do provedor determina o conteúdo das telas seguintes.

.. image:: /figuras/ucloud_databases_003.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

Nesta etapa o usuário deve clicar com o cursor do mouse sobre o ícone do **MySQL** provedor de serviço de nuvem apresentado nesta tela.

* **Botão Selecione**: Após selecionar qualquer uma das opções de banco de dados o usuário deve clicar com o cursor do mouse no botão Selecionar para a Plataforma uCloud apresentar a tela da Etapa 3, descrito a seguir.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 2 Seleção do Banco de Dados (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta tela permite ao usuário selecionar qual o mecanismo (“engine”) de gerenciamento de bancos de dados. Abaixo é apresentada uma tela capturada do ambiente da Azure, apenas como um exemplo didático.

.. image:: /figuras/ucloud_databases_013c.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

Nesta etapa o usuário deve clicar com o cursor do mouse sobre o ícone do MySQL provedor de serviço de nuvem apresentado nesta tela.

* **Botão Selecione**: Após selecionar qualquer uma das opções de banco de dados o usuário deve clicar com o cursor do mouse no botão Selecionar para a Plataforma uCloud apresentar a tela da Etapa 3, descrito a seguir.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 3 Especificações do Banco de Dados (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa, o usuário deve informar os parâmetros iniciais do ambiente computacional Azure que dará suporte para a execução da instância de banco de dados.

.. image:: /figuras/ucloud_databases_009.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **VDC**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todos os Virtual Datacenters vinculados ao ambiente Azure.
* **Região**: Este campo é obrigatório do tipo “dropdown” , quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas as regiões do provedor de serviço de nuvem selecionado na Etapa 1. Importante mencionar que cada provedor possui identificação de regiões específicas, este campo reflete suas especificidades.
* **Flavor**: Este campo é obrigatório do tipo “dropdown” , quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas as configurações de hardware (“flavor”), criadas pelo provedor de serviço de nuvem e dedicadas (especializadas) para executar instâncias de Bancos de Dados.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 4 Configurações de acesso ao Banco de Dados (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros de acesso à instância de banco de dados.

.. image:: /figuras/ucloud_databases_010.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo dois [2] e no máximo oito [8] caracteres) com o qual deseja identificar o Banco de Dados. Sugerimos utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Usuário**: Este campo é obrigatório ele deve ser preenchido com a sequência de caracteres (no mínimo um [1] e no máximo quinze [15] caracteres) que é utilizada para identificar as credenciais do usuário “Master” para o processo de login no Gerenciador Banco de Dados. Como sugestão, utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Senha**: Este campo é obrigatório, ele deve ser preenchido com a sequência de caracteres da senha do usuário. Importante ressaltar que esta sequência deve ser maior que quatro (04) caracteres alfanuméricos. Deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”. A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres e deve conter caracteres de três das seguintes categorias:

  * Letras maiúsculas e minúsculas (A a Z)
  * Números de base 10 (de 0 a 9)
  * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' <>,.? /) – Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política.

* **Confirmar Senha**: Este campo é obrigatório, ele deve ser preenchido com a mesma sequência de caracteres informados no campo anterior. Caso a sequência informada neste campo seja diferente da anterior, o botão Próximo permanece inativo.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 5 Especificações de Rede e Segurança (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros de Rede e de Grupo de Segurança para o acesso à infraestrutura que executa a instância de banco de dados (máquina virtual).

.. image:: /figuras/ucloud_databases_011.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Rede**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista somente com redes provisionadas na Região selecionada na Etapa 3.
* **Subnet**: Este campo é obrigatório do tipo “dropdown”, ao clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas sub-redes (subnets) vinculadas a rede informada no campo acima.
* **Grupo de Segurança**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todos os Grupos de Segurança (Security Group) que foram provisionados para a mesma Região e Rede informados nas etapas anteriores.
* **Porta do Banco de Dados**: Este campo é obrigatório ele deve ser preenchido com a Porta TCP-IP específica para o acesso a Bancos de Dados, a Plataforma uCloud apresenta a Porta TCP-IP padrão 3306. É sugerido manter esta informação.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse, por engano, sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 6 Parâmetro de Cópia de Segurança (MySQL & Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros para definir o processo de cópia de segurança (backup) da instância de banco de dados.

.. image:: /figuras/ucloud_databases_012.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Período de Retenção do Backup**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com números que representam o número de dias que a cópia de segurança (backup) permanecerá armazenada no ambiente do provedor de serviço de nuvem. Um número maior ou igual a um (01) indica que o usuário tem interesse em manter uma cópia de segurança (backup) ativo. Caso o usuário selecione “zero” (0) isto configura que o usuário não manterá nenhuma cópia de segurança (backup) do banco de dados no ambiente.
* **Janela do Backup**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta as duas opções disponíveis:

  * **Sem Preferência**: Esta opção indica que o usuário não deseja programar a cópia de backup em uma janela de tempo específica. Desta forma, a rotina de backup será efetuada na data agendada.
  * **Selecionar Janela**: Esta opção permite ao usuário determinar o horário da programação da cópia de segurança. Esta definição de data e hora, utiliza o agendamento em Tempo Universal Coordenado (UTC – Coordinated Universal Time). Quando selecionada esta opção, a Plataforma uCloud apresenta campos para o usuário definir o horário de início da rotina de backup e o tempo máximo para que este backup seja efetuado.

    * *Exemplo*: Início às 2h00 UTC duração 2 horas, significa que a rotina de backup inicia às 2h00 da manhã UTC e encerra às 4h00 manhã UTC (tempo máximo de 2 horas).

* **Ícone Agendar**: Este permite ao usuário agendar o provisionamento do Banco de Dados, o valor padrão é Desabilitado (cor vermelho).

.. image:: /figuras/ucloud_databases_006b.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

  * **Ícone Desabilitado** (|icone_desb_verm|): Este ícone indica que não existe agendamento estabelecido. Isto significa que este Banco de Dados será provisionado imediatamente no ambiente do provedor de serviço de nuvem, basta o usuário clicar com o cursor do mouse no botão Criar (cor verde).
  * **Ícone Habilitado** (|icone_habil_verde|): Este ícone indica que o usuário pretende agendar uma data para que o Banco de Dados seja provisionado no ambiente do provedor de serviço de nuvem. Este processo permite escolher a melhor data para que o recurso computacional de nuvem possa iniciar sua cobrança de valores em datas pré-definidas pela empresa usuária da Plataforma uCloud. Ao alternar o ícone para habilitado (cor verde), a Plataforma uCloud permite que o usuário preencha o campo com a data desejada.
  * **Ícone Calendário** (|icone_agenda|): Basta o usuário clicar sobre o ícone do calendário para a Plataforma uCloud apresentar o pop-up, permitindo ao usuário selecionar a data desejada, conforme a tela abaixo:

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse, por engano, sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da última etapa de seleção do Banco de Dados.
* **Botão Criar**: Nesta etapa, é necessário que todos os parâmetros fundamentais para a criação da instância de Banco de Dados tenham sido informados corretamente, o usuário verifica que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros do Banco de Dados para o provedor de serviço de nuvem (via API-Rest) selecionado.
  Caso este botão não esteja habilitado (cor cinza) significa que algum parâmetro anterior foi deixado em branco, desta forma, a Plataforma uCloud não permite o provisionamento do Banco de Dados.

Criação de Banco de Dados (MySQL & GCP)
---------------------------------------

Nas telas a seguir na ilustração, será utilizada a tela com o exemplo para o provedor Google Cloud Platform (GCP), ele demonstra as pequenas diferenças de suporte a mecanismos de gerenciamento de bases de dados e seus parâmetros.

Na tela a seguir apresentada pela Plataforma uCloud, a seleção do provedor determina o conteúdo das telas seguintes.


Etapa 1 Seleção do Provedor de Serviço de Nuvem (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nas telas seguintes utilizaremos telas de exemplo para o provedor GCP que demonstra o suporte a apenas dois mecanismos de gerenciamento de bases de dados.
Importante ressaltar que, para efeito didático e apenas como exemplo, iremos seguir as etapas de criação de um Banco de Dados MySQL.
A Plataforma uCloud apresenta a tela abaixo ao usuário, a seleção do provedor determina o conteúdo das telas seguintes.

.. image:: /figuras/ucloud_databases_003.png
   :alt: Scaling Group AWS - Exemplo
   :scale: 60 %
   :align: center

----

Nesta etapa o usuário deve clicar com o cursor do mouse sobre o ícone do provedor de serviço de nuvem Google Cloud apresentado nesta tela.

Etapa 2 Seleção do Banco de Dados (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta tela permite ao usuário selecionar qual o mecanismo (“engine”) de gerenciamento de bancos de dados. Abaixo é apresentada uma tela capturada do ambiente da GCP, apenas como um exemplo didático.

.. image:: /figuras/ucloud_databases_013d.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

Nesta etapa o usuário deve clicar com o cursor do mouse sobre o ícone do **MySQL** provedor de serviço de nuvem apresentado nesta tela.

* **Botão Selecione**: Após selecionar qualquer uma das opções de bancos de dados o usuário deve clicar com o cursor do mouse no botão Selecionar para a Plataforma uCloud apresentar a tela da Etapa 3, descrito a seguir.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 3 Especificações do Banco de Dados (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa o usuário deverá informar os parâmetros iniciais do ambiente computacional GCP que dará suporte para a execução da instância de banco de dados.

.. image:: /figuras/ucloud_databases_014.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Região**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas as regiões do provedor de serviço de nuvem selecionado na Etapa 1. Importante mencionar que cada provedor possui identificação de regiões específicas, este campo reflete suas especificidades.
* **Flavor**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas as configurações de hardware (“flavor”), criadas pelo provedor de serviço de nuvem e dedicadas (especializadas) para executar instâncias de Bancos de Dados.
* **Tipo de Storage**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas as opções de tipos de discos de armazenamento (“storage”). Para mais informação consultar a documentação online da GCP (usado neste exemplo como forma didática) para entender as diferenças entre as características entre a opção SSD e HDD.
* **Tamanho do Disco**: Este campo é obrigatório ele deve ser informado como um número inteiro que define o tamanho máximo do recurso computacional de Disco de Armazenamento. Este número deve ser informado em Gigabytes. Importante ressaltar que no ambiente GCP o tamanho máximo do disco de armazenamento (tamanho do arquivo de banco de dados) está relacionado com o flavor selecionado no campo acima. O usuário deve verificar a mensagem em vermelho abaixo do campo flavor.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 4 Configurações de acesso ao Banco de Dados (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros de acesso à instância de banco de dados.

.. image:: /figuras/ucloud_databases_015.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo dois [2] e no máximo oito [8] caracteres) com o qual deseja identificar o Banco de Dados. Sugerimos utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Usuário**: Este campo é obrigatório ele deve ser preenchido com a sequência de caracteres (no mínimo um [1] e no máximo quinze [15] caracteres) que é utilizada para identificar as credenciais do usuário “Master” para o processo de login no Gerenciador Banco de Dados. Como sugestão, utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Senha**: Este campo é obrigatório, ele deve ser preenchido com a sequência de caracteres da senha do usuário. Importante ressaltar que esta sequência deve ser maior que quatro (04) caracteres alfanuméricos. Deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”. A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres e deve conter caracteres de três das seguintes categorias:

  * Letras maiúsculas e minúsculas (A a Z)
  * Números de base 10 (de 0 a 9)
  * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' <>,.? /) – Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política.

* **Confirmar Senha**: Este campo é obrigatório, ele deve ser preenchido com a mesma sequência de caracteres informados no campo anterior. Caso a sequência informada neste campo seja diferente da anterior, o botão Próximo permanece inativo.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse por engano sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 5 Especificações de Rede e Segurança (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros de Rede e de Grupo de Segurança para o acesso à infraestrutura que executa a instância de banco de dados (máquina virtual).

.. image:: /figuras/ucloud_databases_016.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Rede**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista somente com redes provisionadas na Região selecionada na Etapa 3.
* **Subnet**: Este campo é obrigatório do tipo “dropdown”, ao clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todas sub-redes (subnets) vinculadas a rede informada no campo acima.
* **Grupo de Segurança**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todos os Grupos de Segurança (Security Group) que foram provisionados para a mesma Região e Rede informados nas etapas anteriores.
* **Porta do Banco de Dados**: Este campo é obrigatório ele deve ser preenchido com a Porta TCP-IP específica para o acesso a Bancos de Dados, a Plataforma uCloud apresenta a Porta TCP-IP padrão 3306. É sugerido manter esta informação.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse, por engano, sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da primeira etapa de seleção do Banco de Dados.

Etapa 6 Parâmetro de Cópia de Segurança (MySQL & GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta etapa devem ser informados os parâmetros para definir o processo de cópia de segurança (backup) da instância de banco de dados.

.. image:: /figuras/ucloud_databases_017.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

* **Período de Retenção do Backup**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com números que representam o número de dias que a cópia de segurança (backup) permanecerá armazenada no ambiente do provedor de serviço de nuvem. Um número maior ou igual a um (01) indica que o usuário tem interesse em manter uma cópia de segurança (backup) ativo. Caso o usuário selecione “zero” (0) isto configura que o usuário não manterá nenhuma cópia de segurança (backup) do banco de dados no ambiente.
* **Janela do Backup**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta as duas opções disponíveis:

  * **Sem Preferência**: Esta opção indica que o usuário não deseja programar a cópia de backup em uma janela de tempo específica. Desta forma, a rotina de backup será efetuada na data agendada.
  * **Selecionar Janela**: Esta opção permite ao usuário determinar o horário da programação da cópia de segurança. Esta definição de data e hora, utiliza o agendamento em Tempo Universal Coordenado (UTC – Coordinated Universal Time). Quando selecionada esta opção, a Plataforma uCloud apresenta campos para o usuário definir o horário de início da rotina de backup e o tempo máximo para que este backup seja efetuado.

    * *Exemplo*: Início às 2h00 UTC duração 2 horas, significa que a rotina de backup inicia às 2h00 da manhã UTC e encerra às 4h00 manhã UTC (tempo máximo de 2 horas).

* **Ícone Agendar**: Este permite ao usuário agendar o provisionamento do Banco de Dados, o valor padrão é Desabilitado (cor vermelho).

.. image:: /figuras/ucloud_databases_006b.png
   :alt: Scaling Group AWS - Exemplo
   :align: center

----

  * **Ícone Desabilitado** (|icone_desb_verm|): Este ícone indica que não existe agendamento estabelecido. Isto significa que este Banco de Dados será provisionado imediatamente no ambiente do provedor de serviço de nuvem, basta o usuário clicar com o cursor do mouse no botão Criar (cor verde).
  * **Ícone Habilitado** (|icone_habil_verde|): Este ícone indica que o usuário pretende agendar uma data para que o Banco de Dados seja provisionado no ambiente do provedor de serviço de nuvem. Este processo permite escolher a melhor data para que o recurso computacional de nuvem possa iniciar sua cobrança de valores em datas pré-definidas pela empresa usuária da Plataforma uCloud. Ao alternar o ícone para habilitado (cor verde), a Plataforma uCloud permite que o usuário preencha o campo com a data desejada.
  * **Ícone Calendário** (|icone_agenda|): Basta o usuário clicar sobre o ícone do calendário para a Plataforma uCloud apresentar o pop-up, permitindo ao usuário selecionar a data desejada, conforme a tela abaixo:

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Banco de Dados, caso tenha clicado no cursor do mouse, por engano, sobre o botão “Criar Banco de Dados”. A Plataforma uCloud encerra a tela do Banco de Dados e retorna à tela anterior.
* **Botão Voltar**: Este botão se encontra ativo, por se tratar da primeira etapa do processo, o usuário pode retornar para a Etapa 1, seleção do provedor de serviço de nuvem.
* **Botão Próximo**: Este botão se encontra inativo, por se tratar da última etapa de seleção do Banco de Dados.
* **Botão Criar**: Nesta etapa, é necessário que todos os parâmetros fundamentais para a criação da instância de Banco de Dados tenham sido informados corretamente, o usuário verifica que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros do Banco de Dados para o provedor de serviço de nuvem (via API-Rest) selecionado.
  Caso este botão **não esteja habilitado (cor cinza)** significa que algum parâmetro anterior foi deixado em branco, desta forma, a Plataforma uCloud não permite o provisionamento do Banco de Dados.


Menu Virtual Datacenters
========================

Um Virtual Datacenters (VDC) corresponde a um agrupamento lógico de recursos computacionais de um container e que pode ser associado a um contrato. Este termo é exclusivo para o ambiente da Plataforma uCloud, e não existe nada similar em qualquer provedor de serviço de nuvem.

A representação do *Virtual Datacenter* conforme a figura abaixo, exemplifica a estrutura lógica da organização decorrente de um Virtual Datacenter. No exemplo abaixo, está referenciado o provedor de serviço Amazon AWS, mas o VDC, pode ser vinculado a qualquer provedor de serviço computacional de rede público e/ou privado.

.. image:: /figuras/ucloud_virtualdatacenter_conceito.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 70 %
   :align: center

----

Um VDC contém uma segmentação (sub-grupo) virtual de recursos computacionais específicos de um provedor de serviço de nuvem, pode ser utilizado para representar:

* um departamento;
* uma subsidiária;
* um grupo de usuários;
* uma iniciativa.

Este conceito de agrupamento de recursos computacionais apoia o pilar de Governança Financeira das empresas, de forma que restringe os usuários de consumir recursos computacionais diferentes dos que foram disponibilizados a eles e estão disponíveis no Virtual Datacenter.

A segmentação de recursos computacionais, pode retirar da lista disponível para o usuário, os recursos computacionais mais caros, se necessário, desta forma, um usuário não pode consumir um recurso computacional de alto custo (ex.: máquinas virtuais com 12 CPUs e 120 Giga RAM). Um provedor de serviço de nuvem pode possuir uma relação muito grande de Templates (configuração de hardware) e de tipos de sistemas operacionais (flavors), de regiões de presença global, de tipos de armazenamento (storage), entre outros. Todos estes recursos computacionais são passíveis de serem retirados da lista para o usuário. Importante ressaltar que o recurso computacional não é excluído do ambiente do provedor de serviço de nuvem, o recurso computacional tem a sua apresentação "inibida" ao usuário na interface da Plataforma uCloud.

O Virtual Datacenter (VDC) é utilizado em vários pontos, telas, formulários na Plataforma uCloud, a seleção de um VDC por parte do usuário, restringe a lista de recursos computacionais apresentados. Caso o usuário não possua acesso a um recurso computacional específico, este pode ser adicionado (ou removido) de forma muito fácil e rápida, e o efeito desta alteração é imediato na Plataforma uCloud.

Quando o usuário acessa a opção de menu Virtual Datacenter, a Plataforma uCloud apresenta uma listagem de todos os VDCs provisionados no ambiente, conforme a tela abaixo:

.. image:: /figuras/ucloud_virtualdatacenter001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Gerenciando Virtual Datacenters
-------------------------------

Quando o usuário clicar com o cursor do mouse em uma das linhas da lista de VDCs, a Plataforma uCloud apresenta uma tela com diversas seções (cards), segue abaixo a descrição de cada seção:

.. image:: /figuras/ucloud_virtualdatacenter002.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

A seguir cada seção está descrita de forma individual, para detalhar suas informações e funcionalidades.

* **Botão Excluir Virtual Datacenter** |botao_exclui_VDC|: O usuário deve clicar com o cursor do mouse sobre este botão quando for necessário remover um Virtual Datacenter previamente provisionado. Importante ressaltar que o conceito de VDC existe somente dentro da Plataforma uCloud e todo recurso computacional de nuvem, existe dentro do ambiente do provedor de serviço. Desta forma, a exclusão de um Virtual Datacenter não expurga (remove) qualquer máquina virtual existente. Quando clicar sobre este botão a Plataforma uCloud apresenta uma tela para o usuário possa confirmar a remoção.

* **Seção Geral**: Esta seção apresenta as características gerais do Virtual Datacenter. Nesta seção é possível alterar a lista dos recursos computacionais que serão visualizados pelo usuário, quando selecionado este VDC.

  * **Nome**: Este campo apresenta o nome do VDC com o qual este foi identificado no momento do seu provisionamento na Plataforma uCloud.
  * **Container**: Este campo apresenta o nome do provedor de serviço de nuvem, ao qual este VDC está vinculado. A vinculação de um VDC a um provedor de serviço de nuvem é única e exclusiva.
  * **Ícone de Desconectar** |icone_desconecta|: Este ícone permite ao usuário desconectar (unplug) o Virtual Datacenter do provedor de serviço de nuvem. O efeito desta ação causa impacto em todas as máquinas virtuais vinculadas a este VDC na Plataforma uCloud. Importante ressaltar que esta ação não remove (delete) a máquina virtual do ambiente do provedor de serviço de nuvem. Esta ação remove o Virtual Datacenter do inventário da base de dados da Plataforma uCloud, portanto, não mais será listado em qualquer tela ou formulário. Quando o usuário clicar com o cursor do mouse sobre este ícone a Plataforma uCloud apresenta uma tela para o usuário possa confirmar a ação.
  * **Ícone de Edição Ativo (|icone_edita_on|)**: Através deste ícone, o usuário pode alterar a lista de recursos computacionais específicos do VDC. Este procedimento será coberto no item Editando um Virtual Datacenter.
  * **Max.Máquinas Virtuais**: Este campo permite para a empresa um possa ter controle de Governança de Custos, pois pode definir que este VDC fique limitado a um número específico de máquinas virtuais, de forma que a Plataforma uCloud poderá não efetuar o provisionamento de uma nova máquina virtual quando este limite for alcançado. O valor padrão (default) é ‘99999’ que praticamente significa ‘ilimitado’.

    * **Ícone de Edição Ativo** |icone_edita_on|: Através deste ícone, o usuário pode alterar o valor informado no campo da quantidade máxima de máquinas virtuais do VDC. Após clicar com o cursor do mouse no ícone de edição, a Plataforma uCloud permite ao usuário informar um número inteiro (1 – 99.999) que estabelece o limite máximo da quantidade de máquinas virtuais vinculadas a este VDC.
    * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo é alterada permanentemente nas bases de dados da Plataforma uCloud.
    * **Ícone de Cancelamento** |icone_cancela_vermelho|: Caso o usuário tenha clicado sobre o ícone de edição por engano, ou não deseja que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho, para cancelar as alterações e o conteúdo do campo retorna para os valores iniciais, antes de qualquer preenchimento ou alteração.

* **Seção Regiões**: Esta seção apresenta somente as regiões globais, do provedor de serviço de nuvem, que foram definidas para ficar disponíveis aos usuários quando estes selecionarem o VDC.

.. image:: /figuras/ucloud_virtualdatacenter004.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Seção Redes**: Esta seção apresenta somente as Redes TCP-IP (e subnets) do provedor de serviço de nuvem, que foram definidas para ficar disponíveis aos usuários quando estes selecionarem o VDC.

* **Seção Templates**: Esta seção apresenta somente os templates do provedor de serviço de nuvem, que foram definidos para ficar disponíveis aos usuários quando estes selecionarem o VDC.

* **Seção Flavors**: Esta seção apresenta somente os flavors do provedor de serviço de nuvem, inicialmente definidos e disponíveis aos usuários quando da seleção do VDC.

* **Seção Storages**: Esta seção apresenta somente opções de armazenamento (storage) do provedor de serviço de nuvem, anteriormente definidos e disponíveis aos usuários quando estes selecionarem o VDC.

* **Seção Grupos de Segurança**: Esta seção apresenta somente os Grupos de Segurança do provedor de serviço de nuvem, anteriormente definidos e disponíveis aos usuários quando estes selecionarem o VDC.

* **Seção Catálogo**: Esta seção apresenta somente as Ofertas do Catálogo de Serviços que o usuário Administrador do Contrato provisionou e selecionou para ficarem disponíveis aos usuários quando estes selecionarem o VDC.

* **Seção Máquinas Virtuais**: Esta seção apresenta a lista de todas as máquinas virtuais que foram criadas ao selecionar o VDC durante o processo de provisionamento de uma máquina virtual.

  * **Nome**: Nesta coluna será apresentado o nome da máquina virtual informado no momento da sua criação no console do provedor de serviço de nuvem, ou quando configurado através do uCloud. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de máquinas virtuais de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **Usuário**: Esta coluna apresenta as credenciais do usuário registrado, em uma sessão na Plataforma uCloud, o qual foi o responsável pelo provisionamento da máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **IP Privado**: Esta coluna apresenta o endereço TCP-IP vinculado a esta máquina virtual no momento de sua criação. Importante ressaltar que este endereçamento TCP-IP pertence ao ambiente de rede privada do provedor de serviço de nuvem (recebe do servidor DHCP interno do provedor) e, este endereço, pode mudar quando a máquina virtual for reiniciada (reboot). Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de endereços TCP-IP de forma crescente ou decrescente.
  * **IP Público**: Esta coluna pode estar em ‘branco’, pois nesta coluna é apresentado o endereço TCP-IP Público que foi vinculado a esta máquina virtual em um momento posterior ao provisionamento da máquina virtual. O Endereço TCP-IP Público, é um endereço fixo e pode incorrer em custos mensais para sua manutenção e vinculação a uma máquina virtual provisionada. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **Memória**: Nesta coluna é apresentado o número da quantidade de memória RAM configurada nesta máquina virtual, expressa sempre em Gigabytes. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de máquinas virtuais com base no tamanho da memória de forma crescente ou decrescente.
  * **CPUs**: Nesta coluna é apresentado o número da quantidade de CPU(s) configurada nesta máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de máquinas virtuais com base na quantidade de CPU(s), de forma crescente ou decrescente.
  * **Status**: Esta coluna apresenta o status corrente da máquina virtual. Importante ressaltar que status é obtido do provedor de serviço de nuvem, pois a máquina virtual está instalada e sendo executada na infraestrutura do provedor de serviço de nuvem. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica o status da lista de máquinas virtuais de forma alfabética crescente (a – z) ou decrescente (z – a). A Plataforma uCloud apresenta os seguintes status:

    * **Running**: Status indica que a máquina virtual está em funcionamento normal.
    * **Stopped**: Status indica que a máquina virtual está parada.
    * **Suspended**: Este status indica que a máquina virtual está em um estado suspenso, demanda um tempo de inicialização (boot) mais rápido que o estado parado (stopped).
    * **Unrecognized**: Este status pode ser apresentado, pois se refere a um estado, temporário, onde momentaneamente não foi possível distinguir se a máquina está parada ou rodando (falha de comunicação entre a Plataforma uCloud e o console do provedor de serviço de nuvem pública).
    * **Deallocated**: Este status é particular da nuvem Azure, e se refere a uma máquina virtual que se encontra parada, e que não está sendo cobrada. Este estado faz a liberação de alguns recursos e seu tempo para inicialização (boot) será maior. Para maiores detalhes, consultar material de documentação do Azure.
    * **Orphan**: Este status somente será apresentado quando uma máquina não é encontrada no provedor de serviço de nuvem ou no ambiente de virtualização do datacenter privado (hypervisor).

  * **Ações Ícone de Desconectar** |icone_desconecta|: Este ícone permite ao usuário desconectar (unplug) a máquina virtual do Virtual Datacenter. Importante ressaltar que esta ação não remove (delete) a máquina virtual do ambiente do provedor de serviço de nuvem. Quando o usuário clicar com o cursor do mouse sobre este ícone a Plataforma uCloud desconecta a máquina virtual do VDC de forma imediata, apresenta uma mensagem pop-up, no canto superior direito da tela a qual solicita confirmar a ação:

.. image:: /figuras/ucloud_virtualdatacenter005.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Editando um Virtual Datacenter
------------------------------

Esta ação permite ao usuário alterar o conjunto de recursos computacionais disponíveis no VDCs, de forma que a Plataforma uCloud apresenta as características corretas onde este VDC for necessário.

* **Seção Geral**: Esta seção apresenta as características gerais do Virtual Datacenter. Nesta seção é possível alterar a lista de recursos computacionais que serão visualizados pelo usuário, ao selecionar este VDC.

.. image:: /figuras/ucloud_virtualdatacenter003.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * **Ícone de Edição Ativo** |icone_edita_vdc|: Através deste ícone, o usuário pode alterar o conjunto de recursos computacionais vinculados a este VDC. Importante mencionar que os recursos apresentados, são exclusivos do provedor de serviço de nuvem ao qual este VDC está vinculado. Portanto, a tela apresentada abaixo pode se adaptar a características únicas de cada provedor de serviço de nuvem (público e/ou privado). Ao clicar com o cursor do mouse sobre o ícone, a Plataforma uCloud apresenta a seguinte tela para o usuário (o exemplo usa o ambiente da Amazon AWS):

  * **Ícone para Ampliar a Seleção** |icone_amplia_vdc|: Para que a Plataforma uCloud possa apresentar a lista de recursos computacionais respectivos de cada seção abaixo, o usuário deve clicar com o cursor do mouse sobre o ícone de cada seção desejada.
    Quando o usuário amplia a seção desejada, os procedimentos para incluir (ou excluir) são os mesmos para qualquer uma das seções a seguir, portanto as informações usam como exemplo a seção Regiões, pois os processos são idênticos.

  * **Coluna Acionável**: Cada linha está representada por um caixa selecionável (tipo “check box”). Quando o usuário seleciona uma linha, ou várias, a Plataforma uCloud apresenta o ícone com status marcado, e um número ao lado do nome da seção com a quantidade selecionada de linhas referente a seção. Veja o exemplo abaixo:

.. image:: /figuras/ucloud_virtualdatacenter006.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * Se o usuário deseja selecionar todas as linhas da seção de uma única vez, este deve clicar com o cursor do mouse no ícone acionável que fica localizado na linha do cabeçalho da seção. Desta forma, a Plataforma uCloud preenche todos os ícones de forma imediata e atualiza o número de linhas selecionadas no título da seção, de acordo com a quantidade de opções da seção. Veja o exemplo abaixo:

.. image:: /figuras/ucloud_virtualdatacenter007.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

É necessário repetir estes procedimentos para cada uma das seções, até que a relação de recursos computacionais de nuvem, de cada seção, atinja a quantidade e características ideais para o seu uso na Plataforma uCloud.

* **Regiões**: Esta seção apresenta todas as regiões globais disponíveis no provedor de serviço de nuvem, após a seleção somente as regiões que foram definidas permanecem disponíveis aos usuários, quando o mesmo selecionar o VDC.
* **Templates**: Esta seção apresenta todos os templates disponíveis no provedor de serviço de nuvem, após a seleção somente as regiões que foram definidas permanecem disponíveis aos usuários, no momento de selecionar o VDC.
* **Redes**: Esta seção apresenta todas as Redes existentes, bem como, as que foram provisionadas no provedor de serviço de nuvem. Após a seleção somente as Redes que foram definidas ficarão disponíveis aos usuários, ao selecionar o VDC.
* **Storage**: Esta seção apresenta todos os tipos de storages disponíveis no provedor de serviço de nuvem, após a seleção somente os storages que foram definidos ficarão disponíveis para os usuários quando estes selecionarem o VDC.
* **Flavors**: Esta seção apresenta todos os flavors disponíveis no provedor de serviço de nuvem, após a seleção somente os flavors previamente definidos permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **Máquinas Virtuais**: Esta seção, quando expandida, apresenta a lista de todas as máquinas virtuais que foram criadas e selecionado o provedor de serviço de nuvem ao qual o VDC está vinculado. O usuário pode incluir, ou remover, máquinas virtuais vinculadas ao VDC. Este número será considerado no parâmetro Max.Máquinas Virtuais, que permite definir que este VDC tenha um número específico de máquinas virtuais.
* **Grupos de Segurança**: Esta seção, quando expandida, apresenta a lista de todos os Grupos de Segurança foram provisionados e disponíveis no provedor de serviço de nuvem ao qual o VDC está vinculado. O usuário pode incluir, ou remover, Grupos de Segurança vinculadas ao VDC.
* **Catálogo**: Esta seção, quando expandida, apresenta a lista de todas as Ofertas do Catálogo de Serviços que o usuário Administrador do Contrato provisionou e selecionou para ficar visível para os usuários ao quais o VDC está vinculado.

Importante ressaltar que toda alteração, seja de inclusão ou de remoção de recursos computacionais, reflete de forma imediata na Plataforma uCloud. Portanto, caso um usuário não seja capaz de visualizar um recurso computacional de nuvem (ex.: um template ou um flavor), o usuário com perfil de acesso correto, pode adicionar o recurso computacional e este recurso será imediatamente visualizado por todos os outros usuários

Criando um Virtual Datacenter
-----------------------------

Acessar o menu Virtual Datacenters, basta o usuário clicar sobre o botão “Criar Virtual Datacenter”, conforme a figura abaixo:

.. image:: /figuras/ucloud_virtualdatacenter001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

O processo inicia quando a Plataforma uCloud apresenta a primeira tela “Criar Virtual Datacenter”:

.. image:: /figuras/ucloud_virtualdatacenter008a.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Container**: Este campo é obrigatório do tipo “dropdown”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta uma lista com todos os provedores de serviço de nuvem configurados no ambiente da Plataforma uCloud, neste momento, basta o usuário selecionar o provedor desejado. *Importante ressaltar que o termo ‘container’ significa nome do provedor de serviço computacional de nuvem (público e/ou privado) previamente configurado no ambiente do uCloud. Esta seleção determina como a Plataforma uCloud apresenta as próximas telas*.

  Assim que o usuário selecionar o provedor de serviço de nuvem (container) a Plataforma uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_virtualdatacenter008b.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres, no máximo 15 caracteres) com o qual deseja identificar este Virtual Datacenter. Sugestão: utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (*ASCII Extendido)*.

* **Ícone para Ampliar a Seleção** |icone_amplia_vdc|: Para que a Plataforma uCloud possa apresentar a lista de recursos computacionais respectivos de cada seção, o usuário deve clicar com o cursor do mouse sobre o ícone de cada seção desejada.
  Quando o usuário amplia a seção desejada, os procedimentos para incluir (ou excluir) são os mesmos para qualquer uma das seções abaixo, portanto os esclarecimentos a seguir usam como exemplo a seção de Regiões, os processos são idênticos.

* **Coluna Acionável**: Cada linha está representada por um caixa selecionável (tipo “check box”). Quando o usuário seleciona uma linha, ou várias, a Plataforma uCloud apresenta o ícone com status marcado, e um número ao lado do nome da seção com a quantidade selecionada de linhas referente a seção. Veja o exemplo abaixo:

.. image:: /figuras/ucloud_virtualdatacenter006.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * Se o usuário deseja selecionar todas as linhas da seção de uma única vez, este deve clicar com o cursor do mouse no ícone acionável que fica localizado na linha do cabeçalho da seção. Desta forma, a Plataforma uCloud preenche todos os ícones de forma imediata e atualiza o número de linhas selecionadas no título da seção, de acordo com a quantidade de opções da seção. Veja o exemplo abaixo:

.. image:: /figuras/ucloud_virtualdatacenter007.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

O usuário deve repetir estes procedimentos para cada uma das seções abaixo, até que a relação de recursos computacionais de nuvem de cada seção abaixo, fique na quantidade e características ideais para o seu uso na Plataforma uCloud.

* **Regiões**: Esta seção apresenta todas as Regiões globais disponíveis no provedor de serviço de nuvem, após a seleção somente as regiões previamente definidas permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **Templates**: Esta seção apresenta todos os Templates disponíveis no provedor de serviço de nuvem, após a seleção somente os templates previamente definidos permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **Redes**: Esta seção apresenta todas as Redes existentes, bem como as que foram provisionadas, no provedor de serviço de nuvem. Após a seleção somente as Redes previamente definidas permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **Storage**: Esta seção apresenta todos os tipos de Storages disponíveis no provedor de serviço de nuvem, após a seleção somente os storages previamente definidos permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **Flavors**: Esta seção apresenta todos os Flavors disponíveis no provedor de serviço de nuvem, após a seleção somente os flavors previamente definidos permanecem disponíveis aos usuários, quando estes selecionarem o VDC.

Importante ressaltar que toda alteração, seja de inclusão ou de remoção, de recursos computacionais reflete de forma imediata na Plataforma uCloud. Caso um usuário não seja capaz de visualizar um recurso computacional de nuvem (por exemplo: um template ou um flavor), ao proceder a adição do recurso computacional, este recurso será imediatamente visualizado por todos os outros usuários.

.. .. raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/embed/_uBTkmLgNJg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Menu Financeiro
===============

No início deste documento estão descritos os cinco pontos de atuação da Plataforma uCloud, esta seção é dedicada ao ponto “Financeiro”. É necessário ressaltar que a Plataforma uCloud não cria ou gera valores de recursos computacionais, estes valores são gerados nos provedores de nuvem pública.

A Plataforma uCloud extrai (ao fazer download) do arquivo de billing (faturamento) destes provedores de nuvem pública os valores gerados pelos recursos computacionais, em seguida, adiciona estas informações em suas bases de dados internas. Para que, posteriormente, de acordo com os critérios comerciais do contrato possam ser aplicados, estes custos são calculados e convertidos para moeda corrente no Brasil.

Desta forma, o usuário permanece informado da evolução dos custos e poderá acompanhar se estes custos se encontram dentro dos critérios da governança financeira da organização. Geralmente, estes custos são apresentados em arquivos texto não estruturados (Comma-Separated Values – CSV) gerados a cada período (em média de 8 horas), a Plataforma uCloud adiciona a informação deste arquivo CSV em suas bases de dados internas, com o objetivo de agilizar e simplificar a apresentação destes valores ao usuário.

Através do menu Financeiro, o usuário pode ter acesso a diversas formas de visualização da evolução dos custos referentes ao consumo dos recursos computacionais de serviços de rede pública.

A Plataforma uCloud possui uma interface de visualização destes custos de forma pronta e finalizada. Não é necessário ao usuário criar ou personalizar, qualquer uma das visualizações existentes na Plataforma uCloud. O conceito de relatório que necessita ser enviado para impressão em papel inexiste. Todas as visualizações são apresentadas de forma dinâmica na tela da Plataforma uCloud.

Algumas informações presentes nas telas dos relatórios, podem ser exportadas para um arquivo texto não formatado separado por vírgulas (.CSV - Comma Separated Values) e pode ser utilizado como base de informações para qualquer software de planilha de cálculo (Excel, Google Sheet, entre outras).

O menu Financeiro é visualizado por qualquer perfil de usuário, o ambiente permite que este usuário verifique e consulte os valores monetários referente ao consumo dos seus recursos utilizados nos recursos computacionais de nuvem pública. A seguir são apresentados os tipos de perfil dos diferentes usuários:

* **Usuário Perfil Normal**: este perfil de usuário visualiza o consumo, o seu próprio e o do seu contrato;
* **Usuário Perfil Administrador de Contrato**: este perfil de usuário visualiza as informações de todos os grupos vinculados ao contrato e de todos os usuários vinculados ao contrato.
* **Usuário Perfil Administrador de Grupo**: este perfil de usuário visualiza as informações do(s) grupo(s) aos quais está vinculado e de todos os usuários vinculados ao grupo.

Outras informações sobre o perfil de usuários, ver no item Menu Administração / Usuários.

A Plataforma uCloud é desenvolvida para atender tanto um ambiente corporativo quanto um ambiente do Governo Federal, Estadual ou Municipal brasileiro, ambiente que possui características próprias de moeda e tarifação.

Empresas Privadas
-----------------

Para o ambiente corporativo, a Plataforma uCloud efetua o *download* das linhas do arquivo de *billing* (também conhecido como *bucket*) do provedor de serviço de nuvem. Este arquivo é um arquivo texto *ASCII* com dados separados por vírgula (arquivo .CSV).

A Plataforma uCloud efetua a sincronização do conteúdo deste arquivo em suas bases de dados internar e calcula conversão dos valores referentes ao período, utilizando os valores informados nos seguintes campos do Contrato:
* *Taxa de faturamento*
* *Moeda*
* *Tipo de cotação* (fixa ou variável)
* *Dia de cotação da moeda* (válido somente para cotação variável a Plataforma uCloud obtém o valor da PTAX do site do Banco Central do Brasil).

Basicamente, quase todos os provedores de serviço de nuvem pública, armazenam seus valores referente ao consumo de recursos computacionais em dólares norte-americanos (US$) e a forma que a Plataforma uCloud efetuar a conversão para Real Brasileiro é:

+--------------------+--------------------------+---+------------------+---+-------------------+
|**Valor Reais (R$)**|Valor US$ Total de Consumo| x |Valor [Fixo] Dólar| x |Taxa de Faturamento|
+--------------------+--------------------------+---+------------------+---+-------------------+
|**Valor Reais (R$)**|Valor US$ Total de Consumo| x |Valor [Dia] PTAX  | x |Taxa de Faturamento|
+--------------------+--------------------------+---+------------------+---+-------------------+

Recentemente, algumas operações brasileiras de provedores de serviço de nuvem estão apresentando os valores de consumo dos recursos computacionais já convertidos para a moeda Real, a conversão utiliza um valor 1 (hum) para a taxa de conversão de Dólar <> Real estipulado pelo provedor de serviço de nuvem. Desta forma, as fórmulas se comportam de forma diferente:

+--------------------+-------------------------+---+-----------------+---+-------------------+
|**Valor Reais (R$)**|Valor R$ Total do Consumo| x |Valor [Fixo] 1,00| x |Taxa de Faturamento|
+--------------------+-------------------------+---+-----------------+---+-------------------+

.. note:: Importante ressaltar que para o cenário de provedores que armazeman seus valores em Reais, o usuário Administrador do Contrato deve alterar o campo valor da **Moeda** para 1,00 e **Tipo de Cotação** FIXA.

Quando o usuário possui a Plataforma uCloud conectada a um ambiente de Data Center Privado (on-premises), o valor por hora de cada tipo de recurso computacional (CPU, Memória, disco, entre outros) deve ser informado individualmente na Seção **Preço dos Recursos** no  contrato. A própria empresa deverá calcular estes valores e informá-los na Plataforma uCloud. A Plataforma uCloud calcula o consumo mensal apenas dos recursos computacionais que possuem seu valor informado.

+--------------------+-------------------------+---+-------------------+
|**Valor Reais (R$)**|Valor R$ Total de Consumo| x |Taxa de Faturamento|
+--------------------+-------------------------+---+-------------------+

.. attention:: O valor referente às taxas de impostos para emissão de nota fiscal no território brasileiro não é apresentado por nenhum provedor e, também, não é calculado pela Plataforma uCloud. Os valores de taxas e impostos são calculados pelo emissor do documento final da Nota Fiscal, a Plataforma uCloud não é uma plataforma de emissão de documento fiscais.

Empresas Públicas (USN)
-----------------------

Devido a constante variação do valor da taxa de câmbio (Dólar <> Real), o Governo Federal brasileiro criou uma formatação inteligente e facilitada para controlar seus limites orçamentários para computação em nuvem pública, de forma a nunca descumprir os limites da Lei de Diretrizes Orçamentárias (LDO), com a finalidade de atender em sua totalidade a Lei nr. 8.666/93, de 21 de junho de 1993, para a contratação do serviço de que institui o pregão - que é uma modalidade de licitação aplicável à aquisição de bens e serviços comuns - a base legal aplicada para as contratações da Administração Pública Federal, as quais devem ser seguidas a rigor.

Cabe destacar que, nessas leis são estabelecidos os critérios de classificação das propostas para a determinação do ganhador do processo licitatório e que cada provedor de serviço em nuvem oferece serviços e forma de comercialização distintos, o que faz com que seja um desafio a ser discutido, na definição do modelo, o critério a ser utilizado para determinar a proposta mais vantajosa para a Administração Pública Federal [1]_.

Esta abordagem única e especial, permite a qualquer órgão de Governo brasileiro (Federal, Estadual ou Municipal) consumir recursos de computação em nuvem pública permitindo que o valor dos serviços em Unidade de Serviço em Nuvem (USN) seja calculado utilizando o preço em dólar comercial do dia do pregão, fixo ao longo do contrato, acrescido dos percentuais de impostos, contribuições, tributos, lucro e custos da empresa dividido pelo valor da USN cotada no pregão.

A definição de valores dos recursos computacionais de nuvem, pode ser individualizado e constar no corpo de cada edital (de cada órgão interessado na contratação de serviços de processamento de nuvem), este documento relacionado ao edital deve vir acompanhado de um Anexo, no qual o órgão define os valores específicos.

Os preços dos recursos em USN são definidos através das tags, na seção **Preço dos Recursos** do Contrato na Plataforma uCloud, a plataforma possibilita adicionar / configurar tags que identificam cada recurso listado no anexo, com o respectivo valor em USN.

Para calcular o custo do recurso em USN, é feita a somatória da quantidade utilizada do recurso pelo preço que foi definido; no caso de recursos que são máquinas virtuais, o preço é multiplicado pela quantidade de CPU, ou pela quantidade de memória em GB. O que define será por CPU ou por memória é a tag aplicada aos recursos. Se não houver tag do tipo USN no recurso, o cálculo não é feito.

Em casos específicos de recursos sem *TAG* assume-se o valor que vem informado no arquivo de Billing (.CSV) do provedor de serviço de nuvem pública.

Neste ambiente, a Plataforma uCloud após baixar o arquivo de billing do provedor de serviço de nuvem (arquivo .CSV) efetua a conversão dos valores referentes ao período, utilizando os valores informados nos seguintes campos do Contrato:

* *Preço de Recurso em USN por Hora*
* *Taxa de faturamento*
* *Tipo de cotação* (fixa/variável)
* *Dia de cotação da moeda* (válido somente para cotação variável a Plataforma uCloud obtém o valor da PTAX do site do Banco Central do Brasil)

Portanto, a fórmula para apresentação dos valores dos recursos computacionais em nuvem pública expressos em USN é bem diferente:

+-----------------------+-------------------+----+-------------------+----+-------------+----+----------------------+
|| **Valor Reais (R$)** || Valor do Recurso ||   || Somatória Mensal ||   || Valor US$  ||   || Taxa de Faturamento |
||    Total Mensal      || em USN/h         || x || do Consumo USN   || x || [Dia] PTAX || x ||                     |
+-----------------------+-------------------+----+-------------------+----+-------------+----+----------------------+
|| **Valor Reais (R$)** || Valor do Recurso ||   || Somatória Mensal ||   || Valor US$  ||   || Taxa de Faturamento |
||    Total Mensal      || em USN/h         || x || do Consumo USN   || x || [Fixa]     || x ||                     |
+-----------------------+-------------------+----+-------------------+----+-------------+----+----------------------+


.. [1] Informações gerais obtidas da monografia: *Desafios da contratação de serviços em nuvem no setor público*: critérios para a contratação no Senado Federal (Rubens Vasconcellos Terra Neto – 2019) - Instituto Legislativo Brasileiro ILB – Senado Federal Brasileiro. https://www2.senado.leg.br/bdsf/handle/id/569196.


Menu Financeiro (Ambiente Corporativo)
======================================

Antes de iniciarmos a apresentação dos relatórios é importante esclarecer o conceito de Contrato e os benefícios para as empresas quando adotam a Plataforma uCloud para melhorar o controle e monitoração da Governança de Custos e de Recursos Computacionais.

O Contrato é o ponto principal onde a organização usuária da Plataforma uCloud estabelece a forma como gerencia os aspectos comerciais, os limites financeiros (ou dos recursos computacionais), define seus valores para recursos computacionais de forma individualizada (isto é válido somente para uma nuvem privada), vincula os grupos e os usuários.

No contrato se estabelece a forma da conversão da moeda estrangeira para a moeda local (e o valor de conversão é fixo ou variável) e as taxas de impostos aplicadas aos custos do contrato.

Entre vários aspectos do Contrato, na Seção Regras de Faturamento o Administrador do Contrato pode personalizar as regras de como os valores dos custos do contrato podem ser convertidos para moeda local, também personaliza, se para o cálculo de conversão de moeda aplicará no fator de conversão: um valor fixo ou um valor variável. Para o valor variável, a Plataforma uCloud está configurada para obter a taxa do valor de conversão diretamente do site do Banco Central do Brasil, local onde pode extrair o valor da taxa PTAX referente ao dia que está informado no Contrato.

No Contrato o usuário seleciona e define em qual a moeda os valores de todos os Relatórios Financeiros serão apresentados.

.. note:: Importante mencionar que todas as telas dos relatórios apresentados neste documento, os valores estão sendo convertidos para Real (R$).

Quando o usuário acessar o Menu Financeiro, a Plataforma uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_menu_financeiro001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

A Plataforma uCloud apresenta relatórios com base em dois conceitos financeiros diferentes:

* **Painéis Baseados em Consumo**: Este conjunto de relatórios em tela (*dashboards*) se referem aos valores acumulados dos recursos computacionais consumidos/utilizados no mês corrente até o dia corrente ou até o último período (ou janela) de processamento dos valores pelo provedor.

  O termo *janela* se refere ao período que o provedor efetua a gravação dos valores dos recursos computacionais no arquivo de Bucket. O tempo médio desta janela de tempo está por volta de doze (12) horas.

  Isto significa que poderão haver discrepâncias de apresentação de valores caso os relatórios forem consultados, antes ou depois, desta janela de processamento.

.. note:: Importante ressaltar que o provedor não informa (ou deixa público) de qualquer forma, a hora inicial e hora final de sua *janela* de processamento de valores, portanto a Plataforma uCloud não poderá ser responsabilizada em caso de visualização de valores que possam apresentar diferenças, mesmo que consultados dentro do mesmo dia.

* **Painéis Baseados em Fatura**: Este conjunto de relatórios em tela (dashboards) apresentam o valor total de consumo dos recursos computacionais do provedor de serviço de nuvem (público /ou privado) apenas do período ao mês anterior do mês corrente. Todos os valores de consumo de recursos computacionais de nuvem (do mês anterior) serão contabilizadas e apresentados nestes relatórios.

  Este custo se refere somente aos valores acumulados dos recursos computacionais consumidos no mês anterior ao faturamento, cuja respectiva data de faturamento será o dia inicial do mês subsequente ao consumo. Por exemplo, um contrato que tem data de faturamento com vencimento no dia 8, a fatura do mês de agosto será no dia 08/08 e fará referência aos valores consumidos/utilizados durante todo o mês anterior a esta data (no exemplo acima, do dia 08 do mês 07 (julho) ao dia 07 do mês 08, agosto)

  Este conceito é o mesmo aplicado aos valores das contas de serviços de concessionárias de serviços, que cobra os valores de serviços fornecidos no mês anterior.

  Para ilustrar um cenário, caso o campo “Dia da Fatura” esteja preenchido com o dia primeiro do mês (1), o período do faturamento inicia às 0 horas, 0 minutos e 0 segundos do dia primeiro do mês e encerra às 23 horas, 59 minutos e 59 segundos do dia 30/31 do mês anterior.

.. note:: Importante ressaltar que a Plataforma uCloud estabelece o período do **mês do faturamento** com a informação do campo “Dia da Fatura” na seção *Regras de Faturamento do Contrato*.


Painéis Baseados em Consumo
---------------------------

Como mencionado, este custo se refere aos valores acumulados do consumo dos recursos computacionais no mês corrente até o dia corrente ou até a última ‘janela’ de processamento dos valores pelo provedor.

Relatório Histórico de Serviço
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este relatório permite ao administrador de custos acompanhar a evolução (mensal, semanal ou diária) dos custos de cada PRODUCT NAME registrado no provedor de serviço denuvem pública. Estes custos são separados em custos com e sem etiquetas (*tags*).

O recurso de etiquetas (*tag*) é a forma mais usual e a forma indicada pelo provedor de serviço de nuvem pública para que as empresas possam aplicar alguma identificação aos custos recorrentes desua infraestutura de nuvem pública. Cada provedores possuem suas  características específicas de quais serviços ou produtos **não são passíveis (não é permitido)** aplicar etiquetas (*tags*), em utras palavras não seráo todos seus serviços e produtos que podem receber uma etiqueta (*tag*).

A característica de *não permitir vincular etiquetas (tags)* em todos seus produtos pode levar às empresas a um erro conceitual para a aplicação e distribuição de custos por departamentos, centros de custos, projetos ou qualquer outra aplicação para as etiquetas (*tags*).

A experiência acumulada da Equipe de Desenvolvimento **Ustore**, acompanhada de contatos com os provedores de serviço de nuvem pública, a correta identificação dos custos **que não permitem atribuição de etiquetas** em cada provedor.

Portanto, a Plataforma uCloud irá apresentar, discriminar e segregar a somatória dos valores de cada *Product Name* dos provedores de serviço de nuvem pública de forma que o administrador de custo das empresas possa identificar corretamente os totais com e sem etiquetas (*tags*).

Em uma abordagem de trabalho de FinOps tudo começa por identificar quais são os recursos com mais consumo. Neste caso o menu histórico de serviços o cliente poderá visualizar a listagem dos recursos que mais são consumidos em sua fatura. Eles são agrupados por ProductName e por Product Family.

Ao selecionar a opção do menu HISTÓRICO DE SERVIÇO será solicitado que escolha um CONTRATO, tipo de INTERVALO e o PERÍODO, através desse relatório é possível analisar os custos de forma detalhada conforme apresentado nas imagens abaixo.

Quando selecionado este relatório, a Plataforma uCloud apresenta a tela abaixo, onde o usuário deve informar ou selecionar apenas um único contrato:

.. image:: /figuras/ucloud_menu_financeiro002.png
   :alt: Menu Financeiro - Histórico de Serviço
   :scale: 60 %
   :align: center

----

* **Contrato**: A Plataforma uCloud irá apresentar uma lista com somente os contratos aos quais o usuário está vinculado, o usuário deve informar ou selecionar apenas um contrato por vez. Ao selecionar o contrato desejado a Platafoam uCloud irá apresentar a tela abaixo:

.. image:: /figuras/ucloud_menu_financeiro002b.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Abaixo descrevemos os campos para apresentação deste relatório:

* **Intervalo**: Este campo é do tipo "dropdown" e o usuário pode selecionar o período ideal para avaliar os dados de consumo de sem ambiente. Quando fazemos uma análise comparando mensalmente o cliente poderá entender como a sua fatura evolui ao longo do tempo de acordo com o faturamento do provedor. Quando clicar com o cursor do mouse a Plataforma uCloud apresenta as opções:
  
  * **MENSAL**: Quando selecionada a análise mensal o cliente poderá entender como a sua fatura evolui ao longo do tempo de acordo com o faturamento do provedor. Esta visão permite entender o consumo dos produtos de acordo com a fatura do cliente, no exemplo abaixo iremos selecionar o campo PERÍODO então MENSAL, dessa forma o calendário com os meses ficará disponível para seleção. É possível escolher mínimo 1 mês e máximo todos os meses do ano. Para exemplificar, selecionamos os últimos 3 meses, conforme imagem abaixo.

.. image:: /figuras/ucloud_menu_financeiro002c.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * **SEMANAL**: Este filtro permite ter uma visão mais granular do consumo, podendo entender e identificar picos de consumos em semanas aos longos dos meses. Neste caso pode trazer indicativos de aplicações ou comportamento que geram picos de consumo em uma determinada semana e não em outra. Importante ressaltar que no presente momento a Plataforma do uCloud trabalha apenas com o conceito de semanas fechadas do mês (domingo a sábado), e estas semanas são numeradas sequencialmente de 1 a 52 e apresentadas ao lado esquerdo do calendário apresentado. O campo PERÍODO irá mostrar o calendário SEMANAL. Conforme imagem abaixo:

.. image:: /figuras/ucloud_menu_financeiro002d.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * **DIÁRIO**: Este filtro permite ter uma visão na menor granularidade de período possível. Com esta granularidade será possível entender e identificar picos de consumos ao longo dos dias. Neste caso pode trazer indicativos de aplicações ou comportamento que geram picos de consumo em uma determinado dia e não em outro. O campo PERÍODO irá mostrar o calendário DIÁRIO. Conforme imagem abaixo:

.. image:: /figuras/ucloud_menu_financeiro002e.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Período**: A Plataforma uCloud altera este campo em após o usuário selecionar o período no campo anteritor. Este campo é obrigatório.
* **Container**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta relação de todos os containers provisionados aos quais o usuário está vinculado para uso.

* **Linked Account**: O termo Containers na Plataforma uCloud é utilizado para representar um ambiente de nuvem seja este público e/ou privado. Um container é uma abstração lógica para agrupar todos os recursos (máquinas virtuais, servidores, discos, storages) de um determinado tipo de hypervisor. Todos os provedores adotam uma estrutura organizacional **LÓGICA** para criar seu ambiente de totalização de custos. Para a Plataforma uCloud, provisioná-se um **Contêiner** que pode ser a conta "**RAIZ**" da empresa. A Plataforma uCloud denomina "**Sub Account**" as subdivisões desta conta principal (Unidades Oranizacionais-OU, Contas Filhas, etc.) que as empresas possam criar para alocar custos de computação de nuvem para diferentes unidades, centros de custos etc. Este campo é do tipo "dropdown" e irá listar todas as *Sub Accounts* que foram provisionadas para a conta raiz, conforme exemplo na tela abaixo:

.. image:: /figuras/ucloud_menu_financeiro002f.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Botão Filtrar**: U usuário deve clicar com o cursor do mouse sobre este botão após o completo preenchimento de todos os filtros desejados, neste momento a Plataforma uCloud irá processar as informações armazenadas em suas bases de dados e apresentar o relatório em tela. Abaixo apresentamos uma tela para ilustrar **como simples exemplo** o resultado após o processamento para apresentação do relatório:

.. image:: /figuras/ucloud_menu_financeiro002g.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----


Dentro do HISTÓRICO DE SERVIÇO temos o quadrante VALOR TOTAL que apresenta o consumo da nuvem do mês selecionado nos campos de filtros.

Com essa informação já é possível ter uma visibilidade de como o ambiente está se comportando e dessa forma começar a montar uma estratégia para descobrir formas de optimização. Abaixo iremos nos aprofundar como esses gastos estão sendo distribuídos entre os produtos das nuvens.

* **Seção Gráficos Histórico de Custo por Categoria**:

No quadrante histórico de custo por categoria, o painel irá mostrar um gráfico para cada mês selecionado e a relação de todos os serviços da nuvem, referido também como PRODUCT NAME respectivo de cada provedor de serviço de nuvem pública.
Seguindo o padrão de nomenclatura de cada uma das nuvens, as barras irão mostrar o quanto foi gasto e quanto o serviço representa no consumo total da fatura. Ao passar o mouse em cima das barras o painel irá apresentar o nome do produto e seus respectivo gasto, conforme imagem abaixo:

.. image:: /figuras/ucloud_menu_financeiro002k.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

A apresentação padrão destes gráficos pela Plataforma uCloud é um gráfico de barras independentes, com o valor separado para cada PRODUCT NAME do provedor de serviço denuvem pública. A Plataforma uCloud permite que o usuário alterne para apresentação de gáfico com barras sobrepostas (*Stacked Columns*).

Existe uma *aba* **Configurações do Gráfico** na parte inferiorda tela que o usuário pode personalizar a forma de apresentação destes gráficos. Basta o usuário clicar com o cursor do mouse sobre a *aba* que a Plataforma uCloud irá apresentar as opções de confivutação:

.. image:: /figuras/ucloud_menu_financeiro002h.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Nesta aba o usuário pode elecionar se deseja apresentar, ou remover, dos gráficos algum PRODUCT NAME do provedor de serviço de nuvem pública.

No canto direito, desta aba, o usuário encontra um ícone que permite alternar entre o modo de apresentação das barras |icone_grafico_barra01| ou |icone_grafico_barra02|

.. image:: /figuras/ucloud_menu_financeiro002k.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

.. image:: /figuras/ucloud_menu_financeiro002m.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Seção Visualização de Dados por Custo**:

No quadrante visualização de dados por custo o painel irá apresentar os itens de serviços (PRODUCT NAME) e ao lado os meses escolhidos com seus respectivos gastos totais separado em duas categorias, COBRANÇAS DIRETAS e COBRANÇAS INDIRETAS, conforme o exemplo ilustrativo da tela abaixo:

.. image:: /figuras/ucloud_menu_financeiro002i.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Cobranças Diretas**: A categoria DIRETAS é a somatória dos valores de todos os produtos e/ou serviços os quais o provedor de serviço de nuvem pública **permite SIM vincular** alguma forma de identificação, ou etiqueta (*TAG*), que quando vinculada aos recursos computacionais pelo proprietário do(s) recurso(s) é a forma mais usual para identificação e alocação dos valores recorrentes entre departamentos, centros de custos, projetos, iniciativas etc.

* **Cobranças Indiretas**: A categoria INDIRETAS é a somatória dos valores de todos os produtos e serviços que os provedores de serviço de nuvem pública **NÃO PERMITE/ACEITA** que sejam assinaladas quaquer tipo de etiqueta (*TAG*) seja vinculada aos recursos computacionais pelo proprietário do(s) recurso(s). Cada provedor de serviço de nuvem pública tem a sua especificidade em quais produtos e serviços as etiquetas não são passiveis de serem vinculadas.

A informação explicitamente segmentada e apresentada na forma deste relatório pode apoiar a tomada de decisão (*insights*) para alinhar a distribuição dos custos internamente na empresa (*charge back*). Esta apresentação está apoiada nas melhores práticas de *FinOps* para a correta identificação de custos recorrentes de recursos computacionais de nuvem pública.

.. note:: |nota| Não é objetivo deste relatório apresentar as respectivas etiquetas (*tags*) no corpo do relatório, mas sim apresentar ao administrador de custos o total de valores os quais será possível identificar o departamento, centro de custo, projeto que são atribuídas via etiquetas (*tag*). A Plataforma uCloud permite ao administrador de custos consultar os valores por etiqueta (*tag*) em diversos outros relatórios financeiros.


Relatório Custo Cadenciado
~~~~~~~~~~~~~~~~~~~~~~~~~~

O relatório CUSTO CADENCIADO apresenta a variação de valores dos recursos computacionais de cada serviço (PRODUCT NAME) e demonstra a variação de seus de valores no mês corrente (atual) comparado somente com os valores do mês anterior. A Plataforma uCloud não permite mudar a visualização para outros meses.

Adicionalmente, a Plataforma uCloud demonstra a variação dos valores dos recuros computacionais em dois quadros diferentes:

A. *Um primeiro quadro* que apresenta a variação de valores com o período iniciando no primeiro dia calendário (dia 01) do mês corrente até o dia que o usuário estiver consultando este relatório na Plataforma uCloud (nos exemplos ilustrativos nas telas apresentadas = dia 22).

B. *Um segundo quadro* que apresenta a somatória do valor total de consumo de todo o mes anterior e a **previsão** de fechamento do mês corrente (mesmo que ainda não existam valores no *billing ou bucket* deste provedor de serviço de nuvem pública.

  A infromação referente a variação de valores do mês anterior versus mês atual permite identificar e visualizar variação dos valores financeiros comparado ao mês anterior e a **previsão** de valores de fechamento da fatura para o mês corrente.

  Importante ressaltar que mesmo que não existam dados de *billing ou bucket* provedor de serviço de nuvem pública,a Plataforma uCloud utiliza um algoritimo que projeta os valores (mesmo que estes valores não existam), com base na média de consumo dos seis (06) últimos meses armazenados nas bases de dados internas da Plataforma uCloud.

Com a visão deste relatório é possível identificar e visualizar os diferentes tipos de custos - tanto os normalmente esperados, bem como os sazonais ou inesperados - para o fechamento do mês. Este relatório permite identificar e projetar uma melhor alocação de fluxo de caixa contábil da empresa.

Importante mencionar que todas as telas dos relatórios apresentados neste documento, os valores estão sendo convertidos para moeda Real brasileiro (R$) - mesmo que o provedor armazene os valores em Dólares americanos. O valor da Taxa de Conversão Dólar <> Real está informada no Contrato na seção *Regras de Faturamento*.

* **Contrato**: A Plataforma uCloud irá apresentar uma lista com somente os contratos aos quais o usuário está vinculado, o usuário deve informar ou selecionar apenas um contrato por vez. Ao selecionar o contrato desejado a Platafoam uCloud irá apresentar a tela abaixo:

.. image:: /figuras/ucloud_menu_financeiro002.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 80 %
   :align: center
----

No momento que o contrato é selecionado a Plataforma uCloud iniciar o processamento e cálculo dos valores armazenados em sua base de dados interna e apresenta a tela do relatório. A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro003b.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 60 %
   :align: center
----

Abaixo descrevemos as seções deste relatório.

* **Quadros de Períodos**: Nesta seção são apresentados os dois quadros com as informações de valores do período e do mês

.. image:: /figuras/ucloud_menu_financeiro003d.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 80 %
   :align: center
----

  * **Quadro Laranja**: Este *primeiro quadro* apresenta a somatória dos custos de todos recursos computacionais referente ao período iniciando no primeiro dia calendário do mês corrente (dia 01) até o presente dia que o usuário estiver efetuando a consulta deste relatório na Plataforma uCloud (nos exemplos ilustrativos nas telas apresentadas = dia 22). Na parte superior deste quadro a Plataforma uCloud apresenta o valor total de custos referente ao período atual. Neste quadro a plataforma uCloud apresenta em destaque um valor que se refere ao valor do mês atual descontado (subtraído) dos valores do período do mes anterior. Na parte inferior deste quadro a Plataforma uCloud apresenta a somatória de custos de todos os recursos computacionais do período do mês anterior.

  * **Quadro Branco**: Este *segundo quadro* apresenta a *previsão* do valor para o fechamento do mês dos custos de todos os recursos computacionais para o mês corrente (mesmo que ainda não existam valores no *billing ou bucket* deste provedor de serviço de nuvem pública). Esta *previsão* é obtida pela cálculo da variação aritmética dos valores dos seis (06) últimos meses armazenados na base de dados internas da Plataforma uCloud. Estando o usuário em visualizando este relatório em uma data anterior à data de fechamento da fatura, será uma previsão. Esta *previsão* pode ser bem assertiva caso o usuário visualize este relatório em uma data próxima ao fechamento da fatura (por ex.: dia 29 do mês corrente). Neste quadro, também, a plataforma uCloud apresenta em destaque um valor que se refere ao valor do mês atual descontado (subtraído) dos valores do mes anterior. Na parte inferior deste quadro a Plataforma uCloud apresenta a somatória de custos de todos os recursos computacionais do mês anterior.

A Plataforma uCloud utiliza um ícone para demonstrar a tendência destes resultados e utilizando os seguintes ícones:

* **Ícone Seta Acima** |icone_seta_acima|: Este ícone representa um resultado superior (tendência de alta) ao mês anterior.
* **Ícone Seta Abaixo** |icone seta_abaixo|: Este ícone representa um resultado inferior (tendência de baixa) ao mês anterior.
* **Ícone Neutro** |icone_neutro|: Este ícone representa um resultado igual (tendência de estável) ao mês anterior.

Para os casos em que uma empresa se utilize a Plataforma uCloud em um período inferior a seis (06) meses, podem não existir dados de faturamento armazenados que sejam suficientes para cálculo destas variações - dados insuficientes tanto no billing/bucket do provedor quanto nas bases de dados internas. Nestas situações a Plataforma uCloud poderá apresentar estes quadros com valores zerados (em branco), conforme o exeplo abaixo:

.. image:: /figuras/ucloud_menu_financeiro003m.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 80 %
   :align: center
----

.. attention:: |atencao| Isto **não é um erro**, significa que: podem não existir valores e/ou dados armazenados nas bases de dados internas; ou a configuração de acesso ao arquivo de billing/bucket não está corretamente provisionda; ou não foi efetuado/iniciado o processado de cálculo do billing até o presente momento. Nestes casos pedimos que entre em contato com a Equipe de Suporte da Ustore (chamados@usto.re) para lhe acompanhar na correta configuração de suas credenciais aos ambientes de provedores de nuvem pública.

----

* **Seção Top 15 Custo por Grupo**: Nesta seção a Plataforma uCloud apresenta a lista dos quinze (15) primeiros Grupos que acumulam os maiores valores de custos de recursos computacionais. A quantidade de Grupos apresentada está diretamente relacionada com a organização dos Grupos provisionados no Contrato de seu ambiente na Plataforma uCloud. Importante mencionar que mesmo que existam vários Grupos, somente os quinze (15) Grupos que acumulam os maiores valores serão relacionados nesta seção. A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro003e.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 80 %
   :align: center
----

Abaixo descrevemos as colunas deste seção:

  * **Grupos**: Esta coluna apresenta o nome do(s) Grupo(s) da forma como foram provisionados na Plataforma uCloud.
  * **Mês Atual**: Esta coluna apresenta a somatória do valores de todos os recursos computacionais do provedor de nuvem pública, do mês corrente (atual), que estão vinculados a todos os usuários que fazem parte deste Grupo  - mesmo que este relatório seja consultado em data anterior à data de encerramento da fatura.
  * **Último mês**: Esta coluna apresenta a somatória do valores de todos os recursos computacionais do provedor de nuvem pública, do mês imediatamente anterior ao mês atual (último mês), que estão vinculados a todos os usuários que fazem parte deste Grupo  - valores do fechamento do mês anterior armazenado nas baes de dados internas.
  * **Projeção**: Esta coluna apresenta a projeção do valor para o mês atual de todos os recursos computacionais que estão vinculados a todos os usuários que fazem parte deste Grupo  - mesmo que este relatório seja consultado em data anterior à data de encerramento da fatura.
  * **Projeção Δ**: Esta coluna apresenta a diferença numérica do valor financeiro para o mês atual, comparado com o mês anterior, de todos os recursos computacionais que estão vinculados a todos os usuários que fazem parte deste Grupo - mesmo que este relatório seja consultado em data anterior à data de encerramento da fatura.
  * **Δ%**: Esta coluna apresenta a diferença percentual do valor financeiro para o mês atual, comparado com o mês anterior, de todos os recursos computacionais que estão vinculados a todos os usuários que fazem parte deste Grupo - mesmo que este relatório seja consultado em data anterior à data de encerramento da fatura.
  * **ìcone Indicador de Tendência**: Esta coluna apresenta um ícone que representa a tendência da variação dos valores do mês atual frente o mês anterior.

    * **Ícone Seta Acima** |icone_seta_acima|: Este ícone representa um resultado superior (tendência de alta) ao mês anterior.
    * **Ícone Seta Abaixo** |icone seta_abaixo|: Este ícone representa um resultado inferior (tendência de baixa) ao mês anterior.
    * **Ícone Neutro** |icone_neutro|: Este ícone representa um resultado igual (tendência de estável) ao mês anterior.

----

* **Seção Top 15 Custo por Serviços**: Nesta seção a Plataforma uCloud apresenta a lista dos quinze (15) primeiros Serviços (*PRODUCT NAME*) do provedor de serviço de nuvem pública que acumulam os maiores valores no mês atual. A quantidade de Serviços (*product name*) apresentada está diretamente relacionada com a soma total de seus valores acumulados no arquivo de *billing* e armazanados nas bases de dados internas da Plataforma uCloud. Importante mencionar que mesmo que existam uma grande diversidade de outros serviços (*product name*), somente os quinze (15) que acumulam os maiores valores serão relacionados nesta seção. A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro003p.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 80 %
   :align: center
----

  * **Serviços**: Esta coluna apresenta o nome dos Serviços (*product name*) da forma como estão expressos no arquivo de *billing* do provedor de serviço de nuvem pública.
  * **Mês Atual**: Esta coluna apresenta a projeção de valores de todos as incidências deste Serviço (*product name*) do provedor de nuvem pública, para o mês corrente (atual) - mesmo que este relatório seja consultado em data anterior à data de encerramento da fatura.
  * **Último mês**: Esta coluna apresenta a somatória de valores Serviços (*product name*) no provedor de nuvem pública, do mês imediatamente anterior ao mês atual (último mês) - valores do fechamento do mês anterior armazenado nas baes de dados internas.
  * **Projeção**: Esta coluna apresenta a projeção do valor para o Serviço (*product name*) para o mês atual - mesmo que este relatório seja consultado em data anterior à data de encerramento da fatura.
  * **Projeção Δ**: Esta coluna apresenta a diferença numérica (*delta*) do valor financeiro para o mês atual, comparado com o mês anterior - mesmo que este relatório seja consultado em data anterior à data de encerramento da fatura.
  * **Δ%**: Esta coluna apresenta a diferença percentual (*delta*) do valor financeiro para o mês atual, comparado com o mês anterior - mesmo que este relatório seja consultado em data anterior à data de encerramento da fatura.
  * **ìcone de Indicador de Tendência**: Esta coluna apresenta um ícone que representa a tendência da variação dos valores do mês atual frente o mês anterior.

    * **Ícone Seta Acima** |icone_seta_acima|: Este ícone representa um resultado superior (tendência de alta) ao mês anterior.
    * **Ícone Seta Abaixo** |icone seta_abaixo|: Este ícone representa um resultado inferior (tendência de baixa) ao mês anterior.
    * **Ícone Neutro** |icone_neutro|: Este ícone representa um resultado igual (tendência de estável) ao mês anterior.

----

* **Seção Exportar Relatórios**: 

Esta seção, na parte inferior da tela, permite exportar relatórios no formato CSV de todos os serviços, consumo e gastos de maneira detalhada, sendo permitido selecionar intervalos MENSAL, SEMANAL e DIÁRIO, a critério do usuário.

.. image:: /figuras/ucloud_menu_financeiro003c.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 50 %
   :align: center
----

  * **Botão Exportar Detalhado**: Nesta opção a Plataforma uCloud cria um arquivo CSV com o nome CADENCE-DETAILED-NOME_DO_CONTRATO-MES-ANO.CSV apresentará 8 Colunas.

  * **Botão Exportar Serviços**: Nesta opção a Plataforma uCloud cria um arquivo CSV com o nome CADENCE-SERVICES-NOME_DO_CONTRATO-MES-ANO.CSV apresentará 5 Colunas.

.. image:: /figuras/ucloud_menu_financeiro003c.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 50 %
   :align: center
----

  * **Botão Exportar Relatório Δ**: Nesta opção a Plataforma uCloud cria um arquivo CSV que irá demonstrar a diferença do consumo dos *Product Name* e *Family Name* dos provedores com os dados do mês atual, comparando com o mês anterior. De possse dessa informação é possível ter visibilidade de como cada um dos serviços estão se comportando, podendo assim tomar ações de controle e apuração mais efetiva e direcionada focada no *PRODUCT NAME* da nuvem.

  No arquivo CSV, a coluna VARIAÇÃO MÊS ANTERIOR % irá mostrar o percentual da variação e a coluna VARIAÇÃO MÊS ANTERIOR $ irá mostrar a variação em dólar. Conforme imagens abaixo, Financeiro/Custo Cadenciado/Intervalo/Período/Exportar Relatório Detalhado.

  O export de relatório delta é enviado por email, caso queira ver em tela este se encontra no quadrante acima do exporte relatórios, mostrado anteriormente.

  Para receber o relatório por email basta inserir um email válido e clicar em enviar conforme imagem abaixo:

.. image:: /figuras/ucloud_menu_financeiro003k.png
   :alt: Menu Financeiro - Relatorio Custo Cadenciado
   :scale: 50 %
   :align: center
----

  A Plataforma uCloud pode demandar um certo tempo para selecionar, calcular e enviar este arquivo. Mas ao final do processamento, envia o arquivo CSV e confirma o envio com uma mensagem popup ao usuário.

.. note:: Para os casos em que o usuário não receba qualquer email, verificar a pasta SPAM/Lixo com e-mail origem *noreply@dominio.com.br*. Alguns sistemas de e-mail bloqueiam, mensagens com "noreply@...", ou encaminham automaticamente para a pasta/folder SPAM/Lixo.

----

**Resumo do Relatório Custo Cadenciado**
########################################

No primeiro quadrante é possível notar o período da análise, que se refere ao dia 01/07/21 ao dia 22/07/21 (data atual).

Logo abaixo temos o gasto efetuado no mesmo intervalo de tempo mas referente ao mês anterior, no exemplo, referente ao mês de JUNHO (06/21) entre os dias 01 à 22. Conforme imagem abaixo. Importante mencionar que todas as telas dos relatórios apresentados neste documento, os valores estão sendo convertidos para Real (R$).

Podemos verificar que a diferença de gastos é de $ - 49.999,73 entre os dias 01/06/21 até 22/06/21 (mês anterior) e 01/07/21 até 22/07/21 (mês atual) ou seja, houve uma economia de $ 49,999,73 com relação ao mês passado, conforme mostra a imagem acima.

====

Relatório Custo Relacional de Produto
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este relatório permite ao administrador de custos acompanhar a evolução (mensal, semanal ou diária) dos custos detalhados de consumo de cada PRODUCT NAME e sua respectiva FAMILY NAME (sub-recursos) por provedor de serviço (*Container*) e por sub-conta(s).

O grande benefício deste relatório é análizar a real composição de custos de um recurso (*Product Name*) em particular, com a apresentação detalhada dos valores de seus sub-recursos (Family Name) distribuídos no período selecionado na preparação do relatório.

Para os ambientes de multi-nuvem, cada provedor de serviço utiliza denominações e identificações específicas depara cada provedor de serviço de nuvem pública. A Plataforma uCloud facilita, de forma muito prática, a análize da composução de custos de um produto.

Lembre-se que a Plataforma uCloud **sincroniza e unifica** a fonte de dados original do provedor de serviço de nuvem - o arquivo de billing do provedor (CSV, SQL, etc) - em suas bases de dados de forma que este relatório permite ter a mesma visão independentemente de como cada provedor de serviço de nuvem pública identifica (*nomeia*) seus produtos e os sub-produtos.

De regra geral, todos os provedores de serviço de nuvem pública, possuem o conceito de:

* **Total da Conta do Provedor de Serviço de Nuvem Pública é**:

  * Account (uCloud: Container)

    * Sub-Account (uCloud: Linked Account)

      * Product Name (uCloud: Nome do Produto)

        * Family Name (uCloud: Família de Produto)

          * Custo (Valor Final no período - diário, semanal, mensal)

.. image:: /figuras/ucloud_menu_financeiro012a.png
   :alt: Menu Financeiro - Histórico de Serviço
   :scale: 60 %
   :align: center

----

Na figura acima (meramente ilustrativa) podemov ver que os custos de cada item de um *Family Name* compõe o valor do Product Name e a somatória destes custos totalizam o valor do período consultado (diário, semanal, mensal).

Este relatório permite ao usuário analizar os custos individuais de cada *Family Name* de apenas um *Product Name* por vez.

Neste relatório, será posível acompanhar a evolução do consumo de um *Family Name* dentro de uma *Sub-Account* para o período selecionado, mesmo que este seja abrangente (vários dias, semanas, meses).

Ao selecionar a opção do menu CUSTO RELACIONAL DE PRODUTO será solicitado que escolha um CONTRATO, tipo de INTERVALO, PERÍODO, NUVEM (*Container*) e *Linked-Account (sub-conta)*, através desse relatório é possível analisar os custos de forma detalhada conforme apresentado nas imagens abaixo.

Quando selecionado este relatório, a Plataforma uCloud apresenta a tela abaixo, onde o usuário deve informar ou selecionar apenas um único contrato:

.. image:: /figuras/ucloud_menu_financeiro002.png
   :alt: Menu Financeiro - Histórico de Serviço
   :scale: 60 %
   :align: center

----

Após selecionado o contrato a Plataforma uCloud apresenta os campos a tela inicial do relatório com campos onde o usuário pode informar os critérios necessários para a apresentação do relatório, a figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro012b.png
   :alt: Menu Financeiro - Histórico de Serviço
   :scale: 60 %
   :align: center

----

Abaixo descrevemos os 

* **Contrato**: Este campo se apresenta preenchido com o contrato informado na tela anterior, e o relatório será apresentado somente com as informações financeiras referentes a este contrato.

* **Botão Lupa** |icone_lupa|:  Se a credencial do usuário, que está com uma sessão ativa (*login*) está associado a mais de um contrato, este usuário poderá consultar outro contrato. Para isto deve clicar com o cursor do mouse sobre o ícone da *lupa* para Plataforma uCloud apresentar a tela para informar o nome de outro contrato para emissão do relatório.

* **Intervalo**: Este campo é do tipo "dropdown" e o usuário pode selecionar o período ideal para avaliar os dados de consumo de sem ambiente. Quando fazemos uma análise comparando mensalmente o cliente poderá entender como a sua fatura evolui ao longo do tempo de acordo com o faturamento do provedor. Quando clicar com o cursor do mouse a Plataforma uCloud apresenta as opções:
  
  * **MENSAL**: Quando selecionada a análise mensal o cliente poderá entender como a sua fatura evolui ao longo do tempo de acordo com o faturamento do provedor. Esta visão permite entender o consumo dos produtos de acordo com a fatura do cliente, no exemplo abaixo iremos selecionar o campo PERÍODO então MENSAL, dessa forma o calendário com os meses ficará disponível para seleção. É possível escolher mínimo 1 mês e máximo todos os meses do ano. Para exemplificar, selecionamos os últimos 3 meses, conforme imagem abaixo.

.. image:: /figuras/ucloud_menu_financeiro002c.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * **SEMANAL**: Este filtro permite ter uma visão mais granular do consumo, podendo entender e identificar picos de consumos em semanas aos longos dos meses. Neste caso pode trazer indicativos de aplicações ou comportamento que geram picos de consumo em uma determinada semana e não em outra. Importante ressaltar que no presente momento a Plataforma do uCloud trabalha apenas com o conceito de semanas fechadas do mês (domingo a sábado), e estas semanas são numeradas sequencialmente de 1 a 52 e apresentadas ao lado esquerdo do calendário apresentado. O campo PERÍODO irá mostrar o calendário SEMANAL. Conforme imagem abaixo:

.. image:: /figuras/ucloud_menu_financeiro002d.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * **DIÁRIO**: Este filtro permite ter uma visão na menor granularidade de período possível. Com esta granularidade será possível entender e identificar picos de consumos ao longo dos dias. Neste caso pode trazer indicativos de aplicações ou comportamento que geram picos de consumo em uma determinado dia e não em outro. O campo PERÍODO irá mostrar o calendário DIÁRIO. Conforme imagem abaixo:

.. image:: /figuras/ucloud_menu_financeiro002e.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Período**: A Plataforma uCloud altera este campo em após o usuário selecionar o período no campo anteritor. Este campo é obrigatório.

* **Container**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta relação de todos os containers provisionados aos quais o usuário está vinculado para uso.

* **Botão Pesquisar**: Após selecionados os campos de período, o usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud permita que o usuário selecione os próximos campos para apresentação do relatório.

* **Linked Account**: Este campo é do tipo "*check mark*" e a Plataforma uCloud apresenta a relação de todas as *Linked Accounts - Sub-Accounts* que fazem parte do(s) container(s) que estão vinculados ao contrato do usuário cm uma sessão ativa (*login*). Neste momento o usuário deve selecionar uma (ou várias) *Linked Accounts* que serão objeto da emissão do reltório. Importante mencionar que esta seleção irá interagir com outro campo do relatório, desta forma o usuário poderá comparar o consumo de recursos entre diferentes *Linked Accounts* para o período selecionado.

* **Ícone Próximo** |icone_next_ativo|: O usuário deve clicar com o cursor do mouse sobre este ícone para a Plataforma uCloud permitir seguir para o próximo campo de filtragem de dados. Caso este ícone esteja desativado |icone_next_off| significa que não existe seleção ativa para este campo de filtragem e a Plataforma uCloud não está customizada para o próximo campo de filtragem.

* **Produto**: Este campo é do tipo "*radio button*" e a Plataforma uCloud apresenta a relação de todos os *Product Name** que estão fazem parte do arquivo de *billing (CSV)* que está sincronizado com as bases de dados internas. O usuário deve clicar com o cursor do mouse sobre o produto desejado para apresentção do relatório - **apenas um Product Name é permitido**. Importante mencionar que serão listados todos os *Product Name* que estão no arquivo de *billing* que possuem (ou não) valores de custo para o período selecionado.

* **Ícone Próximo** |icone_next_ativo|: O usuário deve clicar com o cursor do mouse sobre este ícone para a Plataforma uCloud permitir seguir para o próximo campo de filtragem de dados. Caso este ícone esteja desativado |icone_next_off| significa que não existe seleção ativa para este campo de filtragem e a Plataforma uCloud não está customizada para o próximo campo de filtragem.

* **Família do Produto**: Este campo é do tipo "*check mark*" e a Plataforma uCloud apresenta a relação de todos as *Family Name** que estão fazem parte do *Product Name* selecionado no campo anterior. O usuário pode selecionar todos (ou apenas um) *Family Name*, basta clicar com o cursor do mouse sobre todos os *Family Name* desejados para apresentção do relatório.

* **Botão Limpar**: O usuário deve clicar com o cursor do mouse sobre este botão somente quando necessita redefinir todos os campos de filtragem para reiniciar a apresentação do relatório desde seu início. Este é o procedimento padrão quando o usuário necessita analizar o relatório com outros *Produtos* e outros *Família de Produtos*.

* **Botão Fazer Busca**: Após selecionados os campos de período, o usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud apresente o relatório. A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro012c.png
   :alt: Menu Financeiro - Histórico de Serviço
   :scale: 60 %
   :align: center

----

Abaixo descrevemos os quadros deste relatório:

* **Seção Selecione uma Linked**: Neste quadro o usuário pode alternar a forma como a Platafrma uCloud apresenta o gráfico de barras ao lado confirme as opçõe abaixo:

  * **Selecione todas as Linkeds**: Esta é a opção padrão de apresentação deste relatório, e a Plataforma uCloud apresenta um gráfico de barra, com a pilha dos valores de cada *Family Name*. Cada barra representa uma *Linked Account* totalizada em somente uma barra. Importante mencionar que a Plataforma uCloud apresenta a legenda de cores na parte superior do gráfico. A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro012d.png
   :alt: Menu Financeiro - Histórico de Serviço
   :scale: 60 %
   :align: center

----

  * **Selecionar SOMENTE UMA LINKED**: Esta é a opção padrão de apresentação deste relatório, e a Plataforma uCloud apresenta um gráfico de barra, com a pilha dos valores de cada *Family Name*. Cada barra representa uma *Linked Account* totalizada em somente uma barra. Importante mencionar que a Plataforma uCloud apresenta a legenda de cores na parte superior do gráfico. Importante mencionar que as linkeds desativadas não possuem dados no intervalo de tempo selecionado, e podem apresentar valor ZERO (0). A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro012e.png
   :alt: Menu Financeiro - Histórico de Serviço
   :scale: 60 %
   :align: center

----

A última parte deste relatório a Plataforma uCloud apresenta a lista com as informações e valores que foram utilizados para a geração do gráfico acima. Esta listagem possui as seguintes colunas:

* **Linkeds**: Esta primeira coluna apresenta a lista de todas as *Linked Accounts*, que foram selecionadas no campo de filtragem *Linked Account* acima, e somente quando o usuário seleciona a opção **Selecione todas as Linkeds** no quadro anterior. Importante mencionar que esta coluna pode alternar para apresentar as **datas** do período selecionado. Como resultado desta seleção, a listagem da cluna *Família de Produto* apresenta a somatória de todas as incidências desta Família de Produto no período selecionado.

* **Datas**: Esta primeira coluna apresenta a lista de todas as *Datas*, que foram selecionadas no campo de filtragem *Período* acima, e somente quando o usuário seleciona a opção **SOMENTE UMA LINKED** no quadro anterior. Importante mencionar que esta coluna pode alternar para apresentar as **Linked Accounts** do período selecionado. Se a seleção do campo período incluir uma ampla sequencia de datas, a Plataforma uCloud apresenta as datas de forma cronológica ascendente.

* **Nome do produto**: Nesta coluna a Plataforma uCloud apresenta somente o *Nome do Produto* que foi selecionado no campo de filtragem *Produto* acima.

* **Família do Produto**: Esta coluna a Plataforma uCloud relaciona o *Nome do Produto* que foi selecionado no campo de filtragem *Produto* acima e pode alternar entre duas informações diferentes:

  #. Caso o usuário tenha selecionado **Todas as Linkeds** na seção anterior, o resultado desta seleção é a somatória de todas as incidências desta *Família de Produto* no período selecionado.

  #. Caso o usuário tenha selecionado **SOMENTE UMA LINKED** na seção anterior, a Plataforma uCloud pode apresentar diversas linhas com a mesma incidência da *Família de Produto*, e os seus respectivos valores em cada data relacionada na primeira coluna (*Datas*).

* **Valor**: Nesta coluna a Plataforma uCloud apresenta a somatória dos custos referente ao período selecionado.

**Resumo do Relatório Custo Relacional de Produto**
###################################################

Atravé deste relatório o usuário pode comparar os custos de *Família de Produtos* tanto dentro de uma (ou várias) *Linked Account*, bem como alternar para a visão da evolução dos custos de *Família de Produtos* dentro de um período selecionado (diário, semanal, mensal).

Este relatório tem uma grande valia na inteligência de negócio, pois pode ajudar ao Administrador de Custos preparar visões Orcamentárias (*Previsto vs. Realizado*) que não estavam muito claras, devido a aomplexidade de análise dos arquivos de *billing (CSV)* do provedor de serviço de nuvem pública, quando existem diversas *Linked Accounts* no cenário de organização de contas.

====

Relatório Visualização de Recursos
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Importante mencionar que no presente momento, a Plataforma do uCloud somente consegue apresentar o relatório de “*Visualização de Recursos*” apenas com os dados do provedor de serviço de nuvem pública **AWS** (*Amazon Web Services*), por razão das características de granularidade das informações existentes no arquivo *Cost and Usage Report* (**CUR**) - arquivo texto formato CSV que contém o billing da AWS. Estamos trabalhando para inclusão de outros provedores de serviço de nuvem pública. A evolução e inclusão de outros provedores de serviço de nuvem pública será tema do documento Release Notes ou nas evoluções da Plataforma uCloud.

.. important:: Até o presente mmento, a Plataforma do uCloud, não disponibila qualquer ação sobre os botões referente a outros provedores (Azure, GCP e Oracle), estes botões não estão ativos!

----

Ao selecionar a opção do menu VISUALIZAÇÃO DE RECURSOS será solicitado que escolha um CONTRATO, o tipo de INTERVALO e o PERÍODO, através desse relatório é possível analisar os custos de forma detalhada conforme apresentado nas imagens abaixo.

Quando selecionado este relatório, a Plataforma uCloud apresenta a tela abaixo, onde o usuário deve informar ou selecionar apenas um único contrato:

.. image:: /figuras/ucloud_menu_financeiro002.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

* **Contrato**: A Plataforma uCloud irá apresentar uma lista com somente os contratos aos quais o usuário está vinculado, o usuário deve informar ou selecionar apenas um contrato por vez. Ao selecionar o contrato desejado a Platafoam uCloud irá apresentar a tela abaixo:

  No momento que o contrato é selecionado a Plataforma uCloud iniciar o processamento e cálculo dos valores armazenados em sua base de dados interna e apresenta a tela do relatório. A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro005a.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 60 %
   :align: center
----

Abaixo descrevemos os campos para apresentação deste relatório:

* **Intervalo**: Este campo é do tipo "dropdown" e o usuário pode selecionar o período ideal para avaliar os dados de consumo de sem ambiente. Quando fazemos uma análise comparando mensalmente o cliente poderá entender como a sua fatura evolui ao longo do tempo de acordo com o faturamento do provedor. Quando clicar com o cursor do mouse a Plataforma uCloud apresenta as opções:
  
  * **MENSAL**: Quando selecionada a análise mensal o cliente poderá entender como a sua fatura evolui ao longo do tempo de acordo com o faturamento do provedor. Esta visão permite entender o consumo dos produtos de acordo com a fatura do cliente, no exemplo abaixo iremos selecionar o campo PERÍODO então MENSAL, dessa forma o calendário com os meses ficará disponível para seleção. É possível escolher mínimo 1 mês e máximo todos os meses do ano. Para exemplificar, selecionamos os últimos 3 meses, conforme imagem abaixo.

.. image:: /figuras/ucloud_menu_financeiro002c.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * **SEMANAL**: Este filtro permite ter uma visão mais granular do consumo, podendo entender e identificar picos de consumos em semanas aos longos dos meses. Neste caso pode trazer indicativos de aplicações ou comportamento que geram picos de consumo em uma determinada semana e não em outra. Importante ressaltar que no presente momento a Plataforma do uCloud trabalha apenas com o conceito de semanas fechadas do mês (domingo a sábado), e estas semanas são numeradas sequencialmente de 1 a 52 e apresentadas ao lado esquerdo do calendário apresentado. O campo PERÍODO irá mostrar o calendário SEMANAL. Conforme imagem abaixo:

.. image:: /figuras/ucloud_menu_financeiro002d.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * **DIÁRIO**: Este filtro permite ter uma visão na menor granularidade de período possível. Com esta granularidade será possível entender e identificar picos de consumos ao longo dos dias. Neste caso pode trazer indicativos de aplicações ou comportamento que geram picos de consumo em uma determinado dia e não em outro. O campo PERÍODO irá mostrar o calendário DIÁRIO. Conforme imagem abaixo:

.. image:: /figuras/ucloud_menu_financeiro002e.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Botão Pesquisar**: Após selecionados os campos de período, o usuário deve clicar com o cursor do mouse sobre este botão para a Plataforma uCloud iniciar o cálculo e apresentação do relatório. A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

A Plataforma uCloudd permite selecionar entre os três (3) tipos de recursos computacionais que acumulam valores e custos mensais. O usuário pode selecionar qual tipo de recurso que deseja visualizar entre: Máquinas Virtuais, Banco de Dados e *Storage*.

**Visualização de Custos por Máquinas Virtuais**
################################################

* **Botão VM**: Quando o usuário clicar com o cursor do mouse sobre este botão a Plataforma uCloud apresenta o relatório que demonstra o Custo Total do consumo realizado do serviço de Compute, ou seja, quanto foi gasto em dólares com máquinas virtuais (CPU e memória) agrupados por tipos de flavors.

.. image:: /figuras/ucloud_menu_financeiro005g.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

O relatório de visualização de recursos entrega de maneira detalhada quais os tipos de combinação de memória e CPU, conhecido como *FLAVORS*, as máquinas virtuais, os bancos de dados e os autoscale estão utilizando.

Com essa visibilidade é possível tomar decisões no âmbito financeiro e no operacional, auxiliando na decisão de qual flavor é melhor financeiramente e tecnicamente para determinado sistema e ou projeto.

Os provedores possuem centenas de tipos de flavors que por sua vez possuem custos e performance diferentes, por essa razão esse relatório é uma ótima ferramenta para toda equipe de TI.

.. image:: /figuras/ucloud_menu_financeiro005b.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

É possível saber quanto custou cada tipo de flavor individualmente passando o mouse em cima das barras coloridasA figura abaixo é meramente ilustrativa e serve apenas como exemplo:

  * **Custo Total**: Este campo a Plataforma uCloud apresenta o valor total acumulado no mês dos recursos (*product Name*) máquina virtual. Este valor é a somatória de máquinas virtuais isoladas (por consumo mensal ou instância reservada) e o valor das instâncias de escalabilidade horizontal (*Autoscale*).

  * **Custo Autoscale**: Este campo apresenta o valor acumulado no mês dos recursos máquina virtual UNICAMENTE referente aos recursos de máquina virtual que foram provisionadas automaticamente via o recurso de **Autoscale**. A funcionalidade de *Autoscale* comum a todos os provedores de serviço de nuvem pública, permite aumentar e diminuir, de maneira automática, o número de máquinas virtuais para manter o nível de serviço disponível e performático, a partir de premissas definidas com base no percentual de consumo de memória e ou CPU pré estabelecidos. Geralmente estas máquinas virtuais são provisionadas e desprovisionadas (removidas) automaticamente com intervalos e períodos de execução não esperados, podendo ser criadas e removidas em questões de minutos.

  * **Custo sem Autoscale**: Este campo a Plataforma uCloud apresenta o valor total acumulado no mês dos recursos (*product Name*) máquina virtual *sem o AUTOSCALE*, ou seja, o gasto das máquinas reais que estão sendo utilizadas que acabam tendo um impacto financeiro muito mais significativo que necessita análise.

----

* **Seção Custo por Flavor**: Nesta seçãao a Plataforma uCloud apresenta um gráfico de barra, com detalhes de todos os flavors utilizados, separado por cores. Quando o usuário o passar o cursos do mouse sobre a cor desejada, a Plataforma uCloud apresenta o nome do tipo de flavor e o seu CUSTO TOTAL acumulado no mês. Para os cenários em que sã selecionados mais de um mês, uma semana, um dia a Plataforma uCLoud apresenta cada período agrupado em barras que representam cada período. Esta visualizção é extremamente útil para acompanhar a variação de valores do recurso computacional entre cada período (as barras).

----

* **Seção Tabela de Custo pos Flavor**: Esta seção apresenta a origem dos valores dos botões acima e é a base de dados para a geração do gráfico. Esta tabela possui algumas colunas e descrevemos as colunas abaixo.

  * **Digite o Nome do Flavor**: Neste campo o usuário pode digitar qualquer combinação de caracteres que identificam os *flavors* para restrigir a apresentação destes nesta tabela.
  * **Flavor**: Nesta coluna a Plataforma uCloud apresenta o identificação do *flavor* conforme está identificado no provedr de serviço de nuem pública (na ilustração estão presentes apenas as identificações de *flavors* presentes na AWS). Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de *flavors** de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **Quantidade**: Nesta coluna a Plataforma uCloud apresenta a quantidade total de instâncias de máquinas virtuais que existem no arquivo de billing do provedor de serviço de nuvem pública. Importante ressaltar que aqui está o volume total de instâncias e representam tanto máquinas virtuais isoladas (individuais) quanto as máquinas virtuais possuem configuração de *autoscale*. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de valores de *flavors* de forma numérica crescente ou decrescente.
  * **Linked Account**: Nesta coluna a Plataforma uCloud apresenta a identificação da *Linked Account* em que a(s) máquina(s) vitual(is) estáo vinculadas. A *Linked Account* é um termo da AWS e é uma forma de agrupamento (ou sub-agrupamento) de diversas contas AWS em uma única conta Master IAM. É importante salientar que a partir do momento que essas contas são consolidadas em uma mesma conta Master IAM, o seu faturamento também é consolidado. Adicionalmente, a cobrança da utilização da nuvem AWS é feita também com preços por volume, o uso da combinação e consolidação de várias contas em uma mesma organização pode acarretar em descontos através da qualificação da conta principal ou da conta pagadora. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud irá agrupar a lista de *flavors* de forma a apresentar *Linked Accounts* de forma agrupada.
  * **Custo**: Nesta coluna a Plataforma uCloud apresenta a somatória dos valores da(s) máquina(s) virtual(is) com o seu valor no(s) mês(es) de consulta do relatório. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de valores dos custos de forma numérica crescente ou decrescente.
  * **AutoScale**: Nesta coluna a Plataforma uCloud, apresenta a indicação se esta máquina virtual possui uma configuração de *autoscale* SIM ou NÃO vinculada a este *flavor*. Esta informação é importante para que o administrador de custos possa efetuar o cálculo correto do custo indivudual de cada tipo de *flavor* e identificar os tipos de *flavor* que são mais dispendiosos ou mais econônicos. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud irá agrupar a lista de *flavors* de forma a apresentar *Autoscale* SIM e *Autoscale* NÃO.

----

**Visualização de Custos por Banco de Dados**
#############################################

.. image:: /figuras/ucloud_menu_financeiro005k.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

* **Botão Banco de Dados**: Quando o usuário clicar com o cursor do mouse sobre este botão a Plataforma uCloud apresenta o relatório que demonstra o Custo Total do consumo realizado do serviço de Banco de dados (**RDS**), ou seja, quanto foi gasto em valores com máquinas virtuais (CPU e memória) para suportar os bancos de dados, agrupados por tipos de *flavors* ou por *Linked Accounts*. Esse relatório irá apresentar o Custo Total do consumo realizado do serviço de Compute, ou seja, quanto foi gasto em dólares com máquinas virtuais (CPU e memória) agrupados por tipos de flavors.

.. image:: /figuras/ucloud_menu_financeiro005c.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

Existem três quadros neste relatório com informações de inteligência de negócios para avaliar os custos relativos ao suporte para execução de instâncias de banco de dados no provedor de serviço de nuvem pública.

 É possível saber a quantidade de instâncias de banco de dados ativas e o valor total no período selecionado, a quantidade de cópias instantâneas (*snapshots*) e a quantidade de maquinas virtuais na modalidade de **Instância Reservada** vinculadas unicamente para execução de bancos de dados. A figura acima é meramente ilustrativa e serve apenas como exemplo:

  * **Quantidade de RDS**: Neste quadro a Plataforma uCloud apresenta a quantidade total de instâncias de banco de dados ativas e a somatória do respectivo valor total de RDS para o período selecionado.

  * **Quantidade de Snapshots de RDS**: Neste quadro a Plataforma uCloud apresenta a quantidade total de quantidade de cópias instantâneas (*snapshots*) que foram criadas no período selecionado.

  * **Quantidade de instancias reservadas de RDS**: Neste quadro a Plataforma uCloud apresenta a quantidade total de maquinas virtuais na modalidade de **Instância Reservada** vinculadas unicamente para execução de bancos de dados.

* **Seção Quantidade de gasto por RDS por Flavor/Linked Account**: Nesta seçãao a Plataforma uCloud apresenta um gráfico de barra, com detalhes de todos os flavors utilizados, separado por cores, que estão vinculados à execução de instâncias de base de dados. Quando o usuário o passar o cursos do mouse sobre a cor desejada, a Plataforma uCloud apresenta o nome do tipo de flavor e o seu CUSTO TOTAL acumulado no mês. No lado superior direito desta seção o usuário encontra um botão onde é possível alternar a forma como a Plataforma uCloud agrupa os valores deste gráfico.

  * **Quantidade de gasto por RDS por Flavor/Visualizar por Linked**: Este gráfico apresenta um gráfico de barras sobrepostas, separados por cores, com o nome e o valor de cada *flavor* existente no período selecionado. Quando o usuário passa com o cursor do mouse sobre a cor desejada a Plataforma uCloud apresenta uma etiqueta que identifica o *flavor* e o valor total referente ao período selecionado. Para os cenários em que são selecionados mais de um mês, uma semana, um dia a Plataforma uCLoud apresenta cada período agrupado em barras que representam cada período. Esta visualizção é extremamente útil para acompanhar a variação de valores do recurso computacional entre cada período (as barras). A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro005h.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----


* **Quantidade de gasto por RDS por Linked/Visualizar por Flavor**: Este gráfico apresenta um gráfico de barra com o nome e o valor de cada *Linked Account* existente no período selecionado. Quando o usuário passa com o cursor do mouse sobre a barra desejada a Plataforma uCloud apresenta uma etiqueta que identifica a *Linked Account* e o valor total referente ao período selecionado. Para os cenários em que são selecionados mais de um mês, uma semana, um dia a Plataforma uCloud apresenta cada período agrupado em barras que representam cada período. Esta visualizção é extremamente útil para acompanhar a variação de valores do recurso computacional de cada *Linked Account* entre cada período (as barras). A figura abaixo é meramente ilustrativa e serve apenas como exemplo:

.. image:: /figuras/ucloud_menu_financeiro005j.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----


**Visualização de Custos por Storage**
######################################

.. image:: /figuras/ucloud_menu_financeiro005m.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

* **Botão Storage**: Quando o usuário clicar com o cursor do mouse sobre este botão a Plataforma uCloud apresenta o relatório que demonstra o Custo Total do consumo do serviço de armazenamento de dados (*Storage*), ou seja, apresenta a quantidade alocada referente ao serviço de armazenamento de dados. Esse relatório irá apresentar o número referente ao total de área de armazenamento (tamanho em *Gigabytes*), e um gráfico com o nome e a percentual de tamanho das maiores área de armazenamento, referente ao período de consulta.

.. image:: /figuras/ucloud_menu_financeiro005d.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

* **Seção Total de Storage**: Este quadro apresenta o valor total de alocação de armazenamento existente referente ao período de consulta. O número apresentado neste quadro está sempre expresso em *Gigabytes*.

* **Seção Bucket**: Este quadro apresenta número total de áreas de armaznamento que e encontram ativas, para o período de consulta.

* **Seção Storage**: Este quadro apresenta uma lita com o(s) nome(s), e o respectivo tamanho alocagdo (em *Gigabytes*), das principais áreas de armazenamento ativas e existentes referente ao perído consultado. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título do nome do Storage, a Plataforma uCloud classifica a lista de nomes de *storages* de forma alfabética crescente (a – z) ou decrescente (z – a). Ao clicar com o botão do mouse no título do tamanho (total), a Plataforma uCloud classifica a lista tamanho crescente ou decrescente.

* **Grafico Consumo por tipo de armazenameto**: Este quadro apresenta um gráfico (tipo pizza) que reflete a proporção de área de armazenamento referente a lista dos nomes de áreas de armazenamento no quadro **Storage**. Quando o usuário passa o mouse sobre qualquer uma das áreass do gráfico, a Plataforma uCloud apresenta uma janela popup com a(s) informação(ões) de cada nome de área de armazenamento.


.. Custos de Budgets
.. ~~~~~~~~~~~~~~~~~

.. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Maecenas porttitor congue massa. Fusce posuere, magna sed pulvinar ultricies, purus lectus malesuada libero, sit amet commodo magna eros quis urna.
.. Nunc viverra imperdiet enim. Fusce est. Vivamus a tellus.
.. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Proin pharetra nonummy pede. Mauris et orci.
.. Aenean nec lorem. In porttitor. Donec laoreet nonummy augue.
.. Suspendisse dui purus, scelerisque at, vulputate vitae, pretium mattis, nunc. Mauris eget neque at sem venenatis eleifend. Ut nonummy.

.. Teste de Nivel 4
.. ################


Painéis Baseados em Fatura
--------------------------

Os Painéis Baeados em Fatura apresentam informações de valores financeiros unicamente referente a um período já encerrado (*Mês anterior*) para o pagamento no mês subsequênte. Podemos usar o mesmo exemplo da fatura de "Cartão de Crédito". Na fatura constam o consumo somente do mês anterior, para o pagamento no mês corrente.

Os valores apresentados nesta opção de menu deve levar em conta que a Plataforma do uCloud possui três tipos de usuários que podemos identificar como ‘perfis básicos’ conforme descritos abaixo:

  A. **Usuários do sistema**: são os usuários regulares que acessam o sistema para consumir os recursos.
  B. **Usuários Administradores de Grupo**: são usuários que estão associados a um grupo de usuários, eles podem provisionar e alterar outros usuários na plataforma.
  C. **Usuários Administradores de Contrato**: são os usuários que estão associados a um contrato e sobre este contrato podem definir regras de bilhetagem, provisionar e alterar outros usuários na plataforma.

Quando um **Usuário do Sistema** inicia uma sessão na Plataforma do uCloud, e possui a permissão de visualizar o Menu Financeiro e a opção Minha Fatura, os valores apresentados nos relatórios se referem somente aos recursos computacionais que este usuário está vinculado e possui permissão de visualizar o menu “Fatura” e os seus custos. Este usuário não possui permissão de visualizar os valores da Fatura de outro usuário, ou do Grupo ao qual este faz parte ou o valor total do Contrato.

Quando um **Usuário Administrador de Grupo** inicia uma sessão na Plataforma do uCloud, os valores apresentados nos relatórios se referem aos valores dos recursos computacionais deste usuário e de todos os usuários que estão vinculados ao Grupo. Este usuário não tem a permissão de visualizar o valor total do Contrato.

Quando um **Usuário Administrador de Contrato** inicia uma sessão na Plataforma do uCloud, os valores apresentados nos relatórios se referem aos valores dos recursos computacionais deste usuário.
Este usuário possui perfil para permissão para visualizar o valor total acumulado do(s) Contrato(s) aos quais seu usuário foi provisionado no campo Administrador. Por consequência este usuário pode visualizar o consumo no(s) grupo(s) que foram vinculados ao(s) contrato(s), e por fim os valores de todos os usuários que estão vinculados aos Grupos.

Para ilustrar este relatório e os seus valores, iremos utilizar uma credencial com o nível de Usuário Administrador de Contrato neste documento. As imagens utilizadas são meramente ilustrativas e servem apenas como exemplo.


Minha Fatura
~~~~~~~~~~~~

Os Painéis Baeados em Fatura apresentam informações de valores financeiros unicamente referente a um período já encerrado (*Mês anterior*) para o pagamento no mês subsequênte. Podemos usar o mesmo exemplo da fatura de "Cartão de Crédito". Na fatura constam o consumo somente do mês anterior, para o pagamento no mês corrente.

Importante ressaltar que este relatório, específicamente, apresenta os valores de consumo mensal dos recursos computacionais referente apenas ao usuário que está com uma sessão ativa na Plataforma uCloud.

Através deste relatório o usuário que possui credencial de acesso válida a Plataforma do uCloud pode acompanhar a evolução dos custos mês a mês.

Quando o usuário clica com o cursor do mouse sobre o botão **Minha Fatura** a Plataforma uCloud apresenta o relatório do mês corrente, a figura abaixo é meramente ilustrativa:

.. image:: /figuras/ucloud_menu_financeiro010a.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

Abaixo descrevemos os quadros deste relatório.

* **Campo Mês Atual**: Este campo apresenta o mês e ano atual que a Plataforma uCloud se baseia para apresentar os valores do mês anterior para pagamento no mês corrente. Para alterar o conteúdo deste campo basta o usuário clicar com o cursor do mouse sobre este campo e a Plataforma uCloud apresenta uma tela *popup* que permite alterar a seleção de mês para consulta das informações deste relatório.

.. image:: /figuras/ucloud_menu_financeiro010n.png
   :alt: Menu Financeiro - Relatorio Visualização de Recursos
   :scale: 80 %
   :align: center
----

Neste ponto o uauário pode selecionar a opção "Mês Passado" para que a plataforma uCloud apresente os valores referentes ao mês anterior.

O usuário pode, também, selecionar qualquer mês e ano, basta clicar com o cursor do mouse sobre o campo indicado com o nome do mês, que a Plataforma uCloud apresenta um lista "dropdown" com os doze mees do ano. COmo opcional, é possível consultar os valores de um mês em ano anterior ao ano corrente.

Por padrao a Plataforma uCloud apresenta os três primeiros quadros:

* **Cotação do dolar**: R$ 1 (em 01/12/2021) R$ 5,581 (em 30/12/2021)

  * **Total**: R$ 1.363,1492
  * **Consumo**: R$ 1.234,58
  * **Créditos**: -R$ 37,0373
  * **Impostos**: R$ 165,6100
  * **Período**: (01/12/2021 - 31/12/2021)

* **Consumo de recursos durante o mês**:

* **Distribuição de recursos durante o mês**:

* **Itens Bilhetados**: QT. 9603
  Total: R$ 1.234,5765
  * **Botão Detalhes*: 

* **Créditos**: QT. 256
  Total: -R$ 37,0373
  * **Botão Detalhes**: 

* **Impostos**: QT. 015
  Total: R$ 165,6100
  * **Botão Detalhes**: 


Financeiro
~~~~~~~~~~

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Maecenas porttitor congue massa. Fusce posuere, magna sed pulvinar ultricies, purus lectus malesuada libero, sit amet commodo magna eros quis urna.
Nunc viverra imperdiet enim. Fusce est. Vivamus a tellus.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Proin pharetra nonummy pede. Mauris et orci.
Aenean nec lorem. In porttitor. Donec laoreet nonummy augue.
Suspendisse dui purus, scelerisque at, vulputate vitae, pretium mattis, nunc. Mauris eget neque at sem venenatis eleifend. Ut nonummy.

* Máquinas Virtuais

* Assinaturas

* Snapshots

* IPs Públicos

* Balanceadores

* Zonas DNS

* VPNs

* Itens não gerenciados


Relatório Consolidado de Faturamento
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Maecenas porttitor congue massa. Fusce posuere, magna sed pulvinar ultricies, purus lectus malesuada libero, sit amet commodo magna eros quis urna.
Nunc viverra imperdiet enim. Fusce est. Vivamus a tellus.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Proin pharetra nonummy pede. Mauris et orci.
Aenean nec lorem. In porttitor. Donec laoreet nonummy augue.
Suspendisse dui purus, scelerisque at, vulputate vitae, pretium mattis, nunc. Mauris eget neque at sem venenatis eleifend. Ut nonummy.


Tendência de faturamento
~~~~~~~~~~~~~~~~~~~~~~~~

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Maecenas porttitor congue massa. Fusce posuere, magna sed pulvinar ultricies, purus lectus malesuada libero, sit amet commodo magna eros quis urna.
Nunc viverra imperdiet enim. Fusce est. Vivamus a tellus.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Proin pharetra nonummy pede. Mauris et orci.
Aenean nec lorem. In porttitor. Donec laoreet nonummy augue.
Suspendisse dui purus, scelerisque at, vulputate vitae, pretium mattis, nunc. Mauris eget neque at sem venenatis eleifend. Ut nonummy.


.. Menu Financeiro (USN)
.. ---------------------

.. Ambiente Governo Brasileiro
.. ---------------------------


.. Menu Financeiro / USN Billing
.. =============================


.. Menu Ordem de Serviço
.. =====================

.. Gerenciando a Ordem de Serviço
.. ------------------------------

.. Seção Geral - Ordem de Serviço
.. ------------------------------

.. Seção Estimativa de Custo (USN)
.. -------------------------------

.. Configuração de Estimativa de Custo (UST)
.. -----------------------------------------


.. De Acordo
.. ---------

Menu Containers
===============

O termo Containers na Plataforma uCloud é utilizado para representar um Hypervisor, seja este público e/ou privado. Um container é uma abstração lógica para agrupar todos os recursos (máquinas virtuais, servidores, discos, storages) de um determinado tipo de hypervisor. Por exemplo, um container privado representa a conexão com uma instância do VMware vCenter, com um Pool do XenSever ou com o Keystone do Openstack.

Em relação aos provedores de serviço de nuvem pública, a Plataforma uCloud está preparada para se conectar com as seguintes plataformas de nuvem pública:

* Amazon Web Services (AWS)
* Google Cloud Platform (GCP)
* Microsoft Azure

Atualmente, a Plataforma uCloud está preparada para se conectar com as seguintes plataformas (hypervisors) de gerenciamento de ambiente de nuvem privada:

* VMware (vCenter Versões 5.0, 5.1, 5.5, 6.0, 6.5, 6.7, 7.x ou superior)
* Hyper-v (Windows 2008R2, Windows 2012, Windows 2012R2 e Windows 2016, ou superior)
* vCloud
* Openstack
* Xen Server
* XCP-NG
* KVM

A Plataforma uCloud, além das funções de CSB, também é um agregador de funcionalidades que permite aos usuários, de forma simples e centralizada, o controle de diversas consoles de gerenciadores de ambientes virtualizados (hypervisors) seja do ambiente privado on-premisses quanto do ambiente de fornecedores de nuvem pública. Agregamos funcionalidades de monitoração, fluxo de trabalho na nuvem (Cloud Work Flow) e implementar um repositório ‘biblioteca’ centralizado de arquivos (playbooks) de referência para uso de ferramentas de infraestrutura como código (Infrastructure as a Code).

Depois do provisionamento de um container, a Plataforma uCloud efetua a ‘importação’ de todas as suas características e recursos computacionais para que o usuário possa interagir neste ambiente através da interface do uCloud. A qualquer momento um container pode ser descontado do uCloud, esta operação é considerada operação interna ao banco do uCloud, por isso não causa nenhuma modificação ou ação no ambiente do cliente. Durante a importação, as máquinas virtuais do container devem ser ‘importadas’ para um Virtual Datacenter (VDC) e, este VDC deve estar desvinculado de qualquer outro container.

Quando o usuário acessa o menu Containers, a Plataforma uCloud apresenta uma lista com os containers provisionados no ambiente do uCloud.

.. image:: /figuras/ucloud_menu_container001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 80 %
   :align: center

----

* **Botão Conectar Container**: Este botão permite ao usuário configurar e conectar um novo container.
* **Botão Refresh**: A Plataforma uCloud se comunica com o console dos provedores através da API Rest, toda ação executada ou configurada, nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes então executem a ação desejada. Ao atualizar apenas o conteúdo das seções de tela (ou as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, em seguida ao clique, a Plataforma uCloud executa apenas a atualização das informações contidas em nossas bases de dados.
* **Nome**: Esta coluna apresenta o nome do container informado e identificado no momento do seu provisionamento na Plataforma uCloud.
* **Endereço do Container**: Esta coluna apresenta o endereço lógico do container, esta informação é extraída automaticamente do ambiente do provedor de serviço de nuvem (público e/ou privado).
* **Tipo**: Esta coluna apresenta o tipo do container, em outras palavras, o tipo do provedor de serviço de nuvem (público/privado) de forma resumida.

Gerenciando um Container
------------------------

Ao selecionar o menu Container, a Plataforma uCloud, apresenta uma extensa tela com diversas seções (card). Para efeito didático, houve um recorte na imagem total da tela, com o objetivo de descrever e detalhar cada seção de forma individual.

.. image:: /figuras/ucloud_menu_container002.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 80 %
   :align: center

----

A seguir a descrição detalhada de cada seção:

* **Botão Sync Container**: Este botão pode ser acionado quando o usuário deseja sincronizar todos os dados referente a ‘importação’ do container de um provedor de serviço de nuvem pública (AWS, Azure, GCP) com a Plataforma uCloud. Importante ressaltar que a sincronização do container é automática, ocorrendo a cada período de duas (02) horas. Este botão pode ser útil ao usuário que deseja ativar a sincronização de forma manual a qualquer instante.
* **Botão Rebuild Consoles**: Este botão pode ser acionado quando o usuário deseja sincronizar todos os dados referente a ‘importação’ do container de um provedor de serviço de nuvem privada (VMware, vCloud, Hyper-v, KVM, Openstack) com a Plataforma uCloud. Este botão pode ser útil ao usuário que deseja ativar a sincronização de forma manual a qualquer instante.
* **Botão Excluir Container**: O usuário deve clicar com o cursor do mouse sobre este botão quando for necessário remover um Container previamente provisionado. Importante ressaltar que a remoção do container irá somente “desconectar” a Plataforma uCloud das credenciais de acesso do provedor de serviço de nuvem (público e/ou privado). Portanto, a exclusão de um Container não expurga (remove) qualquer máquina virtual existente. Quando clicar sobre este botão a Plataforma uCloud solicita a confirmação da remoção do Container.

* **Seção Geral**: Esta seção apresenta as informações básicas referentes ao container, conforme a tela abaixo:

.. image:: /figuras/ucloud_menu_container003.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 80 %
   :align: center

----

  * **Nome**: Este campo apresenta o nome informado pelo usuário no momento da configuração do Container. Veja no documento Manual do Administrador uCloud para detalhes e procedimentos de configuração de um container na Plataforma uCloud.

  * **Provider Name**: Este campo apresenta a identificação genérica do Container informado pelo usuário no momento da configuração do container. Veja no documento Manual do Administrador uCloud para detalhes e procedimentos de configuração de um container na Plataforma uCloud.

  * **Endereço IP**: Este campo apresenta a identificação do Endereço TCP-IP do provedor de serviço de nuvem pública. Este campo é preenchido e atualizado automaticamente pela conexão da Plataforma uCloud com o provedor de serviço de nuvem pública, o usuário não tem nenhuma interação com este conteúdo.

  * **Tipo do Container**: Este campo exibe o nome do tipo do Container que a Plataforma uCloud apresenta na lista tipo “dropdown” selecionado no processo de configuração de um container pelo usuário.

  * **Dono**: Este campo apresenta as credenciais do usuário responsável pelo provisionamento e configuração do container no ambiente da Plataforma uCloud. Importante ressaltar que apenas o usuário com perfil “Administrador” pode efetuar a configuração de um container. Veja no documento Manual do Administrador uCloud para detalhes e procedimentos de configuração de um container na Plataforma uCloud.

  * **Configurações do Financeiro**: Neste campo está representada a configuração de como a Plataforma uCloud deve obter o arquivo de billing do provedor de serviço de nuvem pública (.CSV). Cada provedor (AWS, Azure e GCP) possui uma configuração específica e particular, consultar o documento Manual do Administrador uCloud para detalhes e procedimentos de configuração do billing de um container na Plataforma uCloud. **ATENÇÃO não alterar ou apagar a configuração provisionada neste campo, esta ação irá remover e apagar toda a informação para a obtenção do billing dos recursos computacionais deste provedor de serviço de nuvem**.

  * **Configurações de monitoramento e Kubernetes**: Este campo permite informar uma credencial que permite o monitoramento de recursos computacinais de nuvem, bem como o *token* de acesso para o ambiente de monitoramento Kubernete. **ATENÇÃO Não altere ou apague a informação contida neste campo, esta ação irá desligar e desconectar por completo o ambiente de monitoramento deste container**.

  * **Enviar Alerta de Erro de Faturamento**: Este botão quando ativado irá enviar qualquer mensagem de correio eletrônico, para o email das credenciais informadas no campo Dono acima, nos eventos que a Plataforma uCloud defrontar com qualquer tipo de incoerência (um erro) durante o processo de sincronização do arquivo de billing (.csv) do provedor de serviço de nuvem pública.

  * **Sincronização Automática**: Este botão permite ao usuário selecionar a ativação do processo de sincronização do container de forma automática ou não. Importante mencionar: quando selecionado ‘Auto Sync: Não’ o usuário deve efetuar a sincronização manual das informações do container.

* **Seção Template**: Nesta seção estão listadas todas as opções referente ao recurso computacional template (sistema operacional) específico do provedor de serviço de nuvem pública selecionado. Esta relação não é passível de ser editada nesta tela, pois esta relação é obtida no processo de sincronização do container. O usuário vinculado, como Administrador de Grupo ou Administrador de Contrato, pode restringir a exibição destas opções através da edição de recursos do Virtual Datacenter. Veja o item Editando um Virtual Datacenter.

* **Seção Storages**: Nesta seção estão listadas todas as opções referente ao recurso computacional storage (armazenamento) específico do provedor de serviço de nuvem pública selecionado. Esta relação não é passível de ser editada nesta tela, pois esta relação é obtida no processo de sincronização do container.

* **Seção Flavors**: Nesta seção estão listadas todas as opções referente ao recurso computacional flavor (configuração do hardware da máquina virtual, CPU, memória e disco) específico do provedor de serviço de nuvem pública selecionado. Esta relação não é passível de ser editada nesta tela, pois esta relação é obtida no processo de sincronização do container. O usuário vinculado, como Administrador de Grupo ou Administrador de Contrato, pode restringir a exibição destas opções através da edição de recursos do Virtual Datacenter. Veja o item Editando um Virtual Datacenter.

* **Seção Regiões**: Nesta seção estão listadas todas as opções referente ao recurso computacional Região Global específica do provedor de serviço de nuvem pública selecionado. Esta relação não é passível de ser editada nesta tela, pois esta relação é obtida no processo de sincronização do container. O usuário vinculado como Administrador de Grupo ou Administrador de Contrato, pode restringir a exibição destas opções através da edição de recursos do Virtual Datacenter. Veja o item Editando um Virtual Datacenter.

* **Seção Redes**: Nesta seção estão listadas todas as opções referente ao recurso computacional de rede de dados, específica do provedor de serviço de nuvem pública selecionado. Esta relação não é passível de ser editada nesta tela, pois a relação é obtida no processo de sincronização do container. O usuário vinculado como Administrador de Grupo ou Administrador de Contrato, pode restringir a exibição destas opções através da edição de recursos do Virtual Datacenter. Veja o item Editando um Virtual Datacenter.

* **Seção Políticas de Permissionamento**: Nesta seção é possível criar Políticas de Permissionamento específicas para cada ambiente do provedor de serviço de nuvem pública. Desta forma mesmo que esta seja provisionada através da Plataforma uCloud, a política de permissionamento ficará válida para quaisquer ações efetuadas através da interface da Plataforma uCloud e, também, fica válida para quaisquer ações efetuadas pelo usuário diretamente no console do provedor de serviço de nuvem pública.

* **Seção Máquinas Virtuais**: Nesta seção a Plataforma uCloud apresenta a lista de máquinas virtuais que existiam no ambiente do provedor de serviço de nuvem pública e, durante o processo de provisionamento do container, o usuário Administrador do Contrato selecionou a opção *Importar sem Recursos desligado*. Esta opção desligada indica a Plataforma uCloud para importar todos os recursos computacionais de serviço de nuvem pública exitentes. Desta forma, após a conexão do Container e terminada a sincronização, serão exibidas nesta tabela todas as máquinas virtuais previamente exitentes no ambiente e que ficarão vinculadas a este container. Esta relação de máquinas virtuais poderá ser alterada (adição e remoção) por decorrência de quaisquer alterações no ambiente do provedor de serviço de nuvem pública - sejam estas ações executadas através do console do provedor ou através do provisionamento/operação de recursos computacionais através da interface da Plataforma uCloud.

* **Seção Notificações**: Esta seção apresenta uma relação diária de mensagens (*log*) do ambiente do provedor de serviço de nuvam pública, decorrente da comunicação via API-Rest com a Plataforma uCloud. Esta relação pode ser útil para identificar potenciais problemas de comunicação da Plataform uCloud com o console do provedor de serviço de nuvem pública.


Criando Novo Container
----------------------

O processo de provisionamento de Container é restrito para usuários com perfil Administrdor de Contrato e com permissão de criação de novas credenciais no console do provedor de serviço de nuvem.

Entre em contato com a equipe de Suporte Tecnico (chamados@usto.re) e solicite o acesso a documentação específica do processo de provisionamento de credenciais IAM no console do provedor de serviço de nuvem pública e, também, acesso a documentação do Administrador da Plataforma uCloud, para provisionar um novo container para seu ambiente.


Menu Hosts
==========

O termo “Hosts” na Plataforma uCloud é utilizado para representar um servidor físico (hardware) encarregado de dar suporte e executar um hypervisor on-premises (privado). Portanto, somente após o completo provisionamento do recurso de hardware (physical host - servidor físico) este deve ser provisionado e vinculado a uma nuvem privada (container) na Plataforma uCloud. Por exemplo, um novo servidor privado que seja responsável por executar uma instância do VMware vCenter ou um Pool do XenServer ou com o Keystone do OpenStack.

Atualmente, a Plataforma uCloud está preparada para conectar-se com as seguintes plataformas (hypervisors) de gerenciamento de ambiente de nuvem privada:

* VMware (vCenter Versões 5.0, 5.1, 5.5, 6.0, 6.5, 6.7, 7.x ou superior)
* Hyper-v (Windows 2008R2, Windows 2012, Windows 2012R2 e Windows 2016, ou superior)
* vCloud
* OpenStack versão Mitaka ou superior
* Xen Server versão 7.0 ou superior
* XCP-NG versão 7.5 ou superior
* KVM

Depois do provisionamento de um host, a Plataforma uCloud efetua a ‘importação’ de todas as suas características e dos recursos computacionais, desta forma o usuário pode interagir neste ambiente através da interface do uCloud.

A qualquer momento um host pode ser desconectado da plataforma do uCloud, esta operação é considerada uma operação interna ao banco do uCloud, desta forma não causa modificação ou ação no ambiente do cliente. Durante a importação, as máquinas virtuais do container devem ser ‘importadas’ para um Virtual Datacenter (VDC) e este VDC não pode estar vinculado a qualquer outro container.

Quando o usuário acessar o Menu “Hosts” a Plataforma uCloud exibe a tela abaixo:

.. image:: /figuras/ucloud_menu_hosts001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 80 %
   :align: center

----

Abaixo segue a descrição das colunas desta lista de hosts:

* **Nome**: Esta coluna apresenta o nome do Host informado pelo usuário no momento do seu provisionamento, ele pode apresentar um Endereço TCP-IP para os Hosts que foram identificados no campo ‘Nome’. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no título desta coluna, a Plataforma uCloud permite ao usuário digitar uma sequência de caracteres para limitar a lista de Hosts.
* **IP**: Esta coluna apresenta o Endereço TCP-IP do Host, informado pelo usuário no momento do seu provisionamento. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no título desta coluna, a Plataforma uCloud permite ao usuário digitar uma sequência de caracteres para limitar a lista de Hosts.
* **Nome do Container**: Esta coluna apresenta o nome do Container ao qual o Host está vinculado, no momento do seu provisionamento. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no título desta coluna, a Plataforma uCloud permite ao usuário digitar uma sequência de caracteres para limitar a lista de Hosts.

Visualizando um Host
--------------------

Quando o usuário clica com o cursor do mouse sobre uma das linhas querepresenta um *Host* provisionado a Plataforma uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_menu_hosts002.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 80 %
   :align: center

----

Abaixo descrevemos o conteúdo de cada seção desta tela.

* **Seção General**: Esta seção apresenta os dados iniciais referente ao *host*:
  * **Nome**: Este campo apresenta o nome do *host* que foi informado no momento de seu provisionamento.
  * **Endereço IP**: Este campo apresenta o endereço TCP-IP que foi informado no momento de seu provisionamento.
  * **Container**: Este campo apresenta o nome do *Container - Nuvem* que este host foi vinculado. Este campo é obtido da informação do campo nome do *Container*, que foi informado no momento do provisionamento.
  * **Tipo do Container**: Este campo apresenta a informação do tipo do container, que foi selecionado no momento do provisionamento do *Container*.

* **Seção Custo**: Esta seção apresenta a smatória dos valores de todas as instâncias virtuais (máquinas virtuais) que estão sendo executadas neste respectivo *host*. Os valores das máquinas vão ser calculados, apenas, se o valor do host for cadastrado antes para o mês correspondente.
* **Seção Performance Instantânea**: Esta seção apresenta um gráfico com a informação de ocupação de Memória e vCPUs deste host. No momento inicial de consulta desta tela, a Plataforma uCloud pode não apresentar um gráfico em branco. A Plataforma uCLoud coleta e atualiza a informação de ocupação de memória total e utilização de CPU a cada 5 minutos.
* **Seção Máquinas Virtuais**: Esta seção apresenta a lista de máquinas virtuais que foram provisionadas e existem na infraestrutura do host.

  * **Nome**: Nesta coluna será apresentado o nome da máquina virtual informado no momento da sua criação no console do provedor de serviço de nuvem, ou quando configurado através do uCloud. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de máquinas virtuais de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **Usuário**: Esta coluna apresenta as credenciais do usuário registrado, em uma sessão na Plataforma uCloud, o qual foi o responsável pelo provisionamento da máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **IP Privado**: Esta coluna apresenta o endereço TCP-IP vinculado a esta máquina virtual no momento de sua criação. Importante ressaltar que este endereçamento TCP-IP pertence ao ambiente de rede privada do provedor de serviço de nuvem (recebe do servidor DHCP interno do provedor) e, este endereço, pode mudar quando a máquina virtual for reiniciada (reboot). Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de endereços TCP-IP de forma crescente ou decrescente.
  * **IP Público**: Esta coluna pode estar em ‘branco’, pois nesta coluna é apresentado o endereço TCP-IP Público que foi vinculado a esta máquina virtual em um momento posterior ao provisionamento da máquina virtual. O Endereço TCP-IP Público, é um endereço fixo e pode incorrer em custos mensais para sua manutenção e vinculação a uma máquina virtual provisionada. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **Memória**: Nesta coluna é apresentado o número da quantidade de memória RAM configurada nesta máquina virtual, expressa sempre em Gigabytes. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de máquinas virtuais com base no tamanho da memória de forma crescente ou decrescente.
  * **CPUs**: Nesta coluna é apresentado o número da quantidade de CPU(s) configurada nesta máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de máquinas virtuais com base na quantidade de CPU(s), de forma crescente ou decrescente.
  * **Busca Rápida**: O usuário poderá observar que logo abaixo do nome de cada coluna existe um campo em ‘branco’, este campo permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de eventos de login. Basta preencher o campo em ‘branco’ com uma sequência de caracteres que possam ser relevantes e a Plataforma uCloud atualizará a tela de forma a representar este padrão de busca.


Menu Redes
==========

Esta opção de menu é útil aos usuários da Plataforma uCloud, devido a diversidade de funcionalidades encontradas no seu submenu. Através deste menu o usuário pode criar Subnets, Grupos de Segurança, Par de Chaves, VPN entre outros.

Redes
-----

Ao utilizar este submenu o usuário poderá provisionar novos segmentos de rede TCP-IP, bem como suas respectivas sub-redes para atender ao isolamento de tráfego de projetos ou para atender a demanda da arquitetura lógica de rede de um ambiente de servidores, tanto na nuvem pública quanto na nuvem privada.

A criação de sub-redes auxilia tanto do ponto de vista da segurança da infraestrutura à conectividade entre ambientes virtualizados, quanto sobre otimizar o tráfego de pacotes TCP-IP. A infraestrutura de rede pode ajudar o usuário a obter o máximo da sua nuvem ou ambiente de TI híbrido.

.. attention:: Todas as Redes (e sub-redes) existentes e listadas na tela da Plataforma uCloud são pré-existentes, ou foram provisionadas, nos ambientes do provedor de serviço de nuvem pública e/ou privada. Portanto, qualquer alteração ou exclusão (delete) de uma rede pode afetar o ambiente operacional ou a comunicação entre as máquinas virtuais (as cargas de trabalho),  entre as aplicações instaladas no respectivo ambiente. Portanto, a Plataforma uCloud não tem responsabilidade sobre as ações executadas (através da sua interface) por um usuário registrado no ambiente de rede de um provedor de serviço de nuvem pública e/ou privada.

Gerenciar Rede
--------------

No submenu Redes é permitido gerenciar as redes nos diversos ambientes suportados pela plataforma do uCloud, sejam eles on-premises ou nos provedores de serviço de nuvem pública. Devido ao fato da Plataforma uCloud ser um ambiente híbrido multi-cloud, o usuário pode notar que cada ambiente de nuvem (pública e/ou privada) está representado nesta tela com abas (tabs).

Ao clicar com o cursor do mouse sobre a aba do provedor de nuvem desejado, a Plataforma uCloud apresenta a lista de Redes (e sub-redes) específicas do provedor selecionado:

.. image:: /figuras/ucloud_menu_rede001.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

.. note:: Atenção: para atualizar apenas o conteúdo das seções da tela (ou as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão **Refresh**, ele executa apenas a atualização das informações contidas na base de dados da plataforma do uCloud.

A seguir a descrição e os detalhes com as informações sobre as colunas desta lista:

* **Botão “Criar Rede”**: Caso o usuário necessite criar uma rede no ambiente do provedor de serviço de nuvem (público ou privado), basta clicar com o cursor do mouse sobre este botão, em seguida acompanhar as instruções nos itens abaixo: A. Criar Rede em Provedores de Serviço de Nuvem Pública e B. Criar Rede Privada.

* **Botão Refresh**: A Plataforma uCloud comunica-se com o console dos provedores através da API Rest, portanto, toda ação executada e/ou configurada na plataforma do uCloud passa a ser apresentada imediatamente na tela do usuário, a qual envia as ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada.

* **Nome**: Esta coluna apresenta o nome da rede informada pelo usuário no momento do seu provisionamento. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no título desta coluna, a Plataforma uCloud permite ao usuário digitar uma sequência de caracteres para limitar a lista de redes.

* **Subnets**: Esta coluna apresenta uma lista de todas as sub-redes provisionadas para esta rede, no momento da sua criação. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no título desta coluna, a Plataforma uCloud permite ao usuário digitar uma sequência de números para limitar a lista de sub-redes.

* **Região**: Esta coluna apresenta a Região Global do provedor de serviço de nuvem pública, na qual a Rede e suas sub-redes estão vinculadas. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no título desta coluna a plataforma do uCloud permite ao usuário digitar uma sequência de caracteres para limitar a lista de regiões.

* **Ação**: Esta coluna apresenta dois ícones, os quais permitem ao usuário interação com a Rede selecionada:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova esta Rede (e sub-redes) de forma imediata e definitiva. Esta ação é efetivada no ambiente de rede selecionado (público e/ou privado) e o tempo necessário para que a referida ação seja aplicada será totalmente dependente do tempo do ambiente destino (público e/ou privado), a Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - Consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada.
  * **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela que permite editar as configurações da respectiva Rede, conforme a tela abaixo.

.. image:: /figuras/ucloud_menu_rede002.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

Abaixo a descrição das seções presentes nesta tela:

.. attention:: Para atualizar apenas o conteúdo das seções da tela (ou as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, ele executa apenas a atualização das informações contidas na base de dados da plataforma do uCloud.

* **Seção Geral**: Esta seção apresenta as informações genéricas da rede que foram informadas pelo usuário no momento do seu provisionamento:

  * **Nome**: Neste campo consta o nome informado pelo usuário, para identificar esta rede no ambiente do provedor de serviço de nuvem (público e/ou privado).
  * **CIDR (exclusivo AWS)**: Este campo será exibido, exclusivamente, para as Redes da aba (tab) AWS, ele apresenta o CIDR informado no momento do provisionamento da Rede pelo usuário no ambiente da AWS.
  * **Tipo**: Para as redes criadas nos provedores de serviço de nuvem pública, este campo será sempre identificado com a etiqueta “NONE” ela indica que trata-se de um tipo de rede pública controlada pelo ambiente do provedor de serviço de nuvem pública. Para as redes criadas nos ambientes privados (on-premises) este campo será nomeado com a etiqueta “VLAN”, que identifica que esta é uma rede virtual criada através da interface com o SDN (Software Defined Network).
  * **Nome do Container**: Este campo apresenta o nome do container ao qual a Rede está vinculada.
  * **Internet Gateway (exclusivo AWS)**: Este campo será exibido somente para Redes da aba (tab) AWS, ele apresenta a etiqueta que identifica se a rede está conectada a um Internet Gateway no ambiente da AWS. Esta etiqueta pode representar que a conexão ao Gateway está ativa (Enable) ou inativa (Disable).
  * **Botão Habilitar/Desabilitar (exclusivo AWS)**: Este botão é um tipo “checkbox” que o usuário pode operar para trocar o seu modo atual. A cor verde indica que a conexão com Gateway está HABILITADA. A cor vermelha indica que a conexão com o Gateway está DESABILITADA. Para alternar entre os estados, basta clicar com o cursor do mouse e o campo será ativado apresentando a cor verde (habilitado). Estando na cor verde, basta clicar com o mouse e o campo será desativado exibindo a cor vermelha (desabilitado).

* **Seção Sub Redes**: Nesta seção são apresentadas as especificações técnicas da rede e sua(s) respectiva(s) sub-rede(s).

  * **Botão Refresh**: A Plataforma uCloud comunica-se com o console dos provedores através da API Rest, portanto, toda ação executada e/ou configurada na plataforma do uCloud passa a ser exibida imediatamente na tela do usuário, a qual envia as ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada.
  * **Botão “Adicionar Sub-Rede”**: Caso o usuário necessite criar uma sub-rede no ambiente do provedor de serviço de nuvem (público ou privado), basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud apresenta a tela seguinte ao usuário, é indicado acompanhar as instruções nos itens abaixo:
  * **Nome (válido para todas Redes)**: Esta coluna apresenta o nome da sub-rede informado pelo usuário no momento do seu provisionamento.
  * **CIDR (válido para todas Redes)**: Este campo apresenta a máscara do endereçamento TCP-IP da sub-rede, informado pelo usuário no momento do seu provisionamento. Esta máscara está representada conforme o padrão definido na RFC 1519.

    No caso do usuário clicar com o cursor do mouse em qualquer um dos CIDR apresentados nesta lista, a Plataforma uCloud apresenta uma tela que relaciona o nome das máquinas virtuais que estão associadas a esta Subnet, seus respectivos endereços MAC e TCP-IP, veja o exemplo abaixo:

.. image:: /figuras/ucloud_menu_rede003.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

    * **Zona de Disponibilidade (exclusivo AWS)**: Esta coluna será apresentada exclusivamente para as redes da aba (tab) AWS, ela apresenta a Região Global na qual a sub-rede está vinculada, selecionada no momento do provisionamento realizado pelo usuário no ambiente da AWS.

    * **Range-Start (apenas Azure & GCP)**: Esta coluna apresenta o endereço TCP-IP inicial da sub-rede informada pelo usuário no momento do provisionamento.

    * **Range-End (apenas Azure & GCP)**: Esta coluna apresenta o endereço TCP-IP final da sub-rede informada pelo usuário no momento do provisionamento.

    * **Gateway (apenas Azure & GCP)**: Esta coluna apresenta o endereço TCP-IP do Gateway de rede informado pelo usuário no momento do provisionamento da sub-rede.

    * **Conectar ao SDN (apenas Azure & GCP)**: Esta coluna apresenta a informação se a sub-rede permanece conectada ao endereço TCP-IP do servidor que está executando o software do SDN.

    * **Ações (válido para todas as redes)**: Esta coluna apresenta dois ícones para que o usuário possa interagir com a sub-rede selecionada:

       * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para a Plataforma uCloud remover esta sub-rede de forma imediata e definitiva. Esta ação será efetivada no ambiente de rede selecionado (público e/ou privado), o tempo necessário para que a referida ação seja aplicada será totalmente dependente do tempo do ambiente destino (público e/ou privado). A Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - Consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada.

       * **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone para que a Plataforma uCloud possa alternar todos os campos das colunas para o modo edição, de forma que o usuário possa corrigir o conteúdo dos campos e alterar as configurações da respectiva Sub-Rede. ATENÇÃO: Importante ressaltar que qualquer alteração das configurações de uma sub-rede, gerará impacto nos ambientes computacionais, nas máquinas virtuais vinculadas a esta sub-rede, nas comunicações entre aplicações e o acesso dos usuários (tanto às máquinas virtuais, como às aplicações por estas executadas). A Plataforma uCloud não pode ser responsabilizada por problemas que possam derivar desta ação.

       * **Ícone de Confirmação** |icone_confirma|: Quando o usuário deseja confirmar a intenção de alterar o conteúdo do campo escolhido, a Plataforma uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma uCloud.

       * **Ícone de Cancelamento** |icone_cancela|: No caso do usuário clicar sobre o ícone de edição, por engano ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o botão vermelho. O botão vermelho cancela as alterações e o conteúdo do campo retorna para os valores iniciais, antes de proceder qualquer preenchimento ou alteração.

* **Seção Contratos Associados**: Esta seção apresenta informações referente à vinculação da da Rede ao Virtual Datacenter que está presente no contrato. Portanto, esta vinculação é indireta.

  * **Nome**: Este campo apresenta o nome do contrato no qual a Rede está vinculada através da associação ao Virtual Datacenter e ao qual esta Rede pertence.

* **Botão “Adicionar Sub-Rede”**: Caso o usuário necessite criar uma sub-rede no ambiente do provedor de serviço de nuvem (público ou privado), basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud apresenta as telas específicas para cada provedor específico (AWS, Azure, GCP, VMware) basta acompanhar as instruções abaixo.

Adicionar “Sub-Rede” no ambiente AWS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A seguir a descrição dos campos a provisionar uma “Sub-rede” no ambiente AWS selecionado:

.. image:: /figuras/ucloud_menu_rede004.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar esta Sub-Rede. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **CIDR**: Este campo é obrigatório, o usuário deve informar a máscara do endereçamento TCP-IP. O endereçamento CIDR usa a notação ‘/’ (barra) para indicar a quantidade de bits que o usuário deseja identificar na rede e, por consequência, a quantidade de bits que identificam hosts dentro da rede. (por exemplo: 192.1.0.0/23)
* **Zona de Disponibilidade**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud lista todas as Zonas de Disponibilidade livres para o ambiente da AWS.
* **Descrição**: Este campo é opcional e de livre digitação, seu conteúdo pode ser utilizado para descrever o objetivo da Sub-Rede.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de uma Sub-rede. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação da Sub-Rede no ambiente AWS, o botão Criar alterna para o modo ativo (cor verde). Ao clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento de uma Sub-Rede. Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, a Plataforma uCloud não permite o provisionamento da Sub-Rede.

Adicionar “Sub-Rede” no ambiente Azure
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A seguir a descrição dos campos para provisionar uma “sub-rede” no ambiente AZURE selecionado:

.. image:: /figuras/ucloud_menu_rede004b.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar esta Sub-Rede. Sugerimos utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **CIDR**: Este campo é obrigatório, o usuário deve informar a máscara do endereçamento TCP-IP. O endereçamento CIDR usa a notação ‘/’ (barra) para indicar a quantidade de bits que o usuário deseja identificar na rede e, por consequência, a quantidade de bits que identificam hosts dentro da rede. (por exemplo: 192.1.0.0/23)
* **Range Start**: Este campo é obrigatório, o usuário deve informar o primeiro endereço TCP-IP (inicial) a ser provisionado para esta sub-rede.
* **Range End**: Este campo é obrigatório, o usuário deve informar o último endereço TCP-IP (final) a ser provisionado para esta sub-rede.
* **Gateway**: Este campo é obrigatório, o usuário deve informar o endereço TCP-IP do Gateway para esta sub-rede.
* **Botão Cancelar**: O usuário pode acionar este botão para cancelar o processo de criação de uma Sub-Rede. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação da Sub-Rede no ambiente AWS, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento de uma Sub-Rede. Caso este botão não esteja habilitado (cor cinza), significa que o usuário deixou de preencher algum parâmetro, logo a Plataforma uCloud não permite o provisionamento da Sub-Rede até que tudo esteja preenchido.

Adicionar “Sub-Rede” no ambiente GCP
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A seguir a descrição dos campos a provisionar uma “Sub-Rede” no ambiente GCP selecionado:

.. image:: /figuras/ucloud_menu_rede004c.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar esta Sub-Rede. Sugerimos utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **CIDR**: Este campo é obrigatório, o usuário deve informar a máscara do endereçamento TCP-IP. O endereçamento CIDR usa a notação ‘/’ (barra) para indicar a quantidade de bits que o usuário deseja identificar na rede e, por consequência, a quantidade de bits que identificam hosts dentro da rede. (por exemplo: 192.1.0.0/23)
* **Range Start**: Este campo é obrigatório, o usuário deve informar o primeiro endereço TCP-IP (inicial) a ser provisionado para esta sub-rede.
* **Range End**: Este campo é obrigatório, o usuário deve informar o último endereço TCP-IP (final) a ser provisionado para esta sub-rede.
* **Gateway**: Este campo é obrigatório, o usuário deve informar o endereço TCP-IP do Gateway para esta sub-rede.
* **SDN Interface IP**: Este campo é obrigatório, o usuário deve informar o endereço TCP-IP do Gateway SDN específico da Google Cloud Platform (GCP). *Consultar a documentação online do ambiente da GCP para entender as características do ambiente de Nuvem Privada Virtual (Virtual Private Cloud - VPC) GCP e como a infraestrutura de rede VPC do Google Cloud é desenvolvida com base em um modelo de rede definida por software (SDN, na sigla em inglês)*.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de uma Sub-Rede. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação da Sub-Rede no ambiente AWS, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento de uma Sub-Rede. Caso este botão não esteja habilitado (cor cinza), significa que o usuário deixou de preencher algum parâmetro, logo a Plataforma uCloud não permite o provisionamento da Sub-Rede até que tudo esteja preenchido.

Adicionar “Sub-Rede” no ambiente Privado (ex.: VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A seguir a descrição dos campos a provisionar uma “Sub-Rede” no ambiente privado VMWare:

.. image:: /figuras/ucloud_menu_rede004d.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

* **Edit Subnet**: Quando o usuário inicia a criação de uma rede privada, a Plataforma uCloud integrada com o módulo uSDN, preenche os campos desta tela de forma automática com configurações pré-definidas. Caso o usuário necessite alterar as configurações automáticas, deve clicar com o cursor do mouse sobre este campo tipo “checkbox”, ao ser selecionado permite editar os campos da tela com as configurações desejadas, desde que o perfil do usuário que está logado permita proceder a alteração.
* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar esta Sub-Rede. A sugestão é utilizar apenas os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **CIDR**: Este campo é obrigatório, o usuário deve informar a máscara do endereçamento TCP-IP. O endereçamento CIDR usa a notação ‘/’ (barra) para indicar a quantidade de bits que o usuário deseja identificar na rede e, por consequência, a quantidade de bits que identificam hosts dentro da rede. (por exemplo: 192.1.0.0/23)
* **Range Start**: Este campo é obrigatório, o usuário deve informar o primeiro endereço TCP-IP (inicial) a ser provisionado para esta Sub-rede.
* **Range End**: Este campo é obrigatório, o usuário deve informar o último endereço TCP-IP (final) a ser provisionado para esta Sub-rede.
* **Gateway**: Este campo é obrigatório, o usuário deve informar o endereço TCP-IP do Gateway para esta Sub-rede.
* **Conectar ao SDN**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse no botão Conectar ao SDN a Plataforma uCloud apresenta as duas opções disponíveis:

  * **TRUE**: Esta opção quando selecionada confirma que o módulo do uSDN gerenciará o provisionamento da Sub-Rede na rede local do Data Center Privado.
  * **FALSE**: Esta opção quando selecionada confirma que as configurações de rede informadas, já existem no ambiente de rede do usuário e este provisionamento não será gerenciado através do módulo do uSDN. *ATENÇÃO: é importante ressaltar a recomendação para entrar em contato com a área de Suporte Técnico da Ustore antes de selecionar esta opção, pois o controle desta Sub-rede será de inteira responsabilidade da área técnica da empresa usuária da Plataforma uCloud*.

* **Descrição**: Este campo é opcional e de livre digitação, seu conteúdo pode ser utilizado para descrever o objetivo da Sub-Rede.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de uma Sub-Rede. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação da Sub-Rede no ambiente AWS, o botão ‘Criar’ alterna para o modo ativo (cor verde). Ao clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento de uma Sub-Rede.Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, a Plataforma uCloud não permite o provisionamento da Sub-Rede.

.. note:: Este manual não tem o objetivo de documentar todos os outros ambientes de redes privadas, favor entrar em contato com o suporte da Ustore para esclarecimentos detalhados específicos do seu ambiente privado.

Criar Nova Rede
---------------

Conforme mencionado acima, o usuário pode provisionar novos segmentos de rede TCP-IP bem como suas respectivas sub redes para atender ao isolamento de tráfego de projetos ou para atender a demandas de arquitetura lógica de rede de um ambiente de servidores, tanto na nuvem pública quanto na nuvem privada. A Plataforma uCloud conecta-se diretamente, via API-Rest, com o ambiente dos provedores de serviço de nuvem pública e envia tarefas a estes ambientes para provisionar novas redes em seus respectivos espaços.

De natureza igual a acima mencionada, para ambientes on-premises o uCloud possui o módulo uSDN que é uma solução Ustore para a função de SDN/NFV (Software Defined Network / Network Function Virtualization [2]_) que tem a incumbência de ser a interface com os elementos de gestão de redes do hypervisors em Data Center Privados suportados pelo uCloud. Este módulo permite a gestão de segmentos de redes. Importante ressaltar que sem a presença do módulo uSDN a plataforma do uCloud não possui a capacidade de “Criar Redes” em ambientes privados.

No momento que o usuário clica com o cursor do mouse sobre o botão “Criar Rede”, a plataforma do uCloud inicia o processo solicitando ao usuário o container, conforme o exemplo da tela abaixo:

.. image:: /figuras/ucloud_menu_rede005.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

Importante ressaltar que alguns provedores de serviço de nuvem pública não solicitam o endereçamento TCP-IP inicial, após a criação da rede o usuário deve acionar quantas sub-redes forem necessárias para acomodar seu ambiente computacional de rede TCP-IP.

Abaixo segue a descrição de ambos processos de criação de redes, tanto em ambientes de provedores de serviço de nuvem pública quanto nos ambientes de redes privadas.


.. [2] *A virtualização de funções de rede (Network Functions Virtualization - NFV) é uma maneira de virtualizar serviços de rede, como roteadores, firewalls e balanceadores de carga, que tradicionalmente são executados em hardware proprietário*.

Criar Rede em Provedores de Serviço de Nuvem Pública
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para criar uma nova rede na AWS, o usuário deve solicitar a opção ‘Criar Rede’ e indicar:

a. o container no qual deve ser associado esta nova rede;
b. o nome da rede;
c. o CIDR associado a esta rede;
d. a região na qual esta rede será criada.

Após o procedimento acima, o usuário deve criar uma sub-rede dentro da rede que foi criada. Deste modo ele deve informar:

a. nome da sub-rede;
b. CIDR da mesma;
c. Zona de disponibilidade;
d. e uma descrição sobre a mesma.

Alguns provedores de rede pública exigem que outras informações sejam passadas para a criação das redes. O uCloud possui botões e labels explicativos para estes casos.


Criar Rede em Ambiente Privado (On-Premisses)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para ambientes on-premisses, o uCloud possui um módulo próprio de SDN/NFV que se comunica com os elementos de gestão de redes dos hypervisors suportados pelo uCloud que permite a gestão de segmentos de redes.

Neste caso, ao selecionar a opção ‘Criar rede’ o usuário deve informar:

* o container a ser utilizado;
* o tipo de isolamento da rede, normalmente VLAN;
* o nome a ser atribuído ao segmento de rede;
* Se quiser especificar um VLAN ID pre-configurado no uCloud, deve marcar a opção editar VLAN ID. Se não fizer, o uCloud seleciona uma VLAN da sua lista de VLANs.

Após esta etapa o usuário deverá solicitar a criação da sub-rede dentro da rede criada. Neste caso, precisa informar:

* Nome da sub-rede;
* CIDR a ser utilizado. É possível, redes distintas terem o mesmo CIDR;
* Range Start, endereço de IP inicial pertencente ao CIDR que será utilizado para a alocação;
* Range End, endereço de IP final pertencente ao CIDR que será utilizado para a alocação;
* Gateway, endereço IP do gateway a ser utilizado;
* Conectar ao SDN, no caso desta sub-rede estar ou não conectada ao módulo de SDN/NFV da Ustore;
* Descrição da sub-rede.

.. image:: /figuras/ucloud_menu_rede006.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----


Criar Rede em Provedores de Serviço de Nuvem Público (AWS)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Caso o usuário necessite selecionar um ambiente na AWS para provisionar uma nova rede, a tela será alterada conforme os campos exibidos abaixo:

.. image:: /figuras/ucloud_menu_rede007.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

A seguir a descrição detalhada dos campos da tela apresentada:

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) que deseja identificar esta Rede. A sugestão é utilizar apenas os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres especiais, de pontuação ou caracteres acentuados (ASCII Estendido).

* **CIDR**: Este campo é obrigatório, o usuário deve informar a máscara do endereçamento TCP-IP. O endereçamento CIDR usa a notação ‘/’ (barra) para indicar a quantidade de bits que o usuário deseja identificar na rede e, por consequência, a quantidade de bits que identificam hosts dentro da rede. (por exemplo: 192.1.0.0/23)

* **Região**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud lista todas as Regiões Globais do ambiente da AWS.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de uma Rede. A Plataforma uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação da Rede no ambiente AWS, o botão Criar alterna para o modo ativo (cor verde). Ao clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento de uma Rede. Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, a Plataforma uCloud não permite o provisionamento da Rede.

Criar Rede em Provedores de Serviço de Nuvem Público (Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Caso o usuário necessite selecionar um ambiente na Azure para provisionar uma nova rede, antes de iniciar o processo de criação a Plataforma uCloud apresenta uma mensagem de aviso informando ao usuário não efetuar a criação de novas redes em regiões em que sua assinatura dos serviços deste provedor não esteja vinculada:

.. image:: /figuras/ucloud_menu_rede008a.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

Muito importante o objetivo da mensagem acima, pois a API deste provedor pode bloquear a tentativa de criação de uma nova rede em regiões diferentes. Após o usuário clicar com o cursor do mouse sobre o botão “OK” a plataforma do uCloud exibe a tela abaixo:

.. image:: /figuras/ucloud_menu_rede008.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

A seguir a descrição detalhada dos campos da tela exibida acima:

* **Virtual Datacenter**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud lista todos os Virtual Datacenters provisionados na Plataforma uCloud. Importante ressaltar que o usuário deve selecionar um Virtual Datacenter que esteja vinculado ao ambiente Microsoft Azure, pois todos os provedores de serviço de nuvem devem ser apresentados na lista. Recomendamos muita atenção para evitar criar uma rede que corre o risco de não ser visualizada no ambiente Azure, posteriormente.

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar esta Rede. A sugestão é utilizar apenas os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres especiais, de pontuação ou caracteres acentuados (ASCII Estendido).

* **CIDR**: Este campo é obrigatório, o usuário deve informar a máscara do endereçamento TCP-IP. O endereçamento CIDR usa a notação ‘/’ (barra) para indicar a quantidade de bits que o usuário deseja identificar na rede e, por

* **Região**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud lista todas as Regiões Globais do ambiente da AWS.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de uma Rede. A Plataforma uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação da Rede no ambiente AWS, o botão ‘Criar’ alterna para o modo ativo (cor verde). Ao clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento de uma Rede. Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, a Plataforma uCloud não permite o provisionamento da Rede.

Criar Rede em Provedores de Serviço de Nuvem Público (GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Caso o usuário necessite selecionar um ambiente na GCP para provisionar uma nova rede, a tela será alterada com apresentada conforme os campos exibidos abaixo:

.. image:: /figuras/ucloud_menu_rede009.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

A seguir a descrição detalhada dos campos da tela exibida acima:

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) que deseja identificar esta Rede. A sugestão é utilizar apenas os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres especiais, de pontuação ou caracteres acentuados (ASCII Estendido).

* **Região**: Este campo é obrigatório, do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud lista todas as Regiões Globais do ambiente da GCP.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de uma Rede. A Plataforma uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação da Rede no ambiente AWS, o botão ‘Criar’ alterna para o modo ativo (cor verde). Ao clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento de uma Rede. Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, a Plataforma uCloud não permite o provisionamento da Rede.


Criar Rede em Ambiente Privado (ex: VMware)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para ambientes on-premises o uCloud possui o módulo uSDN que é uma solução Ustore para a função de SDN/NFV (Software Defined Network / Network Function Virtualization [2]_) que tem a incumbência de ser a interface com os elementos de gestão de redes do hypervisors em Data Center Privados suportados pelo uCloud. Este módulo permite a gestão de segmentos de redes.

.. image:: /figuras/ucloud_menu_rede010.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-shadow

----

Neste caso ao selecionar a opção de criação de redes o usuário deve informar:

* **Tipo de Isolamento**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta a opção para este ambiente (neste caso VMware) é obrigatório selecionar a opção VLAN.
* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) que deseja identificar esta Rede. A sugestão é utilizar apenas os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres especiais, de pontuação ou caracteres acentuados (ASCII Estendido).
* **VLAN ID**: Este campo é opcional, pois a conexão da Plataforma uCloud com o módulo do uSDN, deve assinalar a próxima identificação disponível configurada no ambiente privado de rede corporativa.
* **Edit VLAN ID**: Quando o usuário inicia a criação de uma rede privada, a Plataforma uCloud integrada com o módulo uSDN, preenche os campos desta tela de forma automática com as configurações pré-definidas. Caso o usuário necessite configurar uma VLAN ID específica, este deve clicar com o cursor do mouse sobre o campo tipo “checkbox”, quando selecionado permite ao usuário editar os campos anteriores com as configurações desejadas, desde que o perfil do usuário logado permita proceder a alteração.

Após esta etapa o usuário deve iniciar o provisionamento de uma Sub-rede dentro da Rede Privada criada. Neste caso deve preencher o que segue abaixo:

.. image:: /figuras/ucloud_menu_rede011.png
   :alt: Menu Rede - Exemplo
   :scale: 80 %
   :align: center
   :class: with-border

----

* **Nome**: Este campo é obrigatório, o usuário deve informar o nome (no mínimo 3 caracteres) que deseja identificar a Sub-rede. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).

* **CIDR**: Este campo é obrigatório, o usuário deve informar a máscara do endereçamento TCP-IP. O endereçamento CIDR usa a notação ‘/’ (barra) para indicar a quantidade de bits que o usuário deseja identificar na Sub-rede e, por consequência, a quantidade de bits que identificam hosts dentro da Sub-rede. (por exemplo: 192.1.0.0/23)

* **Range Start**: Este campo é obrigatório, o usuário deve informar o primeiro endereço TCP-IP (inicial) a ser provisionado para esta Sub-rede.

* **Range End**: Este campo é obrigatório e o usuário deve informar o último endereço TCP-IP (final) a ser provisionado para esta Sub-rede.

* **Gateway**: Este campo é obrigatório, o usuário deve informar o endereço TCP-IP do Gateway para esta Sub-rede.

* **Conectar ao SDN**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse no botão Conectar ao SDN a Plataforma uCloud apresenta as duas opções disponíveis:

  * **TRUE**: Esta opção quando selecionada confirma que o módulo do uSDN gerenciará o provisionamento da Sub-Rede na rede local do Data Center Privado.
  * **FALSE**: Esta opção quando selecionada confirma que as configurações de rede informadas, já existem no ambiente de rede do usuário e este provisionamento não será gerenciado através do módulo do uSDN. *ATENÇÃO: é importante ressaltar a recomendação para entrar em contato com a área de Suporte Técnico da Ustore antes de selecionar esta opção, pois o controle desta Sub-rede será de inteira responsabilidade da área técnica da empresa usuária da Plataforma uCloud*.

* **Descrição**: Este campo é opcional e de livre digitação, seu conteúdo pode ser utilizado para descrever o objetivo da Sub-Rede.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de uma Sub-Rede. A Plataforma uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação da Sub-Rede no ambiente AWS, o botão ‘Criar’ alterna para o modo ativo (cor verde). Ao clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud envia todos os parâmetros para o ambiente da AWS, para o completo provisionamento de uma Sub-Rede. Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, e a Plataforma uCloud não permite o provisionamento da Sub-Rede.

.. note:: *Este manual não tem o objetivo de documentar todos os outros ambientes de redes privadas, favor entrar em contato com o suporte da Ustore para esclarecimentos detalhados específicos do seu ambiente privado*.

IPs Públicos
------------

O menu **IPs Públicos** permite ao usuário do uCloud solicitar um endereço IP Público que será dedicado para o mesmo em um provedor de nuvem pública ou nos ambientes on-premisses. Este usuário pode associar o endereço IP solicitado a qualquer Máquina Virtual (VM) que esteja sob a sua gestão.

.. image:: /figuras/ucloud_ip_publico001.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

O submenu IPs Públicos permite ao usuário da Plataforma uCloud provisionar e vincular um Endereço TCP-IP Público e ‘Estático’, do provedor de serviço de nuvem pública, a uma máquina virtual do mesmo ambiente, de forma dedicada e estática.

Este Endereço TCP-IP pertence unicamente ao ambiente de rede do provedor de serviço de nuvem pública, carrega um custo mensal após a solicitação deste, mesmo que este Endereço TCP-IP não esteja associado a uma máquina virtual ativa. Uma característica importante é que nenhum usuário tem qualquer forma de interferir ou permissão para alterar as características deste Endereço TCP-IP.

Como esclarecimento, após o processo de provisionamento de uma máquina virtual, esta recebe automaticamente um endereço TCP-IP ‘flutuante/aleatório’, do ambiente do provedor de serviço de nuvem pública (via DHCP interno). A característica deste endereço ‘flutuante’ é que sempre será um Endereço TCP-IP diferente a cada processo de reinício (reboot) da máquina virtual.

Após o provisionamento do Endereço TCP-IP Público, o usuário pode associar este a qualquer máquina virtual, tendo em vista que este usuário tem a permissão de gerenciar.

.. attention:: Importante ressaltar que todas as ações relativas a endereços TCP-IP Público podem gerar impacto nos ambientes computacionais, nas máquinas virtuais que utilizam os Endereços TCP-IP Públicos. A ação de remover um endereço público retorna a máquina virtual para um Endereço IP Privado e "dinâmico (DHCP)", logo pode haver problemas para se conectar com o console desta máquina virtual, nas comunicações entre as aplicações e o acesso dos usuários (tanto às máquinas virtuais, como as aplicações por estas executadas). A Plataforma uCloud não pode ser responsabilizada por problemas que possam resultar devido a ação de remover um endereço TCP-IP Público de uma máquina virtual.

Quando o usuário acessar esta tela, a Plataforma uCloud apresenta uma lista com todos os provedores de serviço de nuvem (pública e/ou privada), os quais o usuário registrado na plataforma do uCloud tem a permissão de gerenciar.

.. image:: /figuras/ucloud_ip_publico002.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

A seguir a descrição detalhada das colunas e campos da tela exibida acima:

* **Botão Solicitar IP Público**: Basta clicar com o cursor do mouse para efetuar a solicitação de um Endereço TCP-IP Público, o processo está descrito abaixo, no item Solicitando um IP Público.

* **Botão Refresh**: A Plataforma uCloud comunica-se com o console dos provedores através da API Rest, portanto, toda ação executada e/ou configurada na plataforma do uCloud passa a ser exibida imediatamente na tela do usuário, a qual envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada.

* **Nome do Container**: Esta coluna apresenta o nome registrado para o Container. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no campo "Busca Rápida - abaixo do título da coluna", a Plataforma uCloud lista todos os Containers que o usuário registrado está vinculado, para restringir a lista de Endereços TCP-IP Públicos específicos do Container selecionado.

* **IP Público**: Esta coluna pode estar em "branco", pois nesta coluna será apresentado o Endereço TCP-IP Público que foi solicitado para ser provisionado. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.

* **IP Privado**: Esta coluna apresenta o endereço TCP-IP vinculado a esta máquina virtual no momento da sua criação. Importante ressaltar que este endereçamento TCP-IP pertence ao ambiente de rede privada do provedor de serviço de nuvem (recebe do servidor DHCP interno do provedor). Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de endereços TCP-IP de forma crescente ou decrescente.

* **Máquina Virtual**: Esta coluna apresenta o nome da máquina virtual informado no momento da sua criação no console do provedor de serviço de nuvem, ou na etapa de configuração por meio da plataforma do uCloud. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de máquinas virtuais de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Grupo de Segurança**: Esta coluna apresenta o nome do Grupo de Segurança vinculado à máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de Grupos de Segurança de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Usuário**: Esta coluna apresenta o nome do usuário registrado na Plataforma uCloud que solicitou o Endereço TCP-IP Público. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Ações**: Esta coluna apresenta três opções de ação a ser realizada pelo usuário por intermédio dos ícones e ele possa interagir com o Endereço TCP-IP Público selecionado:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud remove (exclui) este Endereço TCP-IP Público do ambiente do provedor de serviço de nuvem (pública e/ou privada), de forma imediata e definitiva.

  Este ícone é apresentado somente para os Endereços TCP-IP Públicos, os que não estão associados a qualquer máquina virtual. O tempo necessário para que a referida ação seja aplicada é totalmente dependente do tempo do ambiente destino (público e/ou privado), a Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada. Além disso, esta ação remove o custo recorrente do recurso da conta do provedor de serviço de nuvem (pública e/ou privada).

  Quando o usuário clicar com o cursor do mouse sobre este ícone “Lata de Lixo” a Plataforma uCloud apresenta uma tela para confirmar a ação do usuário.

  * **Ícone de Desassociar da VM** |icone_desassocia_vm|: Basta o usuário clicar sobre este ícone para que a Plataforma uCloud desvincule o Endereço TCPIP Público da máquina virtual, de forma definitiva e imediata. Esta ação não remove o custo recorrente do recurso da conta do provedor de serviço de nuvem (pública e/ou privada) e, não apaga o Endereço TCP-IP Público do ambiente do provedor de serviço de nuvem (pública e/ou privada).
    Quando o usuário clicar com o cursor do mouse sobre este ícone, a Plataforma uCloud apresenta uma tela e uma pergunta, para confirmar a ação do usuário.

  * **Ícone de Associar a VM** |icone_associa_vm|: Basta o usuário clicar com o cursor do mouse sobre este ícone quando for necessário associar o Endereço TCP-IP Público a uma máquina virtual. Quando selecionado o ícone desejado, a Plataforma uCloud apresenta uma tela abaixo, a qual deve ser preenchida para efetuar a associação:

.. image:: /figuras/ucloud_ip_publico003.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

A seguir a descrição dos campos a serem preenchidos para associar IP Público:

.. note:: Somente usuários com perfil de Administrador de Grupo ou Administrador de Contrato, tem permissão e podem completar esta operação.

* **Usuário**: Este campo é obrigatório, ele aparece preenchido com o login do usuário registrado corrente na Plataforma uCloud. Este usuário é utilizado como referência para filtrar as máquinas virtuais específicas que foram provisionadas por este, no campo abaixo. Se for necessário alterar a vinculação ao usuário, basta clicar com o cursor do mouse sobre o botão de Edição “ ” e digitar os caracteres que fazem parte do login do usuário que deve ser vinculado a este Grupo de Segurança, em seguida, a Plataforma uCloud apresenta uma lista de logins de usuário que possuem a sequência de caracteres digitado, basta selecionar o login desejado da lista.

* **Máquina Virtual**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta a relação de máquinas virtuais criadas pelo login do usuário, informado no campo anterior. É necessário selecionar a máquina virtual desejada, o usuário deve clicar com o cursor do mouse no botão ‘cor verde’ para confirmar a associação do Endereço TCP-IP Público com a máquina virtual. O tempo necessário para que a referida ação seja aplicada será totalmente dependente do tempo do ambiente destino (público e/ou privado). A Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - Consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada.

* **Busca Rápida**: O usuário pode notar que logo abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de Endereços TCP-IP Públicos. Basta preencher o campo em branco com uma sequência de caracteres que possa ser relevante e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca.

Solicitando um IP -Público (**AWS e GCP**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Quando o usuário clica com o cursor do mouse sobre o botão Solicitar IP Público a plataforma do uCloud apresenta a seguinte tela:

.. image:: /figuras/ucloud_ip_publico004.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

A seguir a descrição detalhada dos campos desta tela:

* **Container**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta a relação de todos os containers provisionados aos quais o usuário está vinculado para uso. Esta tela é idêntica tanto para os provedores de serviço de nuvem pública AWS (Amazon Web Services) e GCP (Google Cloud Platform).

* **Quantidade**: Este campo é obrigatório, o usuário deve informar um número inteiro que representa a quantidade de Endereços TCP-IP Públicos que deseja solicitar para o ambiente do provedor de serviço de nuvem (pública e/ou privada).

* **Região**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta a relação de todas as Regiões Globais específicas do provedor de serviço de nuvem pública. Esta tela é idêntica tanto para os provedores de serviço de nuvem pública AWS (Amazon Web Services) e GCP (Google Cloud Platform).

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de solicitação de um Endereço TCP-IP Público. A Plataforma uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a solicitação de Endereço(s) TCP-IP Público(s), nos ambientes AWS e GCP, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão "Criar" para que a Plataforma uCloud envie todos os parâmetros para os ambientes, para a tarefa de solicitar o(s) Endereço(s) TCP-IP Público(s).
  Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, a Plataforma uCloud não permite a solicitação de um Endereço TCP-IP Público.

Solicitando um IP Público (**Azure**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Quando o usuário clica com o cursor do mouse sobre o botão Solicitar IP Público a plataforma do uCloud apresenta a seguinte tela:

.. image:: /figuras/ucloud_ip_publico004b.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

A seguir a descrição detalhada dos campos desta tela:

* **Container**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta a relação de todos os containers provisionados aos quais o usuário esteja vinculado para uso. Após selecionado o provedor de serviço de nuvem pública Microsoft Azure, a tela exibe os campos descritos abaixo.

* **Virtual Datacenters Concedidos**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta relação de todos os Virtual Datacenters provisionados e vinculados ao provedor de serviço de nuvem pública Microsoft Azure.

* **Quantidade**: Este campo é obrigatório, o usuário deve informar um número inteiro que representa a quantidade de Endereços TCP-IP Públicos que deseja solicitar para o ambiente do provedor de serviço de nuvem (pública e/ou privada).

* **Região**: Este campo é obrigatório do tipo "drop down", quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta a relação de todas as Regiões Globais específicas do provedor de serviço de nuvem pública Microsoft Azure.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de solicitação de um Endereço TCP-IP Público. A Plataforma uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a solicitação de Endereço(s) TCP-IP Público(s), no ambiente Azure, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão ‘Criar’ para que a Plataforma uCloud envie todos os parâmetros para os ambientes, na tarefa de solicitar o(s) Endereço(s) TCP-IP Público(s).
  Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, a Plataforma uCloud não permite a solicitação de um Endereço TCP-IP Público.

Solicitando um IP Público (ambiente privado ex: **VMware vCenter**)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Importante mencionar que este manual não tem o objetivo de documentar todos os outros ambientes de redes privadas, favor entrar em contato com o suporte da Ustore para esclarecimentos detalhados específicos de seu ambiente privado.

Abaixo descrevemos o ambiente de rede privado de um container (hypervisor) VMware vCenter com o objetivo de documentar a flexibilidade da Plataforma uCloud.

Quando o usuário clica com o cursor do mouse sobre o botão Solicitar IP Público a plataforma do uCloud apresenta a seguinte tela:

A seguir a descrição detalhada dos campos da tela exibida acima:

* **Container**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta a relação de todos os containers provisionados aos quais o usuário esteja vinculado para uso. Após selecionado o provedor de serviço de nuvem privada (neste exemplo: Cloud - vCenter), a tela exibe os campos descritos abaixo.

* **Quantidade**: Este campo é obrigatório, o usuário deve informar um número inteiro que representa a quantidade de Endereços TCP-IP Públicos que deseja solicitar para o ambiente do provedor de serviço de nuvem (pública e/ou privada).

* **IPV4**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicacom o cursor do mouse a Plataforma uCloud apresenta as duas opções que o usuário deseja para a versão do protocolo TCP-IP:

  * **IPV4**: Para solicitar um Endereço TCP-IP na versão 4, com o padrão 32 bits.
  * **IPV6**: Para solicitar um Endereço TCP-IP na versão 6, com o padrão 128 bits.

* **Ícone Agendar**: Este ícone permite ao usuário agendar o provisionamento da solicitação do Endereço TCP-IP Público, o valor padrão é Desabilitado (vermelho).

  * **Ícone Desabilitado** |icone_habilita_verde|: Este ícone indica que não existe agendamento estabelecido. Isto significa que este Endereço TCPIP Público será imediatamente provisionado no ambiente do provedor de serviço de nuvem privado, basta o usuário clicar com o cursor do mouse no botão Criar (verde).
  * **Ícone Habilitado** |icone_desabilita_verm|: Este ícone indica que o usuário pretende agendar uma data para o provisionamento de um Endereço TCP-IP Público no ambiente do provedor de serviço de nuvem privada. Este processo permite escolher a melhor data para que o recurso computacional de nuvem possa iniciar sua cobrança de valores em datas pré-definidas pela empresa usuária da Plataforma uCloud.
    Quando alterar o ícone para habilitado (verde), a Plataforma uCloud permitirá ao usuário inserir uma data desejada.

  * **Ícone Calendário** |icone_agenda|: Basta o usuário clicar sobre o ícone do calendário para a Plataforma uCloud apresentar o pop-up na tela e permitir ao usuário selecionar a data desejada, conforme abaixo:

.. image:: /figuras/ucloud_calendario.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

  * **Hora / Minuto**: Este campo é apresentado no padrão de 24 horas, basta o usuário selecionar a hora e minuto desejado. Quando selecionado, este será o horário programado para que a Plataforma uCloud possa enviar a tarefa ao provedor de serviço de nuvem privada para o provisionamento do Endereço TCP-IP Público.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de solicitação de um Endereço TCP-IP Público. A Plataforma uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais ara a solicitação de Endereço(s) TCP-IP Público(s), nos ambientes de nuvem privada VMware vCenter, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão ‘Criar’ para que a Plataforma uCloud envie todos os parâmetros para os ambientes, na tarefa de solicitar o(s) Endereço(s) TCP-IP Público(s).
  Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser atendido e o campo está em branco, a Plataforma uCloud não permite a solicitação de um Endereço TCP-IP Público.

Grupos de Segurança e ACLs
--------------------------

O menu de Grupos de Segurança permite que sejam criados Grupos de Segurança (Security Groups - SG) e Listas de Controle de Acesso (Access-Control List - ACLs) que podem ser associados a máquinas virtuais. Esta funcionalidade permite que sejam criadas ACLS (regras) para tráfegos de entrada e saída que serão aplicados pelos usuários as suas máquinas virtuais.

Um Grupo de Segurança atua como “firewall” virtual para as máquinas virtuais, com o objetivo de controlar o tráfego de dados TCP-IP de entrada e de saída. O usuário pode provisionar regras específicas para cada Grupo de Segurança que permite tráfego de entrada ou de saída nas máquinas virtuais associadas. É possível modificar as regras de um Grupo de Segurança a qualquer momento, as regras novas e modificadas são aplicadas automaticamente para todas as máquinas virtuais nas quais o Grupo de Segurança está associado.

.. image:: /figuras/ucloud_grupo_seguranca001.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

Lista de Controle de Acesso (Access-Control List - ACL) é uma lista de permissões associadas a um recurso do sistema (objeto). Uma ACL especifica quais usuários ou processos do sistema têm acesso concedido aos objetos, bem como quais operações são permitidas em determinados objetos. Cada entrada em uma ACL típica especifica um assunto e uma operação.

A Plataforma uCloud comunica-se com o console dos provedores através da API Rest, portanto, toda ação executada e/ou configurada na plataforma do uCloud passa a ser apresentada imediatamente na tela do usuário, a qual envia as ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada.

Ao acessar este menu "Grupo de Segurança" a Plataforma uCloud apresenta ao usuário a tela com a lista geral dos Grupos de Segurança provisionados anteriormente no uCloud, conforme a tela a seguir:

.. image:: /figuras/ucloud_grupo_seguranca002.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

Esta tela pode apresentar-se extensa, pois a quantidade exibida está relacionada tanto com a quantidade de máquinas virtuais quanto com a quantidade de provedores de serviço de nuvem (pública e/ou privada) provisionados na Plataforma uCloud.

A seguir a descrição detalhada das colunas desta tela:

* **Botão “Criar Grupo de Segurança”**: Caso o usuário necessite criar um novo Grupo de Segurança no ambiente do provedor de serviço de nuvem (público ou privado), basta clicar com o cursor do mouse sobre este botão e seguir as instruções no item abaixo: B. Criar Grupo de Segurança.

* **Botão Refresh**: A Plataforma uCloud comunica-se com o console dos provedores através da API Rest, toda ação executada e/ou configurada na plataforma do uCloud passa a ser apresentada imediatamente na tela do usuário, a qual envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada. Para atualizar apenas o conteúdo das seções da tela (ou as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, ele executa apenas a atualização das informações contidas nas bases de dados da plataforma do uCloud.

* **Nome**: Esta coluna apresenta o nome do Grupo de Segurança informado pelo usuário no momento que este foi provisionado através da Plataforma uCloud.

O usuário pode notar que alguns nomes podem ser extremamente extensos ou diferentes dos quais o usuário criou, isto pode ocorrer quando um Grupo de Segurança foi provisionado diretamente no console do provedor de serviço de nuvem pública e o processo de sincronização da Plataforma uCloud com o Container extrai este nome diretamente do ambiente do provedor de serviço de nuvem pública. Importante ressaltar que estes nomes são considerados críticos e devem ser alterados diretamente no console do provedor de serviço de nuvem pública. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de Grupos de Segurança de forma alfabética, em ordem crescente (a – z) ou decrescente (z – a).

* **Nome do Container**: Esta coluna apresenta o nome do Container. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no campo "Busca Rápida - abaixo do título da coluna", a Plataforma uCloud lista todos os Containers que o usuário registrado está vinculado, para restringir a lista de Grupos de Segurança específicos ao Container selecionado.

* **Criado Por**: Esta coluna apresenta as credenciais de login do usuário que estava registrado na Plataforma uCloud e é o responsável pelo provisionamento do Grupo de Segurança. No caso desta coluna estar em branco, sem informação alguma, significa que o Grupo de Segurança foi provisionado diretamente no console do provedor de serviço de nuvem pública, e o processo de sincronização da Plataforma uCloud importou este Grupo de Segurança. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de Grupos de Segurança de forma alfabética, na ordem crescente (a – z) ou decrescente (z – a).

* **Ação**: Esta coluna apresenta duas opções de ação a ser realizada pelo usuário, por intermédio dos ícones e ele possa interagir com a rede selecionada:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud remove (exclui) este Grupo de Segurança, de forma imediata e definitiva. Esta ação será efetivada no ambiente de rede selecionado (público e/ou privado), o tempo necessário para que a referida ação seja aplicada é totalmente dependente do tempo do ambiente destino (público e/ou privado), a Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - Consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada.
  * **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela que permite a edição das configurações do Grupo de Segurança, o usuário pode seguir as instruções do item: A. Gerenciar Grupo de Segurança.

* **Busca Rápida**: O usuário pode notar que logo abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de Grupos de Segurança. Basta preencher o campo em branco com uma sequência de caracteres que possa ser relevante e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca.

Gerenciar Grupo de segurança
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A Plataforma uCloud permite ao usuário alterar as configurações de um Grupo de Segurança, para isso, existem duas opções: tanto o usuário pode clicar sobre o nome do Grupo de Segurança, quanto clicar sobre o ícone de Edição de um grupo de segurança, as duas formas são apresentadas pela Plataforma uCloud, conforme a tela abaixo:

.. image:: /figuras/ucloud_grupo_seguranca003.png
   :alt: Menu Rede - IP Público
   :scale: 60 %
   :align: center
   :class: with-border

----

A seguir a descrição detalhada de cada seção desta tela:

* **Botão Excluir Grupo de Segurança**: Basta o usuário clicar com o cursor do mouse sobre o botão e a Plataforma uCloud remove (exclui) este Grupo de Segurança do ambiente do provedor de serviço de nuvem (pública e/ou privada), de forma imediata e definitiva.
  O tempo necessário para que a referida ação seja aplicada é totalmente dependente do tempo do ambiente destino (público e/ou privado), a Plataforma uCloud não acrescenta ou reduz qualquer tempo nestas ações - Consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada. Esta ação também remove o custo recorrente do recurso da conta do provedor de serviço de nuvem (pública e/ou privada).
  Quando o usuário clicar com o cursor do mouse sobre este ícone, a Plataforma uCloud exibe um ‘pop up’ na tela e solicita ao usuário confirmar a ação.

* **Seção Geral**: Esta seção apresenta as informações genéricas do Grupo de Segurança.

* **Seção Regras**: Esta seção apresenta duas ‘abas’ (tabs) as quais apresentam as regras (de entrada e saída) configuradas para este Grupo de Segurança; assim, o usuário deve clicar com o cursor do mouse sobre cada aba com o objetivo de visualizar as respectivas configurações, separadamente. Por padrão, a Plataforma uCloud apresenta o conteúdo das configurações da ‘aba’: Entrada.

* **Botão Editar Regras**: Basta o usuário clicar sobre este ícone para que a Plataforma uCloud possa alternar todos os campos das colunas para o modo de edição, de forma a possibilitar ao usuário corrigir o conteúdo dos campos e alterar as configurações da aba selecionada (entrada ou saída) do Grupo de Segurança.

  * **Botão Salvar Regras**: Basta clicar com o cursor do mouse sobre este botão para confirmar a alteração do conteúdo no campo desejado. Após finalizar a alteração do conteúdo deste campo, o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação, a informação no campo será alterada permanentemente nas bases de dados da Plataforma uCloud e nas configurações no ambiente do provedor de serviço de nuvem (pública e/ou privada).
  * **Botão de Adicionar Regra**: Basta clicar com o cursor do mouse sobre este botão para a Plataforma uCloud acrescentar uma nova linha em branco, deste modo o usuário poderá adicionar uma nova regra ao Grupo de Segurança. Ver o procedimento de criação de regras no item abaixo: B. Criar Grupo de Segurança.
  * **Botão de Cancelamento**: Caso o usuário tenha clicado sobre o ícone de edição, por engano, ou não deseja que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o botão vermelho. O botão vermelho cancela as alterações e o conteúdo do campo retorna aos valores iniciais, antes de proceder qualquer preenchimento ou alteração.

* **Seção Máquinas Virtuais Associadas**: Nesta seção estão listadas todas as máquinas virtuais, as quais este Grupo de Segurança está vinculado para controlar o tráfego de pacotes de dados TCP-IP. Basta clicar com o cursor do mouse sobre o nome da máquina virtual, para a Plataforma uCloud apresentar a tela de Gerenciando Máquina Virtual (Menu Máquina Virtual).

.. attention:: |atencao| Importante ressaltar que qualquer alteração das configurações de um Grupo de Segurança rede, podem gerar impacto nos ambientes computacionais, nas máquinas virtuais vinculadas, nas comunicações entre as aplicações e o acesso dos usuários (tanto às máquinas virtuais, como as aplicações por estas executadas). A Plataforma uCloud não pode ser responsabilizada por problemas que possam resultar desta ação.


Criar Grupo de Segurança
~~~~~~~~~~~~~~~~~~~~~~~~

O processo de provisionamento de um Grupo de Segurança, para criá-lo é efetuado através da tela da Plataforma uCloud

.. note:: Importante ressaltar que somente os usuários com perfil de Administrador de Grupo ou Administrador de Contrato, podem completar esta operação.

A seguir a descrição detalhada dos campos desta tela:

* **Usuário**: Este campo é obrigatório, ele vem preenchido com o login do usuário registrado presente na Plataforma uCloud. Este usuário é utilizado como referência para filtrar os Grupos de Segurança específicos, provisionados por este no campo abaixo. Se for necessário alterar a vinculação ao usuário, basta clicar com o cursor do mouse sobre o botão de edição “ ” e digitar os caracteres que fazem parte do login do usuário que ficará vinculado a este Grupo de Segurança, a Plataforma uCloud apresenta uma lista de logins de usuário que possuem a sequência de caracteres digitado. Basta selecionar o login desejado na lista.

* **Container**: Este campo é obrigatório do tipo “drop down”, ao clicar com o cursor do mouse a Plataforma uCloud apresenta relação de todos os containers provisionados na Plataforma uCloud, aos quais o usuário está vinculado para uso.

* **Virtual Datacenter (exclusivo Azure)**: Virtual Datacenters Concedidos: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação de todos os Virtual Datacenters provisionados e vinculados ao provedor de serviço de nuvem pública Microsoft Azure.

* **Região**: Este campo é obrigatório do tipo "drop down", quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta a relação de todas as Regiões Globais específicas do provedor de serviço de nuvem pública.

* **Rede**: Este campo é obrigatório do tipo "drop down", quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta a relação de todas as Redes (e Sub-Redes) provisionadas no ambiente específico do provedor de serviço de nuvem (pública e/ou privada) definido no campo Container. Importante ressaltar que ao vincular o Grupo de Segurança à Rede, este atuará apenas nas máquinas virtuais que pertencerem à mesma rede (e sub-rede) selecionada.

* **Descrição**: Este campo é opcional e de livre digitação, seu conteúdo pode ser utilizado para descrever o objetivo da Sub-Rede.

* **Entrada**: Por padrão, na Plataforma uCloud o Botão Adicionar Regra apresenta os campos para configurar uma Regra de Acesso de Entrada, conforme a tela abaixo:

  * **Tipo**: Este campo é obrigatório do tipo "drop down", ao clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação de todos os tipos de tráfego de serviços de dados TCP-IP, basta o usuário clicar com o cursor do mouse sobre o tipo desejado.
  * **Protocolo**: Este campo não é editável, ele será preenchido automaticamente, após o usuário selecionar a identificação do Tipo do Protocolo no campo anterior, ele pode apresentar:
    * ICMP
    * TCP
    * UDP
    * All

  * **Port Range**: Este campo não é editável, ele será preenchido automaticamente, após o usuário selecionar a identificação do Tipo do Protocolo no campo anterior. Este campo será preenchido com a faixa de portas padronizadas (TCP, UDP ou ICMP) de acordo com o Tipo de Protocolo selecionado acima.

  * **Origem**: Este campo é opcional e permite ao usuário aumentar o nível de segurança de acesso ao recurso da máquina virtual. Este campo permite ao usuário informar uma das três opções:
    * **Endereço TCP-IP Único**: (notação CIDR) Somente este Endereço TCP-IP específico será o único autorizado, ele terá acesso de entrada através da definição deste Grupo de Segurança. Esta opção carrega o mais alto nível de segurança de acesso entrante.
    * **Endereços TCP-IP de Sub Rede**: (notação CIDR) O usuário pode informar Endereço TCP-IP com ‘/’ (barra) para indicar todos os Endereços TCP-IP subsequentes dentro da rede. (por exemplo: 192.1.0.0/23). Desta forma, todos os Endereços TCP-IP desta rede estarão autorizados a acesso entrante através desta definição de Grupo de Segurança. Esta opção carrega um nível intermediário de segurança de acesso entrante.
    * **Endereço TCP IP Genérico** (default): Por padrão, a Plataforma uCloud apresenta este campo preenchido com a notação “0.0.0.0/0”, significa que o Grupo de Segurança aceitará o acesso entrante vindo de qualquer endereço TCP-IP da Rede Mundial. Esta opção possui o mais baixo nível de segurança de acesso entrante.

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova (exclua) esta regra do Grupo de Segurança, de forma imediata e definitiva.

* **Saída**: Basta o usuário clicar com o cursor do mouse sobre esta aba para configurar um Regra para o fluxo de pacotes TCP-IP de saída, conforme a tela abaixo:

  * **Tipo**: Este campo é obrigatório do tipo "drop down", quando o usuário clicar neste campo, com o cursor do mouse, a Plataforma uCloud apresenta a relação de todos os tipos de tráfego de serviços de dados TCP-IP sainte, basta o usuário clicar com o cursor do mouse sobre o tipo desejado.
  * **Protocolo**: Este campo não é editável, ele será preenchido automaticamente, após o usuário selecionar a identificação do Tipo do Protocolo no campo anterior, pode apresentar:
    * ICMP
    * TCP
    * UDP
    * All

  * **Port Range**: Este campo não é editável, ele será preenchido automaticamente, após o usuário selecionar a identificação do Tipo do Protocolo no campo anterior. Este campo será preenchido com a faixa de portas padronizadas (TCP, UDP ou ICMP), de acordo com o Tipo de Protocolo selecionado acima.

  * **Destino**: Este campo é opcional, ele permite ao usuário aumentar o nível de segurança de acesso ao recurso da máquina virtual. Neste campo o usuário poderá informar uma das três opções:
    * **Endereço TCP-IP Único**: (notação CIDR) A máquina virtual enviará pacotes de dados somente a este Endereço TCP-IP específico, o qual será o único autorizado, com o qual haverá conexão de saída de dados através da definição deste Grupo de Segurança. Esta opção carrega o mais alto nível de segurança de acesso aos pacotes de dados.
    * **Endereços TCP-IP de Sub Rede**: (notação CIDR) O usuário poderá informar Endereço TCP-IP com ‘/’ (barra) para indicar todos os Endereços TCP-IP subsequentes dentro da rede com o qual haverá conexão sainte de pacotes de dados, através da definição deste Grupo de Segurança (por exemplo: 192.1.0.0/23). Desta forma, todos os Endereços TCP-IP da rede serão os únicos, os quais a máquina virtual enviará os pacotes de dados através desta definição de Grupo de Segurança. Esta opção carrega um nível intermediário de segurança de acesso aos pacotes de dados.
    * **Endereço TCP IP Genérico** (default): Por padrão, a Plataforma uCloud apresenta este campo preenchido com a notação “0.0.0.0/0” isto significa que o Grupo de Segurança enviará os dados saintes para qualquer endereço TCP-IP da rede mundial. Esta opção possui o mais baixo nível de segurança de acesso aos pacotes de dados.

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud remova (exclua) esta regra do Grupo de Segurança, de forma imediata e definitiva.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de provisionamento de um Grupo de Segurança. Após clicar, a Plataforma uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais das regras de um Grupo de Segurança, nos ambientes do provedor de serviços de nuvem (pública e/ou privada), o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar para que a Plataforma uCloud possa enviar todos os parâmetros para os ambientes, de forma a provisionar um Grupo de Segurança.

  Caso este botão não esteja habilitado (cor cinza), isto significa que algum parâmetro anterior deixou de ser preenchido e o campo está em branco, logo a Plataforma uCloud não conclui o provisionamento do Grupo de Segurança.


Par de Chaves
-------------

O menu **Par de Chaves** contém todas as chaves criadas por um usuário para acessar as suas máquinas, sejam em ambientes de nuvem pública ou on-premisses.

O usuário pode criar uma chave nova, para isso ele deve indicar o container e o nome da chave, ou ainda, o usuário pode importar uma chave pública. Para executar esta operação, ele deve indicar o container, o nome e a chave.

Um Par de Chaves consiste em uma chave privada e uma chave pública, trata-se de um conjunto de credenciais de segurança usadas para provar a identidade ao conectar-se a uma máquina virtual. De um lado, o provedor de serviço de nuvem (pública e/ou privada) armazena a chave pública, do outro lado o usuário armazena a chave privada. Para o usuário poder conectar-se ao prompt do sistema operacional da máquina virtual criada deve utilizar a chave privada, ao invés de uma senha, para um acesso seguro e autenticado. Qualquer usuário com a chave privada pode conectarse às máquinas virtuais, por isso, é importante armazenar as chaves privadas em um lugar seguro.

Durante o processo de criação de uma máquina virtual, um par de chaves será solicitado para permanecer vinculado a esta máquina virtual. No caso do usuário planejar conectar-se usando SSH, ele deve especificar um par de chaves. É possível escolher um par de chaves existentes ou criar um novo.

A Plataforma uCloud permite importar chaves SSH no caso da empresa usuária já possuir as chaves SSH próprias. Ao conectar-se ao prompt da máquina virtual usando SSH, o usuário deve especificar a chave privada que corresponde ao conteúdo da chave pública para fazer login. Para obter outras informações sobre como conectar-se à sua máquina virtual, favor consultar a documentação online do seu provedor de serviço de nuvem.

Ao acessar o menu Par de Chaves, a Plataforma uCloud apresenta ao usuário uma tela com a lista que contém todas as chaves criadas por todos os usuários, elas são destinadas ao acesso às suas máquinas virtuais existentes em todos os provedores de serviço de nuvem nuvem (pública e/ou privada) que o seu login de acesso permite visualizar.

.. image:: /figuras/ucloud_par_de_chaves001.png
   :alt: Menu Rede - IP Público
   :scale: 50 %
   :align: center
   :class: with-border

----

A seguir a descrição detalhada das colunas desta tela:

* **Botão “Criar Par de Chaves”**: Caso o usuário necessite criar um novo Grupo de Segurança no ambiente do provedor de serviço de nuvem (pública e/ou privada), basta clicar com o cursor do mouse sobre este botão, depois seguir as instruções no item abaixo: B. Criar Par de Chaves.

* **Botão “Importar Par de Chaves”**: Caso o usuário necessite criar um novo Grupo de Segurança no ambiente do provedor de serviço de nuvem (pública e/ou privada), basta clicar com o cursor do mouse sobre este botão, e prosseguir nas instruções no item abaixo: C. Importar Par de Chaves.

* **Botão Refresh**: A Plataforma uCloud comunica-se com o console dos provedores através da API Rest, toda ação executada e/ou configurada na plataforma do uCloud passa a ser apresentada imediatamente na tela do usuário, a qual envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada. Para atualizar apenas o conteúdo das seções da tela (ou as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, ele executa apenas a atualização das informações contidas nas bases de dados da Plataforma uCloud.

* **Nome do Container**: Esta coluna apresenta o nome do Container. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no campo ‘Busca Rápida - abaixo do título desta coluna’, a Plataforma uCloud lista todos os Containers que o usuário registrado está vinculado, para restringir a lista de Grupos de Segurança específicos ao Container selecionado. Lembrando que para a Plataforma uCloud, um Container representa um provedor de serviço de nuvem (pública e/ou privada).

* **Nome**: Esta coluna apresenta o nome do Par de Chave informado pelo usuário no momento que este foi provisionado através da Plataforma uCloud. O usuário pode notar que alguns nomes podem ser extremamente extensos ou diferentes dos quais o usuário tenha criado, geralmente, estes nomes ocorrem quando um Par de Chaves foi provisionado diretamente no console do provedor de serviço de nuvem pública e o processo de sincronização da Plataforma uCloud com o Container extrai este nome diretamente do ambiente do provedor de serviço de nuvem pública.

.. important:: |importante| Estes nomes considerados críticos, devem ser alterados diretamente no console do provedor de serviço de nuvem pública. Como forma de simplificar a visualização, o usuário pode digitar uma sequência de caracteres para aproximar a busca desejada e recuperar na lista, a Plataforma uCloud filtra o conteúdo indexado e lista todas as incidências de nomes que contenham a sequência digitada.

* **Fingerprint**: Esta coluna apresenta o conteúdo do fingerprint (impressão digital) do Par de Chaves gerado a partir dos seus pares de chaves. De forma genérica, uma impressão digital será calculada usando uma função hash SHA-1. O usuário pode usar a impressão digital SSH2 exibida nesta coluna para verificar se a chave privada pertencente a sua máquina local corresponde à chave pública armazenada no provedor de serviço de nuvem (pública e/ou privada).

* **Criado Por**: Esta coluna apresenta as credenciais de login do usuário que estava registrado na Plataforma uCloud e foi o responsável pelo provisionamento do Par de Chaves. Como forma de simplificar a visualização, o usuário pode digitar uma sequência de caracteres para aproximar a busca desejada e recuperar na lista, a Plataforma uCloud filtra o conteúdo indexado e lista todas as incidências de login de usuário que contenham a sequência digitada.

* **Ação**: Esta coluna apresenta apenas um ícone para que o usuário possa interagir com a rede selecionada:
  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão “Lata de Lixo” e a Plataforma uCloud remove (exclui) este Par de Chaves, de forma imediata e definitiva. Esta ação será efetivada no ambiente de rede selecionado (público e/ou privado), o tempo necessário para que a referida ação seja aplicada é totalmente dependente do tempo do ambiente destino (público e/ou privado), a Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - Consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada.

    * Ao excluir um par de chaves, o usuário só exclui a cópia da chave pública do provedor de serviço de nuvem (pública e/ou privada). Aexclusão de um par de chaves não afeta a chave privada, armazenada no seu computador pessoal, e também, não afeta a chave pública em nenhuma instância já executada usando esse par de chaves. O usuário não poderá provisionar uma nova máquina virtual usando um par de chaves excluído, mas pode continuar a conectar-se a quaisquer instâncias executadas usando um par de chaves excluído, desde que este ainda tenha o arquivo de chaves privadas (.pem).
    * Importante mencionar: se o usuário houver provisionado um Scaling Group (Grupo de Escalabilidade), é relevante certificar-se de que o par de chaves que está sendo excluído não esteja especificado na sua configuração de execução. Os provedores de serviço de nuvem (pública e/ou privada) utilizam a chave pública armazenada para a máquina virtual padrão para ser clonada no evento de lançamento de uma nova instância da máquina virtual, e a falta da chave pública pode detectar uma instância não íntegra; e, por consequência, a execução da instância falha se o Par de Chaves não for encontrado. A Plataforma uCloud não pode ser responsabilizada por problemas que possam resultar desta ação.

Gerenciar um Par de Chaves
~~~~~~~~~~~~~~~~~~~~~~~~~~

Quando o usuário clicar com cursor do mouse no nome de um Par de Chaves, a Plataforma uCloud apresenta uma tela com as informações específicas deste:

.. image:: /figuras/ucloud_par_de_chaves002.png
   :alt: Menu Rede - IP Público
   :scale: 50 %
   :align: center
   :class: with-border

----

A seguir a descrição detalhada das seções e dos campos a preencher nesta tela:

* **Seção Geral**

  * **Nome**: Este campo indica o nome do Par de Chaves informado pelo usuário durante o seu provisionamento. No caso de haver um nome extremamente longo ou diferente do que o usuário criou, isto indica que este Par de Chaves foi provisionado diretamente no console do provedor de serviço de nuvem pública e o processo de sincronização da Plataforma uCloud com o container extraiu este nome diretamente do ambiente do provedor de serviço de nuvem pública
  * **Usuário**: Este campo apresenta as credenciais de login do usuário que está registrado na Plataforma uCloud, o responsável pelo provisionamento do Par de Chaves. No caso deste campo não apresentar informação alguma (estar em branco), isto indica que o Par de Chaves foi provisionado diretamente no console do provedor de serviço de nuvem pública, o processo de sincronização da Plataforma uCloud importou este Par de Chaves.
  * **Descrição**: Este campo apresenta o conteúdo que descreve o objetivo deste Par de Chaves, desde que tenha sido informado pelo usuário no momento do provisionamento.

* **Seção Máquinas Virtuais**

  * **Nome**: Esta coluna indica o nome da Máquina Virtual informado pelo usuário durante o processo do seu provisionamento. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud recupera e classifica a lista com os nomes das máquinas virtuais, de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **Usuário**: Esta coluna apresenta as credenciais de login do usuário que está registrado na Plataforma uCloud, o responsável pelo provisionamento da Máquina Virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud recupera e classifica a lista de nomes de máquinas virtuais, de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **IP Privado**: Esta coluna apresenta o Endereço TCP-IP Privado que o provedor de serviço de nuvem (pública e/ou privada) associou a esta máquina virtual no momento de sua criação. Este Endereço TCP-IP é um endereço estático. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud recupera e classifica uma lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **IP Público**: Esta coluna apresenta o Endereço TCP-IP Público solicitado ao provedor de serviço de nuvem (pública e/ou privada) que foi vinculado pelo usuário a esta máquina virtual. Caso a informação desta coluna permaneça em branco, isto significa que esta máquina virtual possui um Endereço TCPIP Público dinâmico que é fornecido pelo ambiente do provedor de serviço de nuvem (pública e/ou privada). Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud recupera e classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **Memória**: Esta coluna apresenta a configuração da quantidade de memória RAM da máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud recupera e classifica a lista de endereços TCP-IP, de forma crescente ou decrescente.
  * **CPUs**: Esta coluna apresenta a configuração da quantidade de CPUs da máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud recupera e classifica a lista de endereços TCP-IP, de forma crescente ou decrescente. ○ Status: Esta coluna apresenta o status da máquina virtual. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud recupera com base no status da máquina e classifica a lista de nomes de máquinas virtuais, de forma alfabética crescente (a – z) ou decrescente (z – a).

Criando um Par de Chaves
~~~~~~~~~~~~~~~~~~~~~~~~

O usuário pode criar um novo Par de Chaves, para isso ele deve vincular o Par de Chaves ao Container e ao nome do usuário que importou (ou criou) uma chave pública, desta forma é mandatório informar os containers, o usuário e o nome do Par de Chaves.

.. image:: /figuras/ucloud_par_de_chaves003.png
   :alt: Menu Rede - IP Público
   :scale: 50 %
   :align: center
   :class: with-border

----

Abaixo segue a descrição dos campos desta tela:

.. important:: Somente os usuários com perfil de Administrador de Grupo ou Administrador de Contrato, podem completar esta operação.

* **Usuário**: Este campo é obrigatório ele vem preenchido com o login do usuário registrado presente na Plataforma uCloud. Este usuário é utilizado como referência para filtrar o Par de Chaves específico que foi provisionado por ele. Se for necessário alterar a vinculação ao usuário, basta clicar com o cursor do mouse sobre o botão de Edição “ ” e digitar os caracteres que fazem parte do login do usuário que será vinculado a este Par de Chaves, a Plataforma uCloud apresenta uma lista de logins de usuário que possuem a sequência de caracteres digitado. Em seguida, o usuário deve selecionar na lista o login desejado para associar ao Par de Chaves.
* **Container**: Este campo é obrigatório do tipo “drop down”, ao clicar com o cursor do mouse a Plataforma uCloud apresenta relação de todos os containers provisionados na Plataforma uCloud, aos quais o usuário está vinculado para uso.
* **Nome da Chave**: Este campo é obrigatório, nele o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar este Par de Chaves. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de provisionamento de um Par de Chaves. Após clicar, a Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais das regras de um Par de Chaves, nos ambientes do provedor de serviços de nuvem (pública e/ou privada), o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar para que a Plataforma uCloud possa enviar todos os parâmetros para os ambientes, de forma a provisionar um Grupo de Segurança. Caso este botão não esteja habilitado (cor cinza), isto significa que algum parâmetro anterior deixou de ser preenchido e o campo está em branco, logo a Plataforma uCloud não conclui o provisionamento do Par de Chaves.

Importando um Par de Chaves
~~~~~~~~~~~~~~~~~~~~~~~~~~~

O processo de importação de Par de Chaves permite e possibilita a uma organização que já possui suas chaves públicas levar estas chaves para o ambiente do provedor de serviços de nuvem (pública e/ou privada). A importação não substitui as chaves públicas que o provedor de serviço de nuvem possui, este processo adiciona novas chaves públicas e padroniza o processo de vinculação das chaves corporativas com as máquinas virtuais criadas no ambiente do provedor de serviço de nuvem (pública e/ou privada).

.. important:: O usuário deve consultar a documentação online do seu provedor de serviço de nuvem, no qual será armazenada a nova chave pública, para conhecer as características corretas do formato do arquivo da chave pública. O usuário pode utilizar o software da sua preferência (prompt de Linux ou aplicação Windows) para gerar a sua chave privada. A Plataforma uCloud não possui a funcionalidade de geração de Chaves Públicas.

Quando o usuário clicar com o cursor do mouse sobre o botão de Importar Par de Chaves, a Plataforma uCloud apresenta a seguinte tela:

.. image:: /figuras/ucloud_par_de_chaves004.png
   :alt: Menu Rede - IP Público
   :scale: 30 %
   :align: center
   :class: with-border

----

A seguir a descrição detalhada destes campos:

* **Usuário**: Este campo é obrigatório e vem preenchido com o login do usuário registrado corrente na Plataforma uCloud. Este usuário será utilizado como referência para filtrar os Paresde Chaves específicos que foram provisionados por este, no campo abaixo. Se for necessário alterar a vinculação ao usuário, basta clicar com o cursor do mouse sobre o botão de edição “ ” e digitar os caracteres que fazem parte do login do usuário que ficará vinculado a este grupo de segurança, que a Plataforma uCloud apresenta uma lista de logins de usuário que possuem a sequência de caracteres digitado. Basta selecionar o login desejado da lista. Importante ressaltar que somente usuários com perfil de Administrador de Grupo ou Administrador de Contrato, poderão completar esta operação.
* **Container**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta a relação de todos os containers provisionados na Plataforma uCloud, aos quais o usuário está vinculado para uso.
* **Nome da Chave**: Este campo é obrigatório, nele o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar este Par de Chaves. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **Conteúdo da Chave Pública**: Este campo é obrigatório, o usuário deve colar (paste) o conteúdo da chave pública neste campo.
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de provisionamento de um Par de Chaves. Após clicar, a Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais das regras de um Par de Chaves, nos ambientes do provedor de serviços de nuvem (pública e/ou privada), o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar para que a Plataforma uCloud possa enviar todos os parâmetros para os ambientes, de forma a provisionar um Par de Chave.
  Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser preenchido e o campo está em branco, logo a Plataforma uCloud não conclui o provisionamento do Par de Chaves.

Balanceadores
-------------

O menu Balanceadores contém todos os balanceadores de carga criados por um usuário para acessar as suas máquinas, sejam em ambientes de nuvem pública ou onpremisses. Para criar um balanceador o usuário deve informar os dados exigidos por cada provedor, porém alguns são sempre solicitados por todos, tais como:
a. container no qual o balanceador está associado;
b. nome do balanceador;
c. protocolo: HTTP, HTTPS ou TCP;
d. porta TCP associada ao balanceador;
e. membros, máquinas virtuais, as quais o balanceador de carga solicita os dados.

Para as informações específicas de cada provedor de nuvem e/ou ambiente onpremisses o uCloud exibe os Hints explicativos, ou seja, as sugestões e dicas explicativas.

.. image:: /figuras/ucloud_balanceador001.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

Um Balanceador distribui o tráfego (carga de trabalho) entre duas ou mais máquinas virtuais. Usar um Balanceador (Classic Load Balancer) aumenta a disponibilidade e a tolerância às falhas dos aplicativos.
O usuário deve configurar as “verificações de integridade” que monitoram a “saúde” e a integridade das máquinas virtuais, para permitir ao balanceador enviar solicitações apenas para as máquinas virtuais que estão em condições ideais de funcionamento. A Plataforma uCloud apresenta o status da(s) máquina(s) virtual(is) identificando tanto o bom funcionamento quanto qualquer alteração das condições ideais de verificação da saúde e da integridade de uma ou várias máquinas virtuais(is).
Quando o usuário acessar o menu Balanceadores, a Plataforma uCloud apresenta uma tela com a lista de todos os Balanceadores de Carga provisionados por um usuário para acessar as suas máquinas sejam em ambientes de nuvem públicas e/ou privadas (onpremises).

.. image:: /figuras/ucloud_balanceador002.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

Abaixo segue a descrição das colunas desta lista:

* **Container**: Esta coluna apresenta o nome do Container ao qual o Balanceador está vinculado. Como forma de simplificar a visualização, o usuário pode digitar uma sequência de caracteres que deseja encontrar na lista, a Plataforma uCloud recupera o conteúdo da lista com todas as incidências de nomes que contenham a sequência digitada. Lembrando que para a Plataforma uCloud, um container representa um provedor de serviço de nuvem (público e/ou privado).
* **Endereço**: O usuário pode notar que alguns endereços podem ser extremamente extensos, pois estes endereços são obtidos do provedor de serviço de nuvem pública através do processo de sincronização da Plataforma uCloud com o Container. Como forma de simplificar a visualização, o usuário pode digitar uma sequência de caracteres que deseja encontrar na lista, em seguida a Plataform do uCloud recupera o conteúdo da lista com todas as incidências de nomes que contenham a sequência digitada.
* **Nome**: Esta coluna apresenta o nome do Balanceador informado pelo usuário no momento que este foi provisionado através da Plataforma uCloud. Como forma de simplificar a visualização, o usuário pode digitar uma sequência de caracteres que deseja encontrar na lista, a Plataforma uCloud recupera o conteúdo da lista com todas as incidências de nomes que contenham a sequência digitada.
* **Criado Por**: Esta coluna apresenta as credenciais de login do usuário que estava registrado na Plataforma uCloud e é o responsável pelo provisionamento do Balanceador. No caso desta coluna estar em branco, sem informação alguma, significa que o Grupo de Segurança foi provisionado diretamente no console do provedor de serviço de nuvem pública, e o processo de sincronização da Plataforma uCloud importou este Balanceador. Como forma de simplificar a visualização, o usuário pode digitar uma sequência de caracteres para aproximar a busca desejada e recuperar na lista, a Plataforma uCloud recupera o conteúdo indexado e lista todas as incidências de nomes que contenham a sequência digitada.
* **Ações**: Esta coluna pode apresentar dois ícones para que o usuário possa interagir com o Balanceador selecionado:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão “Lata de Lixo” e a Plataforma uCloud remove (exclui) este Balanceador do ambiente do provedor de serviço de nuvem (pública e/ou privada), de forma imediata e definitiva.
  * **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone para que a Plataforma uCloud possa apresentar uma tela que permite a edição das configurações do Balanceador, o usuário pode seguir as instruções no item a seguir: A. Gerenciando Balanceador.

.. nota:: O tempo necessário para que a referida ação seja aplicada é totalmente dependente do tempo do ambiente destino (público e/ou privado), a Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - Consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada. Esta ação também remove o custo recorrente do recurso da conta do provedor de serviço de nuvem (pública e/ou privada). Quando o usuário clicar com o cursor do mouse sobre este ícone, a Plataforma uCloud apresenta uma tela para confirmar a ação do usuário.


Gerenciando Balanceador
~~~~~~~~~~~~~~~~~~~~~~~

Quando o usuário clicar com o cursor do mouse sobre o nome de um Balanceador, a Plataforma uCloud apresenta a tela dividida em seções conforme abaixo:

.. image:: /figuras/ucloud_balanceador003.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

A seguir a descrição detalhada dos campos de cada seção:

* **Seção Geral**: Nesta seção são apresentadas informações básicas do Balanceador.

  * **Container**: Este campo apresenta o nome do Container ao qual o Balanceador está vinculado.
  * **Região**: Este campo apresenta a Região Global do provedor de serviço de nuvem pública que foi selecionada pelo usuário logado durante o provisionamento do Balanceador.
  * **Rede**: Este campo apresenta a Rede (e Sub-rede) do provedor de serviço de nuvem pública selecionada pelo usuário logado durante o provisionamento do Balanceador.
  * **Endereço**: Este campo apresenta o Endereço do Balanceador obtido do provedor de serviço de nuvem pública através do processo de sincronização da Plataforma uCloud com o Container. Este endereço é gerado internamente pelo provedor de serviço de nuvem pública, a Plataforma uCloud não possui qualquer controle ou interação.
  * **Nome**: Este campo apresenta o nome do Balanceador informado pelo usuário durante o seu provisionamento.
  * **Criado por**: Este campo apresenta as credenciais de login do usuário que estava registrado na Plataforma uCloud e é o responsável pelo provisionamento do Balanceador.
  * **Certificate**: Este ícone “ ” permite que o usuário possa adicionar (upload) as configurações de um certificado digital SSL para um Balanceador. Quando o usuário clicar com o cursor do mouse sobre este ícone a Plataforma uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_balanceador004.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

Abaixo segue a descrição dos campos:

* **Certificate Name**: Este campo é obrigatório, o usuário deve informar o nome com o qual deseja identificar o certificado que será importado.
* **Certiicate Public Key**: Este campo é obrigatório, o usuário deve informar a sequência de caracteres específicos da chave pública do certificado que será importado.
* **Certificate Private Key**: Este campo é obrigatório, o usuário deve informar a sequência de caracteres específicos da chave privada do certificado que será importado.
* **Certificate Chain**: Este campo é obrigatório, o usuário deve informar a sequência de caracteres específicos da chave pública do certificado que será importado.

* **Seção Listeners**: Esta seção apresenta a configuração das portas de ‘escuta (listeners)’ que é a forma como o Balanceador pode verificar a disponibilidade/integridade da aplicação/serviço que está sendo executada na máquina virtual.
  * **Protocolo**: Esta coluna apresenta o tipo de Protocolo TCP-IP selecionado para ser a ‘escuta’ e verificar a disponibilidade da aplicação/serviço. As opções padrões são:
    * HTTP
    * HTTPS
    * TCP
    * SSL

  * **Porta**: Esta coluna apresenta a Porta TCP-IP padrão que está relacionada diretamente com o tipo do Protocolo TCP-IP selecionado no campo anterior. Qualquer assinalamento diferente das portas padronizadas pode gerar impacto na eficiência do Balanceador, pois uma alteração nesta configuração deve estar em sincronia com a aplicação/serviço no sistema operacional da máquina virtual.
  * **Instance Protocol**: Esta coluna apresenta o tipo de Protocolo TCP-IP selecionado para ser o ‘escutado’, está configurado desta mesma forma no prompt do sistema operacional da máquina virtual para verificar a disponibilidade da aplicação/serviço. As opções padrões são as mesmas descritas acima na coluna Protocol.
  * **Instance Port**: Esta coluna apresenta a Porta TCP-IP padrão que está relacionada diretamente com o tipo do Protocolo TCP-IP selecionado no campo anterior, ele deve estar configurado desta mesma forma no prompt do sistema operacional da máquina virtual para verificar a disponibilidade da aplicação/serviço.
  * **Ações**: Esta coluna pode apresentar apenas um ícone para que o usuário possa interagir com o Balanceador selecionado:
    * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão “Lata de Lixo” e a Plataforma uCloud remove (exclui) esta configuração de Listener deste Balanceador, de forma imediata e definitiva. ○ Botão Adicionar: Basta clicar com o cursor do mouse sobre o botão ‘Adicionar’ quando o usuário precisar acrescer um Protocolo adicional como Listener neste Balanceador. A Plataforma uCloud acrescenta uma nova linha nesta lista, com todos os campos em branco, assim o usuário pode configurar como

  * **Botão Adicionar**: Basta clicar com o curor do mouse sobre o botão ‘Adicionar’ quando o usuário precisar acrescer um Protocolo adicional como Listener neste Balanceador. A Plataforma uCloud acrescenta uma nova linha nesta lista, com todos os campos em branco, assim o usuário pode configurar como for necessário, conforme a tela abaixo:

.. image:: /figuras/ucloud_balanceador005.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

A seguir, a descrição simplificada das colunas:

* **Protocolo**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar nele, com o cursor do mouse, a Plataforma uCloud listará as mesmas opções descritas no campo Protocolo acima descrito.
* **Porta**: Este campo é obrigatório, o usuário deve informar as Portas TCP-IP Padrão para o tipo do Protocolo selecionado no campo anterior.
* **Instance Protocol**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar nele, com o cursor do mouse, a Plataforma uCloud lista as mesmas opções descritas no campo Protocolo acima descrito. ○ Instance Port: Este campo é obrigatório, o usuário deve informar as Portas TCP-IP Padrão para o tipo do Protocolo selecionado no campo anterior.
* **Ações**: Esta coluna pode apresentar dois ícones, os quais permitem ao usuário a interação com o Balanceador selecionado:
  * **Ícone de Confirmação**: Quando o usuário desejar confirmar a configuração dos parâmetros informados na linha, a tela da Plataforma uCloud apresenta a opção deste ícone de confirmação. Após ter finalizado a inclusão do novo parâmetro de um Listener o usuário deve clicar com o cursor do mouse no botão verde para confirmar a inclusão.
  * **Ícone de Cancelamento**: Caso o usuário tenha clicado sobre o Botão de Adicionar, por engano ou não desejar que a inclusão de um novo Listener seja armazenado (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. Após acionar o ícone vermelho, ele cancela as alterações e o conteúdo do campo retorna aos valores iniciais, antes de proceder qualquer preenchimento ou alteração.

* **Seção Health Check**: Esta seção apresenta os parâmetros configurados que permitem verificar a “integridade e saúde” da máquina virtual, assim é possível estabelecer um período de tempo limite (threshold) ocioso configurado que se aplica às suas conexões. Se nenhum pacote houver sido enviado ou recebido até o tempo limite do período de inatividade finalizar, o Balanceador encerra a conexão automaticamente. Favor consultar a documentação online do seu provedor de serviço de nuvem pública, para verificar as melhores indicações para cada ambiente.

  * **Ping Target**: Neste campo o usuário deve informar a combinação Tipo do Protocolo:Porta TCP-IP padrão que será utilizada para conectar-se com a instância (ex. TCP:80). Este parâmetro é importante, pois no caso do Balanceador não conseguir conectar-se com a máquina virtual na porta TCP-IP específica, dentro do período de tempo limite de resposta configurado, a máquina virtual será considerada fora de serviço (out-of-service).
  * **Timeout**: Neste campo o usuário deve informar um número inteiro, ele representa a quantidade de tempo (em segundos) de espera ao receber uma resposta da verificação de integridade. Os valores podem variar entre 2 a 60 segundos - Favor consultar a documentação online do ambiente do provedor de serviço de nuvem, para validar os valores específicos do seu ambiente.
  * **Interval**: Neste campo o usuário deve informar um número inteiro que representa a quantidade (em segundos) de tempo entre cada verificação de integridade. Os valores podem variar entre 5 a 300 segundos - Favor consultar a documentação online do ambiente do provedor de serviço de nuvem para validar os valores específicos do seu ambiente.
  * **Unhealthy threshold**: Neste campo o usuário deve informar um número inteiro que representa a quantidade de verificações de integridade consecutivas com falha que devem ocorrer antes do Balanceador declarar uma máquina virtual fora de serviço (out-of-service) - Favor consultar a documentação online do ambiente do provedor de serviço de nuvem para validar os valores específicos do seu ambiente..
  * **Healthy threshold**: Neste campo o usuário deve informar um número inteiro que representa a quantidade de verificações de integridade consecutivas bemsucedidas que devem ocorrer para o Balanceador declarar uma máquina virtual em serviço (in-service) - Favor consultar a documentação online do ambiente do provedor de serviço de nuvem para validar os valores específicos do seu ambiente.
  * **Botão Editar**: Basta o usuário clicar sobre este botão Editar e a Plataforma uCloud alterna todos os campos das colunas para o modo edição, de forma a permitir o usuário corrigir o conteúdo dos campos e alterar as configurações específicas do Health Check.

.. important:: Importante mencionar: a Porta TCP-IP deste campo deve conter a mesma informada no campo Porta, na Seção Listener.

* **Seção Máquinas Virtuais**: Nesta seção a Plataforma uCloud apresenta a lista de máquinas virtuais que estão sendo monitoradas pelo Balanceador para equilibrar a carga de trabalho da aplicação/servidor.

  * **Nome**: Esta coluna apresenta uma lista com o nome das máquinas virtuais que estão vinculadas ao Balanceador.
  * **Status**: Esta coluna apresenta o status da “saúde” obtido de cada máquina que atende os parâmetros das configurações da seção Health Check, no qual cada máquina virtual pode apresentar o status:
  * **InService**: Máquina virtual em serviço efetivo (OPERACIONAL).
  * **OutOfService**: Máquina virtual fora de serviço efetivo (NÃOOPERACIONAL)
  * **Ações**: Esta coluna apresenta apenas o Ícone de Desconectar VM |icone_associa_vm|: Basta o usuário clicar sobre este ícone para que a Plataforma uCloud desconecte a máquina virtual selecionada do Balanceador, de forma definitiva e imediata. Esta ação não exclui (delete) a máquina virtual do ambiente do provedor de serviço de nuvem (pública e/ou privada). Quando o usuário clicar com o cursor do mouse sobre este ícone, a Plataforma uCloud apresenta uma mensagem pop-up no canto superior direito que solicita a confirmação da ação pelo usuário.

.. image:: /figuras/ucloud_balanceador006.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

  * **Botão Adicionar**: Basta clicar com o cursor do mouse sobre o botão Adicionar, quando for necessário que o usuário acrescente a uma nova máquina virtual um Balanceador. A Plataforma uCloud acrescenta uma nova linha nesta lista conforme a tela abaixo:

.. image:: /figuras/ucloud_balanceador007.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

A seguir a descrição simplificada das colunas:

  * **Nome**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar neste campo com o cursor do mouse, a Plataforma uCloud lista todas as máquinas virtuais ativas, as que pertençam ao mesmo provedor e com as quais o usuário com a sessão ativa tem permissão de interagir.
  * **Ações**: Esta coluna pode apresentar dois ícones, os quais permitem ao usuário a interação com o Balanceador selecionado:
    * **Ícone de Confirmação**: Quando o usuário deseja confirmar a configuração dos parâmetros informados na linha, a tela da Plataforma uCloud apresenta a opção deste ícone de confirmação. Após ter finalizado a inclusão o usuário deve clicar com o cursor do mouse no botão verde para confirmar a inclusão.
    * **Ícone de Cancelamento**: Caso o usuário tenha clicado sobre o Botão de Adicionar, por engano ou não desejar que a inclusão de uma nova máquina virtual seja finalizada, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho para cancelar a alteração.

* **Seção Grupos de Segurança**: Esta seção apresenta o Grupo de Segurança que configura a segurança das Portas TCP-IP e controla o tráfego de pacotes de dados TCP-IP de entrada e saída das máquinas virtuais que estão vinculadas a este Balanceador.

  * **Nome**: Esta coluna apresenta o nome do Grupo de Segurança conforme informado pelo usuário, no momento do seu provisionamento.
  * **Criado Por**: Esta coluna apresenta a credencial de login do usuário responsável pelo provisionamento do Grupo de Segurança.
  * **Ações**: Esta coluna apresenta apenas o Ícone de Desconectar Grupo de Segurança , basta o usuário clicar sobre este ícone para que a Plataforma uCloud possa desconectar o Grupo de Segurança das máquinas virtuais vinculadas ao Balanceador, de forma definitiva e imediata. Esta ação não exclui (delete) o Grupo de Segurança do ambiente do provedor de serviço de nuvem (pública e/ou privada).
  * **Botão Adicionar**: Basta clicar com o cursor do mouse sobre o botão adicionar, quando for necessário para que o usuário acrescente um novo Grupo de Segurança para as máquinas virtuais deste Balanceador. A Plataforma uCloud acrescentará uma nova linha nesta lista conforme a tela abaixo:

.. image:: /figuras/ucloud_balanceador007.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

A seguir a descrição simplificada das colunas:

  * **Nome**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar neste campo com o cursor do mouse, a Plataforma uCloud lista todos os Grupos de Segurança que pertençam ao mesmo provedor e com os quais o usuário com a sessão ativa tem permissão de interagir. ○ Ações: Esta coluna pode apresentar dois ícones, os quais permitem ao usuário a interação com o Balanceador selecionado:
    * **Ícone de Confirmação**: Quando o usuário deseja confirmar a configuração dos parâmetros informados nesta linha, a Plataforma uCloud apresenta um ícone de confirmação, no qual o usuário deve clicar com o cursor do mouse no ícone verde para confirmar a inclusão.
    * **Ícone de Cancelamento**: Caso o usuário tenha clicado sobre o Botão de Adicionar, por engano ou não desejar que a inclusão de uma nova máquina virtual ocorra, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho para cancelar a alteração.


Criando Balanceador (Ambientes AWS e GCP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O processo de provisionamento de um Balanceador por intermédio da Plataforma uCloud é sempre efetuado através de uma interface via API-Rest, desta forma os parâmetros necessários para os ambientes dos provedores de nuvens públicas Amazon Web Services (AWS) e Google Cloud Platform (GCP) solicitam informações similares e a tela de provisionamento para ambos é similar.
Quando o usuário clicar com cursor do mouse sobre o botão Criar Balanceador, a Plataforma uCloud apresenta a tela global abaixo:

.. image:: /figuras/ucloud_balanceador008.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

.. important:: Somente usuários com perfil de Administrador de Grupo ou Administrador de Contrato, tem permissão e podem completar esta operação.

A seguir a descrição detalhada dos campos desta tela:

* **Usuário**: Este campo é obrigatório, ele aparece preenchido com o login do usuário registrado corrente na Plataforma uCloud. Este usuário é utilizado como referência para filtrar as máquinas virtuais específicas que foram provisionadas por este, no campo abaixo. Se for necessário alterar a vinculação ao usuário, basta clicar com o cursor do mouse sobre o botão de Edição “ ” e digitar os caracteres que fazem parte do login do usuário que deve ser vinculado a este Balanceador, em seguida, a Plataforma uCloud apresenta uma lista de logins de usuário que possuem a sequência de caracteres digitado, basta selecionar o login desejado da lista.
* **Container**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta relação de todos os containers provisionados aos quais o usuário está vinculado para uso. Quando o usuário seleciona os provedores AWS ou GCP, a plataforma do uCloud é alterada e apresenta a tela abaixo a ser preenchida:

.. image:: /figuras/ucloud_balanceador009.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

A seguir a descrição dos campos desta tela:

* **Região**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse, neste campo, a Plataforma uCloud apresenta a relação de todas as Regiões Globais que o provedor de serviço de nuvem selecionado acima possui presença.
* **Rede**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta relação de todas as Redes que foram provisionadas para o ambiente do provedor de serviço de nuvem, as quais o usuário com a sessão ativa possui permissão de visualizar.
* **Internal**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta duas opções para que o usuário possa configurar se este Balanceador será para provisionado para atender uma das opções abaixo:
  * **YES**: Selecionar esta opção quando o usuário deseja distribuir o tráfego apenas entre as máquinas virtuais dentro das redes internas do seu ambiente no provedor de serviço de nuvem (pública e/ou privada). Esta opção não contempla qualquer tráfego entrante externo da rede pública (Internet).
  * **NO**: Selecionar esta opção quando o usuário deseja distribuir o tráfego entrante da rede pública (Internet) para as máquinas virtuais dentro das redes internas do seu ambiente no provedor de serviço de nuvem (pública e/ou privada). Esta opção não contempla qualquer tráfego interno do seu ambiente.

* **Nome**: Este campo é obrigatório, nele o usuário deve informar o nome (no mínimo 3 caracteres - no máximo 15 caracteres) com o qual deseja identificar o Balanceador. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).

* **Aba/Tab Listener**: Esta aba é obrigatória, ela permite ao usuário configurar os parâmetros do Protocolo e Porta TCP-IP, do Balanceador e da Máquina Virtual para ser a ‘escuta’ e verificar a disponibilidade da aplicação/serviço. Abaixo a descrição simplificada das colunas:

.. image:: /figuras/ucloud_balanceador010.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

  * **Botão Adicionar**: O usuário deve clicar com o cursor do mouse sobre o botão Adicionar, para acrescentar uma nova linha de configuração de Listener ao Balanceador. A Plataforma uCloud acrescenta uma nova linha nesta lista, com os campos a preencher, conforme a tela acima:
  * **Protocolo do Balanceador**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar nele, com o cursor do mouse, a Plataforma uCloud lista as mesmas opções descritas no campo Protocolo acima descrito. Este campo configura os parâmetros do Protocolo TCP-IP aplicado ao Balanceador.
  * **Porta do Balanceador**: Este campo é obrigatório, o usuário deve informar as Portas TCP-IP Padrão para o tipo do Protocolo selecionado no campo anterior. Este campo configura os parâmetros da Porta TCP-IP aplicado ao Balanceador.
  * **Protocolo da Instância**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar nele, com o cursor do mouse, a Plataforma uCloud lista as mesmas opções especificadas no campo Protocolo acima descrito. Este campo configura os parâmetros do Protocolo TCP-IP aplicado à Máquina Virtual.
  * **Porta da Instância**: Este campo é obrigatório, o usuário deve informar as Portas TCP-IP Padrão para o tipo do protocolo selecionado no campo anterior. Este campo configura os parâmetros da Porta TCP-IP aplicado à Máquina Virtual.
  * **Ação**: Esta coluna apresenta apenas o Ícone da Lata de Lixo “ ”: Basta clicar com o cursor do mouse sobre este botão “Lata de Lixo” e a Plataforma uCloud remove (exclui) esta configuração de Listener deste Balanceador, de forma imediata e definitiva.

* **Aba/Tab Máquina Virtual**: Esta aba é obrigatória, ela permite ao usuário vincular as máquinas virtuais que tem seu tráfego monitorado através do Balanceador para equilibrar as cargas de trabalho. Abaixo a descrição simplificada da coluna:

.. image:: /figuras/ucloud_balanceador011.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

  * **Botão Adicionar**: O usuário deve clicar com o cursor do mouse sobre o botão Adicionar, para acrescentar uma nova máquina virtual ao Balanceador. O usuário deve repetir este procedimento até incluir todas as máquinas virtuais que tem seu tráfego controlado pelo Balanceador (quantas forem necessárias). A Plataforma uCloud acrescenta uma nova linha nesta lista, com os campos a preencher, conforme a tela acima:
  * **Nome**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar neste campo com o cursor do mouse, a Plataforma uCloud lista todas as máquinas virtuais ativas, as que pertençam ao mesmo provedor (região e rede/sub-rede), com as quais o usuário com a sessão ativa tem permissão de interagir.
  * **Ação**: Esta coluna apresenta apenas o Ícone da Lata de Lixo “ ”: Basta clicar com o cursor do mouse sobre este botão “Lata de Lixo” e a Plataforma uCloud remove (exclui) esta máquina virtual deste Balanceador, de forma imediata e definitiva.

* **Aba/Tab Grupos de Segurança**: Esta aba é obrigatória, e permite ao usuário vincular um (ou mais) Grupo de Segurança às máquinas virtuais que terão seu tráfego monitorado para equilibrar o tráfego da carga de trabalho. Abaixo a descrição simplificada da coluna.

.. image:: /figuras/ucloud_balanceador012.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

  * **Botão Adicionar**: O usuário deve clicar com o cursor do mouse sobre o botão Adicionar, para acrescentar um novo Grupo de Segurança ao Balanceador. O usuário deve repetir este procedimento até incluir todos os Grupos de Segurança (quantos forem necessários). A Plataforma uCloud acrescenta uma nova linha nesta lista, com os campos a preencher, conforme a tela acima:
  * **Nome**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar neste campo com o cursor do mouse, a Plataforma uCloud lista todos os Grupos de Segurança provisionados para o provedor de serviço de nuvem (região e rede/sub-rede) e com as quais o usuário com a sessão ativa tem permissão de interagir.
  * **Ação**: Esta coluna apresenta apenas o Ícone da Lata de Lixo |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão “Lata de Lixo” e a Plataforma uCloud remove este Grupo de Segurança deste Balanceador, de forma imediata e definitiva.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de provisionamento de um Balanceador. Após clicar, a Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para o correto funcionamento do Balanceador, nos ambientes do provedor de serviços de nuvem (pública e/ou privada), o usuário pode checar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros para os ambientes, de forma a provisionar um Balanceador.
  Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser preenchido e o campo está em branco, logo a Plataforma uCloud não permitirá o provisionamento do Balanceador.


Criando Balanceador (Ambiente Azure)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O processo de provisionamento de um Balanceador por intermédio da Plataforma uCloud é sempre efetuado através de uma interface via API-Rest, desta forma os parâmetros necessários para o ambiente do provedor de nuvem pública Microsoft Azure possui diferenças sutis em relação aos provedores anteriormente apresentados.

Quando o usuário clicar com cursor do mouse sobre o botão Criar Balanceador, a Plataforma uCloud apresenta a tela global abaixo:

.. image:: /figuras/ucloud_balanceador008.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----


.. important:: Somente usuários com perfil de Administrador de Grupo ou Administrador de Contrato, tem permissão e podem completar esta operação.

A seguir a descrição dos campos desta tela:

* **Usuário**: Este campo é obrigatório, ele aparece preenchido com o login do usuário registrado corrente na Plataforma uCloud. Este usuário é utilizado como referência para filtrar as máquinas virtuais específicas que foram provisionadas por este, no campo abaixo. Se for necessário alterar a vinculação ao usuário, basta clicar com o cursor do mouse sobre o botão de Edição “ ” e digitar os caracteres que fazem parte do login do usuário que deve ser vinculado a este Balanceador, em seguida, a Plataforma uCloud apresenta uma lista de logins de usuário que possuem a sequência de caracteres digitado. Basta selecionar o login desejado da lista.

* **Container**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse a Plataforma uCloud apresenta relação de todos os containers aos quais o usuário está vinculado. Quando o usuário seleciona o provedor Azure, a plataforma do uCloud é alterada e apresenta um aviso referente ao ambiente do provedor de serviço de nuvem Microsoft Azure, pois é mandatório ao usuário selecionar apenas as máquinas virtuais que estejam associadas a um único Grupo de Disponibilidade, favor visualizar a tela abaixo:

.. image:: /figuras/ucloud_balanceador013.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

Após o usuário clicar com o cursor do mouse no botão OK para aceitar o aviso, a Plataforma uCloud apresenta a tela seguinte, a qual solicita provisionar um Balanceador no ambiente do provedor de serviço de nuvem pública Azure:

.. image:: /figuras/ucloud_balanceador014.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

A seguir a descrição dos campos desta tela:

* **Virtual Datacenter**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse, neste campo, a Plataforma uCloud apresenta relação de todos os Virtual Datacenters vinculados a Azure, aos quais o usuário com uma sessão registrada está vinculado.
* **Região**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar com o cursor do mouse, neste campo, a Plataforma uCloud apresenta a relação de todas as Regiões Globais Azure que estão presentes na configuração do Virtual Datacenter selecionado no campo anterior.
* **Rede**: Este campo é obrigatório do tipo “drop down”, quando o usuário clica com o cursor do mouse, neste campo, a Plataforma uCloud apresenta a relação de todas as Redes da Azure que estão presentes na configuração do Virtual Datacenter selecionado no campo anterior
* **Nome**: Este campo é obrigatório, nele o usuário deve informar o nome (no mínimo 3 caracteres - no máximo 15 caracteres) com o qual deseja identificar o Balanceador. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **Protocolo**: Este campo é obrigatório do tipo “drop down”, nele o usuário clica com o cursor do mouse e a Plataforma uCloud apresenta a relação de todos os Tipos de Protocolo TCP-IP disponíveis, apenas para o ambiente do provedor de serviço de nuvem pública Azure, que serão configurados ao Balanceador (Favor consultar a documentação online do provedor para esclarecer o comportamento do Balanceador em relação a cada tipo de protocolo):
  * TCP
  * UDP
*  **Porta**: Este campo é obrigatório, o usuário deve informar o número (inteiro) referente as Portas TCP-IP Padrão para o tipo do Protocolo selecionado no campo anterior. Este campo configura os parâmetros da Porta TCP-IP aplicado ao Balanceador.

* **Aba/Tab Máquina Virtual**: Esta aba é obrigatória, ela permite ao usuário vincular as máquinas virtuais que tem seu tráfego monitorado através do Balanceador para equilibrar as cargas de trabalho. Abaixo a descrição simplificada da coluna:

.. image:: /figuras/ucloud_balanceador015.png
   :alt: Menu Rede - Balanceador
   :scale: 50 %
   :align: center
   :class: with-border

----

  * **Botão Adicionar**: O usuário deve clicar com o cursor do mouse sobre o botão Adicionar, para acrescentar uma nova máquina virtual ao Balanceador. O usuário deve repetir este procedimento até incluir todas as máquinas virtuais que tem o seu tráfego controlado pelo Balanceador (quantas forem necessárias). A Plataforma uCloud acrescenta uma nova linha nesta lista, com campos a preencher, conforme a tela acima:
  * **Nome**: Este campo é obrigatório do tipo “drop down”, quando o usuário clicar neste campo com o cursor do mouse, a Plataforma uCloud lista todas as máquinas virtuais ativas, as que pertençam ao mesmo provedor (região e rede/sub-rede), com as quais o usuário com a sessão ativa tem permissão de interagir.
  * **Ação**: Esta coluna apresenta apenas o **Ícone da Lata de Lixo** |icone_lixo|. Basta clicar com o cursor do mouse sobre este botão “Lata de Lixo” e a Plataforma uCloud remove (exclui) esta máquina virtual deste Balanceador, de forma imediata e definitiva.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de provisionamento de um Balanceador. Após clicar, a Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para o correto funcionamento do Balanceador, nos ambientes do provedor de serviços de nuvem (pública e/ou privada), o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros para os ambientes, de forma a provisionar um Balanceador.
  Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser preenchido e o campo está em branco, logo a Plataforma uCloud não permitirá o provisionamento do Balanceador.


.. Zonas DNS
.. ---------
.. todos ites de DNS abaixo estão comentados, não aparecem no texto html

.. O serviço Domain Name System (DNS) é um serviço hierárquico e distribuído lobalmente de gestão de nomes para computadores, serviços ou qualquer máquina conectada à Internet ou a uma rede privada, O sistema de nomes de domínio (DNS) converte nomes legíveis por humanos (www.exemplo.com) em endereços IP numéricos (192.0.2.1) legíveis e utilizados pelos computadores para conexões entre si. Todos os provedores do serviço de nuvem pública (AWS, Azure e GCP) possuem a facilidade de criar uma Zona DNS.
.. O Sistema de Nomes de Domínio (DNS) é a lista telefônica da Internet. Os seres humanos acessam informações on-line por meio de nomes de domínio, como ustore.com.br. Os navegadores da Internet interagem por meio de endereços IP (Protocolo de Internet). O DNS converte nomes de domínio em endereços IP para que os navegadores possam carregar os recursos da Internet.
.. Para os ambientes de nuvem privada (on-premises) um pré-requisito a ser atendido é o fato da Plataforma uCloud estar corretamente configurada e integrada ao servidor de Rede Definida por Software (SDN) privado (o módulo uSDN) - caso contrário não é possível provisionar Zonas DNS através da interface da Plataforma uCloud. Não é o objetivo deste documento descrever todos os ambientes de nuvem privada, pois cada ambiente possui características únicas, a integração do servidor de SDN (e suas funcionalidades) com a rede de dados corporativa (Corporate LAN) pode não permitir o provisionamento de uma Zona DNS, através da API Rest, como projetado na Plataforma uCloud.
.. O menu Zonas DNS contém todas as zonas de DNS criadas por um usuário em um ambiente de nuvem pública ou on-premises. Para criar uma zona DNS, o usuário deve indicar o container e o nome da zona DNS e uma descrição sobre a Zona DNS a ser criada. Após criado tal zona de DNS, o usuário pode selecionar para editar a mesma e adicionar registros ou editar registros para a zona criada.

.. .. image:: /figuras/ucloud_menu_DNS001.png
   :alt: Menu Rede - Zona DNS
   :scale: 80 %
   :align: center
   :class: with-border

----

.. Quando o usuário acessa o menu Zonas DNS, a Plataforma uCloud apresenta uma lista com todas as zonas de DNS criadas por um usuário no ambiente de um provedor de serviço de nuvem (pública e/ou privada).

.. .. image:: /figuras/ucloud_menu_DNS002.png
   :alt: Menu Rede - Zona DNS
   :scale: 80 %
   :align: center
   :class: with-border

----

.. A seguir a descrição das colunas desta tela:

.. * **Botão “Criar Zona DNS”**: Caso o usuário necessite criar uma Zona DNS no ambiente do provedor de serviço de nuvem privada, basta clicar com o cursor do mouse sobre este botão, favor acompanhar as instruções nos itens abaixo: D. Criar Zona DNS Privada - Observação.
.. * **Botão Criar “Zona DNS Pública”**: Caso o usuário necessite criar uma Zona DNS no ambiente do provedor de serviço de nuvem pública, basta clicar com o cursor do mouse sobre este botão, favor acompanhar as instruções nos itens abaixo: B. Criar ZONA DNS Pública (AWS e GCP) e C. Criar ZONA DNS Pública (Azure).
.. * **Botão Refresh**: A Plataforma uCloud comunica-se com o console dos provedores através da API Rest, portanto, toda ação executada e/ou configurada na plataforma do uCloud passa a ser apresentada imediatamente na tela do usuário, a qual envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes possam executar a ação desejada.

.. .. attention:: Para que o atualizar apenas o conteúdo das seções da tela (ou as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, ele executa apenas a atualização das informações contidas na base de dados da plataforma do uCloud.

.. * **Container**: Esta coluna apresenta o nome do Container em que a Zona DNS foi provisionada.
.. * **Domínio**: Esta coluna apresenta o nome do Domínio, da forma que foi informado pelo usuário no momento deste ser provisionado através da Plataforma uCloud.
.. * **Descrição**: Esta coluna apresenta o conteúdo do campo que descreve o domínio, informado pelo usuário no momento deste ser provisionado através da Plataforma uCloud.
.. * **Criado Por**: Esta coluna apresenta as credenciais de login do usuário que estava registrado na Plataforma uCloud e é o responsável pelo provisionamento da Zona DNS.
.. * **Ação**: Esta coluna apresenta duas opções de ação a ser realizada pelo usuário, por intermédio dos ícones e o usuário possa interagir com a Zona DNS selecionada:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud remove (exclui) esta Zona DNS, de forma imediata e definitiva. Esta ação será efetivada no ambiente de rede selecionado (público e/ou privado), o tempo necessário para que a referida ação seja aplicada é totalmente dependente do tempo do ambiente destino (público e/ou privado), a Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - Consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada.
  * **Ícone Edição**: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela que permite a edição das configurações da Zona DNS, o usuário pode seguir as instruções do item: A. Gerenciar Zona DNS.

.. * **Busca Rápida**: O usuário pode notar que logo abaixo do nome da coluna existe um campo em ‘branco’ que permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de Zonas DNS. Basta preencher o campo em branco com uma sequência de caracteres que possa ser relevante e a Plataforma uCloud atualiza a tela de forma a representar este padrão de busca.

.. Gerenciar Zona DNS Pública
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~

.. Inicialmente, importa destacar que o objetivo deste documento não é esclarecer o leitor nas características técnicas da funcionalidade e seus parâmetros, Zona DNS.

.. Indicamos fortemente ao usuário procurar certificar-se de que possui o correto embasamento técnico para alterar qualquer parâmetro de uma Zona DNS existente.

.. Qualquer alteração nos parâmetros de uma Zona DNS pode desencadear impactos negativos na experiência dos usuários externos (na web, Internet). Favor consultar a documentação online de seu provedor de serviço de nuvem pública para compreender o correto comportamento da Zona DNS por ele oferecida.

.. Quando o usuário clicar com o cursor do mouse sobre algum domínio apresentado na lista ou no ícone de edição, a Plataforma uCloud apresenta uma tela com as informações específicas de uma Zona DNS pública, conforme a tela abaixo:

.. .. image:: /figuras/ucloud_menu_DNS003.png
   :alt: Menu Rede - Zona DNS
   :scale: 80 %
   :align: center
   :class: with-border

----

.. A seguir, a descrição das seções desta tela:

.. * **Botão Excluir “Zona DNS”**: Basta o usuário clicar com o cursor do mouse sobre este botão e a Plataforma uCloud remove (exclui) esta Zona DNS do ambiente do provedor de serviço de nuvem (pública e/ou privada), de forma imediata e definitiva.

..  O tempo necessário para que a referida ação seja aplicada será totalmente dependente do tempo do ambiente destino (público e/ou privado), a Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - favor consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada. Esta ação também remove o custo recorrente do recurso da conta do provedor de serviço de nuvem (pública e/ou privada).

..  Quando o usuário clicar com o cursor do mouse sobre este ícone, a Plataforma uCloud exibe um ‘pop up’ na tela e solicita confirmar a ação do usuário:

.. * **Seção Geral**: Nesta seção são apresentadas as informações genéricas da rede que foram informadas pelo usuário no momento do seu provisionamento:

..  * Container (exclusivo AWS): Este campo apresenta o nome do Container ao qual a Zona DNS está vinculada.
..  * Rede (exclusivo AWS): Este campo apresenta o nome da Rede (e Sub-Rede) ao qual a Zona DNS está vinculada.
..  * Domínio: Este campo apresenta o nome do domínio provisionado no ambiente do provedor de serviço de nuvem pública.
..  * Descrição: Este campo apresenta a descrição referente ao domínio provisionado no ambiente do provedor de serviço de nuvem pública.
..  * Criado por: Este campo apresenta as credenciais de login do usuário que estava registrado na Plataforma uCloud, ele será o responsável pelo provisionamento da Zona DNS.

.. * **Seção Registros do DNS**: Nesta seção são apresentadas as informações técnicas e específicas da Zona DNS, as quais são obtidas através sincronização da Plataforma uCloud com o ambiente do provedor de serviço de nuvem pública.
..   * **Registro**: Este campo apresenta a lista de todos os registros dos nomes que foram provisionados pelos usuário(s) a partir da criação do domínio. Favor consultar a documentação online do seu provedor de serviço de nuvem pública para entender as características específicas para o ambiente do provedor de serviço.
..   * **Tipo**: Este campo apresenta a característica específica do Tipo de registro (ex.: servidor de nome {NS} e de início de autoridade {SOA} para a ZonaDNS). Favor consultar a documentação online do seu provedor de serviço de nuvem pública para entender as características específicas para o ambiente do provedor de serviço.
..   * **TTL**: A configuração de TTL (Time To Live) de um registro determina por quanto tempo o usuário deseja que os resolvedores de DNS armazenem o registro e usem as informações em cache. A configuração de TTL típica para o registro de Name Service é de 172.800 segundos ou dois dias. Favor consultar a documentação online do seu provedor de serviço de nuvem pública para entender as características específicas para o ambiente do provedor de serviço.

..   * **Valor**: Este campo apresenta o conteúdo do registro anteriormente provisionado pelo usuário. Favor consultar a documentação online do seuprovedor de serviço de nuvem pública para entender as características específicas para ambiente do provedor de serviço.

..   * **Ações**: Esta coluna pode apresentar apenas uma ação ao exibir o Ícone Edição “ ”, quando o usuário clicar sobre este ícone a Plataforma uCloud alterna todos os campos das colunas, para o modo ‘Edição’, de forma que permite o usuário corrigir o conteúdo dos campos e alterar as configurações do registro selecionado:

..     * **Ícone de Confirmação**: Quando o usuário deseja confirmar aconfiguração dos parâmetros informados nesta linha, a Plataforma uCloud apresenta um ícone de confirmação. Após ter finalizado aconfiguração do registro, o usuário deve clicar com o cursor do mouse no botão verde para confirmar as alterações ou inclusão.
..     * **Ícone de Cancelamento**: Caso o usuário tenha clicado sobre um botão por engano ou não deseja que a inclusão de um novo registro seja armazenado (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna para os valores iniciais, antes de proceder qualquer preenchimento ou alteração:

..   * **Botão “Adicionar Registro DNS”**: Caso o usuário necessite criar um novo Registro DNS no ambiente do provedor de serviço de nuvem (público ou privado), basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud acrescenta uma nova linha nesta lista com todos os campos em branco, permite ao usuário configurar da forma necessária, conforme a tela abaixo:

.. .. image:: /figuras/ucloud_menu_DNS004.png
   :alt: Menu Rede - Zona DNS
   :scale: 80 %
   :align: center
   :class: with-border

----

.. Após incluir todas as informações necessárias para provisionar o novo registro, basta o usuário clicar com o cursor do mouse no Ícone de Confirmação o que permite a Plataforma uCloud provisionar o novo registro, de forma definitiva no ambiente do provedor de serviço de nuvem pública. Favor consultar a documentação online do seu provedor de serviço de nuvem pública, se precisar entender as características específicas para ambiente do provedor de serviço.

.. Criar Zona DNS Pública (AWS e GCP)
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. nunca vi o processo não sei como documentar


.. Criar Zona DNS Pública (Azure)
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
.. nunca vi o processo não sei como documentar

.. Criar Zona DNS Privada - Observação
.. ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. Para os ambientes de nuvem privada (on-premises) um pré-requisito é o de que a Plataforma uCloud esteja corretamente configurada e integrada ao servidor de SDN privado (módulo uSDN), caso contrário não é possível provisionar Zonas DNS através da interface da Plataforma uCloud. Não é objetivo deste documento descrever todos os ambientes de nuvem privada, pois cada ambiente possui características únicas, a integração do servidor de SDN (suas funcionalidades) com a rede de dados corporativa (Corporate LAN) pode não permitir o provisionamento de uma Zona DNS, através da API Rest, como projetado na Plataforma uCloud.

.. Favor entrar em contato com a Equipe de Suporte Técnico da Ustore para verificar se a integração do módulo uSDN está corretamente configurado no seu ambiente e integrado com a rede corporativa local (LAN).

.. A Equipe de Suporte Técnico pode apresentar as melhores práticas e orientar o correto processo de provisionamento de Zona DNS em ambiente de rede corporativa privada (on-premises).

VPN
---

O termo conexão Virtual Private Network (VPN) possui sentido amplo, mas, neste documento, o termo se refere especificamente à conexão entre as redes do ambiente de rede do provedor de serviço de nuvem pública (dentro da qual estão os recursos computacionais de nuvem) e sua rede local (com seus recursos computacionais dentro da rede corporativa). A VPN de local para local oferece suporte para as conexões VPN da Internet Protocol Security (IPsec).

Por padrão, os recursos de máquinas virtuais existem dentro do ambiente do provedor de serviço de nuvem pública, portanto, não podem comunicar-se com sua rede corporativa local, pois a rede do provedor é uma rede remota. O usuário pode habilitar o acesso a esta rede remota, basta criar uma conexão VPN e configurar o roteamento para transmitir o tráfego através desta conexão.

Importante estabelecer alguns conceitos básicos neste documento, pois o processo de provisionamento de uma VPN envolve algumas etapas, como descrito:

O usuário pode seguir os principais conceitos do Site-to-Site VPN:

A. **Conexão VPN**: uma conexão para o tráfego seguro de pacotes de dados TCP-IP em uma conexão encriptada entre a sua rede local corporativa e o ambiente de rede do provedor de serviço de nuvem pública.
B. **Túnel VPN**: um link criptografado em que os dados podem transmitir da rede do cliente para a rede do provedor de serviço de nuvem pública ou vice-versa. Cada conexão VPN pode incluir dois túneis VPN, os quais o usuário pode usar simultaneamente, para alta disponibilidade.
C. **Customer Gateway**: um recurso lógico do provedor de serviço de nuvem pública que fornece informações para o provedor sobre o dispositivo de gateway do cliente.
D. **Virtual Private Gateway**: é um dispositivo físico ou uma aplicação de software, situada no ambiente do cliente que será o ponto de conexão do Site-to-Site VPN.

.. image:: /figuras/ucloud_menu_vpn001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 10 %
   :align: center

----

Quando o usuário acessar o menu VPN, a Plataforma uCloud apresentará todas as VPNs (e os seus componentes) vinculados ao contrato ao qual o usuário registrado está vinculado. Esta lista inclui todas as VPNs provisionadas por todos os usuários do mesmo contrato.
O menu VPN contém todas as VPNs criadas por um usuário em um ambiente de nuvem pública ou on-premisses.

Quando o usuário acessar o menu VPN, a Plataforma uCloud apresentará todas as VPNs (e os seus componentes) vinculados ao contrato ao qual o usuário registrado está vinculado. Esta lista inclui todas as VPNs provisionadas por todos os usuários do mesmo contrato.

O menu VPN contém todas as VPNs criadas por um usuário em um ambiente de nuvem pública ou on-premisses.

.. image:: /figuras/ucloud_menu_vpn002.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

.. note:: Os Endereços TCP-IP apresentados na tela acima são ilustrativos.

Esta tela possui uma seção para cada configuração, segue detalhamento das informações apresentadas nas colunas de cada seção:

* **Seção Customer Gateway**: Esta seção apresenta as informações específicas do Custmer Gateway.

  * **Container**: Esta coluna apresenta o nome do Container no qual o Customer Gateway está vinculado, selecionado pelo usuário logado, no momento do provisionamento.
  * **Região**: Esta coluna apresenta o nome da Região Global, a qual o Customer Gateway está vinculado, selecionada pelo usuário logado, no momento do provisionamento.
  * **Nome**: Esta coluna apresenta o nome informado pelo usuário durante o provisionamento do Customer Gateway.
  * **Endereço IP**: Esta coluna apresenta o CIDR do Endereço TCP-IP, informado pelo usuário durante o provisionamento do Customer Gateway.
  * **BGP ASN**: Esta coluna apresenta a informação do Border Gateway Protocol (BGP) e do Autonomous System Number (ASN) ele é disponibilizado apenas quando um Customer Gateway elege o roteamento dinâmico. Quando selecionado o roteamento estático, esta coluna pode apresentar o CIDR do Endereço TCP-IP.
  * **Criado Por**: Esta coluna apresenta o nome do usuário que estava com a sessão ativa na Plataforma uCloud no momento da criação, foi o responsável pelo provisionamento do Customer Gateway.
  * **Ações**: Esta coluna apresenta apenas um ícone de ação |icone_lixo|, ela permite ao usuário remover o Customer Gateway. O usuário deve clicar com o cursor do mouse sobre o Ícone Lata de Lixo e a Plataforma uCloud apresenta uma tela *pop up* , a qual solicita ao usuário confirmar a exclusão da configuração de Customer Gateway.

* **Seção Virtual Private Gateway**: Esta seção apresenta as informações específicas do Private Gateway.

  * **Container**: Esta coluna apresenta o nome do Container no qual o Virtual Private Gateway está vinculado, selecionado pelo usuário logado, no momento do provisionamento.
  * **Região**: Esta coluna apresenta o nome da Região Global, a qual o Virtual Private Gateway está vinculado, selecionado pelo usuário logado, no momento do provisionamento.
  * **Nome**: Esta coluna apresenta o nome informado pelo usuário durante o provisionamento do Virtual Private Gateway.
  * **Rede**: Esta coluna apresenta a identificação da Rede (e o CIDR do Endereço TCP-IP) selecionado pelo usuário durante o provisionamento do Virtual Private Gateway. Somente podem ser vinculadas às Redes que foram criadas para a Região apresentada na coluna anterior.
  * **Criado Por**: Esta coluna apresenta o nome do usuário que estava com a sessão ativa na Plataforma uCloud no momento da criação, o responsável pelo provisionamento do Virtual Private Gateway.
  * **Ações**: Esta coluna pode apresentar três ícones de ação, ela permite ao usuário interagir com o Virtual Private Gateway selecionado:

    * **Ícone Conectar a uma Rede** |icone_conecta_rede|: Quando o usuário necessita vincular o Virtual Private Gateway a uma rede existente na Região, basta clicar com o cursor do mouse sobre este ícone e a Plataforma uCloud apresenta a tela abaixo, nela o usuário pode selecionar a Rede que deseja vincular ao Virtual Private Gateway.

.. image:: /figuras/ucloud_menu_vpn003.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

    O campo Rede é um campo do tipo *drop down*, basta o usuário clicar com o cursor do mouse sobre o campo para a Plataforma uCloud apresentar uma lista de todas as redes provisionadas para a Região. Após selecionar a rede desejada o usuário deve clicar com o cursor do mouse sobre o botão “Attach” para vincular o Virtual Private Gateway à rede. Neste momento, a Plataforma uCloud fecha esta tela e retorna à tela anterior.

    * **Ícone Desconectar VM**: Basta o usuário clicar sobre este ícone e a Plataforma uCloud desconecta a rede do Virtual Private Gateway, de forma definitiva e imediata. Esta ação não exclui (delete) a rede da região do ambiente provedor de serviço de nuvem (pública e/ou privada).
    * **Ícone Lata de Lixo**: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela *pop up* a qual solicita ao usuário confirmar a exclusão da configuração de Customer Gateway, ver a seguir o exemplo:

* **Seção VPN**

  * **Container**: Esta coluna apresenta o nome do Container no qual o Túnel VPN está vinculado, selecionado pelo usuário logado, no momento do provisionamento.
  * **Região**: Esta coluna apresenta o nome da Região Global, a qual o Túnel VPN está vinculado, selecionado pelo usuário logado, no momento do provisionamento.
  * **Nome**: Esta coluna apresenta o nome informado pelo usuário durante o provisionamento do Túnel VPN.
  * **Virtual Private Gateway**: Esta coluna apresenta o nome do Virtual Private Gateway ao qual o Túnel VPN está vinculado.
  * **Customer Gateway**: Esta coluna apresenta o nome do Customer Gateway ao qual o Túnel VPN está vinculado.
  * **Static IP Prefixes**: Esta coluna apresenta a identificação CIDR (Endereços TCP-IP) do lado do gateway do cliente (no local) que tem permissão para se comunicar pelos túneis de VPN. O padrão é 0.0.0.0/0 (todo e qualquer endereço de dentro da rede corporativa).
  * **Criado Por**: Esta coluna apresenta o nome do usuário que estava com a sessão ativa na Plataforma uCloud no momento da criação, o responsável pelo provisionamento do Túnel VPN.
  * **Ações**: Esta coluna apresenta dois ícones de ação, ela permite ao usuário interagir com o Túnel VPN selecionado:
    * **Ícone de Download**: Para que o usuário possa efetuar o download da configuração do Túnel VPN, ele necessita clicar com o cursor do mouse sobre este ícone ‘Download’ para a Plataforma uCloud apresentar a tela abaixo:

.. image:: /figuras/ucloud_menu_vpn004.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

    Cada campo apresentado nesta tela é do tipo “drop down”, basta o usuário clicar sobre o campo e a Plataforma uCloud apresenta as opções disponíveis a serem selecionadas pelo usuário.
    Após selecionar uma das três opções desta tela, basta o usuário clicar no botão “Download” para que a Plataforma uCloud possa armazenar esse arquivo de configuração no folder ou diretório padrão para download configurado no navegador de Internet (Internet Browser) do usuário. Depois de encontrar o arquivo, o usuário deve seguir os procedimentos especificados pelo fabricante selecionado para iniciar e estabelecer a conexão segura do Túnel VPN da sua rede corporativa local com o ambiente de rede do provedor de serviço de nuvem pública.

    * **Ícone Lata de Lixo** |icone_lixo|: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela "pop up’ com a solicitação de que o usuário confirme a exclusão da configuração do Túnel VPN.

.. important:: As opções disponíveis são extraídas diretamente do ambiente selecionado do provedor de serviço de nuvem pública (Container), a Plataforma uCloud não limita ou adiciona qualquer uma das opções apresentadas. Cada ambiente de provedor de serviço de nuvem pública possui suporte a determinadas plataformas e suas versões de software de VPN do fornecedor preferido.


Criar a VPN em 3 Passos
~~~~~~~~~~~~~~~~~~~~~~~

Caro usuário, mais uma vez é enfatizada, fortemente, a ação de buscar informação e conhecimento ao consultar a documentação online do provedor de serviço de nuvem pública específico, para verificar a disponibilidade de fornecedores de tecnologia de VPN, antes de iniciar o provisionamento da conectividade VPN.

Ao criar uma VPN em nuvem pública o usuário deve seguir a seguinte ordem no processo de provisionar corretamente uma conexão VPN (Túnel VPN), é necessário provisionar cada item isolado e sequencialmente:

#. Customer Gateway
#. Private Gateway
#. Túnel VPN

Abaixo segue a descrição de cada etapa do processo.

Criar Customer Gateway
~~~~~~~~~~~~~~~~~~~~~~

A primeira atividade do processo de criação é o provisionamento de um Customer Gateway, um recurso lógico do provedor de serviço de nuvem pública que fornece informações para o provedor sobre o dispositivo de gateway do cliente. Para isso, o usuário deve seguir os seguintes passos:

* **Botão “Criar Customer Gateway”**: O usuário deve clicar com o cursor do mouse sobre o botão Customer Gateway e a Plataforma uCloud apresenta a seguinte tela:

.. image:: /figuras/ucloud_menu_vpn005.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Abaixo a descrição dos campos desta tela:

* **Usuário**: Este campo aparece na tela preenchido (por padrão), apresenta as credenciais do usuário logado, ou seja, com sessão ativa na Plataforma uCloud. Este usuário é vinculado e identificado como o responsável pelo provisionamento deste Customer Gateway.
* **Container**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse a Plataforma uCloud apresenta a relação de todos os Containers aos quais o usuário, com uma sessão ativa, está vinculado.
* **Nome**: Este campo é obrigatório, nele o usuário deve informar o nome (no mínimo 3 caracteres - no máximo 15 caracteres) com o qual deseja identificar este Customer Gateway. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **Região**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação de todas as Regiões Globais, as quais o usuário, com uma sessão ativa, possui permissão para visualizar ou está vinculado.
* **Roteamento**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud lista as duas opções:

  * **Estático**: Quando selecionada esta opção cabe ao usuário informar o Endereço TCP-IP estático, no campo a seguir.
  * **Dinâmico Requer (BGP)**: Quando selecionada esta opção, o usuário deve informar o Endereço TCP-IP do Border Gateway Protocol (BGP) ASN do seu gateway client. O usuário pode usar um ASN existente atribuído à sua rede. No caso de não ter um, pode usar um ASN privado no intervalo 64512-65534.

* **Endereço IP**: Este campo é obrigatório, o usuário deve informar o Endereço TCP-IP do gateway da VPN: Por representar um CIDR da rede interna do provedor, o usuário deve verificar se existe alguma Rede (Sub-rede) anteriormente provisionada para a região global selecionada no campo anterior.
* **Agendar**: Este ícone permite ao usuário agendar o provisionamento do Customer Gateway, o valor padrão é Desabilitado (cor vermelha).
* **Ícone Desabilitado** |icone_desb_verm|: Este ícone indica que não existe agendamento estabelecido. Isto significa que este Customer Gateway será imediatamente provisionado no ambiente do provedor de serviço de nuvem pública, basta o usuário clicar com o cursor do mouse no botão Criar (cor verde).
* **Ícone Habilitado** |icone_habil_verde|: Este ícone indica que o usuário pretende agendar uma data para o provisionamento de um Customer Gateway, no ambiente do provedor de serviço de nuvem pública. Este processo permite escolher a melhor data para que o recurso computacional de nuvem possa iniciar sua cobrança de valores em datas pré-definidas, pela empresa usuária da Plataforma uCloud. Quando o usuário clicar no botão e alterar o ícone para habilitado (cor verde), a Plataforma uCloud permite inserir a data desejada.
* **Ícone Calendário** |icone_agenda|: Basta o usuário clicar sobre o ícone do calendário para a Plataforma uCloud apresentar na tela o ‘pop-up’ que permite o usuário selecionar a data desejada, conforme a imagem abaixo:

.. image:: /figuras/ucloud_menu_maquinas_virtuais_035b.png
   :alt: Virtual Datacenter - Exemplo
   :align: center

----

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Customer Gateway. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação do Customer Gateway, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros para o ambiente do provedor de serviço de nuvem pública, para o completo provisionamento de um Customer Gateway. Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser preenchido e o campo está em branco, logo a Plataforma uCloud não permitirá o provisionamento do Customer Gateway, o recurso lógico do provedor de serviço de nuvem pública que fornece informações para o provedor sobre o dispositivo de gateway do cliente.

Criar Private Gateway
~~~~~~~~~~~~~~~~~~~~~

Após a criação do Customer Gateway o usuário deve criar o Virtual Private Gateway, o dispositivo físico e/ou uma aplicação de software, situada no ambiente do cliente que será o ponto de conexão do Site-to-Site VPN. O qual deve ser vinculado ao Customer Gateway.

* **Botão “Criar Virtual Private Gateway”**: Para criar o Virtual Private Gateway o usuário deve clicar com o cursor do mouse sobre este botão, como resultado a Plataforma uCloud apresenta a seguinte tela:

.. image:: /figuras/ucloud_menu_vpn006.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

A seguir a descrição detalhada dos campos desta tela:

* **Usuário**: Este campo aparece na tela preenchido (por padrão) com as credenciais do usuário logado, com uma sessão ativa na Plataforma uCloud. Este usuário é vinculado ao Private Gateway e é identificado como o usuário responsável pelo provisionamento.
* **Container**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação de todos os Containers, aos quais o usuário, com uma sessão ativa, está vinculado.
* **Região**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação de todas as Regiões Globais, as quais o usuário, com uma sessão ativa, possui permissão para visualizar ou está vinculado.
* **Nome**: Este campo é obrigatório nele o usuário deve informar o nome (no mínimo 3 caracteres - no máximo 15 caracteres) com o qual deseja identificar este Private Gateway. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Private Gateway. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação do Private Gateway, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros para o ambiente do provedor de serviço de nuvem pública, para o completo provisionamento de um Private Gateway. Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser preenchido e o campo está em branco, logo a Plataforma uCloud não permitirá o provisionamento do Private Gateway. O dispositivo físico ou uma aplicação de software, situada no ambiente do cliente que será o ponto de conexão do Site-to-Site VPN.

Criar Túnel VPN
~~~~~~~~~~~~~~~

Para criar o túnel VPN que é um link criptografado em que os dados podem transmitir da rede do cliente para a rede do provedor de serviço de nuvem pública e vice-versa. E que cada conexão VPN pode incluir dois túneis VPN, os quais podem ser utilizados simultaneamente, para a alta disponibilidade.
Deste modo, após a criação do Customer Gateway o usuário deve criar o Virtual Private Gateway que será vinculado ao Customer Gateway. O usuário deve clicar no botão Criar VPN e a plataforma do uCloud exibe a tela a seguir:

.. image:: /figuras/ucloud_menu_vpn007.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Abaixo segue a descrição dos campos desta tela:

* **Usuário**: Este campo (por padrão) aparece na tela preenchido com as credenciais do usuário logado que está com uma sessão ativa na Plataforma uCloud. Este usuário será vinculado ao Túnel VPN para ser identificado como o usuário responsável pelo provisionamento deste.
* **Container**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação de todos os Containers, aos quais o usuário, com uma sessão ativa, está vinculado.
* **Virtual Datacenter (exclusivo para Azure)**: Este campo é do tipo “drop down”, apresentado apenas quando selecionada uma nuvem Azure como provedor de serviço de nuvem pública. Basta o usuário clicar com o cursor do mouse, a Plataforma uCloud exibe a lista de todos os VDC’s vinculados ao ambiente Azure.
* **Região**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação de todas as Regiões Globais, as quais o usuário, com uma sessão ativa, possui permissão para visualizar ou está vinculado.
* **Nome**: Este campo é obrigatório e o usuário deve informar o nome (no mínimo 3 caracteres) com o qual deseja identificar este Túnel VPN. Sugerimos utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido).
* **Virtual Private Gateway**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a lista com todos os Virtual Private Gateway provisionados e vinculados ao Container e Região os quais o usuário, com uma sessão ativa, foi vinculado.
* **Customer Gateway**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud exibe a lista de todos os Customer Gateway provisionados e vinculados ao Container, Região e Virtual Private Gateway os quais o usuário, com uma sessão ativa, foi vinculado.
* **Senha**: Este campo é obrigatório, o usuário deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”, conforme a documentação encontrada nos websites online dos provedores de serviço de nuvem pública. Ela deve ser preenchida com a sequência de caracteres da senha do usuário.
  **Importante ressaltar**: esta sequência deve ser no mínimo de oito (08) caracteres alfanuméricos e no máximo setenta e dois (72) caracteres, ela deve conter caracteres de três das seguintes categorias:

  * Letras maiúsculas e minúsculas (A a Z);
  * Números de base 10 (de 0 a 9);
  * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' <>,.? /) – Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Túnel VPN. A Plataforma uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após o usuário informar todos os parâmetros fundamentais para a criação do Túnel VPN, o usuário pode verificar que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão Criar e a Plataforma uCloud envia todos os parâmetros para o ambiente do provedor de serviço de nuvem pública, para o completo provisionamento de um Túnel VPN. Caso este botão não esteja habilitado (cor cinza), significa que algum parâmetro anterior deixou de ser preenchido e o campo está em branco, logo a Plataforma uCloud não permitirá o provisionamento do Túnel VPN.

Para o caso de criar VPNs IPSEC, a plataforma do uCloud abre um *pop up* para exibir as três opções de sub-menus, neste momento o usuário deve preencher as seguintes informações:

.. image:: /figuras/ucloud_menu_vpn008.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

**Aba: General**

  * **Usuário**: Este campo (por padrão) aparece na tela preenchido com as credenciais do usuário logado, com uma sessão ativa na Plataforma uCloud. Este usuário é vinculado ao VPN IPSec e identificado como o responsável pelo provisionamento. Ou seja, o usuário é o proprietário do container no qual o Gateway será criado.
  * **Nome**: Este campo é obrigatório nele o usuário deve informar o nome (no mínimo 3 caracteres - no máximo 15 caracteres) com o qual deseja identificar esta VPN. A sugestão é utilizar somente os caracteres ASCII padrão (letras ou números), não usar espaços em branco caracteres de pontuação ou caracteres acentuados (ASCII Estendido). Ou seja, o nome da VPN a ser criada.
  * **Container**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação de todos os Containers, aos quais o usuário está vinculado, com uma sessão ativa. Neste container a VPN é criada.
  * **Virtual Datacenter (exclusivo para Azure)**: Este campo é do tipo “drop down", apresentado apenas quando selecionada uma nuvem Azure como provedor de serviço de nuvem pública. Basta o usuário clicar com o cursor do mouse, a Plataforma uCloud exibe a lista de todos os VDC’s vinculados ao ambiente Azure no qual a VPN está vinculada. Ou seja, o VDC no qual a VPN é criada.
  * **Subnet**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a lista de todas as Sub-Redes, as quais o usuário está com uma sessão ativa e a VPN está vinculada. É a Subnet na qual a CPN será criada.
  * **Redes Remotas**: Este campo é obrigatório, o usuário deve informar o Endereço TCP-IP CIDR das redes que são roteadas pela VPN.

**Aba: Network**

* **IPsec Remote Gateway**: Este campo é obrigatório nele o usuário deve informar o Endereço TCP-IP do Gateway da VPN Remota.
* **Rede Remota**: Este campo é obrigatório neste o usuário deve informar o Endereço TCP-IP CIDR das redes a serem roteadas pela VPN.
* **Shared Secret PSK**: Este campo é obrigatório nele o usuário deve informar a Shared Key definida para esta VPN.
* **Remote IKE ID**: Este campo é obrigatório nele o usuário deve informar ID do IKE (Internet Key Exchange) da rede remota.
* **Local IKE ID**: Este campo é obrigatório, o usuário deve informar ID do IKE (Internet Key Exchange) da rede local.

**Aba: Proposal**

  Ao clicar neste último submenu, são exibidas fases novas nos sub-menus internos, são elas: (i) o IKE (Phase 1) Proposal e (ii) o IKE (Phase 2) Proposal. A seguir documentadas:

.. image:: /figuras/ucloud_menu_vpn009.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  **Sub-menu interno : IKE (Phase 1) Proposal**

    * **DH Group**: Este campo é obrigatório nele o usuário deve definir o tamanho das chaves podendo ser de 256 bits a 2048 bits com ou sem curvas elípticas.
    * **Encryption**: Este campo é obrigatório, neste o usuário deve informar os algoritmos de criptografia simétrica podendo ser AES 128 e 256.
    * **Authentication**: Este campo é obrigatório nele o usuário deve informar o método de autenticação, pode ser SHA1.
    * **Lifetime (seconds)**: Este campo é obrigatório, neste o usuário deve informar o tempo de vida do IKE (Fase 1) Proposal

  **Sub-menu interno: IKE (Phase 2) Proposal**

    * **Active PFS**: Este campo é obrigatório nele o usuário deve configurar e/ou analisar se habilita a opção de não repetir chaves já negociadas.
    * **Encryption**: Este campo é obrigatório, o usuário deve informar os algoritmos de criptografia simétrica podendo ser AES 128 e 256.
    * **Authentication**: Este campo é obrigatório nele o usuário deve informar o método de autenticação, pode ser SHA1.
    * **Lifetime (seconds)**: Este campo é obrigatório, o usuário deve informar o tempo de vida do IKE (Fase 2) Proposal.

  Ao finalizar ou concluir todas as fases acima descritas e detalhadas, a Plataforma uCloud acrescenta a recente configuração do Túnel VPN na lista da tela inicial, na seção Túnel VPN, conforme apresenta a tela abaixo:

  O usuário pode perceber que a coluna Ações exibe dois ícones, abaixo detalhados:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela solicitando ao usuário confirmar a exclusão da configuração da VPN, com a frase: “Tem certeza? A VPN não pode ser recuperada” apresenta duas opções: “Não, cancelar” e “Sim, pode excluir”
  * **Ícone Download da Configuração**: Basta o usuário clicar com o cursor do mouse sobre este ícone e a Plataforma uCloud apresenta a tela abaixo, nomeada ‘Selecione'. Nela o usuário pode eleger qual é o fornecedor em sua rede corporativa para obter o script de configuração de acesso e para estabelecer o Túnel VPN correto ao seu ambiente:

.. image:: /figuras/ucloud_menu_vpn010.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  O usuário pode perceber que a coluna Ações exibe dois ícones, abaixo detalhados:
  
    * **Ícone Lata de Lixo** |icone_lixo|: Basta o usuário clicar sobre este ícone e a Plataforma uCloud apresenta uma tela solicitando ao usuário confirmar a exclusão da configuração da VPN.
    * **Ícone Download da Configuração** |icone_download|: Basta o usuário clicar com o cursor do mouse sobre este ícone e a Plataforma uCloud apresenta a tela abaixo, nomeada ‘Selecione'. Nela o usuário pode eleger qual é o fornecedor em sua rede corporativa para obter o script de configuração de acesso e para estabelecer o Túnel VPN correto ao seu ambiente:

.. image:: /figuras/ucloud_menu_vpn011.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  A seguir a descrição detalhada dos campos da tela acima:
  * **Vendor**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a listagem com todas as opções de plataformas disponíveis no ambiente do provedor de serviço de nuvem pública. Importante ressaltar: as opções mostradas neste campo são extraídas do ambiente do provedor de serviço de nuvem pública, a Plataforma uCloud não adiciona ou limita as opções exibidas. Apenas a título ilustrativo é demonstrado um resultado específico das opções de fornecedores para um ambiente de Túnel VPN para AWS:

.. image:: /figuras/ucloud_menu_vpn012.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * **Platform**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação com todas as opções de plataformas disponíveis no ambiente do provedor de serviço de nuvem pública, elas são específicas do fornecedor de tecnologia da VPN selecionado no campo Vendor. Importante ressaltar: as opções mostradas neste campo são extraídas do ambiente do provedor de serviço de nuvem pública, a Plataforma uCloud não adiciona ou limita as opções exibidas.
  * **Software**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud apresenta a relação com todas as opções de versões de software, as plataformas disponíveis no ambiente do provedor de serviço de nuvem pública, elas são específicas do fornecedor de tecnologia da VPN selecionado no campo Vendor.
  * **Botão Cancelar**: O usuário pode usar este botão para cancelar o download da configuração do Túnel VPN. A Plataforma uCloud encerra a tela e retorna à tela anterior.
  * **Botão Download**: Após o usuário informar todos os parâmetros fundamentais basta clicar com o cursor do mouse sobre o botão Download e a Plataforma uCloud inicia a transferência do arquivo de configuração no folder ou diretório padrão para descarregamento, configurado no navegador de Internet (Internet browser) do usuário. Após encontrar o arquivo o usuário deve seguir os procedimentos especificados pelo fabricante selecionado para iniciar e estabelecer a conexão segura do Túnel VPN da sua rede corporativa local com o ambiente de rede do provedor de serviço de nuvem pública.

.. note:: As opções mostradas no campo *Software* são obtidas via API diretamente do ambiente nativo do provedor de serviço de nuvem pública, a Plataforma uCloud não adiciona ou limita as opções exibidas.


Menu Storage
============

Depois do provisionamento de um Container (provedor de nuvem pública), a Plataforma uCloud efetua a ‘importação’ de todas as suas características e recursos computacionais existentes, deste modo permite ao usuário interação neste ambiente através da interface do uCloud, um dos recursos computacionais disponíveis é o recurso de armazenamento (Storage).

Este tipo de recurso não está habilitado para ser alterado através da Plataforma uCloud, toda e qualquer alteração deve ser efetuada por meio do console específico de cada provedor de serviço de nuvem pública. Portanto, o usuário tem disponível apenas a facilidade de visualizar as características do recurso computacional através da interface da Plataforma uCloud.

Quando o usuário acessa o menu Storage, a Plataforma uCloud apresenta uma lista com os recursos de armazenamento provisionados no ambiente do provedor de serviço de nuvem pública.

.. image:: /figuras/ucloud_menu_storage001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

A seguir a descrição das características de cada coluna:
* **Nome do Container**: Esta coluna apresenta o nome do container. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no campo ‘Busca Rápida - abaixo do título desta coluna’, a Plataforma uCloud apresenta a listagem com todos os containers que o usuário registrado está vinculado, para restringir a lista de recursos do Storage, específicos do container selecionado.

.. note:: Para a Plataforma uCloud, um container representa um provedor de serviço de nuvem (pública e/ou privada).

* **Nome**: Esta coluna apresenta o nome do recurso computacional do Storage (armazenamento) tal como existente no ambiente do provedor de serviço de nuvem pública. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud permite ao usuário digitar uma sequência de caracteres para limitar a lista de recursos computacionais do Storage.
* **Tamanho**: Esta coluna apresenta o tamanho total do recurso computacional do Storage (armazenamento) da mesma maneira que este existe no ambiente do provedor de serviço de nuvem pública.
* **Utilizado**: Esta coluna apresenta o valor total da ocupação do recurso computacional do Storage (armazenamento) tal como este se encontra no ambiente do provedor de serviço de nuvem pública.
* **Uso**: Esta coluna apresenta o percentual de ocupação do recurso computacional do Storage (armazenamento) da mesma maneira como este se encontra no ambiente do provedor de serviço de nuvem pública.
* **Upload**: Esta coluna apresenta a informação sobre este recurso computacional do Storage (armazenamento) que está habilitado para receber os dados para serem armazenados diretamente de uma rede externa, esta informação é obtida diretamente do ambiente do provedor de serviço de nuvem pública.


Visualizando um Storage
-----------------------

Para visualizar um Storage na Plataforma uCloud é necessário o usuário clicar com o cursor do mouse sobre qualquer linha de um recurso do Storage, logo o uCloud apresenta a tela abaixo, a qual está segmentada em diversas seções:

.. image:: /figuras/ucloud_menu_storage002.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

A seguir a descrição dos campos de cada seção da tela acima:

* **Seção Geral**: Esta seção apresenta as informações básicas referente ao recurso de armazenamento (Storage) as quais são obtidas direto do ambiente do provedor de serviço de nuvem pública ao qual está vinculado.
  
  * **Nome**: Este campo apresenta o nome do recurso computacional extraído do ambiente do provedor de serviço de nuvem pública. Este campo não é passível de alteração.
  * **Display Name**: Este campo apresenta o nome do recurso computacional da forma como o usuário preferir que este seja identificado, com o objetivo de facilitar sua visualização na interface da Plataforma uCloud. **Importante ressaltar: que este nome é válido apenas para a interface da Plataforma uCloud**
  * **Tipo do Storage**: O conteúdo apresentado neste campo está relacionado, principalmente, aos ambientes de armazenamento das nuvens privadas (on-premises) e, a cada tipo de ambiente de nuvem privada que pode apresentar um tipo específico. Este campo pode apresentar o tipo do Storage do provedor de nuvem pública, caso este apresente-se configurado e a API do provedor entregue esta informação (por ex.: OBJECT).
  * **Container**: Este campo apresenta o nome do container ao qual este recurso de armazenamento (Storage) está vinculado.
  * **Tipo do Container**: Este campo apresenta uma identificação simplificada do nome do provedor de serviço de nuvem pública e/ou privada, ao qual o recurso de armazenamento (Storage) está vinculado.
  * **Compartilhamento**: Este campo apresenta a característica de compartilhamento deste recurso computacional de armazenamento (Storage) por ex.: Não Compartilhado.

* **Seção Tamanho**: Esta seção apresenta o tamanho total do volume de armazenamento deste recurso computacional e a sua taxa de ocupação no presente momento. O valor da ocupação, no presente momento, se refere à soma de todos os recursos de armazenamento presentes nas máquinas virtuais na seção abaixo.

Para os ambientes de nuvem pública a informação pode estar indisponível, por uma característica intrínseca destes ambientes. Nestas nuvens públicas, de um certo ponto de vista, estes recursos são infinitos.

Por outro lado, para os ambientes de nuvem privada, a Plataforma uCloud obtém esta informação diretamente do ambiente do hypervisor. A seguir, a apresentação de um exemplo desta seção em: Ambiente de nuvem privada.


.. image:: /figuras/ucloud_menu_storage003.png
   :alt: Virtual Datacenter - Exemp
   :scale: 60 %
   :align: center

----

* **Seção Máquinas Virtuais**: Esta seção apresenta a relação de todas as máquinas virtuais que possuem um recurso computacional de disco, os quais estão vinculados à mesma região, na qual o recurso computacional de armazenamento está associado.

.. image:: /figuras/ucloud_menu_storage004.png
   :alt: Virtual Datacenter - Exemp
   :scale: 60 %
   :align: center

----

  * **Máquina Virtual**: Esta coluna apresenta o nome da máquina virtual informado pelo usuário, no momento que esta é provisionada através da Plataforma uCloud ou por intermédio do console do provedor de serviço de nuvem pública/privada. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica e exibe a lista de nomes das máquinas virtuais, de forma alfabética na ordem crescente (a – z) ou decrescente (z – a).
  * **Zona de Disponibilidade**: Esta coluna apresenta o nome da Zona de Disponibilidade do provedor de serviço de nuvem pública/privada ao qual o recurso de disco está vinculado. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud exibe a lista de nomes das máquinas virtuais, de forma alfabética na ordem crescente (a – z) ou decrescente (z – a).
  * **Nome do Disco**: Esta coluna apresenta o nome do disco informado pelo o usuário no momento em que este é provisionado através da Plataforma uCloud ou por intermédio do console do provedor de serviço de nuvem pública/privada. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica e exibe a lista de nomes das máquinas virtuais, de forma alfabética na ordem crescente (a – z) ou decrescente (z – a).
  * **Tamanho do Disco**: Esta coluna apresenta o tamanho total do volume do disco definido pelo usuário no momento em que o disco é provisionado. Estes valores podem ser representados em Gigabytes (Gb) ou Terabytes (Tb).

* **Seção Discos Órfãos**: Esta seção apresenta todos os recursos de discos que não estão associados a uma máquina virtual. A denominação de ‘disco órfão" ocorre depois que uma máquina virtual é removida (apagada), esta conta com um o recurso de disco extra que é adicionado devido a alguma necessidade específica (como recurso adicional). Quando a máquina virtual (com “disco extra”) é removida o recurso disco se mantém vinculado ao valor da conta da organização (‘Contrato’) mas sem estar vinculado a uma máquina virtual ativa.

A Plataforma uCloud obtém esta informação de forma regular e constante, através do processo de sincronização do arquivo de Billing.

.. image:: /figuras/ucloud_menu_storage005.png
   :alt: Virtual Datacenter - Exemp
   :scale: 60 %
   :align: center

----

* **Nome do Disco**: Esta coluna apresenta o nome do disco informado pelo o usuário, no momento em que este é provisionado através da Plataforma uCloud ou por intermédio do console do provedor de serviço de nuvem pública/privada.
* **Zona de Disponibilidade**: Esta coluna apresenta o nome da Zona de Disponibilidade do provedor de serviço de nuvem pública/privada ao qual o recurso de disco está vinculado.
* **Ações**: Esta coluna pode apresentar dois ícones de ação “Anexar” e “Remover” os quais permitem ao usuário interagir com o disco órfão selecionado:

  * **Ícone de Anexar**: Basta clicar com o cursor do mouse sobre este botão para a Plataforma uCloud apresentar uma tela que permite vincular (anexar) o disco a uma máquina virtual específica.

.. image:: /figuras/ucloud_menu_storage006.png
   :alt: Virtual Datacenter - Exemp
   :scale: 60 %
   :align: center

----

    * **Máquina Virtual**: Este campo é do tipo “drop down”, quando o usuário clicar com o cursor do mouse, a Plataforma uCloud lista todas as máquinas virtuais existentes e provisionadas na mesma Zona de Disponibilidade, na qual o recurso do armazenamento (storage) está vinculado ao ambiente do provedor de serviço de nuvem pública.
    * **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de “Anexar” um disco a uma máquina virtual. A Plataforma uCloud encerra a tela e retorna à tela anterior.
    * **Botão Anexar**: Após o usuário selecionar a máquina virtual desejada, o usuário verifica que este botão alterna para o modo ativo (cor verde). Basta clicar com o cursor do mouse sobre o botão “Anexar” para que a Plataforma uCloud possa efetuar o processo de Anexar o disco órfão.

* **Ícone de Remover** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud remove (exclui) este disco, de forma imediata e definitiva. Esta ação é efetivada na região de disponibilidade na qual o armazenamento (storage) está vinculado, o tempo necessário para que a referida ação seja aplicada é totalmente dependente do tempo do ambiente destino (público e/ou privado). A Plataforma uCloud não acrescenta ou reduz qualquer tempo nas ações desejadas - *Favor consultar o menu Tarefas para acompanhar a evolução na execução da ação desejada*.

Menu Flavors
============

Um Flavor é a definição do tamanho dos recursos de computação (número de CPUs virtuais, memória e capacidade de armazenamento) que podem ser atribuídos automaticamente a instâncias da máquina virtual em uma configuração de nuvem.

Os ambientes dos provedores de nuvem privada (on-premises) não possuem o conceito de flavors, pois o usuário pode configurar o recurso computacional da forma como desejar. Esta ‘liberdade’ é característica destes ambientes e pode dificultar a movimentação destas máquinas virtuais entre nuvens, o que proporciona um ambiente de recuperação de desastres de maneira transparente.

A Plataforma uCloud permite ao usuário de nuvem privada criar flavors de máquinas virtuais para que encontrem-se compatíveis com as configurações disponíveis nos provedores de nuvem pública. Esta padronização permite a movimentação entre as diversas nuvens (públicas e privadas), de forma transparente e simplificada.

Outro grande benefício da padronização de flavors nos ambientes de nuvem privada é a sua potencial comparação de custos mensais de uma respectiva configuração de um flavor, entre os diversos ambientes de nuvens (públicas e/ou privadas).

O processo de sincronização da Plataforma uCloud com o container permite extrair todas as configurações de flavors existentes no ambiente do provedor de serviço de nuvem pública, após serem extraídas podem ser listadas na tela, conforme exemplo abaixo:

.. image:: /figuras/ucloud_menu_flavor001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

A seguir a descrição detalhada das colunas desta lista:

* **Container**: Esta coluna apresenta o nome do flavor. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no campo *Busca Rápida - abaixo do título desta coluna*, a Plataforma uCloud apresenta a listagem com todos os containers que o usuário registrado está vinculado, para restringir o resultado de Flavors específicos do container listado.
* **Nome**: Esta coluna apresenta o nome do flavor como identificado no provedor do serviço de nuvem (pública). Como forma de simplificar a visualização, ao clicar com o cursor do mouse no campo *Busca Rápida - abaixo do título desta coluna*, a Plataforma uCloud permite ao usuário digitar uma sequência de caracteres, para restringir o resultado de Flavors listados.
* **vCPUs**: Esta coluna apresenta o número da quantidade dos recursos de CPU definidos neste Flavor. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no campo *Busca Rápida - abaixo do título desta coluna*, a Plataforma uCloud permite ao usuário digitar uma sequência de números, para restringir os resultados de Flavors listados.
* **Memória**: Esta coluna apresenta o número com a quantidade dos recursos da memória definidos neste Flavor. Como forma de simplificar a visualização, ao clicar com o cursor do mouse no campo *Busca Rápida - abaixo do título desta coluna*, a Plataforma uCloud permite ao usuário digitar uma sequência de números, para restringir o resultado de Flavors listados. Este valor está representado em Gigabytes (GB).
* **Ações**: Esta coluna pode apresentar apenas um ícone de ação para que o usuário possa interagir com o Flavor selecionado:

  * **Ícone Lata de Lixo** |icone_lixo|: Basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud permite remover (excluir) a configuração do Flavor, de forma imediata e definitiva. A Plataforma uCloud apresenta a tela de *pop up* para solicitar a confirmação do usuário.

.. note:: Importante ressaltar: esta ação remove a configuração do Flavor apenas da base de dados interna da Plataforma uCloud, de forma permanente; Esta ação não efetua a remoção do Flavor do ambiente do provedor de serviço de nuvem pública.

Visualizando um Flavor
----------------------

A Plataforma uCloud apresenta a tela abaixo, quando o usuário seleciona um flavor específico.

.. image:: /figuras/ucloud_menu_flavor002.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

A seguir a descrição dos campos desta tela:

* Botão Excluir: Basta clicar com o cursor do mouse sobre este botão e a Plataforma uCloud permite remover (excluir) este Flavor da base de dados interna do uCloud, de forma imediata e definitiva. Quando o usuário clicar com o cursor do mouse sobre este ícone, a Plataforma uCloud apresenta uma tela para confirmar a ação do usuário.

* **Nome**: Este campo apresenta o nome do flavor como identificado no provedor de serviço de nuvem (pública).
* **Container**: Este campo apresenta o nome do container ao qual este flavor está vinculado.
* **vCPU**: Este campo apresenta o número com a quantidade de recursos CPU definido neste Flavor.
* **Memória**: Este campo apresenta o número da quantidade de recursos de memória definido neste Flavor. Este valor está representado em Gigabytes (GB).
* **Disco**: Este campo apresenta o valor do tamanho do recurso de disco de armazenamento definido neste Flavor. Este valor pode ser apresentado em Gigabytes (GB) ou em Terabytes (TB). Esta é a única configuração do flavor que pode ser personalizada pelo usuário.

  * **Ícone Edição** |icone_edita_on|: Basta o usuário clicar sobre este ícone e a Plataforma uCloud alterna para o modo edição, permite ao usuário corrigir o conteúdo do campo desejado e alterar a configuração do tamanho do disco de armazenamento do Flavor.
  * **Campo de Tamanho do Disco**: O usuário deve informar um número inteiro que representa o tamanho do disco de armazenamento do Flavor. Este campo não aceita valores separados com "vírgula" ou "ponto". Pode ser selecionado o limite em **Gigabytes (GB)** ou em **Terabytes (TB)**.
  * **Ícone de Confirmação** |icone_conf_verde|: Quando o usuário deseja confirmar a intenção de alterar o conteúdo do campo desejado, a Plataforma uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo é alterada permanentemente na base de dados da Plataforma uCloud.
  * **Ícone de Cancelamento** |icone_cancela_vermelho|: No caso do usuário clicar sobre o ícone de edição, por engano ou no caso de não desejar que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o botão vermelho. O botão vermelho cancela as alterações e o conteúdo do campo retorna para os valores iniciais, antes de proceder qualquer preenchimento ou alteração.

.. attention:: É importante ressaltar que qualquer alteração das configurações de um disco de armazenamento de um Flavor, poderá criar alteração nos valores mensais dos custos de armazenamento do billing deste provedor de nuvem pública. A Plataforma uCloud não pode ser responsabilizada por problemas que possam resultar desta ação.

Menu Workflows
==============

Atualmente todo profissional de infraestrutura de TI utiliza diversos *consoles* diferentes para provisionar recursos computacionais, seja dentro da empresa (data center privado) ou em em algum provedor(es) de nuvem(ns). Desta forma, se manter atualizado e preparado, em todas as "consoles" é um dos desafios atuais para qualquer profissional de TI.

Na tentativa de aumentar a produtividade e reduzir o grau de dependência destes *consoles* o mercado desenvolveu o conceito de Infraestrutura como Código (IaC - Infrastructure as a Code). Mas este conceito endereça somente o momento do provisionamento inicial (mesmo com o uso de scripts para instalação de padrões e softwares), mas podem existir demandas em que o profissional de TI terá de se conectar ao *console* do ambiente para executar alguma intervenção na infraestrutura que não é possível através do conceito de IaaC. Estar conectado e ficar alternando entre os diversos consoles de nuvem, demanda uma grande especialização e conhecimento do profissional de TI.

O mercado também criou a demanda de programar a execução de uma sequência de diversos scripts dentro de um fluxo controlado e encadeado de forma que um erro em um destes scripts pode interromper todo o fluxo para evitar o provisionamento de uma infraestrutura computacional sem a devida qualidade.

Mas, muito importante é o nível de permissão das respectivas ações deste profissional seja na nuvem pública ou na nuvem privada. Independente se o profissional executa as ações via console ou via script automatizado, as plataformas de CSB devem possuir mecanismos que de provisionar um Perfil de Permissionamento e que estes possam ser vinculados às credenciais de acesso do usuário para controlar, adequar ou restringir as ações deste usuário.

Os Fluxos de Trabalho (workflows) em ambiente de recursos computacionais, de nuvem pública, automatizam tarefas repetitivas de maneira confiável e podem converter processos manuais em fluxos de trabalho digitais provisionados através da interface da Plataforma uCloud. Ao usar os Fluxos de Trabalho (workflows) em um ambiente de nuvem pública, as organizações podem reduzir as etapas manuais e melhorar a eficiência dos seus fluxos de trabalho, rapidamente, a um custo consideravelmente menor.

A funcionalidade de Fluxos de Trabalho pode desempenhar diversas ações de operação na infraestrutura de recursos computacionais de nuvem pública e/ou privada.

As funcionalidades disponíveis são as seguintes:

#. Desligamento de Máquina Virtual (Shutdown)
#. Ativação de Máquina Virtual (Start/Boot)
#. Cópia Instantânea de um volume (Disk Snapshot)
#. Executar um, ou mais, scripts/playbooks com sintaxe:

  a. Ansible
  b. Terraform
  c. Puppet

Direct Execution
----------------

Nete menu a Plataforma uCloud permite provisionar, personalizar e inspecionar o comprtamento de um Fluxo de Trabalho e aplicar estes em um recurso computacional (por ex.: máquina virtual) do ambiente do provedor de serviço de nuvem pública e/ou nuvem privada.

Quando o usuário seleciona a opção Direct Execution do menu, a seguinte tela é apresentada:

.. figure:: /figuras/ucloud_workflow_dir_exec001.png
   :alt: Menu Workflows
   :scale: 60 %
   :align: center

----

A descrição detalhada dos campos desta tabela segue abaixo:

Através desta tela é possível provisionar um novo fluxo de trabalho ou inspecionar o resultado das ações do script(s)/playbook(s) que está(ão) vinculado(s)

* **Nome**: Nesta tela o usuário pode iniciar o provisionamento de um novo fluxo de trabalho para execução direta. O limite mínimo de caracteres para informar neste campo é três (03) e o máximo é de sessenta e quatro (64) caracteres. Sugerimos utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido). Este campo deve ser preenchido com o nome desejado pelo usuário para identificar o seu Fluxo de Trabalho para execução direta (*Direct Execution*).
* **Descrição**: Neste campo o usuário pode preencher com uma descrição das funcionalidades do fluxo de trabalho.
* **Manual**: Este campo é do tipo "radio button" que configura definitivamente que este fluxo de trabalho somente pode ser executado através de uma intervenção direta do usuário, que deve selcionar este fluxo de trabalho e decidir por sua execução.
* **Automático**: Este campo é do tipo "radio button" que configura definitivamente que este fluxo de trabalho será executado automaticamente sem a necessidade de intervenção direta do usuário. Quando selecionado esta opção, a Plataforma uCloud atualiza a interface e apresenta um novo campo para o usuário selecionar a opção de automação do fluxo de trabalho.

  * **Selecionar Intervalo**: Este campo é do tipo "dropdown" e permite que o usuário programe uma data e/ou hora para a execução deste fluxo de trabalho. As opções são as seguintes:
    * **Uma Vez**: Esta opção configura que este fluxo de trabalho será executado somente uma única vez sem que ocorram repetições automáticas de sua execução. Quando selecionado esta opção a Plataforma uCloud apresenta dois novos campos:

      * **Data**: Neste campo o usuário deve informar o dia, o mês e o ano que deseja programar a execução deste fluxo de trabalho.
      * **Horas**: Neste campo o usuário deve informar a hora e minuto que deseja programar a execução deste fluxo de trabalho para o dia selecionado n campo acima.

    * **Uma vez no dia**: Esta opção configura que este fluxo de trabalho será executado diária e contínuamente todos os dias do ano, repetidamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.
      * **Horas**: Neste campo o usuário deve informar a hora e minuto que deseja programar a execução deste fluxo de trabalho.

    * **Uma vez na semana**: Esta opção configura que este fluxo de trabalho será executado semanalmente e contínuamente todos os semanas do ano, repetidamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.

      * **Dia da Semana**: Este campo é do tipo "dropdown" e o usuário deve selecionar o dia da semana que deseja programar a execução deste fluxo de trabalho. Importantemencionar que esta opção significa que este fluxo de trabalho será executado semanalmente e continuamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.
      * **Horas**: Neste campo o usuário deve informar a hora e minuto que deseja programar a execução deste fluxo de trabalho para o dia da semana selecionado n campo acima.

    * **Uma vez no mês**: Esta opção configura que este fluxo de trabalho será executado diária e contínuamente todos os dias do ano, repetidamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.
  
      * **Dia do Mês**: Neste campo o usuário deve informar o número inteiro que representa o dia do mês que deseja que este fluxo de trabalho seja executado. Importantemencionar que esta opção significa que este fluxo de trabalho será executado mensal e continuamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.
      * **Horas**: Neste campo o usuário deve informar a hora e minuto que deseja programar a execução deste fluxo de trabalho pra o dia do mês selecionado no campo anterior.

* **Repetir mesmo com erro**: Este campo é do tipo "radio-button" e configura que o fluxo d trabalho seja executado por completo, mesmo que existe algum erro em seu código, ou que a plataforma do provedor de serviço de nuvem Pública e/ou Privara, retorne algum erro referente à execução do script(s)/playboo(s).
* **Parar em caso de erro**: Este campo é do tipo "radio-button" e configura que o fluxo d trabalho seja encerrado quando alguma das tasks associadas encontrem algum erro durante sua execução em seu código do script(s)/playbook(s), ou encontrem algum erro na execução dentro da plataforma do provedor de serviço de nuvem Pública e/ou Privada.

* **Botão Criar Workflow**: Este botão permite provisionar (criar) um Fluxo de Trabalho no ambiente da Plataforma uCloud. A descrição detalhada está no item Criando um Workflow a seguir.

* **Seção Workflows Existentes**: Nesta seção a PlataformauCloud apresenta uma relação de todos os fluxos de trabalh que foram provisionados pelo usuário.

  * **Botão “Refresh”**: A Plataforma uCloud se comunica com suas bases de dados internas constantemente, mas sendo esta interface HTML, podem existir atrasos (delays) de comunicação entre o computador do usuário e as instâncias de recursos computacionais que estão suportando e executando a aplicação do uCloud. Para atualizar apenas o conteúdo das seções da tela (ou as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, o qual executa apenas a atualização das informações contidas em nossas bases de dados.
  * **Nome**: Esta coluna apresenta o nome do Fluxo de Trabalho informado no momento do seu provisionamento através da interface da Plataforma uCloud. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes das máquinas virtuais, em forma alfabética crescente (a – z) ou decrescente (z – a).
  * **Intervalo**: Esta coluna apresenta o período do intervalo de tempo do Fluxo de Trabalho informado no momento do seu provisionamento através da interface da Plataforma uCloud. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de intervalos, de forma alfabética crescente (a – z) ou decrescente (z – a).
  * **Status**: Esta coluna apresenta o status atual do Fluxo de Trabalho. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma uCloud classifica a lista de nomes de intervalos de forma alfabética crescente (a – z) ou decrescente (z – a). A Plataforma uCloud pode representar o status de duas formas diferentes:
  
    * **Ativo**: Este status indica que este Fluxo de Trabalho pode ser recorrente, portanto fica ativo indefinidamente, seu status está no modo "Habilitado". Este status pode representar, também, que este Fluxo de Trabalho foi agendado para uma data e horário a frente do horário atual, portanto se manterá ativo até o momento da sua execução.

    * **Concluído**: Este status indica que o Fluxo de Trabalho já executou a sua atividade em uma data anterior e se encontra parado. Este status pode indicar que um usuário alternou a disponibilidade do Fluxo de Trabalho para ‘Desabilitado’.

Editando Workflow
-----------------

Para editar um Fluxo de Trabalho, basta o usuário clicar com o cursor do mouse sobre qualquer uma das linhas da lista, em seguida, a Plataforma uCloud exibe a tela:

.. figure:: /figuras/ucloud_workflow_dir_exec003.png
   :alt: Menu Workflows
   :scale: 60 %
   :align: center

----

* **Seção Nome**: Nesta seção são apresentadas as informações básicas associadas ao Fluxo de Trabalho e a sua configuração de execução:

  * **Nome**: Campo preenchido pelo usuário para identificar o Fluxo de Trabalho, no momento do seu provisionamento na Plataforma uCloud.
  * **Ativo/Parado**: (|icone_wf_ativo|/|icone_wf_parado|): O ícone indica se este Fluxo de Trabalho está configurado como Desabilitado (vermelho = "STOP") ou Habilitado (verde - "ATIVO").
  * **Última execução**: O campo apresenta informação de data e hora que este Fluxo de Trabalho foi executado alguma vez até a presente data. Fluxos de Trabalho configurados com reperições contínuas (sem data de limite), este campo apresenta o texto "nunca".
  * **Configuração**: Campo que apresenta as características configuradas para este Fluxo de Trabalho que podem ser:
    * **Repetir mesmo com erro**: Indica que este Fluxo de Trabalho será executado mesmo que o ambiente computacional possa apresentar algum erro durante sua execução.
    * **Parar em caso de erro**: Indica que este Fluxo de Trabalho será interrompido se o ambiente computacional apresentar algum erro durante sua execução.

  * **Número de execuções**: Este campo representa a quantidade de execuções de cada uma das Tarefas Associadas ao Fluxo de Trabalho. Caso a programação da configuração de agendamento futuro (data e/ou hora) não tenha sido alcançada este campo pode ser representado com zero ("0").
  * **Intervalo**: Este campo apresenta a configuração do tipo de intervalo selecionado:
    * Uma vez.
    * Uma vez ao Dia.
    * Uma vez na Semana.
    * Uma vez ao Mês.

  * **Data**: Este campo apresenta a data no calendário, que foi selecionada para que o Fluxo de Trabalho seja executado.
  * **Hora**: Este campo apresenta o horário selecionado para que o Fluxo de Trabalho seja executado. O campo utiliza a notação de 24 horas e sua apresentação está com a máscara HH-mm-seg (hora - minuto - segundo).
  * **Editar**: Basta o usuário clicar com o cursor do mouse sobre esta palavra e a Plataforma uCloud irá permitir que o usuário reconfigurar completamente o agendamento de execução dete fluxo de trabalho.
  * **Excluir**: Basta clicar com o cursor do mouse sobre esta palavra que a Plataforma uCloud remove toda a configuração de agendamento deste fluxo de trabalho de forma imediata e definitiva. A Plataforma uCloud apresenta uma tela solicitando a confirmação da ação.

* **Seção Task Associada**: Esta seção apresenta todas as Tarefas Associadas para serem executadas no Fluxo de Trabalho, seguindo a ordem das suas Prioridades. Para outras informações, consultar o processo no item Criando Tarefas Associadas.

  * **Icone Lápis** |icone_lapis_workflow|: Este ícone fica ativo *SOMENTE* para os fluxos de trabalho que foram provisionados para que o usuário entre algum tipo de informação para a correta execução deste fluxo de trabalho. Basta o usuário pode clicar com o cursor do mouse sobre o ícone e a Plataforma uCloud apresenta uma janela pop up para que o usuário entre com a informação desejada, conforme o exemplo abaixo:

.. figure:: /figuras/ucloud_workflows009b.png
   :alt: Logo uCLoud
   :scale: 50 %
   :align: center

----

  * **Prioridade**: Esta coluna representa o número referente a ordem de prioridade, a qual esta Tarefa Associada será executada. Sendo zero ("0") a mais alta prioridade, o que significa que esta tarefa será a primeira a ser executada na data e hora programada.
  * **Nome**: Esta coluna apresenta o nome da tarefa associada, informado pelo usuário no momento da sua configuração.
  * **Tipo**: Esta coluna apresenta o tipo da tarefa, selecionada pelo usuário no momento da sua criação.
  * **Status**: Esta coluna apresenta o presente estado desta tarefa para a data e hora correntes; que pode ser Erro ("ERROR"), Aguardando ("Waiting") ou Executada ("CONCLUDED"). A Plataforma uCloud permite visualizar o registro de mensagens de erro (log) ou registro das mensagens de finalização, quando o status da task associada se apresenta como "ERROR" ou "CONCLUDED". A Plataforma uCloud ativa o icone |icone_log_wf|. Basta o usuário clicar com o cursor do mouse sobre este ícone que a Plataforma uCloud apresenta uma janela pop-up com a informação do **log** de registro da(s) atividade(s) do script(s)/Playbook(s) para acompanhamento do usuário. Veja o exemplo de log de sucesso abaixo:

.. figure:: /figuras/ucloud_workflows012.png
   :alt: LOG Workflow - Sucesso
   :scale: 50 %
   :align: center

----

  * **Ações**: Esta coluna apresenta apenas o ícone de Lata de Lixo |icone_lixo|, basta clicar com o cursor do mouse sobre este botão, para que a Plataforma uCloud remova esta Tarefa Associada, de forma imediata e definitiva.

Criando Workflow
----------------

O processo de criação de um fluxo de trabalho deve ser efetuado em duas (02) etapas e todos os Fluxos de Trabalho devem seguir esta etapas obrigatóriamente:

A. Definição do Fluxo de Trabalho (nome e intervalo de execução)
B. Inclusão de uma ou mais Tasks Associadas

Abaixo descrevemos cada uma das etapas indivudualmente.

Definição do Fluxo de Trabalho
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A primeira de provisionamento de um Fluxo de Trabalho deve ser efetuada no momento que o usuário acessa o menu Workflows / Direct Execution e preenche os campos (em destaque) da tela anaixo:

.. figure:: /figuras/ucloud_workflow_dir_exec001b.png
   :alt: LOG Workflow - Sucesso
   :scale: 50 %
   :align: center

----

* **Nome**: Nesta tela o usuário pode iniciar o provisionamento de um novo fluxo de trabalho para execução direta. O limite mínimo de caracteres para informar neste campo é três (03) e o máximo é de sessenta e quatro (64) caracteres. Sugerimos utilizar somente os caracteres ASCII padrão, não usar os caracteres acentuados (ASCII Extendido). Este campo deve ser preenchido com o nome desejado pelo usuário para identificar o seu Fluxo de Trabalho para execução direta (*Direct Execution*).
* **Descrição**: Neste campo o usuário pode preencher com uma descrição das funcionalidades do fluxo de trabalho.
* **Manual**: Este campo é do tipo "radio button" que configura definitivamente que este fluxo de trabalho somente pode ser executado através de uma intervenção direta do usuário, que deve selcionar este fluxo de trabalho e decidir por sua execução.
* **Automático**: Este campo é do tipo "radio button" que configura definitivamente que este fluxo de trabalho será executado automaticamente sem a necessidade de intervenção direta do usuário. Quando selecionado esta opção, a Plataforma uCloud atualiza a interface e apresenta um novo campo para o usuário selecionar a opção de automação do fluxo de trabalho.

  * **Selecionar Intervalo**: Este campo é do tipo "dropdown" e permite que o usuário programe uma data e/ou hora para a execução deste fluxo de trabalho. As opções são as seguintes:
    * **Uma Vez**: Esta opção configura que este fluxo de trabalho será executado somente uma única vez sem que ocorram repetições automáticas de sua execução. Quando selecionado esta opção a Plataforma uCloud apresenta dois novos campos:

      * **Data**: Neste campo o usuário deve informar o dia, o mês e o ano que deseja programar a execução deste fluxo de trabalho.
      * **Horas**: Neste campo o usuário deve informar a hora e minuto que deseja programar a execução deste fluxo de trabalho para o dia selecionado n campo acima.

    * **Uma vez no dia**: Esta opção configura que este fluxo de trabalho será executado diária e contínuamente todos os dias do ano, repetidamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.
      * **Horas**: Neste campo o usuário deve informar a hora e minuto que deseja programar a execução deste fluxo de trabalho.

    * **Uma vez na semana**: Esta opção configura que este fluxo de trabalho será executado semanalmente e contínuamente todos os semanas do ano, repetidamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.

      * **Dia da Semana**: Este campo é do tipo "dropdown" e o usuário deve selecionar o dia da semana que deseja programar a execução deste fluxo de trabalho. Importantemencionar que esta opção significa que este fluxo de trabalho será executado semanalmente e continuamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.
      * **Horas**: Neste campo o usuário deve informar a hora e minuto que deseja programar a execução deste fluxo de trabalho para o dia da semana selecionado n campo acima.

    * **Uma vez no mês**: Esta opção configura que este fluxo de trabalho será executado diária e contínuamente todos os dias do ano, repetidamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.
  
      * **Dia do Mês**: Neste campo o usuário deve informar o número inteiro que representa o dia do mês que deseja que este fluxo de trabalho seja executado. Importantemencionar que esta opção significa que este fluxo de trabalho será executado mensal e continuamente, até que o usuáario exclua ou interrompa a execução deste fluxo de trabalho.
      * **Horas**: Neste campo o usuário deve informar a hora e minuto que deseja programar a execução deste fluxo de trabalho pra o dia do mês selecionado no campo anterior.

* **Repetir mesmo com erro**: Este campo é do tipo "radio-button" e configura que o fluxo d trabalho seja executado por completo, mesmo que existe algum erro em seu código, ou que a plataforma do provedor de serviço de nuvem Pública e/ou Privara, retorne algum erro referente à execução do script(s)/playboo(s).
* **Parar em caso de erro**: Este campo é do tipo "radio-button" e configura que o fluxo d trabalho seja encerrado quando alguma das tasks associadas encontrem algum erro durante sua execução em seu código do script(s)/playbook(s), ou encontrem algum erro na execução dentro da plataforma do provedor de serviço de nuvem Pública e/ou Privada.

* **Botão Criar Workflow**: Este botão permite provisionar (criar) um Fluxo de Trabalho no ambiente da Plataforma uCloud. A descrição detalhada está no item Criando um Workflow a seguir.

Nesta ponto a Plataforma uCloud irá apresentar uma mensagem na tela, informando ao usuário que o Fluxo de Trabalh foi criado e adionado à lista da seção **Workflows Existentes**.

.. figure:: /figuras/ucloud_workflows015.png
   :alt: LOG Workflow - Sucesso
   :scale: 50 %
   :align: center

----

A Plataforma uCloud apresenta a mensagem acima, mas existe a possibilidade que esta mensagem (temporária) possa não ter sido notadapelo usuário. Uma outra forma de validar se a Plataforma uCloud confirmou o provisionamento do Fluxo de Tarefas, o usuário pode acessar o menu **Tarefas** onde é possível confirmar o provisionamento do Fluxo de Trabalho nas bases de dados internas da Plataforma uCloud.

No canto superior direito da tela do navegador de internet (browser) o usuário pode clicar com o cursor do mouse sobre o ícone do sino |icone_sino| que a Plataforma uCloud irá apresentar a lista de Tarefas amis recentes que foram efetuadas pelo usuário com a sessão ativa, para confirmar o correto provisionamento do Fluxo de Trabalho, conforme a tela abaixo:

.. figure:: /figuras/ucloud_workflows016.png
   :alt: LOG Workflow - Sucesso
   :scale: 50 %
   :align: center

----

Caso o nome do fluxo de trabalho não seja apresentado imediatamente, basta o usuário clicar com o botão Refresh |icone_refresh| para que a Plataform uCloud atualizar a relação na seção Workflows Existentes, e o Fluxo de Trabalho recém provisionado aparecerá sempre no final da lista (veriicar o *último da lista*).

Neste ponto o usuário pode seguir para a próxima etapa da criação do Fluxo de Trabalho.

Inclusão de Task Associadas
~~~~~~~~~~~~~~~~~~~~~~~~~~~

Neste ponto o usuário clica com o cursor do mouse sobre nome do Fluxo de Trabalho recém provisionado e a Platafrmo uCloud apresenta a tela para adicionar tasks associadas:

.. figure:: /figuras/ucloud_workflows018.png
   :alt: LOG Workflow - Sucesso
   :scale: 50 %
   :align: center

----

* **Seção Nome**: Nesta seção são apresentadas as informações básicas associadas ao Fluxo de Trabalho e a sua configuração de execução:

* **Seção Task Associada**: Esta seção apresenta uma relação de todas as Tarefas Associadas para serem executadas no Fluxo de Trabalho, seguindo a ordem das suas Prioridades.

O processo de inclusão de Tasks Associadas pode desempenhar diversas funções, e iremos descrevere suas opções e cada um de seus processos no item Criando Tarefas Associadas.

Criando Tarefas Associadas
--------------------------

Os Fluxos de Trabalho (workflows) em ambiente de recursos computacionais, de nuvem pública, automatizam tarefas repetitivas de maneira confiável e podem converter processos manuais em fluxos de trabalho digitais provisionados através da interface da Plataforma uCloud. Ao usar os Fluxos de Trabalho (workflows) em um ambiente de nuvem pública, as organizações podem reduzir as etapas manuais e melhorar a eficiência dos seus fluxos de trabalho, rapidamente, a um custo consideravelmente menor.

A funcionalidade de Fluxos de Trabalho pode desempenhar diversas ações de operação na infraestrutura de recursos computacionais de nuvem pública e/ou privada.

As funcionalidades disponíveis são as seguintes:

#. Desligamento de Máquina Virtual (Shutdown)
#. Ativação de Máquina Virtual (Start/Boot)
#. Cópia Instantânea de um volume (Disk Snapshot)
#. Executar um, ou mais, scripts/playbooks com sintaxe:

  a. Ansible
  b. Terraform
  c. Puppet

Tarefa de Desligamento/Ativação Programado de Máquina Virtual
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O exemplo de desligamento programado, pode ser muito útil para se utilizar da funcionalidade de workflows para desligar (*shutdown*) de um servidor em um horário programado (por ex.: sexta-feira às 23h59) para que as cobranças decorrentes do uso deste servidor sejam interrompidas durante o fim de emana e a empresa possa receber o benefício de economia de custos referentes ao consumo desta infraestrutura.

.. attention:: As aplicações que estão sendo executadas neste servidor, não estarão disponíveis para os usuários durante o horário que esta infraestrutura estiver inoperante.

Esta ação pode ser programada para ser executada diariamente em um horário pré-determinado (ex.: executar desligamento de segunda à sexta-feira às 20 horas). Com a programação semanal (uma vez por semana) é possível criar o agendamente para o desligamento durante os finais de semana; deixando a infraestrutura do servidor e suas aplicações disponível para seus usuários fora do horário comercial (período noturno das 20 às 06 horas) e durante o fim de semana (sábado e domingo).

A Tarefa de desligamento, pode ser seguida de uma programação de ativação (*boot*) do mesmo recurso computacinal de forma diária (ex: executar o início de segunda à sexta-feira às 06 horas). Para os casos que exista somente a programação semanal para o fim de semana (sabado e domingo) o usuário pode criar uma programação semanal para re-iniciar a infraestrutura computacional toda segunda-feira às 06 horas.

Esta implementação pode reduzir os custos recorrentes de recursos de servidores que foram contratados como cobrança por utilização.

Esta funcionalidade de desligamento e ativação programada, pode não ser muito efetiva para redução de custos operacionais para determinados tipos de recursos como instâncias reservadas (Reserved Instances) e SPOT Instances.

.. note:: Cada provedor de serviço de nuvem pública possui um custo pré-fixado para a contratação destas modalidades de infraestrutura de máquinas virtuais e o desligamento programado poderá não acarretar nenhuma redução no custo mensal de utilização.

O usuário deve acessar o menu Workflow / Direct Execution, e após nomear seu fluxo, basta clicar com o cursor o mouse sobre o nome do fluxo de trabalho para adicionar uma **Task Associada** conforma a tela abaixo:

.. figure:: /figuras/ucloud_workflows018.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

Neste ponto o usuário deve clicar com o cursor do mouse sobre o botão **+Criar Tasks Associadas** e a Plataforma uCloud apresenta a tela para 

.. figure:: /figuras/ucloud_workflows019b.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

* **Nome**: Este campo é obrigatório, nele o usuário deve informar o nome da Tarefa Associada que deseja provisionar. O nome da Tarefa Associada deve ter no mínimo quatro (04) caracteres e o limite máximo de setenta (70) caracteres. Como sugestão, utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).
* **Tipo**: Este campo é obrigatório, trata-se de um campo do tipo “dropdown”, quando o usuário clicar sobre este, será apresentada a lista das opções de tipos de Tarefas Associadas disponíveis na Plataforma uCloud, ver as opções abaixo:

  * **Iniciar Máquina Virtual**: Esta opção permite ao usuário criar uma tarefa de iniciar (boot/start) uma máquina virtual, seguindo uma determinada prioridade no Fluxo de Trabalho (workflow). Quando selecionado este tipo de ação, a Plataforma uCloud apresenta os campos específicos nesta tela e o usuário deve consultar a seguir o item
  * **Parar Máquina Virtual**: Esta opção permite ao usuário criar uma tarefa de parar (shutdown/stop) uma máquina virtual seguindo uma determinada prioridade no Fluxo de Trabalho (workflow). Quando selecionado este tipo de ação, a Plataforma uCloud apresenta campos específicos nesta tela e o usuário deve consultar abaixo o item A.Tarefa de Iniciar e Parar Máquina Virtual.

* **Prioridade**: Este campo é obrigatório, nele o usuário deve informar um número inteiro que indica a ordem de prioridade que esta Tarefa Associada será executada. Sendo zero ("1") a mais alta prioridade, o que significa que a tarefa com o menor número informado será a primeira a ser executada na data e hora programada. Este campo permite ao usuário encadear várias tarefas, em outras palavras, executar as Tarefas Associadas em uma sequência específica, de acordo com a prioridade. Importante ressaltar que na eventual existência de duas tarefas diferentes e ambas com a mesma prioridade estas serão executadas em paralelo, a Plataforma uCloud executa Tarefas Associadas de forma sequencial (uma a uma).

* **Virtual Datacenter**: Este campo é obrigatório, ele é um campo do tipo “dropdown”, quando o usuário clicar sobre este, será apresentada a lista de todos os Virtual Datacenters aos quais este usuário está vinculado, ele tem permissão para utilizar os recursos computacionais deste VDC. Importante ressaltar que a seleção de um VDC, restringe (filtra) a relação de máquinas que estão vinculadas (e/ou são exclusivas) deste Virtual Datacenter.

* **Máquina Virtual**: Este campo é obrigatório, ele é um campo do tipo “dropdown”, quando o usuário clicar sobre este, será apresentada a lista de todas as máquinas virtuais as quais este usuário tem permissão de acesso e as máquinas virtuais estão vinculadas ao VDC informado acima. Importante ressaltar que a seleção de um VDC, restringe (filtra) a relação de máquinas que estão vinculadas (e/ou são exclusivas) deste Virtual Datacenter.

* **Botão Criar**: Após preencher todos os campos obrigatórios para provisionar uma nova Tarefa Associada de Iniciar ou Parar, uma máquina virtual, o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma uCloud provisione a nova Tarefa Associada em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório foi deixado sem preenchimento ou a sequência de caracteres do nome pode ser inferior a quatro (04) caracteres. A Plataforma uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que a nova Tarefa Associada foi criada.

Após o clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud atualiza a Seção Task Associadas com a referida tarefa que fará parte do Fluxo de Trabalho conforme o exemplo abaixo (a tela abaix é meramente ilustrativa para efeito de demonstração):

.. figure:: /figuras/ucloud_workflows019c.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

Para os casos em que o usuário tenha inserido algum erro no campo Nome ou no campo Tipo, o usuário deve remover (apagar) a linha com erro, para isto deve clicar com o cursor do mouse sobre o icone |icone_lixo|. Após a remoção da linha o usuário deve efetuar o provisionamento correto novamente.

Se o usuário clicar com o cursor do mouse sobre o botão "**+Executar Agora**" a Plataforma uCloud irá iniciar a execução da sequência de Tasks Associadas dentro deste Fluxo de Trabalho (somente uma ou todas as Tasks Associadas seguindo a sequência definida no campo Prioridade).

Após a execução a Plataforma uCloud irá atualizar a coluna **Status** e apresentar na(s) linha(s) de cada Task Associada o botão |icone_log_wf|, que apresenta o conteúdo da informação do *log* de registro das ações referentes a execução desta Task Associada (erro ou sucesso).


Tarefa de Criar Imagem de Disco (Snapshot)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta atividade pode ser entendida (ou confundida) com a atividade de cópia de segurança (*backup*), mas é importante esclarecer que esta funcionalidade apenas executa uma função nativa dos consoles dos provedores de serviço de nuvem pública e/ou privada, que é a cópia instantânea de um volume de disco em um horário determinado pelo usuário.

Em sistemas de computador, uma cópia instantânea de volume ou captura instantânea de volume (do Inglês: snapshot, tradução literal: foto instantânea) é o estado de um sistema em um determinado ponto no tempo. O termo foi cunhado como uma analogia ao usado em fotografia. Pode se referir a uma cópia real do estado de um sistema ou a um recurso fornecido por determinados sistemas.

Importante mencionar que uma das diferenças entre um storage snapshot e um backup é que o snapshot é armazenado no mesmo local dos dados originais. Portanto, depende completamente da confiabilidade da origem. Isso significa que, no caso de um desastre ou danos aos dados de origem, o snapshot está totalmente comprometido ou ficaria inacessível.

Um disk snapshot não efetua o processo de validação da integridade lógica do processo de cópia do(s) arquivo(s) individualmente, simplesmente executa a ação de cópia instantânea de todo o disco associado a infraestrutura que compreende o servidor.

O usuário pode provisionar a ação de criação de um *disk snapshot* em dias e/ou horários programados e deixar que a Plataforma uCloud envie esta solicitação (via API-REST) para o console do provedor de serviço de nuvem para que o provedor inicie este disk snapshot.

O usuário deve acessar o menu Workflow / Direct Execution, e após nomear seu fluxo, basta clicar com o cursor o mouse sobre o nome do fluxo de trabalho para adicionar uma **Task Associada** conforma a tela abaixo:

.. figure:: /figuras/ucloud_workflows018.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

Neste ponto o usuário deve clicar com o cursor do mouse sobre o botão **+Criar Tasks Associadas** e a Plataforma uCloud apresenta a tela para 

.. figure:: /figuras/ucloud_workflows019d.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

* **Nome**: Este campo é obrigatório, nele o usuário deve informar o nome da Tarefa Associada que deseja provisionar. O nome da Tarefa Associada deve ter no mínimo quatro (04) caracteres e o limite máximo de setenta (70) caracteres. Como sugestão, utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).

* **Tipo**: Este campo é obrigatório, trata-se de um campo do tipo “dropdown”, quando o usuário clicar sobre este, será apresentada a lista das opções de tipos de Tarefas Associadas disponíveis na Plataforma uCloud, ver as opções abaixo:

  * **Criar Snapshot**: Esta opção permite ao usuário criar uma tarefa para que seja iniciada a operação de armazenamento da imagem de disco (snapshot) da máquina virtual seguindo uma determinada prioridade no Fluxo de Trabalho (workflow). Quando selecionado este tipo de ação, a Plataforma uCloud apresenta campos específicos nesta tela e o usuário deve consultar abaixo o item B.Tarefa Criar Imagem de Disco (Snapshot).

* **Prioridade**: Este campo é obrigatório, nele o usuário deve informar um número inteiro que indica a ordem de prioridade que esta Tarefa Associada será executada. Sendo zero ("1") a mais alta prioridade, o que significa que a tarefa com o menor número informado será a primeira a ser executada na data e hora programada. Este campo permite ao usuário encadear várias tarefas, em outras palavras, executar as Tarefas Associadas em uma sequência específica, de acordo com a prioridade. Importante ressaltar que na eventual existência de duas tarefas diferentes e ambas com a mesma prioridade estas serão executadas em paralelo, a Plataforma uCloud executa Tarefas Associadas de forma sequencial (uma a uma).

* **Virtual Datacenter**: Este campo é obrigatório, ele é um campo do tipo “dropdown”, quando o usuário clicar sobre este, será apresentada a lista de todos os Virtual Datacenters aos quais este usuário está vinculado, ele tem permissão para utilizar os recursos computacionais deste VDC. Importante ressaltar que a seleção de um VDC, restringe (filtra) a relação de máquinas que estão vinculadas (e/ou são exclusivas) deste Virtual Datacenter.

* **Máquina Virtual**: Este campo é obrigatório, ele é um campo do tipo “dropdown”, quando o usuário clicar sobre este, será apresentada a lista de todas as máquinas virtuais as quais este usuário tem permissão de acesso e as máquinas virtuais estão vinculadas ao VDC informado acima. Importante ressaltar que a seleção de um VDC, restringe (filtra) a relação de máquinas que estão vinculadas (e/ou são exclusivas) deste Virtual Datacenter.

* **Nome Snapshot**: Este campo é obrigatório nele o usuário deve informar o nome da Imagem de Disco (snapshot) que deseja provisionar. O nome da Tarefa Associada deve ter no mínimo quatro (04) caracteres e no limite máximo de setenta (70) caracteres. Sugerimos utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).

* **Disco**: Este campo é obrigatório, ele é um campo do tipo “dropdown”, quando o usuário clicar sobre ele, será apresentada a lista de todos os recursos de discos de armazenamento vinculados à máquina virtual selecionada acima.

* **Botão Criar**: Após preencher todos os campos obrigatórios para provisionar uma nova Tarefa Associada de Iniciar ou Parar, uma máquina virtual, o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma uCloud provisione a nova Tarefa Associada em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório foi deixado sem preenchimento ou a sequência de caracteres do nome pode ser inferior a quatro (04) caracteres. A Plataforma uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que a nova Tarefa Associada foi criada.

Após o clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud atualiza a Seção Task Associadas com a referida tarefa que fará parte do Fluxo de Trabalho conforme o exemplo abaixo (a tela abaix é meramente ilustrativa para efeito de demonstração):

.. figure:: /figuras/ucloud_workflows019e.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

Para os casos em que o usuário tenha inserido algum erro no campo Nome ou no campo Tipo, o usuário deve remover (apagar) a linha com erro, para isto deve clicar com o cursor do mouse sobre o icone |icone_lixo|. Após a remoção da linha o usuário deve efetuar o provisionamento correto novamente.

Se o usuário clicar com o cursor do mouse sobre o botão "**+Executar Agora**" a Plataforma uCloud irá iniciar a execução da sequência de Tasks Associadas dentro deste Fluxo de Trabalho (somente uma ou todas as Tasks Associadas seguindo a sequência definida no campo Prioridade).

Após a execução a Plataforma uCloud irá atualizar a coluna **Status** e apresentar na(s) linha(s) de cada Task Associada o botão |icone_log_wf|, que apresenta o conteúdo da informação do *log* de registro das ações referentes a execução desta Task Associada (erro ou sucesso).

Tarefa de Script
~~~~~~~~~~~~~~~~

Por padrão, a Plataforma uCloud utiliza a integração nativa com a *Plataforma Github*, e o proprietário deste repositório autoriza usuários a se conectarem neste repositório através de um código de identificação (Token) que deve ser gerado unicamente através de uma sessão no Github, para cada usuário ou usuários. Este token deve possuir a permissão de se conectar neste repositório para ter acesso aos arquivos de scripts/playbooks armazenados e versionados.

A sequência de caracteres que representa o token que permite que as credenciais de login da Plataforma uCloud possa ter acesso ao repositório Github, deve ser informado no cadastro de usuários da Plataforma uCloud, sem esta configuração, o usuário não poderá acessar o repositório de scripts/playbooks para criar o fluxo de trabalho (workflow).

.. important:: A Plataforma uCloud não efetua nenhuma validação prévia se a cadeia de caracteres referente ao token de acesso ao Github é válida ou não. A Plataforma uCloud não irá apresentar qualquer mensagem informativa referente à inclusão deste token à credencial de um usuário.

Atualmente a Plataforma uCloud suporta as seguintes ferramentas de IaC:

* Ansible
* Terraform
* Puppet*

Importante mencionar que a Plataforma uCloud não é, por ela mesma, um ambiente de armazenamento e controle de versionamento dos arquivos de playbooks. No presente momento a Plataforma uCloud permite a integração à uma ferramenta de controle de repositório de arquivos de scripts/playbooks, esta função é reservada a uma ferramenta externa.

.. note:: A Plataforma uCloud, não efetua qualquer validação prévia da coerência ou consistência da estrutura e sintaxe escrita no arquivo de script/playbook; desta forma qualquer erro pré-existente na sintaxe do texto do script, será executado de forma literal, podendo gerar (ou não) um erro que pode ser visualizado através da interface do uCloud.

.. warning:: Puppet = *Atenção a Plataforma uCloud permite criar um workflow que irá ativar um script/playbooks na sintaxe Puppet, mas para que um profissional possa utilizar script/playbook Puppet será necessário um ambiente adicional (na forma de uma infraestrutura de servidor). Este servidor que será encarregado da EXECUÇÃO dos referidos script/playbooks. A Plataforma uCloud não desempenha a função de suporte para a execução de scripts/playbooks Puppet*.

O usuário deve acessar o menu Workflow / Direct Execution, e após nomear seu fluxo, basta clicar com o cursor o mouse sobre o nome do fluxo de trabalho para adicionar uma **Task Associada** conforma a tela abaixo:

.. figure:: /figuras/ucloud_workflows018.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

Neste ponto o usuário deve clicar com o cursor do mouse sobre o botão **+Criar Tasks Associadas** e a Plataforma uCloud apresenta a tela para configurar as Tasks Associadas:

.. figure:: /figuras/ucloud_workflows019f.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

* **Nome**: Este campo é obrigatório, nele o usuário deve informar o nome da Tarefa Associada que deseja provisionar. O nome da Tarefa Associada deve ter no mínimo quatro (04) caracteres e o limite máximo de setenta (70) caracteres. Como sugestão, utilizar somente os caracteres ASCII padrão, não usar espaços em branco ou caracteres acentuados (ASCII Extendido).

* **Tipo**: Este campo é obrigatório, trata-se de um campo do tipo “dropdown”, quando o usuário clicar sobre este, será apresentada a lista das opções de tipos de Tarefas Associadas disponíveis na Plataforma uCloud, ver as opções abaixo:

  * **Ansible**: Esta opção permite ao usuário vincular um arquivo texto com um um script **Ansible**, para que este seja executado em uma máquina determinada virtual seguindo uma determinada prioridade no Fluxo de Trabalho (workflow).
  * **Terraform**: Esta opção permite ao usuário vincular um arquivo texto com um um script **Terraform**, para que este seja executado em uma máquina determinada virtual seguindo uma determinada prioridade no Fluxo de Trabalho (workflow).
  * **Puppet**: Esta opção permite ao usuário vincular um arquivo texto com um um script **Puppet**, para que este seja executado em uma máquina determinada virtual seguindo uma determinada prioridade no Fluxo de Trabalho (workflow). *ATENÇÃO execução dos script(s)/playbook(s) Puppet é mandatório a existência de uma infraestrutura de servidor para executá-los*.

* **Prioridade**: Este campo é obrigatório, nele o usuário deve informar um número inteiro que indica a ordem de prioridade que esta Tarefa Associada será executada. Sendo zero ("1") a mais alta prioridade, o que significa que a tarefa com o menor número informado será a primeira a ser executada na data e hora programada. Este campo permite ao usuário encadear várias tarefas, em outras palavras, executar as Tarefas Associadas em uma sequência específica, de acordo com a prioridade. Importante ressaltar que na eventual existência de duas tarefas diferentes e ambas com a mesma prioridade estas serão executadas em paralelo, a Plataforma uCloud executa Tarefas Associadas de forma sequencial (uma a uma).

* **Tipo de gerenciador de repositórios**: Este campo é obrigatório, trata-se de um campo do tipo “dropdown”, quando o usuário clicar sobre este, será apresentada a lista das opções de tipos de Tarefas Associadas disponíveis na Plataforma uCloud, ver as opções abaixo:

  * **Github**: Selecione esta opção somente se o usuário possui (em seu perfil de usuário) um "Token" que permite acesso ao repositório de arquivos de scrit(s)/palybook(s) estiver armazenado em um ambiente Github.
  * **Gitlab**: Selecione esta opção somente se o usuário possui (em seu perfil de usuário) um "Token" que permite acesso ao repositório de arquivos de scrit(s)/palybook(s) estiver armazenado em um ambiente Gitlab.

.. attention:: |atencao| Importante ressaltar que cada ambiente (Github/Gitlab) é isolado e completamente independentes entre si, pois são empresas completamente diferentes, o prefixo "Git" não significa que as plataformas são as mesmas. Os acessos são diferentes e específicas de cada um, e o seu respectivo "token" de acesso de um serviço não é reconhecido pelo outro serviço. O usuário de um serviço encontra seus arquivos UNICAMENTE no ambiente que este usuário possui autenticação para navegar via "token" de usuário.

* **Repositório**: Neste campo o usuário deve informar o link do repositório existente em um servidor público Github. Este campo deve ser informado com o permalink do arquivo desejado. Exemplo: ``repositorio/folder_repositorio``. Este permalink deve ser obtido através da acesso na interface do serviço selecionado no campo anterior (Github/Gitlab).

* **Container**: Este campo é obrigatório e do tipo “Dropdown” quando o usuário clica com o cursor do mouse, a Plataforma uCloud lista todos os containers configurados na Plataforma uCloud. O usuário deve selecionar um provedor da lista.

* **Máquina Virtual**: |icone_habil_verde|/|icone_desb_verm|: Este botão é um tipo “checkbox” que o usuário pode atuar para indicar que o script/playbook será executado em uma máquina virtual específica. Após esta seleção a Plataform uCloud apresenta os campos abaixo:

  * **Virtual Datacenter**: Este campo é obrigatório e do tipo “Dropdown” quando o usuário clica com o cursor do mouse, a Plataforma uCloud lista todos os Virtual Datacenters os quais o usuário  está vinculado. O usuário deve selecionar um VDC da lista.
  * **Máquina Virtual**: Este campo é obrigatório e do tipo “Dropdown” quando o usuário clica com o cursor do mouse, a Plataforma uCloud lista todas as máquinas virtuais do respectivo Virtual Datacenters selecionado pelo usuário. O usuário deve selecionar uma máquina virtual da lista.

* **Visualização**: Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Maecenas porttitor congue massa. Fusce posuere, magna sed pulvinar ultricies, purus lectus malesuada libero, sit amet commodo magna eros quis urna.
Nunc viverra imperdiet enim. Fusce est. Vivamus a tellus.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Proin pharetra nonummy pede. Mauris et orci.
Aenean nec lorem. In porttitor. Donec laoreet nonummy augue.
Suspendisse dui purus, scelerisque at, vulputate vitae, pretium mattis, nunc. Mauris eget neque at sem venenatis eleifend. Ut nonummy.


* **Versão do Python**: O Python é um ambiente de interpretação de linguagem de programação orientada a objetos e de alto nível com semântica dinâmica que cuida da implantação de aplicativos, gerenciamento de configuração, execução de tarefas e orquestração de vários nós. Este ambiente é mandatório para executar os script/playbook e deve estar instalado no ambiente da máquina virtual que foi informada no campo acima. O usuário deve selecionar a versão correta do Python instalada no ambiente da máquina virtual.

* **Usuário**: Este campo é obrigatório, e deve er preenchido com a credencial de usuário que possui acesso ao prompt do console da máquina virtual informada no campo acima, via uma sessão SSH. Importante ressaltar que a Plataforma uCloud não verifica antecipadamente se a credencial informada é válida e aceita para iniciar uma sessão SSH na máquina virtual informada. Qualquer erro de conexão deverá ser verificado no ícone de "**log**" de registro da Task Associada, somente após este ser executado ao menos uma vez.

* **Botão SSH**: Para associar um arquivo de chave SSH, o usuário deve clicar com o cursor do mouse sobre este botão para encontrar e selecionar o arquivo da chave SSH, específica para a máquina virtual, a qual deseja executar o script Ansible ou Puppet. Importante mencionar que a Plataforma uCloud não valida se o arquivo SSH selecionado pertence realmente à máquina virtual na qual se deseja executar o script Ansible ou Puppet. Não será apresentada qualquer mensagem de erro na interface da Plataforma uCloud, na situação em que a chave SSH não pertença a máquina virtual.

* **Campos Personalizados**: Estes campos podem ser utilizados pelo desenvolvedor do script/playbook para solicitar que usuário entre informções "variáveis" e necessárias para a correta execução do script/playbook. Estes campos enviam o conteúdo das "variáveis" antes da execução dos script/playbook.
  
  * **Label**: Este campo é meramente informativo e será utilizado pela Plataform uCloud para identificar seu conteúdo em uma janela popup a ser apresentado ao usuário.
  * **Chave**: Este campo é importante e determina a identificação da "variável" (seu nome) que foi provisionada pelo desenvolvedor do script/playbook para ser recebida dentro de seu códig de execução.
  * **Valor Padrão**: Este campo é importante e determina a o contaúdo inicial/padrão da "variável" que foi provisionada pelo desenvolvedor do script/playbook para ser recebida dentro de seu códig de execução. Importante ressaltar que a Plataforma uCloud não aceita valores nulos (campo em "branco").
  * **Pedir para Preencher**: Este campo é do tipo "check box" e permite que o desenvolvedor do script/playbook determine (sim/não) para que a Plataform uCloud solicite que o usuário informe o conteúdo para esta "variável", sendo solicitada ao usuário antes da execução do script/playbook.
  * **Obrigatório**: Este campo é do tipo "check box" e permite que o desenvolvedor do script/playbook determine (sim/não) para que a Plataform uCloud solicite o preenchimento obrigatório deste conjunto chave/valor e o usuário deve informe um conteúdo para esta "variável", antes da execução do script/playbook.
  * **Botão Adicionar**: Basta o usuário clicar com o cursor do mouse sobre este botão para que a Plataforma uCloud adicione o conjunto que define a "variável" (chave e valor) na lista abaixo. Imprtante mencionar que a Plataforma uCloud aceita mais de um conjunto de "variáveis" (chave/valor"), de forma a atender à demanda de preenchimento da quantidade de "variáveis" necessárioas para a correta execução do script/playbook criado pelo desenvolvedor.

* **Botão Criar**: Após preencher todos os campos obrigatórios para provisionar uma nova Tarefa Associada de Iniciar ou Parar, uma máquina virtual, o usuário pode clicar com o cursor do mouse no botão verde Criar para que a Plataforma uCloud provisione a nova Tarefa Associada em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, isto indica que algum campo obrigatório foi deixado sem preenchimento ou a sequência de caracteres do nome pode ser inferior a quatro (04) caracteres. A Plataforma uCloud apresenta uma mensagem pop-up, no canto superior direito da tela, com a informação de que a nova Tarefa Associada foi criada.

Após o clicar com o cursor do mouse sobre o botão Criar, a Plataforma uCloud atualiza a Seção Task Associadas com a referida tarefa que fará parte do Fluxo de Trabalho conforme o exemplo abaixo (a tela abaixo é meramente ilustrativa para efeito de demonstração):

.. figure:: /figuras/ucloud_workflows019g.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

Para os casos em que o usuário tenha inserido algum erro no campo Nome ou no campo Tipo, o usuário deve remover (apagar) a linha com erro, para isto deve clicar com o cursor do mouse sobre o icone |icone_lixo|. Após a remoção da linha o usuário deve efetuar o provisionamento correto novamente.

Se o usuário clicar com o cursor do mouse sobre o botão "**+Executar Agora**" a Plataforma uCloud irá iniciar a execução da sequência de Tasks Associadas dentro deste Fluxo de Trabalho (somente uma ou todas as Tasks Associadas seguindo a sequência definida no campo Prioridade).

Após a execução a Plataforma uCloud irá atualizar a coluna **Status** e apresentar na(s) linha(s) de cada Task Associada o botão |icone_log_wf|, que apresenta o conteúdo da informação do *log* de registro das ações referentes a execução desta Task Associada (erro ou sucesso).

Abaixo apresentamos um exemplo da tela de *log* de **falha**:

.. figure:: /figuras/ucloud_workflows010b.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----


Abaixo apresentamos um exemplo da tela de *log* de **sucesso**:

.. figure:: /figuras/ucloud_workflows012.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----


Client Server (Puppet)
----------------------

Puppet é uma ferramenta que ajuda a gerenciar e automatizar a configuração de servidores. Isso se executa escrevendo código de infraestrutura em Domain-Specific Language (DSL) do Puppet — Puppet Code — que você pode usar com uma ampla variedade de dispositivos e sistemas operacionais. O código Puppet é declarativo, o que significa que você descreve o estado desejado de seus sistemas, não as etapas necessárias para chegar lá. Puppet então automatiza o processo de colocar esses sistemas nesse estado e mantê-los lá. O Puppet faz isso por meio do servidor primário Puppet e de um agente Puppet. O servidor primário Puppet é o servidor que armazena o código que define o estado desejado. O agente Puppet traduz seu código em comandos e o executa nos sistemas que você especificar, no que é chamado de execução do Puppet.

O diagrama abaixo mostra como funciona a arquitetura do agente do servidor de uma execução do Puppet.

.. figure:: /figuras/puppet_run.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

O Puppet Server é um aplicativo executado na Java Virtual Machine (JVM) no servidor primário. Além de hospedar terminais para o serviço de autoridade de certificação, ele também alimenta o compilador de catálogos, que compila catálogos de configuração para nós de agentes, usando código Puppet e várias outras fontes de dados.

O servidor primário e o agente fazem parte da plataforma Puppet, descrita em A plataforma Puppet — junto com fatos, catálogos e relatórios (informações extraídas do site de Documentação Online Puppet [*]_).

Quando o uuário acessa o menu Workflows / Client Server a Plataforma uCloud apresenta a lista de todos os Puppet Servers provisionados encarregados de executar a JVM, conforme o exemplo da tela abaixo:

.. figure:: /figuras/ucloud_workflows020a.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

Provisionar um Puppet Server
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para os casos em que não exista um servidor primário ativo, a Plataforma uCloud permite, através de sua interface, o completo provisionamento de uma infraestrutura de servidor primário no ambiente do provedor de serviço de nuvem desejado pelo usuário (Azure, AWS, GCP).

Basta o usuário clicar sobre o botão **Criar** que a Plataforma uCloud apresenta a tela abaixo com todas as configurações necessárias para o perfeito provisionamento de uma infraestrutura de servidor com a configuração necessária para executar o JVM do ambiente Puppet.

.. figure:: /figuras/ucloud_workflows020b.png
   :alt: Workflow - Start/Stop Virtual Machine
   :scale: 50 %
   :align: center

----

Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Maecenas porttitor congue massa. Fusce posuere, magna sed pulvinar ultricies, purus lectus malesuada libero, sit amet commodo magna eros quis urna.
Nunc viverra imperdiet enim. Fusce est. Vivamus a tellus.
Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Proin pharetra nonummy pede. Mauris et orci.
Aenean nec lorem. In porttitor. Donec laoreet nonummy augue.
Suspendisse dui purus, scelerisque at, vulputate vitae, pretium mattis, nunc. Mauris eget neque at sem venenatis eleifend. Ut nonummy.


.. [*] Open Source Puppet site: https://puppet.com/docs/puppet/6/puppet_overview.html


Menu Tarefas
============

Neste menu Tarefas é por meio da API Rest que a Plataforma uCloud, envia ações (tarefas) para o gerenciador de ambiente de nuvem específico (público e/ou privado) para que estes então executem a ação desejada.

Importante ressaltar que não é a Plataforma uCloud que está responsável por executar as ações, mas sim o ambiente do provedor de serviço de nuvem (pública e/ou privada) onde o recurso computacional está localizado. Este ambiente operacional (hypervisor) é o encarregado de executar a tarefa enviada através da API Rest. Caso o resultado não seja refletido na interface da tela do usuário de forma imediata, significa que o console destino pode necessitar um tempo para executar esta tarefa e somente após o término da execução da tarefa o resultado será apresentado na interface do uCloud.

A Plataforma uCloud armazena em suas bases de dados internas todas as ações efetuadas (direta ou indiretamente), seja por usuários ou por atividades de manutenção automática de rotinas internas, ou por agendamentos de tarefas.

O menu **Tarefas** apresenta a lista de ações que foram provisionadas na Plataforma uCloud e estão sendo executadas nos seus respectivos ambientes, o usuário pode acompanhar o percentual de andamento destas tarefas, seu resultado de sucesso ou a mensagem de erro referente a alguma restrição do ambiente destino.

Neste menu, também, serão listadas as tarefas que estão agendadas para uma data futura e tarefas que aguardam a ação de um usuário ‘aprovador’ - o usuário deve ter o perfil de Administrador de Grupo ou Administrador de Contrato.

.. image:: /figuras/ucloud_menu_tarefas001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

As informações apresentadas nesta tela, demonstram todas as ações solicitadas e executadas por todos os usuários, pode ser utilizado com a função de um Log Segurança, pois registra cada evento solicitado pelo usuário e seus resultados (sucesso ou erro), e se a ação está aderente ao anteriormente definido, pelas políticas de permissionamento vinculadas ao usuário para cada ambiente de provedor de serviço de nuvem (pública e/ou privada).

Abaixo segue descrito o significado das duas (ou três) abas e suas respectivas colunas.

.. image:: /figuras/ucloud_menu_tarefas002.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

* **Botão Procurar**: A lista de tarefas pode ser muito extensa (datas antigas) ou no caso do ambiente da empresa possuir uma grande quantidade de usuários. Basta o usuário clicar com o cursor do mouse sobre o botão Procurar e a plataforma do uCloud apresenta alguns campos para refinar a pesquisa:

  * **Início**: Neste campo o usuário pode informar a data inicial que deseja selecionar para filtrar o resultado na lista de tarefas apresentadas nesta tela.
  * **Data Final**: Neste campo o usuário pode informar a data final que deseja selecionar para filtrar o resultado na lista de tarefas apresentadas nesta tela.
  * **User**: Neste campo o usuário pode informar a identificação da credencial de login de um usuário específico para filtrar o resultado na lista de tarefas apresentadas nesta tela.
  * **Status**: Este campo é um campo do tipo “dropdown” quando o usuário clicar com cursor do mouse a Plataforma uCloud apresenta uma lista de opções de Status de uma tarefa, e permite filtrar o resultado na lista de tarefas apresentadas nesta tela. Os tipos de status podem ser os seguintes:

    * Successful:
    * Running
    * Cancelled
    * Failed
    * Created
    * Scheduled
    * Not Approved
    * Approved
    * Approvation Pending

* **Botão Refresh**: A Plataforma uCloud se comunica com o console dos provedores através da API Rest, toda ação solicitada nas telas do uCloud envia ações (tarefas) para o gerenciador de ambiente (console) de nuvem específico (público e/ou privado) para que estes então executem a ação desejada. Para que a plataforma do uCloud possa atualizar apenas o conteúdo das seções de tela (ou as informações contidas nestas seções) é mandatório ao usuário clicar com o mouse sobre o botão Refresh, ele executa apenas a atualização das informações contidas em nossas bases de dados.

Aba Tarefas
-----------

Esta "aba/tab" é a apresentação padrão/default da Plataforma uCloud, ela apresenta todas atividades constantes em sua base de dados, em ordem de data e hora, classificados em ordem decrescente (do mais recente para o mais antigo), conforme o exemplo da tela abaixo:

.. image:: /figuras/ucloud_menu_tarefas003.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Quando o usuário acessar esta tela a Plataforma uCloud apresenta o registro (log) de atividades de todos os usuários, a tela possui as seguintes colunas:

* **Operação**: Esta coluna apresenta a descrição da operação solicitada na interface da Plataforma uCloud, a qual é enviada para o ambiente do provedor de serviço de nuvem (pública e/ou privada).
* Usuário: Esta coluna apresenta as credenciais de login do usuário solicitado na execução da operação, através da interface da Plataforma uCloud.
* **Detalhes**: Este ícone de sinal de adição (“+”) permanece indisponível para as operações que exibem o status de “Successful”. Este ícone fica habilitado somente nas operações que apresentam o status “Failed” e, basta o usuário posicionar o cursor do mouse sobre o ícone para que a mensagem de erro seja apresentada. Veja o exemplo abaixo no ítem Status.
* **Progresso**: Esta coluna apresenta uma barra que representa a porcentagem da evolução da execução da operação, no ambiente do provedor de serviço de nuvem (pública e/ou privada).
* **Data de Início**: Esta coluna apresenta a data (Padrão Brasileiro: dia/mês/ano) e o horário (formato de 24 horas) do início da operação, no ambiente do provedor de serviço de nuvem (pública e/ou privada).
* **Duração**: Esta coluna apresenta o tempo decorrido, necessário, para que o ambiente do provedor de serviço de nuvem (pública e/ou privada) possa completar a operação solicitada. Importante ressaltar que este tempo de duração pertence exclusivamente ao ambiente do provedor de serviço de nuvem (pública e/ou privada), a Plataforma uCloud não interfere na duração das operações no ambiente do provedor de serviço de nuvem (pública e/ou privada).
* **Status**: Esta coluna apresenta o status resultante da operação solicitada, ela permite apresentar os seguintes resultados:

  * *Successful*:
  * *Running*
  * *Cancelled*
  * *Created*
  * *Scheduled*
  * *Not Approved*
  * *Approved*
  * *Approbation Pending*
  * *Failed*: Este status pode representar um erro referente a algum limite do usuário definido no ambiente da Plataforma uCloud, no caso de ocorrência, entrar em contato com a equipe de suporte da Ustore, para o melhor entendimento da causa do referido erro; no exemplo abaixo, o usuário ultrapassa o limite de consumo definido dentro da Plataforma uCloud para o usuário:

.. image:: /figuras/ucloud_menu_tarefas004.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

  * *Failed*: Este status pode representar mensagens de erro que retornam (via API-Rest) do ambiente do provedor de serviço de nuvem pública, no caso de ocorrência, entrar em contato com a equipe de suporte da Ustore, para o melhor entendimento da causa do referido erro; o exemplo abaixo apresenta um erro do provedor AWS:

.. image:: /figuras/ucloud_menu_tarefas005.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Aba Aprovações Pendentes
------------------------

Esta "aba/tab" apresenta a lista de todas as operações de usuários que dependem da aprovação de um Administrador de Grupo, ou Administrador de Contrato, em ordem de data e hora, classificados em ordem decrescente (do mais recente para o mais antigo), conforme o exemplo da tela abaixo:

.. image:: /figuras/ucloud_menu_tarefas006.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Esta "aba/tab" possui as seguintes colunas:

* **Operação**: Esta coluna apresenta a descrição da operação solicitada na interface da Plataforma uCloud, a qual foi enviada para o ambiente do provedor de serviço de nuvem (pública e/ou privada).
* **Usuário**: Esta coluna apresenta as credenciais de login do usuário que solicita a execução da operação, através da interface da Plataforma uCloud.
* **Aprovação**: Esta coluna apresenta dois ícones para que o Administrador do Grupo ou o usuário Administrador do Contrato possam interagir com esta solicitação:
* **Ícone de Confirmação**: Quando o usuário deseja confirmar a operação solicitada, basta clicar com o cursor do mouse no botão verde para confirmar a operação. A confirmação da solicitação significa que a operação será enviada para o ambiente do provedor de serviço de nuvem (pública e/ou provada) para ser executada.
* **Ícone de Cancelamento** “”: Quando o usuário deseja recusar a solicitação da operação, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho, para cancelar a solicitação da operação. O cancelamento da solicitação significa que a operação não será enviada para o ambiente do provedor de serviço de nuvem (pública e/ou provada) para ser executada.
* **Status**: Esta coluna apresenta o status resultante da aprovação ou cancelamento da operação solicitada.

Aba Tarefas Agendadas
---------------------

Esta "aba/tab" apresenta o ambiente no qual o usuário pode verificar as tarefas agendadas para serem executadas em uma data futura (agendamento de provisionamento de máquina virtual ou uma tarefa de um Workflow), conforme o exemplo abaixo:

.. image:: /figuras/ucloud_menu_tarefas007.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Esta "aba/tab" possui as seguintes colunas:

* **Operação**: Esta coluna apresenta a descrição da operação solicitada na interface da Plataforma uCloud, a qual foi enviada para o ambiente do provedor de serviço de nuvem (pública e/ou privada).
* **Usuário**: Esta coluna apresenta as credenciais de login do usuário que solicita a execução da operação, através da interface da Plataforma uCloud.
* **Data da Criação**: Esta coluna apresenta a data (Padrão Brasileiro: dia/mês/ano) e o horário (formato de 24 horas) da operação, solicitada pelo usuário.
* **Data da Execução**: Esta coluna apresenta a data (Padrão Brasileiro: dia/mês/ano) e o horário (formato de 24 horas) programado para execução da operação, solicitada pelo usuário.
* **Tempo restante**: Esta coluna apresenta o tempo (no formato de horas padrão 24 horas) faltante até completar a data e hora programada, para a execução da operação. Este tempo é calculado, constantemente, tem como base a hora corrente que o usuário está consultando esta lista.
* **Ações**: Esta coluna apresenta somente o ícone de remoção (“”) que permite ao usuário remover/apagar o agendamento da tarefa, a ação cancela a execução da tarefa na data e hora programada.

Menu Inventário de Recursos
===========================

A Plataforma uCloud quando corretamente configurada, com as credenciais de acesso ao provedor de serviços de nuvem, extrai um inventário de todos os recursos existentes no ambiente do provedor de serviço de nuvem (pública e/ou privada).

Esta tela de inventário de recursos lista todos os recursos computacionais existentes no provedor de serviço de nuvem, as quais se tem as credenciais de acesso com a permissão de visualizar. Na barra de menu, o usuário encontra a opção Inventário de Recursos, ao selecionar esta opção do menu, é apresentada a seguinte tela abaixo:

.. image:: /figuras/ucloud_menu_inventario_recursos001.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center

----

Através do acesso a esta tela, a Plataforma uCloud permite ao usuário adicionar ou alterar, a informação da etiqueta (tag) que está vinculada a um recurso computacional das nuvens (pública e/ou privada). Esta funcionalidade permite aumentar a granularidade de governança e controle de custos.

A Plataforma uCloud extrai a informação (download) do provedor, se o usuário já houver vinculado uma etiqueta (tag), diretamente no console do provedor de serviço de nuvem, esta informação será apresentada na lista de recursos existentes.

Nas situações em que o usuário não vincular qualquer etiqueta (tag) ao recurso, a coluna será apresentada em branco. Através do acesso a esta tela é possível tanto adicionar, quanto alterar a informação da etiqueta (tag) de um recurso presente na lista.

Na coluna **Tag** o usuário pode encontrar a informação necessária, referente a etiqueta (tag) existente, vinculada ao recurso.

Editor de Etiquetas (tags) Nativo
---------------------------------

Na coluna Ações, o usuário pode encontrar o Ícone de Edição Ativo |icone_edita_on| que permite ao usuário adicionar uma nova tag para o recurso computacional, bem como alterar a informação da etiqueta (tag) da linha do recurso selecionado. Quando o usuário clicar com o cursor do mouse sobre o ícone, em um recurso computacional que não possua nenhuma tag a Plataforma uCloud apresenta a seguinte tela:

.. image:: /figuras/ucloud_menu_inventario_recursos003.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center
   :class: with-border

----

* **Ações**: Nesta coluna o usuário pode encontrar dois ícones diferentes:

  * **Ícone Lata de Lixo** |icone_lixo|: Este ícone permite ao usuário apagar toda a informação referente às etiquetas (tags) do recurso que está sendo editado. Importante ressaltar que esta ação é definitiva, da mesma forma ela é aplicada no recurso do provedor de serviço de nuvem, após a sincronização da ação com a console do provedor.

  * **Ícone de Edição Ativo** |icone_edita_on|: Este ícone permite ao usuário tanto adicionar nova(s) tag(s), bem como alterar o conteúdo da tag da linha do recurso selecionado, quando selecionado a Plataforma uCloud apresenta a tela abaixo:

.. image:: /figuras/ucloud_menu_inventario_recursos002.png
   :alt: Virtual Datacenter - Exemplo
   :scale: 60 %
   :align: center
   :class: with-border

----

    * **Chave**: Neste campo, o usuário deve preencher com a sequência de caracteres referente a chave (key) que deseja vincular ao recurso.
    * **Valor**: Neste campo o usuário deve preencher com informação referente ao valor que deseja vincular a chave do recurso.
    * **Botão Criar**: Após certificar que todas as informações - a chave e o seu valor - foram configuradas (inclusões ou exclusões), o usuário deve clicar com o botão do mouse no botão Criar para aplicar alterações, de forma definitiva e imediata. Este botão é obrigatório, no caso do usuário efetuar a remoção das informações existentes a uma etiqueta (tag), após clicar no botão Lata de Lixo. Em seguida, o usuário deve clicar sobre este botão para a Plataforma uCloud fechar esta tela e retornar à tela anterior, com seu conteúdo atualizado.


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

.. |botao_proximo| image:: /figuras/ucloud_botao_proximo.png

.. |botao_voltar| image:: /figuras/ucloud_botao_voltar.png

.. |botao_criar_off| image:: /figuras/ucloud_botao_criar_cinza.png

.. |botao_criar_on| image:: /figuras/ucloud_botao_criar_verde.png

.. |botao_cencela_verm| image:: /figuras/ucloud_botao_cancela_verm.png

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

.. |icone_amplia_vdc| image:: /figuras/ucloud_icone_amplia_vdc.png

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

.. |icone_revert_snap| image:: /figuras/ucloud_icone_revert_snap.png

.. |icone_wf_ativo| image:: /figuras/ucloud_icone_wf_ativo.png

.. |icone_wf_parado| image:: /figuras/ucloud_icone_wf_parado.png

.. |icone_lapis_workflow| image:: /figuras/ucloud_icone_edita_workflow.png

.. |botao_adicionacarrinho| image:: /figuras/ucloud_botao_colocacarrinho.png

.. |botao_finalizapedido| image:: /figuras/ucloud_botao_finalizapedido.png

.. |icone_log_wf| image:: /figuras/ucloud_icone_info_workflow.png

.. |icone_refresh| image:: /figuras/ucloud_icone_refresh.png

.. |icone_sino| image:: /figuras/ucloud_icone_sino.png

.. |icone_grafico_barra01| image:: /figuras/ucloud_icone_grafico01.png

.. |icone_grafico_barra02| image:: /figuras/ucloud_icone_grafico02.png

.. |icone_graph_large| image:: /figuras/ucloud_icone_big_graph.png

.. |icone_troca_mes| image:: /figuras/ucloud_icone_mes.png

.. |icone_seta_acima| image:: /figuras/ucloud_icone_fatur_acima.png

.. |icone_seta_abaixo| image:: /figuras/ucloud_icone_fatur_abaixo.png

.. |icone_neutro| image:: /figuras/ucloud_icone_fatur_estavel.png

.. |icone_next_ativo| image:: /figuras/ucloud_icone_next_activo.png

.. |icone_next_off| image:: /figuras/ucloud_icone_next_off.png

.. |icone_lupa| image:: /figuras/ucloud_icone_lupa.png
