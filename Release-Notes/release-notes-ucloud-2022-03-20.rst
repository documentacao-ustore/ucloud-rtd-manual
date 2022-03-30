uCloud - Notas Março-2022
=========================

.. figure:: /figuras/ucloud_logo_peq.png
   :alt: Logo uCLoud
   :scale: 50 %
   :align: center

----

Apresentação
============

Atualmente todo profissional de infraestrutura de TI utiliza diversos *consoles* diferentes para provisionar recursos computacionais, seja dentro da empresa (data center privado) ou em em algum provedor(es) de nuvem(ns). Desta forma, se manter atualizado e preparado, em todas as "consoles" é um dos desafios atuais para qualquer profissional de TI.

Na tentativa de aumentar a produtividade e reduzir o grau de dependência destes *consoles* o mercado desenvolveu o conceito de Infraestrutura como Código (IaaC - Infrastructure as a Code). Mas este conceito endereça somente o momento do provisionamento inicial (mesmo com o uso de scripts para instalação de padrões e softwares), mas podem existir demandas em que o profissional de TI terá de se conectar ao *console* do ambiente para executar alguma intervenção na infraestrutura que não é possível através do conceito de IaaC. Estar conectado e ficar alternando entre os diversos consoles de nuvem, demanda uma grande especialização e conhecimento do profissional de TI.

As plataformas de CSB (*Cloud Service Broker*) foram desenvolvidas para ocupar esse nicho e concentrar o inventário dos recursos computacionais de nuvens públicas e privadas em uma única interface e que transfere para o usuário o controle e operação destes recursos multi-nuvem.

Como mencionamos, o próprio mercado desenvolveu as metodologias de provisionamento de recursos computacionais através de scripts automatizados (também chamados de playbooks). Dentre estes formatos existem alguns que o mercado mundial adotou mais largamente, e podemos citar o Ansible, Terraform e Puppet.

O mercado também criou a demanda de programar a execução de uma sequência de diversos scripts dentro de um fluxo controlado e encadeado de forma que um erro em um destes scripts pode interromper todo o fluxo para evitar o provisionamento de uma infraestrutura computacional sem a devida qualidade.

Mas, muito importante é o nível de permissão das respectivas ações deste profissional seja na nuvem pública ou na nuvem privada. Independente se o profissional executa as ações via console ou via script automatizado, as plataformas de CSB devem possuir mecanismos que de provisionar um Perfil de Permissionamento e que estes possam ser vinculados às credenciais de acesso do usuário para controlar, adequar ou restringir as ações deste usuário.

Atenta à evolução constante do mercado brasileiro e às demandas de nossos usuários, a Ustore apresenta as novas funcionalidades que podem transformar a forma de gerenciar nuvens públicas e privadas com o uCloud.
Entre as novidades da nova versão destaca o Switch Roles, o Perfil de Permissionamento, o Catálogo de Serviços e o Workflow; que descreveremos a seguir.

Novas implementações
--------------------

Abaixo apresentamos a lista de novas implementações:

* Switch Roles
* Workflows
* Catálogo de Serviços
* Perfis de Permissionamento

Abaixo iremos esclarecer e descrever as novas implementações acima listadas.

Correções de Erros
------------------

Abaixo descrevemos as ações corretivas devido a situações que foram reportados erros e quais foram as ações corretivas de nossa equipe de desenvolvimento.

Amazon Web Services (AWS)
+++++++++++++++++++++++++
Não existe nenhuma menção referente a qualquer alteração para o presente documento.

Microsoft Azure (Azure)
+++++++++++++++++++++++
Em **janeiro de 2022** a Azure parou de adicionar informações de billing em moeda americana (dólar) e iniciou cobranças dos valores das faturas em moeda brasileira (Real), somente para os contratos CSP.

Isto acarretou que o desde 27 de janeiro de 2022, nenhum novo registro com valor do custo de recurso computacional é adicionado no arquivo de billing em dólar, e o bucket existente não está sendo atualizado e os valores não se encontram mais nesta área de armazenamento (bucket). Desta forma, os valores dos relatórios financeiros das faturas Azure se apresentam zerados. **Isto não é um erro**, pois *a Plataforma uCloud está corretamente configurada para coletar os valores do billing na área dólar americano, mas a Azure não está atualizando mais as informações contidas no arquivo de billing*.

A Azure criou uma nova área de bucket para armazenar o billing em Real, e esta nova área de bucket deve ser corretamente configurada na Plataforma uCloud.

A Plataforma uCloud por padrão pode ser configurada para cobranças em diversas moedas (Real, Dólar Americano, Pesos Colombianos, Pesos Mexicanos e Euro).

Para correção deste cenário, inicialmente deve-se validar se a credencial de billing provisionada na Plataforma uCloud possui acesso a esta nova área de bucket (Real Brasileiro).

Nos casos que a credencial atual permita o acesso à nova área de bucket, deveremos re-configurar a Plataforma uCloud para acessar esta nova área e processar o billing dos meses de fevereiro em diante.

Nos casos em que a credencial atual não permite o acesso à nova área de bucket o usuário com nível de administrador do ambiente Azure, deverá providenciar a criação de uma nova credencial de acesso com permissão Read-Only para esta área do bucket, e configurar esta nova área de bucket e sua respectiva credencial de acesso, na Plataforma uCloud.

Para ambos os casos, indicamos que o usuário entre em contato com a Equipe de Suporte da Ustore (chamados@usto.re) para ajudá-lo nesta configuração do bucket e a respectiva adequação das regras de faturamento do(s) contrato(s) que estão vinculados à Azure CSP.

Google Cloud Platform (GCP)
+++++++++++++++++++++++++++
Não existe nenhuma menção referente a qualquer alteração para o presente documento.

Huawei Web Services (Huawei)
++++++++++++++++++++++++++++
Não existe nenhuma menção referente a qualquer alteração para o presente documento.

VMware 6.5 ou superior (vCenter/vSphere)
++++++++++++++++++++++++++++++++++++++++
Não existe nenhuma menção referente a qualquer alteração para o presente documento.

Atualização e Novas APIs
++++++++++++++++++++++++
Não existe nenhuma menção referente a qualquer alteração para o presente documento.

Switch Roles
============

Quando um usuário de infraestrutura multi-nuvem precisa alternar entre diversos consoles de provedores de nuvem, o processo de login com diversas credenciais em diversos consoles gera um gasto de tempo e pode incorrer em erros de digitação de logins e senhas.

A plataforma do uCloud por ser um ambiente multi-nuvem permite que o usuário possa interagir com os recursos computacionais existentes em diversos provedores de nuvem diferentes de forma simultânea.

Ao iniciar uma sessão na Plataforma uCloud (login) o usuário obtém um conjunto específico de permissões para executar ações que pertencem ao contrato ao qual o usuário está vinculado. O(s) usuário(s) pertencem a um Grupo, e os Grupos pertencem a um contrato. Portanto, as credenciais de acesso do usuário estão vinculadas a um, ou mais, Contratos, Este contrato pode estar provisionado para ter acesso a um (ou mais) credenciais de acesso aos ambientes dos provedores de nuvem pública e/ou privada.

Veja a figura abaixo, que demonstra a vinculação do usuário a um, ou mais, contratos:
  
.. figure:: /figuras/ucloud_arquitetura_conceitual001.png
   :alt: Arquitetura Conceitual
   :align: center

----

O primeiro aspecto da figura acima é que podemos verificar que este cliente possui dois contratos diferentes. O Contrato A está associado a somente um provedor de nuvem pública (ex: AWS) e o Contrato B está associado a dois provedores de nuvem pública diferentes (ex: AWS e Azure).

Switch Roles - Cenário Exemplo
------------------------------

Na figura acima podemos visualizar que os usuários Mariah, João e Carlos pertencem a somente um único contrato e este contrato possui somente um único provedor (ex: AWS).

O usuário Josué está associado a dois contratos diferentes e para evitar que este usuário tenha de alternar entre sessões de registro diferentes (encerrar uma sessão e iniciar outra com outra credencial), a Ustore desenvolveu e implementou a funcionalidade de Switch Roles.

Desta forma apenas o usuário Josué, através da funcionalidade, de Switch Roles pode alternar entre os contratos aos quais ele está vinculado, simplesmente alternando entre os contratos aos quais ele está vinculado.

O usuário Josué é responsável pela total gestão da infraestrutura do ambiente Azure, porém, no ambiente da AWS, ele pode somente visualizar os recursos computacionais, pois não possui a permissão de operar estes recursos computacionais (ex: Read Only).

Através da funcionalidade Switch Roles será possível aplicar esta mudança de papel sem a necessidade de troca do usuário, isso será feito com um através da seleção de contrato e/ou container que este usuário deseja acessar.

A funcionalidade de Switch Roles fica posicionada no canto superior direito da área de tela da Plataforma do uCloud (ao lado do nome do usuário) - veja a tela abaixo:

.. figure:: /figuras/ucloud_dashboard_switch_roles001.png
   :alt: Switch Roles
   :align: center

----

Basta o usuário clicar com o cursor do mouse sobre o nome do contrato e a Plataforma do uCloud apresenta uma janela pop-up que apresenta ao usuário a lista de contratos aos quais este está vinculado para que ele selecione o contrato desejado.
  
.. figure:: /figuras/ucloud_dashboard_switch_roles002.png
   :alt: Switch Roles
   :scale: 50 %
   :align: center

----

Ao selecionar o contrato desejado a Plataforma do uCloud irá atualizar a informação apresentada no canto superior direito da sessão do usuário.

Importante ressaltar que essa janela pop-up lista somente os contratos aos quais o usuário está vinculado. Caso existam outros contratos provisionados na Plataforma uCloud, o usuário não terá acesso a nenhum destes outros contratos.
  
.. figure:: /figuras/ucloud_dashboard_switch_roles003.png
   :alt: Logo uCLoud
   :align: center

----

A funcionalidade Switch Roles possibilita a um usuário alternar tanto seu nível de acesso bem como obter acesso a diferentes contratos com diferentes regras de permissões para cada contrato sem ter de encerrar a sua sessão na Plataforma uCloud.

Com esta nova funcionalidade um único usuário poderá acessar, por exemplo, a nuvem Azure e a nuvem AWS com a possibilidade de ter responsabilidades, permissões e níveis de acesso completamente diferentes e específicos para cada um dos ambientes dos provedores de nuvem pública.

A personalização das permissões de atividades que o usuário poderá possuir será esclarecido no tópico **Perfil de Permissionamento**, neste documento.

Fluxos de Trabalho - Workflows
==============================

A funcionalidade de Fluxos de Trabalho pode desempenhar diversas ações de operação na infraestrutura de recursos computacionais de nuvem pública e/ou privada.

As funcionalidades disponíveis são as seguintes:

#. Desligamento de Máquina Virtual (Shutdown)
#. Ativação de Máquina Virtual (Start/Boot)
#. Cópia Instantânea de um volume (Disk Snapshot)
#. Executar um, ou mais, scripts/playbooks com sintaxe:
  a. Ansible
  b. Terraform
  c. Puppet

Desligamento de Máquina Virtual (Shutdown)
------------------------------------------

O usuário pode programar a ação de desligamento (shutdown) de um servidor após um horário determinado durante a semana, ou para finais de semana. Esta ação pode ser programada para ser executada diariamente em um horário pré-determinado (ex: executar shutdown de segunda a quinta-feira às 21 horas). Outra forma é a programação do desligamento da infraestrutura do servidor durante os finais de semana (ex: desligamento toda sexta-feira às 23 horas).

Esta ação pode ser útil para recursos de servidores de nuvem pública que são cobrados por uso, e as aplicações nele sendo executadas podem ficar indisponíveis em determinados períodos do dia ou aos finais de semana.

Ativação de Máquina Virtual (Start/Boot)
----------------------------------------

Seguindo o exemplo de desligamento programado, o usuário pode utilizar a funcionalidade de workflows para ativar (start) um servidor em um horário programado para que as aplicações que estão sendo executadas neste servidor, estejam disponíveis para os usuários durante o horário comercial.

Esta ação pode ser programada para ser executada diariamente em um horário pré-determinado (ex: executar start de segunda a sexta-feira às 05 horas). Desta forma revertendo assim, o desligamento diário e durante os finais de semana; deixando a infraestrutura do servidor e suas aplicações disponível para seus usuários durante o horário comercial.

Esta implementação pode reduzir os custos recorrentes de recursos de servidores que foram contratados como cobrança por utilização. 

Estas funcionalidades de desligamento e ativação programada, pode não ser muito efetiva para redução de custos operacionais para determinados tipos de recursos como instâncias reservadas (Reserved Instances), ou as instâncias SPOT. Cada provedor de serviço de nuvem pública possui um custo pré-fixado para a contratação destas modalidades de infraestrutura de máquinas virtuais e o desligamento não acarreta uma redução no custo de utilização.

Efetuar Cópia Instantânea de Volume (Disk Snapshot)
---------------------------------------------------

Esta atividade pode ser entendida (ou confundida) com a atividade de cópia de segurança (*backup*), mas é importante esclarecer que esta funcionalidade apenas executa uma função nativa dos consoles dos provedores de serviço de nuvem pública e/ou privada, que é a cópia instantânea de um volume de disco em um horário determinado pelo usuário.

Em sistemas de computador, uma cópia instantânea de volume ou captura instantânea de volume (do Inglês: snapshot, tradução literal: foto instantânea) é o estado de um sistema em um determinado ponto no tempo. O termo foi cunhado como uma analogia ao usado em fotografia. Pode se referir a uma cópia real do estado de um sistema ou a um recurso fornecido por determinados sistemas.

Importante mencionar que uma das diferenças entre um storage snapshot e um backup é que o snapshot é armazenado no mesmo local dos dados originais. Portanto, depende completamente da confiabilidade da origem. Isso significa que, no caso de um desastre ou danos aos dados de origem, o snapshot está totalmente comprometido ou ficaria inacessível.

Um disk snapshot não efetua o processo de validação da integridade lógica do processo de cópia do(s) arquivo(s) individualmente, simplesmente executa a ação de cópia instantânea de todo o disco associado a infraestrutura que compreende o servidor.

O usuário pode provisionar a ação de criação de um *disk snapshot* em dias e/ou horários programados e deixar que a Plataforma uCloud envie esta solicitação (via API-REST) para o console do provedor de serviço de nuvem para que o provedor inicie este disk snapshot.

Executar scripts/playbooks Ansible, Terraform, Puppet
-----------------------------------------------------

Um princípio fundamental de Desenvolvimento e Operação (*DevOps*) é tratar a infraestrutura da mesma forma que os desenvolvedores tratam o código. Um código de um aplicativo tem um formato e uma sintaxe. Se o código não for escrito de acordo com as regras da linguagem de programação, os aplicativos não poderão ser criados. O conteúdo do código é armazenado em um algum sistema de Controle e Gerenciamento de Versionamento, em outras palavras uma plataforma que controla a origem e que registra todo o histórico de desenvolvimento de código, alterações e correções de bugs.

Atualmente o mercado criou o conceito de provisionar Infraestrutura como Código (*IaC - Infrastructure as Code*) que significa aplicar o mesmo rigor do desenvolvimento de código de aplicativo ao provisionamento de infraestrutura. Todas as configurações de um recurso computacional de nuvem pública, devem ser definidas de forma declarativa e armazenadas em um sistema de controle de versão e colaboração (ex: Github, Gitlab), o mesmo que o código do aplicativo. O provisionamento, orquestração e implantação de infraestrutura também devem dar suporte ao uso da infraestrutura como código.

Tradicionalmente, a infraestrutura era provisionada usando uma combinação de scripts e processos manuais. Estes scripts podem ser armazenados em sistemas de controle de versão ou documentados passo a passo em arquivos de texto ou playbooks. Se esses scripts ou playbooks não forem atualizados com frequência, eles podem se tornar um obstáculo nas implantações. Isso resulta na criação de novos ambientes nem sempre repetíveis, confiáveis ou consistentes. Portanto, este é o ponto fundamental da adoção e uso de uma plataforma de repositórios com controle de versionamento, pois é fundamental que o usuário utilize apenas as últimas versões dos *scripts/playbooks* que foram atualizados e revisados.

A funcionalidade de Fluxos de Trabalho (*workflows*) para ambiente de nuvem pública e/ou privada, permite ao profissional de TI conectado na Plataforma uCloud criar uma sequência automática de ativações de arquivos de scripts playbooks para controlar a sequência de ações para provisionar um recurso computacional com as características de configuração, sistema operacional, pacotes de softwares e regras de segurança requeridas pela regulamentação (compliance) de maneira confiável e com a utilização de scripts automatizados.

Por padrão, a Plataforma uCloud utiliza a integração nativa com a *Plataforma Github*, e o proprietário deste repositório autoriza usuários a se conectarem neste repositório através de um código de identificação (Token) que deve ser gerado unicamente através de uma sessão no Github, para cada usuário ou usuários. Este token deve possuir a permissão de se conectar neste repositório para ter acesso aos arquivos de scripts/playbooks armazenados e versionados.

A sequência de caracteres que representa o token que permite que as credenciais de login da Plataforma uCloud possa ter acesso ao repositório Github, deve ser informado no cadastro de usuários da Plataforma uCloud, sem esta configuração, o usuário não poderá acessar o repositório de scripts/playbooks para criar o fluxo de trabalho (workflow).

.. important:: A Plataforma uCloud não efetua nenhuma validação prévia se a cadeia de caracteres referente ao token de acesso ao Github é válida ou não. A Plataforma uCloud não irá apresentar qualquer mensagem informativa referente à inclusão deste token à credencial de um usuário.

Atualmente a Plataforma uCloud suporta as seguintes ferramentas de IaC:

* Ansible
* Terraform
* Puppet*

Importante mencionar que a Plataforma uCloud não é, por ela mesma, um ambiente de armazenamento e controle de versionamento dos arquivos de playbooks. No presente momento a Plataforma do uCloud permite a integração à uma ferramenta de controle de repositório de arquivos de scripts/playbooks, esta função é reservada a uma ferramenta externa.

.. note:: A Plataforma uCloud, não efetua qualquer validação prévia da coerência ou consistência da estrutura e sintaxe escrita no arquivo de script/playbook; desta forma qualquer erro pré-existente na sintaxe do texto do script, será executado de forma literal, podendo gerar (ou não) um erro que pode ser visualizado através da interface do uCloud.

.. warning:: Puppet = *Atenção a Plataforma uCloud permite criar um workflow que irá ativar um script/playbooks na sintaxe Puppet, mas para que um profissional possa utilizar script/playbook Puppet será necessário um ambiente adicional (na forma de uma infraestrutura de servidor). Este servidor que será encarregado da EXECUÇÃO dos referidos script/playbooks. A Plataforma uCloud não desempenha a função de suporte para a execução de scripts/playbooks Puppet*.

Workflows de Scripts/Playbooks - Exemplos de Uso
------------------------------------------------

Vamos usar o exemplo abaixo para imaginarmos um Fluxo de trabalho (workflow) que irá executar uma sequência de ações pré-determinadas e cada uma destas ações pode ser um script/playbook independente.

O objetivo final é ter uma nova máquina virtual, idêntica do ponto de vista de configuração de hardware, sistema operacional e suas atualizações de pacotes de software (patches e hotfixes do Sis.Op.), iniciar esta nova máquina virtual e executar um script/playbook que promove a instalação de softwares complementares e enviar uma notificação de “Sucesso” para indicar que o processo de provisionamento desta máquina virtual foi finalizado.

Mas no caso de que qualquer scripts/playbooks retorne algum erro durante sua execução, desejamos que o recurso computacional da máquina virtual, seja apagado/removido, e enviar uma notificação de “ERRO” para indicar a interrupção do processo de provisionamento desta máquina virtual.

Para este cenário iremos assumir o conceito que cada bloco de ação é um arquivo independente e presente no repositório do Github e através da interface da Plataforma uCloud o usuário pode ‘programar’ a sequência em que cada script/playbook será executado, criando assim um “Fluxo de Trabalho - um Workflow”.

Usando o fluxo gráfico abaixo em que cada caixa (box) representa um script/playbook que está armazenado no repositório do Github.

Para este exemplo, não iremos descrever e fica a critério do leitor a sua melhor metodologia de execução da tarefa de “Envio de Notificação”. O leitor pode se utilizar de qualquer metodologia, aplicação, meio disponível ou preferível para esta finalidade.

.. figure:: /figuras/ucloud_workflows001b.png
   :alt: Logo uCLoud
   |scale| 60 %
   :align: center

----

Assumindo que o usuário está com uma sessão ativa na Plataforma uCloud, e sua credencial possui um token válido para acesso ao repositório no Github, e cada bloco possui um script/playbook armazenado no repositório, o usuário poderá provisionar um fluxo de trabalho que pode conter a sequência de Tarefas Associadas, que ao final poderá ter a seguinte configuração.

.. figure:: /figuras/ucloud_workflows008g.png
   :alt: Logo uCLoud
   :align: center

----

Este é apenas uma figura que apresenta um exemplo da funcionalidade de Fluxo de Trabalho (Workflow) da Plataforma uCloud, depois de configurada por um usuário.

Foi provisionado um workflow denominado “ClonarVM-Ansible”, este fluxo executa a sequência de “Task Associadas” e na coluna Prioridade existe o número sequencial no qual o usuário programou para esta atividade ocorra.

No exemplo acima, demonstramos a possibilidade de execução sequencial, a tarefa com prioridade 2 será executada somente ao final da 1, e assim sucessivamente e na sequência informada, pois este fluxo depende da execução do script/playbook anterior para que o próximo seja executado, existe uma certa dependência sequencial.

Apenas como comentário a Plataforma uCloud permite, também, que dois scripts/playbooks sejam executados em paralelo, tendo ambos o mesmo número no campo Prioridade, mesmo que estejam apresentados na lista de Tasks Associadas, o que determina a execução em paralelo é o número informado na prioridade.

Um detalhe que pode ser muito interessante, é que o usuário pode provisionar um workflow interativo, que pode solicitar informações complementares para a execução, como por exemplo solicitar que seja informado o “nome da Máquina Virtual” antes de executar o script/playbook de clonar uma máquina virtual.

Antes da execução do script, o usuário pode clicar com o cursor do mouse sobre o ícone com a figura o lápis |icone_lapis_workflow|, para que o usuário entre/edite as informações necessárias para execução do script/playbook. Neste momento a Plataforma uCloud irá apresentar uma janela pop up para que o usuário entre com a informação desejada, conforme o exemplo abaixo:

.. figure:: /figuras/ucloud_workflows009b.png
   :alt: Logo uCLoud
   :scale: 50 %
   :align: center

----

A Plataforma uCloud permite ao usuário adicionar a quantidade de campos desejados e suas tags/etiquetas para a execução de uma Tarefas Associada. Adicionalmente permite que o usuário configure quais tags/etiquetas são obrigatórias seu preenchimento, ou personalizar com um conteúdo inicial que será assumido como padrão/default.

Catálogo de Serviços
====================

Acabamos de descrever um exemplo de uso da nova funcionalidade de workflow, e podemos verificar que esta funcionalidade demanda que o usuário provisione cada fluxo individualmente. Além disto, este usuário necessita possuir, token de acesso ao repositório *Github*, possua conhecimento de criação ou uso de arquivos de scripts/playbooks, programe sua repetição e inclua cada script manualmente como uma Tarefas Associadas.

O Menu catálogo de serviços possibilita que o usuário com perfil de Administrador do Contrato, provisionar um catálogo que inclua um ou vários “produto(s)/serviço(s)” pré-formatado(s), e vincular um custo/valor para cada um de forma individual.

Após o provisionamento de todos os serviços do catálogo da empresa, os usuários poderão adquirir o serviço/produto desejado já sabendo o seu valor final. O provisionamento do serviço/produto será executado de uma forma automatizada sem que usuário que necessite adquirir o produto/serviço, tenha que navegar telas da Plataforma uCloud para efetuar o correto provisionamento de recursos computacionais de qualquer provedor de serviço de nuvem pública e/ou privada.

Cada provedor de serviço de nuvem tem sua sequência específica para o correto provisionamento de recurso computacional em seu ambiente. O Catálogo de Serviços é provisionado considerando a sequência correta para entregar o serviço/produto de forma ideal.

Um grande vantagem adicional, é que o Administrador do Contrato, pode incluir dentro do ‘produto/serviço’ a execução de script(s)/playbook(s) que efetue(m) determinadas tarefas complementares ao provisionamento do recurso computacional (por ex: Provisionar nova máquina virtual e incluir um script para validação das regras de segurança e instalação do Tomcat, listar e documentar todos os pacotes e softwares instalados na máquina virtual).

Esta nova funcionalidade pode ser visualizada como uma forma de “esteira de serviços” pois executa todas as atividades necessárias para o correto provisionamento de recursos computacionais, em qualquer provedor de serviço de nuvem, sem que o usuário que deseja adquirir o produto/serviço tenha qualquer conhecimento da console do provedor de serviço, ou tenha qualquer nível de certificação no respectivo provedor de serviço de nuvem ou em script(s)/playbook(s).

Aplicamos o conceito de Carrinho de Compras, pois quando o usuário seleciona o(s) produto(s)/serviço(s), este usuário pode ter o conhecimento prévio do valor inicial do(s) custo(s) de sua(s) decisão(ões). Mencionamos o termo valor inicial, pois este se refere somente ao valor do provisionamento da existência dos recursos computacionais;  os valores de manutenção destes recursos será apresentado na fatura mensal no menu Financeiro da Plataforma uCloud.

Esta nova implementação do Catálogo de Serviços levou a Plataforma uCloud muito mais adiante no conceito de ser uma Plataforma de Auto-Serviço de Nuvem, pois permite que qualquer usuário (com ou sem conhecimento do ambiente do provedor de serviço de nuvem) possa ele mesmo consumir/provisionar recursos computacionais de forma independente e autônoma sem a assistência de um profissional certificado no ambiente do provedor de serviço de nuvem.

Catálogo de Serviço - Cenário Exemplo
-------------------------------------

Quando o usuário acessar o menu Catálogo de Serviço ele irá ser apresentado a lista de Serviços que foi definida pelo usuário Administrador do Contrato. Abaixo vemos uma tela de exemplo de um usuário navegando nas opções do Catálogo de Serviço disponível para visualização deste usuário.
 
.. figure:: /figuras/ucloud_catalogoservico001.png
   :alt: Logo uCLoud
   :align: center

----

Podemos visualizar que existem diferentes produtos/serviços para este usuário, e este usuário pode adquirir o provisionamento de uma máquina virtual no provedor Google (GCP) ou na Amazon Web services (AWS), de forma separada ou optar que a Plataforma uCloud efetue o provisionamento de máquinas virtuais de forma simultânea em ambos os provedores (ex: Instâncias GCP e AWS - *Valor R$ 764,33*).

Outro exemplo é o provisionamento de uma máquina virtual com Linux no provedor AWS e com a instalação do software Tomcat (*Valor de R$ 274,00*).

Para o usuário adquirir um produto, este deve clicar no botão Visualização, e a Plataforma uCloud apresenta a configuração do produto/serviço provisionado:
  
.. figure:: /figuras/ucloud_catalogoservico004.png
   :alt: Logo uCLoud
   :align: center

----

Ao usuário ele pode tanto aceitar as informações padrão ou pode personalizar as informações de acordo com sua demanda, nos campos da seção Configurações Globais, veja o detalhe abaixo:
  
.. figure:: /figuras/ucloud_catalogoservico004b.png
   :alt: Logo uCLoud
   :align: center

----

Após customizar com as informações desejadas, o usuário final deve clicar com o cursor do mouse sobre o botão **Adicionar ao Carrinho** |botao_adicionacarrinho|.

Podemos verificar que este produto/serviço deste catálogo, necessita que o usuário informe os nomes dos recursos: Par de Chave, Grupo de Segurança e Nome da Máquina Virtual. O usuário pode assumir os valores que já foram fornecidos ou alterar para os que sejam adequados para sua demanda.

Neste momento, a Plataforma uCloud adiciona este produto/serviço ao seu *carrinho* de pedidos para que o usuário final possa avaliar se os valores do provisionamento inicial estão adequados ao seu orçamento (budget).

Aplica-se aqui o conceito de Governança Financeira, controlando assim a forma como os usuários consomem recursos computacionais de nuvem. A aplicação de regras de Governança Financeira é um dos principais desafios das empresas atualmente.

Quando o usuário clicar no botão **Finalizar Pedido**, a Plataforma uCloud apresenta uma tela que lista todos os itens de seu carrinho para ele revisar e aceitar/fechar o pedido, conforme o exemplo abaixo:

.. figure:: /figuras/ucloud_catalogoservico004c.png
   :alt: Logo uCLoud
   :align: center

----

A Plataforma uCloud inicia a esteira (sequência) de provisionamento da máquina virtual do usuário após o usuário clicar com o cursor do mouse sobre o botão **Finalizar Comprar**.

O usuário poderá acompanhar cada etapa da execução da esteira do provisionamento do recurso computacional do seu pedido no menu **Tarefas**, desde seu princípio até o momento do final da execução do script/playbook da instalação do Tomcat nesta máquina virtual.

Com esta nova funcionalidade pode-se comprovar o elevado nível em que atingimos para nos tornar uma **Plataforma de Auto Serviço** de recursos de nuvem, com um alto nível de **esteira de automação** com algumas vantagens:

* O usuário não possui credencial na nuvem do provedor (*Governança de Identidade*), pois a é a Plataforma uCloud que está conectada com o console do provedor.
* O usuário não possui liberdade para consumir qualquer tipo de recurso no provedor de nuvem (*Governança de Recursos*).
* O usuário fica limitado aos valores estabelecidos para suas credenciais na Plataforma uCloud (*Governança de Cota de Usuário*)
* O usuário consome somente os produtos/serviços presentes em seu catálogo (*Governança de Operação*)

O custo mensal que decorre da existência deste recurso de máquina virtual, será apresentado na Fatura Mensal visualizada no menu **Financeiro**.

Perfil de Permissionamento
==========================

O Perfil de Permissionamento existe na Plataforma uCloud, desde suas versões iniciais.

Com a implementação do Switch Roles, a uStore atualizou e ampliou o alcance da funcionalidade **Perfil de Permissionamento**, para as novas versões da Plataforma uCloud.

O Perfil de Permissionamento é um conjunto de permissões pré-definidas que podem ser aplicadas aos contratos, aos grupos e aos usuários. Agora permite uma maior granularidade na gestão de permissões que um usuário específico possua para cada Contrato/Nuvem.

Um usuário que alterna entre contratos diferentes (Switch Roles), por exemplo, pode ter níveis de permissão diferentes para cada contrato (ou provedor de nuvem) diferente.

Usando o exemplo do usuário **Josué**, descrito no Switch Roles acima, podemos definir que este usuário tenha níveis de permissões diferentes que estão vinculadas ao contrato de AWS e de Azure.

Antes do *Switch Roles*, o usuário herdava inicialmente um conjunto de permissões que estavam vinculadas a um contrato. Adicionalmente, existe a possibilidade de um grupo de permissões vinculadas ao grupo ao qual este usuário está vinculado. E ainda existe a possibilidade de agregar/editar novas permissões para o usuário individualmente.

Mas as permissões definidas no nível do usuário, que possui um nível de granularidade mais alto que as permissões do Grupo; as permissões do Grupo tem um nível de granularidade mais alto que as permissões do contrato. Mas a *Permissão* precisa estar presente no conjunto de permissões que existem no contrato, caso contrário, o usuário não tem como receber (herdar) uma permissão que não exista no contrato ou no grupo.

Esta granularidade permitia atender a diversas configurações, mas tornava o gerenciamento de permissões um pequeno quebra-cabeça de três níveis (contrato → grupo → usuário).

Nesta visão anterior, teríamos de provisionar duas credenciais de usuário diferentes, e o usuário deveria encerrar a sessão (logoff) com uma credencial e iniciar outra sessão (logon) com outra credencial. 

.. note:: Importante mencionar que esta forma ainda está ativa na Plataforma uCloud, para manter a coerência da base instalada de clientes existentes, que não necessitam das novas facilidades do Perfil de Permissionamento.

A atualização e redesenho da funcionalidade de Perfil de Permissionamento, permite agora provisionar um grupo de Permissões que permite/habilita determinadas ações para um contrato/nuvem e outro Perfil de Permissionamento que bloqueia/desabilita todas (ou parte) das ações para outro contrato/nuvem.

Agora estes dois Perfis de Permissionamento diferentes, podem ser vinculados ao mesmo usuário e com a nova funcionalidade do Switch Roles, o usuário não necessita encerrar/iniciar (logoff/logon) sua sessão. Basta o usuário alternar entre os contratos aos quais está vinculado (Switch Roles) e a Plataforma uCloud aplica o conjunto de permissões definido no Perfil de Provisionamento para o respectivo contrato.

.. figure:: /figuras/ucloud_perfil_permissionamento_011.png
   :alt: Logo uCLoud
   :align: center

----

Perfil de Permissionamento - Cenário Exemplo
--------------------------------------------

Na figura abaixo podemos visualizar que o usuário Mariah, João e Carlos pertencem a somente um único contrato e este contrato possui somente um único provedor (ex: AWS) e todos. Apenas para listras o nosso exemplo, estes usuários não têm acesso ao contrato/nuvem Azure, e portanto possuem somente um único Perfil de Permissionamento vinculado a suas credenciais de acesso a Plataforma uCloud.

.. figure:: /figuras/ucloud_arquitetura_conceitual001.png
   :alt: Logo uCLoud
   :align: center

----
  
O usuário Josué está vinculado a dois contratos diferentes e possui a capacidade de efetuar Switch Roles entre estes dois contratos.

Ainda para ilustrar este exemplo, com a nova implementação de Perfil de Permissionamento, seria possível criar diferentes conjuntos de permissões e vincular cada conjunto (Perfil de Permissionamento) a cada usuário e provisionar um nível de granularidade bem específico.

Cenário exemplo (AWS):
++++++++++++++++++++++

+-------------------------------+-----------+--------------------+------------+
| Perfil de Permissionamento    | Usuário   | Virtual Datacenter | Permissão  |
+===============================+===========+====================+============+
| AWS DevOps Full               | Maria     | DevOps             | Full       |
+-------------------------------+-----------+--------------------+------------+
|| AWS DevOps RO                ||          || DevOps            || Read Only |
|| AWS Homolog Full             ||  João    || Homolog           || Full      |
+-------------------------------+-----------+--------------------+------------+
| AWS Homolog Full              | Carlos    |  Homolog           | Full       |
+-------------------------------+-----------+--------------------+------------+
| AWS Infra Full                | Josué     | Infra              | Full       |
+-------------------------------+-----------+--------------------+------------+

Atualmente é possível provisionar quatro (04) Perfis de Permissionamento diferentes e vincular cada perfil a um usuário específico. No exemplo da tabela acima, é possível visualizar que o usuário João possui dois conjuntos de permissões diferentes que são específicas para cada conjunto de infraestruturas virtuais (Virtual Datacenter - VDC) que este usuário pode acessar. Vemos que o usuário João tem acesso irrestrito ao VDC Homolog, e somente visualização ao VDC DevOps.

Vejamos o exemplo do usuário **Josué** que possui características diferentes para cada contrato.

Cenário Exemplo (AZURE e AWS):
++++++++++++++++++++++++++++++

+-------------------------------+-----------+--------------------+-------------+
| Perfil de Permissionamento    | Usuário   | Virtual Datacenter | Permissão   |
+===============================+===========+====================+=============+
|| Azure Infra RO               ||          || Infra Azure       || Read Only  |
|| AWS Infra Full               ||  Josué   || Infra AWS         || Full       |
+-------------------------------+-----------+--------------------+-------------+

Este é um exemplo da simplicidade e da transparência que advém da ampliação e alteração do novo Perfil de Permissionamento, que permite vincular conjuntos de permissões diferentes ao mesmo usuário, que estão vinculados a contratos diferentes. Podemos verificar que o usuário *Josué* possui acesso irrestrito (*full*) para a infraestrutura do VDC Infra AWS (Contrato AWS) e acesso apenas leitura (*read only*) para o VDC Infra AZURE (Contrato Azure).

Anteriormente o usuário teria de ter duas credenciais diferentes (ex: ``josue.aws/senhaABC`` e ``josue.azure/senha123``) e efetuar diversas sessões de login diferentes na Plataforma uCloud.

Com a combinação do novo Perfil de Permissionamento em conjunto da funcionalidade Switch Roles será possível aplicar esta mudança de tipos de permissões sem a necessidade de troca do usuário, isso será feito com um através da seleção de contrato e/ou container que este usuário deseja acessar.

Conclusão
=========

Este conjunto de novas funcionalidades e ampliação de conceito de funcionalidades existente é parte integrante da mais recente atualização de versão da Plataforma uCloud (``4.1-switchRoles104``), atende a diversas demandas do mercado e de nossos clientes, com o conteúdo deste documento as o desenvolvimento desta nova versão a Ustore reafirma o compromisso da constante evolução de nossa plataforma e o alinhamento com as necessidades do mercado e de nossos clientes.

.. |icone_lapis_workflow| image:: /figuras/ucloud_icone_edita_workflow.png
.. |botao_adicionacarrinho| image:: /figuras/ucloud_botao_colocacarrinho.png
.. |botao_finalizapedido| image:: /figuras/ucloud_botao_finalizapedido.png
