Mangue.io - Manual do usuário
+++++++++++++++++++++++++++++

.. image:: /figuras/mangue-logo-peq.png
    :alt: Logo Mangue
    :scale: 50 %
    :align: center
=====


Soluções em tecnologia da informação que viabilizam implementar uma arquitetura computacional escalável, sólida e confiável em nuvem híbrida.


====


Apresentação
============

Este documento tem como objetivo explicar a utilização da Plataforma “Mangue.io”, uma plataforma de gestão de ambientes de múltiplos orquestradores de container. 

Neste manual são apresentados os conceitos, as telas, as funcionalidades e os comandos de uso deste produto.


====


Introdução
==========

O Mangue.io é uma plataforma de gestão de ambientes de múltiplos orquestradores de container, que permite a orquestração, a implantação (localização e agendamento) e a operacionalização (execução) de containers de aplicações dentro de um ou mais *clusters* computacionais (público ou privado) ou entre eles.

A plataforma opera em um modelo de *multicloud* híbrido e, dessa forma, permite às organizações total controle, suporte para a sustentação de cópias de segurança (*backup*), replicação e migração de ambientes.
Centrado em uma abordagem ágil, segura e produtiva de entrega contínua de aplicações direcionadas à implantação, aos testes e às atualizações com *downtime* zero e *rollback* de *deployments*.

A Plataforma do Mangue.io suporta a implantação e operacionalização de aplicações baseadas em imagens a partir de um serviço de registro. Além disso, permite também a criação de serviços para as aplicações (internos ou externos ao *cluster* ao qual a aplicação pertence).

====


Acesso à plataforma
===================

O acesso à plataforma é feito através de um site, o usuário deve utilizar um navegador de *Internet*, após inserir o endereço da *URL/link* ele visualiza a tela inicial de apresentação.

Após iniciar uma sessão no navegador escolhido, o endereço/caminho para o acesso a aplicação deve ser preenchido da seguinte forma:

https://<mangueserver_IP_Address>:80

https://mangue_Server_Name.com/

Após inserir o endereço corretamente, a tela de login do usuário é similar a imagem abaixo:



.. image:: /figuras/fig_mangue/001_mangue_login.png
    :alt: Tela de login 
    :scale: 80 %
    :align: center
=====


As credenciais para o login e senha são as mesmas da plataforma uCloud, com a qual a plataforma do Mangue.io está integrada. Todo usuário provisionado no uCloud pode, automaticamente, usar suas credenciais para ter acesso ao Mangue.io.

Após entrar com suas credenciais de acesso (usuário e senha) e efetuar o procedimento de login, uma imagem semelhante pode ser apresentada ao usuário, no caso de existir um *cluster* associado ao contrato do usuário no Mangue.io. 
  

.. image:: /figuras/fig_mangue/002_mangue_tela_inicial.png
    :alt: Tela inicial
    :align: center
=====


A imagem acima, representa um exemplo da tela inicial que o usuário visualiza após entrar com as credenciais válidas para o acesso à plataforma do Mangue.io.

====


Configurações de navegação
==========================

No canto superior direito da plataforma existe um menu de configuração que é identificado por uma engrenagem  |icone_engrenagem|, nele o usuário tem a opção de selecionar qual contrato, *cluster* e/ou em qual *namespace* (áreas de trabalho) deseja ter acesso.

Ao clicar em qualquer um dos campos as informações da tela mudam automaticamente.

.. image:: /figuras/fig_mangue/003_mangue_aba_selecao.png
    :alt: Aba de Seleção da Configuração 
    :scale: 80 %
    :align: center
=====



Ao selecionar um contrato, as opções para seleção de *clusters* são atualizadas, lista apenas os que estão  associados ao contrato selecionado, assim como a permissão que o usuário logado tem nestes *clusters* - corresponde ao nível de permissão que ele tem no contrato do uCloud. 

Os contratos que aparecem nessa parte são apenas os que já possuem algum *cluster* integrado ao Mangue.io, na sequência deste documento a descrição de como integrar e/ou criar um *cluster* na aplicação. Na ocasião da seleção é trocado o *cluster* que a plataforma está se comunicando e as informações da tela são atualizadas para este novo contexto.

No momento que o usuário seleciona o *cluster* e o *namespace* os valores da tela de *Overview* são alterados com os dados específicos da seleção do usuário.

====

Tela inicial
============

A tela inicial de *Overview* apresenta alguns gráficos referentes aos valores de consumo de recursos computacionais específicos da seleção do usuário, o detalhamento dos gráficos segue abaixo:


Gráfico do preço mensal do *cluster*
------------------------------------

Este gráfico de barras, apresenta a evolução do custo referente ao uso da infraestrutura computacional que suporta e executa as aplicações.

No eixo vertical, pode-se acompanhar o valor e, no eixo horizontal, é apresentado o valor referente ao consumo de infraestrutura do dia a dia. É possível selecionar o intervalo de tempo para visualizar o consumo da infraestrutura, podendo visualizar os últimos 7 dias, últimos 30 dias, o mês corrente, o mês anterior, assim como personalizar um intervalo de tempo desejado.

Pode-se observar que os valores flutuam em razão do consumo de recursos da infraestrutura computacional para suportar todas as aplicações (*deployments*) que estão ativas no *cluster* selecionado.
  

.. image:: /figuras/fig_mangue/004_mangue_preco_mensal_cluster.png
    :alt: Preço Mensal do Cluster 
    :scale: 80 %
    :align: center
=====

Este gráfico permite acompanhar a variação do **custo real da infraestrutura** necessária para manter e suportar a execução de um *cluster*, dia a dia. Na área: “Título do gráfico” é possível conhecer o valor total acumulado, até o dia presente.

Estes valores são armazenados em uma base de dados interna da plataforma do Mangue.io, então o usuário pode acompanhar a evolução do valor referente ao consumo dos recursos computacionais para suportar um *cluster* ativo e funcional.

Se o usuário desejar, esta base de dados (“Bilhetador”) pode ser limpa, removendo toda a informação armazenada, de forma a “zerar” todos os valores acumulados. 

Para esta finalidade, o usuário deve clicar sobre o ícone “Lata de Lixo” |icone_lata_lixo_preta|. A plataforma do Mangue.io solicita a confirmação do usuário para esta ação apresentando a tela abaixo:


.. image:: /figuras/fig_mangue/005_mangue_deletar_bilhetador.png
    :alt: Deletar Dados Financeiros do Cluster_Bilhetador
    :align: center
=====


Para o usuário confirmar a ação de excluir todos os dados financeiros (valores) de consumo referente ao *cluster* selecionado na aba “Configuração de Navegação”, basta clicar sobre o botão ``Deletar`` de coloração verde. 

Com esta ação todos os valores de consumo do *cluster* são removidos e é iniciado um novo período de coleta de informações, perdendo-se toda a informação acumulada (a série histórica) do *cluster* selecionado.


Cálculo do valor do consumo do cluster
--------------------------------------

Os valores aqui apresentados são calculados com base no valor/hora de vCPU e Memória RAM que está armazenado na base de dados do Mangue.io.

A Plataforma do Mangue.io armazena o consumo de recursos (CPU e Memória) das aplicações a cada minuto; ao término de uma hora (60 min), armazena o valor total do consumo nestes 60 minutos. Ao final de cada dia (24 horas) a Plataforma do Mangue.io armazena o valor referente ao consumo de recursos computacionais, para manter todas as aplicações ativas em cada container.

O preço de CPU e Memória utilizado é o mesmo preço dos recursos do contrato, o valor é definido por meio do uCloud, o preço do contrato pode ser visualizado no Mangue por meio da tela **Permissões / Contrato**:

.. image:: /figuras/fig_mangue/005.1_mangue_formula.png
    :alt: Fórmula mangue.io
    :scale: 80 %
    :align: center
=====


Ao final de cada ciclo de 24 horas, o valor total de consumo dos recursos computacionais é armazenado na base de dados da Plataforma do Mangue.io e apresentada anteriormente no gráfico: Preço Mensal do *Cluster*.


Gráfico do uso total de CPU
---------------------------

Nesta tela, também é possível visualizar o uso de CPU, em MiliCores, de cada recurso *kubernetes*, para isso, o usuário tem que  especificar o *namespace* e os recursos que deseja visualizar o consumo de CPU, e clicar no ícone "Lupa" |icone_lupa_vermelha| para realizar a busca, retornando os últimos trinta minutos de consumo de CPU e Memória.
  

.. image:: /figuras/fig_mangue/006_mangue_uso_total_cpu.png
    :alt: Uso Total de CPU
    :align: center
=====


Gráfico do uso total de memória
--------------------------------

Ao realizar a busca do item Gráfico do uso total de CPU, a plataforma recupera as informações do valor do consumo de memória, em *MegaBytes*, dos últimos trinta minutos de consumo da memória correspondente ao *namespace* e recurso selecionado.
  

.. image:: /figuras/fig_mangue/007_mangue_uso_total_memoria.png
    :alt: Uso Total de Memória
    :align: center
=====


Menu do usuário
===============

A barra de menu do usuário fica localizada à esquerda da tela e, inicialmente, é apresentada no modo expandido, como na figura abaixo.
  

.. image:: /figuras/fig_mangue/008_mangue_menu_usuario_expandido.png
    :alt: Menu Usuário (Modo Expandido) 
    :align: center
=====


Algumas opções de menu possuem um submenu, que são apresentadas quando o usuário posiciona o mouse sobre a indicação (sinal de menor que “<”). Ao clicar sobre este ícone |icone_sinal_menor|, a interface apresenta o submenu desta opção ao usuário, veja o exemplo na figura abaixo.
  

.. image:: /figuras/fig_mangue/009_mangue_submenu_workload.png
    :alt: Exemplo de um Submenu
    :scale: 80 %
    :align: center
=====


Workloads
=========

Nesta opção do menu de usuário *Workloads* o seu *dashboard* apresenta as informações sobre *Deployments*, *Daemonsets*, Horizontal *Autoscaler*, *StatefulSets* e os *Updates*.
  

.. image:: /figuras/fig_mangue/013_mangue_submenu_workload.png
    :alt: Menu Workloads 
    :scale: 80 %
    :align: center
=====


Um **Deployment** é um objeto do *Kubernetes*, orquestrador utilizado pelo Mangue.io, que nada mais é do que um controlador de implantação que fornece atualizações declarativas para outros dois objetos *Kubernetes*: *Pods* e *ReplicaSets*.

Os **Pods** são as menores unidades lógicas (computacionais) implantáveis que podem ser criadas e gerenciadas a partir do Mangue.io. *ReplicaSet* tem por objetivo manter um conjunto estável de réplicas de *Pods* em execução a qualquer momento.

O **StatefulSet** é o objeto da API de carga de trabalho usado para gerenciar aplicações no estado. Ele é o responsável por gerenciar a implantação e o dimensionamento de um conjunto de *Pods* e fornece garantias sobre a ordem e a exclusividade deles.

Os **Daemonsets** gerenciam grupos de *pods* replicados. No entanto, *DaemonSets* tenta aderir a um modelo de um *pod* por 'nó', seja em todo o *cluster* ou em um subconjunto de 'nós'. À medida que você acrescenta 'nós' (*nodes*) a um *cluster*, os *DaemonSets* automaticamente adicionam os *pods* aos novos 'nós', conforme necessário.

O **Autoescalador Horizontal** dimensiona automaticamente o número de *pods* em um controlador de replicação, conjunto de réplicas ou conjunto com estado com base na utilização de CPU observada (ou com suporte às métricas personalizadas, em algumas outras métricas fornecidas pelo aplicativo). Observe que o escalonamento automático horizontal de *pod* não se aplica a objetos que não podem ser escalados, por exemplo, *DaemonSets*.


====

Deployments
-----------

O menu *Workload/Deployments* apresenta todos os *deployments* de um *cluster* em um determinado *namespace*.

Um **Deployment** é um objeto do *Kubernetes*, orquestrador utilizado pelo Mangue.io, que nada mais é do que um controlador de implantação que fornece atualizações declarativas para outros dois objetos *Kubernetes*: *Pods* e *ReplicaSets*.
  


.. image:: /figuras/fig_mangue/014_mangue_workloads_deployments.png
    :alt: Workloads_Deployments
    :align: center
=====


Na tabela são apresentadas as seguintes colunas com suas respectivas informações: 

* **# coluna acionável**: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável |uCloud_icone_coluna_acionavel|. Quando o usuário seleciona uma linha ou várias, a plataforma do Mangue.io apresenta o(s) ícone(s) acima desta coluna, eles representam ações ao usuário para serem executadas de uma única vez em todas as linhas selecionadas. Neste caso são apresentados três ícones com ações bem distintas:

     * **Reversão** |icone_reversao|: Esta opção permite ao usuário efetuar a ação de reverter a atual versão do(s) *deployment(s)* selecionado (s) para sua versão imediatamente anterior à existente na Plataforma do Mangue.io; 
   
     * **Escalar** |icone_escalar|: A função desta ação permite ao usuário informar o número (inteiro) desejado para incrementar o número de réplicas da aplicação (*deployment*);

     * **Lata de lixo** |icone_lixo_vermelho|: Ação que permite ao usuário remover todos os itens selecionados com um único comando;

     * **Alterar versão** |icone_alterar_versao|: Esta opção permite atualizar múltiplos *deployments* de uma vez, ao qual o usuário pode informar a próxima versão de cada um deles;

* **Deploys**: É a representação do nome do *deployment.d*;

* **Labels**: São os identificadores dos *deployments*, usados para ser o elo-de-ligação a um serviço;

* **Instâncias**: Apresentada a quantidade de réplicas que estão operacionais de um *deployment*, e pela quantidade total de réplicas operacionais desejadas para este *deployment*. Estão divididos por uma barra (“/”) onde os valores encontrados antes da barra são as réplicas operacionais, e os valores após a barra representam a quantidade esperada de réplicas operacionais;

* **Status**: O status de um *deployment* identifica seu estado atual. Podem ser apresentados como *Running*, *Pending* ou “*!*” (ponto de exclamação);

     * O *status* **Running** identifica que nenhum erro está acontecendo com o *deployment*;

     * O *status* **Pending** identifica algum estado de transição no *deployment*. Seja por atualização, inicialização do processo do container ou qualquer atividade que identifique um estado de transição;

     * O *status* **!** (ponto de exclamação) identifica um alarme, em outras palavras, que algo errado aconteceu com o *deployment* e suas réplicas. Por exemplo: a imagem de um container é passada com uma versão inexistente, logo, o *download* deste container não ocorre;

* **IP de acesso**: Caso o *deployment* tenha um serviço associado é nesse campo onde o IP do balanceador de carga pode ser um serviço do tipo *loadbalancer*; porta para acesso ao serviço caso seja um serviço externo (tipo *nodePort*) ou a *string* “IP interno” caso seja um serviço interno do cluster (tipo *ClusterIP*);

* **Imagem e Versão**: Caso tenha mais de uma imagem ou versão de um container são listados um abaixo do outro, como no exemplo do 6º *deployment* listado na imagem da tabela de *deployment*;

* **Ações**: A última coluna apresenta um *dropdown* para o menu de ações que podem ser feitas nos *deployments*:


.. image:: /figuras/fig_mangue/015_mangue_dropdown_menu_acoes.png
    :alt: Dropdown Menu_Ações
    :align: center
=====


A. **Adicionar Persistent Volume Claim**

Aplicações que são executadas em containers guardam seus dados em memória, e os containers e *pods* que são executados pelo *Kubernetes* podem eventualmente morrer, o que impacta na perda dos dados guardados em memória. Caso um usuário tenha informações sensíveis para persistir, tais como volumes de banco de dados, deve-se criar um *PersistentVolumeClaim*.

 

.. image:: /figuras/fig_mangue/016_mangue_add_pvc.png
    :alt: Adicionar_PersistentVolumeClaim
    :align: center
=====


Nesta tela o usuário deve preencher os campos com as seguintes informações:

* **Nome:** Informar o nome do volume que se deseja criar;

* **Tamanho:** O usuário deve preencher um número inteiro que representa o tamanho do arquivo de volume que se deseja criar.

* **Unidade de Tamanho:** O usuário deve selecionar a unidade de tamanho que é utilizada para criar o volume. As opções são:

     * **Kilo**: *Kilobytes* quando o usuário deseja criar um arquivo com o valor anterior multiplicado por 1.000;

     * **Mega**: *Megabytes* quando o usuário deseja criar um arquivo com o valor anterior multiplicado por 1.000.000;

     * **Giga**: *Gigabytes* quando o usuário deseja criar um arquivo com o valor anterior multiplicado por 1.000.000.000;

     * **Tera**: *Terabytes* quando o usuário deseja criar um arquivo com o valor anterior multiplicado por 1.000.000.000.000;

     * **Peta**: *Petabytes* quando o usuário deseja criar um arquivo com o valor anterior multiplicado por 1.000.000.000.000.000;


.. attention:: A Plataforma do Mangue.io não valida, previamente, se existe o espaço em disco disponível, no tamanho informado. Ao usuário não é apresentado nenhum aviso, caso o ambiente computacional não disponha o espaço necessário, também não é apresentada nenhuma mensagem de erro no momento da criação deste volume persistente com as características informadas.
	

.. note:: O usuário pode verificar uma indicação de erro, na coluna **Status** na tela do menu *Workloads / Deployments* e consultar o *deployment* específico, ao qual o *PersistentVolume* está associado, conforme a imagem anterior exibida no tópico *Deployments*.
	

* **StorageClass:** O usuário deve selecionar qual o volume de *NFS Storage* estão disponíveis na lista apresentada;

* **Modo de Acesso:** Esta coluna apresenta a configuração de acesso a este volume, esses modos de acesso podem ser três, são eles:

     * **ReadWriteOnce:** O volume é montado e pode receber instruções de leitura e escrita apenas de um único *node*;

     * **ReadOnlyMany:** O volume é montado e tem permissão apenas de leitura, mas de diferentes *nodes* simultaneamente, não sendo permitida a escrita;

     * **ReadWriteMany:** O volume é montado e pode receber instruções de leitura e escrita simultaneamente, mas de diferentes *nodes*;

* **Container:** Quando o usuário clicar sobre este local, é apresentado o nome do container da aplicação com um símbolo semelhante a este |uCloud_icone_coluna_acionavel|;

* **Mount Path:** É o caminho onde o volume é montado no container. Se a base da aplicação é um ambiente Linux o caminho de montagem do volume, deve utilizar a notação do sistema operacional correspondente ao ambiente; se a base do ambiente da aplicação é um ambiente MS-Windows, deve-se utilizar a notação de montagem de volume com as pastas do sistema operacional correspondente;

Para confirmar todos os valores e opções informados, basta o usuário clicar com o mouse no botão ``Finalizar`` para criar o *PersistentVolume* e aguardar o *feedback* de criação, no canto superior direito da tela da Plataforma Mangue.io.



B. **Adicionar Serviço**

A segunda opção deste submenu permite que o usuário possa adicionar um serviço, ao ser clicado abre a seguinte tela de interface modal:
  

.. image:: /figuras/fig_mangue/017_mangue_add_servico.png
    :alt: Adicionar Serviço_Deployment
    :align: center
=====



Nesse modal, o usuário deve preencher os seguintes campos:

* **Nome do serviço**: O usuário deve preencher com o nome do serviço que ele deseja criar;

* **Labels do deployment**: O usuário deve informar as que são associadas a este serviço;

* **Tipos de acesso ao serviço**: Interno, Externo ou *LoadBalancer*:

     * **Interno**: São os serviços que só podem ser acessados de dentro do *cluster*;

     * **Externo**: Corresponde a serviços que possibilitam o acesso de fora do cluster. É fornecida uma porta TCP-IP entre 30.000 –– 32.767;

     * **LoadBalancer**: São integrados diretamente com os *Cloud Providers* (AWS, AZURE, GOOGLE) criando um *loadbalancer* LAYER 7 para o respectivo app;

* **Porta de entrada**: Informar o número da porta TCP-IP do container alocada para a entrada no serviço;

* **Porta de destino para o serviço**: Informar a porta TCP-IP de entrada no container, o serviço vai receber a requisição na porta de entrada e repassar para a porta de destino;

* **Selecionar o protocolo**: TCP ou UDP;

* **Botão** ``Adicionar``: Caso o serviço necessite expor mais de uma porta, o usuário deve retornar para a Porta de Entrada/Porta Destino, e adicionar quantas portas de entrada/saída forem necessárias.

Para confirmar todas as opções acima informadas, o usuário deve clicar com o mouse no botão ``Criar Serviço`` e aguardar o *feedback* de criação.

====

C. **Deletar Deployment**

A terceira opção deste submenu permite que o usuário possa apagar definitivamente um *Deployment* do *cluster* e do *namespace* que foi selecionado na aba **Configurações**; ao ser clicado, abre a seguinte tela de interface modal solicitando a confirmação por parte do usuário:

.. image:: /figuras/fig_mangue/018_mangue_deletar_deployment.png
    :alt: Deletar Deployment 
    :scale: 80 %
    :align: center
=====

Esta ação é imediata e irreversível, a Plataforma do Mangue.io remove o *deployment* selecionado pelo usuário do contrato / *cluster / namespace*.

Basta o usuário clicar sobre o botão ``Deletar`` para confirmar a sua ação e a Plataforma do Mangue.io apaga o *deployment* do ambiente selecionado.


.. note:: Esta ação **não** remove qualquer componente adicional externo a este *deployment* – por ex: um *PersistentVolume* associado, portanto se existe um arquivo externo, este  continua existindo no volume destino. Esta ação apenas remove o *deployment* do ambiente, mas não remove nenhum outro arquivo adicional do ambiente computacional.

====	

D. **Editar Deployment**


Algumas informações não são passíveis de edição através dos formulários do Mangue.io. Elementos, como por exemplo: 

   * Porta do container; 
   * Adicionar alguma variável de ambiente; 
   * Remover alguma variável de ambiente.  

No atendimento de todas as demandas de edição para um *Deployment*, é possível editar diretamente o *YAML* do *Deployment* na plataforma do Mangue.io.

Esta opção apresenta como exemplo a imagem: Editar *Deployment*. O seu conteúdo representa o arquivo.JSON com todas as configurações do *deployment* no *Kubernetes*, o usuário pode editar o que for necessário, confirmar pressionando no botão ``Editar`` e esperar o *feedback* da ação pela Plataforma do Mangue.io.

Essa funcionalidade atende aos usuários que tenham conhecimento no formato dos arquivos do *Kubernetes*.
  

.. image:: /figuras/fig_mangue/019_mangue_editar_deployment.png
    :alt: Editar Deployment
    :align: center
=====


      
E. **Alterar Tags**

A função desta tela permite ao usuário alterar as *Tags* associadas à aplicação selecionada. A partir dela, é possível criar uma *Tag*, ao clicar no ícone adicionar |icone_adicionar| para ser associada à aplicação. 


.. image:: /figuras/fig_mangue/019.1_mangue_alterar_tag.png
    :alt: Alterar Tags 
    :scale: 80 %
    :align: center
=====

.. important:: Para criar uma *Tag* é necessário especificar sua chave e valor.

.. image:: /figuras/fig_mangue/019.2_mangue_criar_tag.png
    :alt: Criar Tag 
    :scale: 80 %
    :align: center
=====

 

F. **Escalar Deployment**

A função desta tela permite ao usuário informar o número (inteiro) desejado para incrementar o número de réplicas da aplicação (*deployment*), as quais são iniciadas automaticamente após a confirmação com o clique do mouse sobre o botão ``Escalar``.

.. image:: /figuras/fig_mangue/020_mangue_escalar_deployment.png
    :alt: Escalar Deployment
    :align: center
=====

Importante ressaltar que há um aumento de consumo no uso de CPU e da memória do *cluster* para suportar a execução simultânea das réplicas desta aplicação na infraestrutura do *cluster*.

====


G. **Migrar Deployment**


Na sexta opção do menu de ações do *Deployment*, há a opção migrar o *deployment* entre diferentes *clusters* configurados na Plataforma do Mangue.io.

O usuário deve selecionar para qual *cluster* integrado ao Mangue.io deseja migrar o *deployment* escolhido.

O campo de *cluster* destinatário é do tipo *“dropdown list”*, quando o usuário clicar sobre este, é apresentado a lista dos *clusters* disponíveis associados ao contrato escolhido no menu de configuração.

Para efetuar a migração, basta o usuário clicar sobre o botão ``Migrar`` e aguardar o *feedback* da ação pela Plataforma do Mangue.io. Como resultado desta ação, é apresentado um alerta de "Sucesso", no menu superior direito da tela.


.. image:: /figuras/fig_mangue/021_mangue_migrar_deployment.png
    :alt: Migrar Deployment
    :align: center
=====


H. **Modificar Versão**


Após clicar em “Atualizar Versão da Aplicação” a plataforma apresenta a imagem "Atualizar Versão de *Deployment*". Por meio deste controle, o usuário pode gerar uma “nova versão” para qualquer *deployment* existente na Plataforma do Mangue.io.


.. image:: /figuras/fig_mangue/022_mangue_atualizar_deployment.png
    :alt: Atualizar versão de Deployment 
    :scale: 80 %
    :align: center
=====

Este campo é alfanumérico e o usuário pode entrar com a informação desejada para identificar a nova versão do *deployment* selecionado. As novas versões são de controle único do usuário, pois se referem às ofertas criadas por este usuário.

Após preencher com a informação desejada, o usuário deve clicar sobre o botão ``Enviar`` para confirmar a ação de criar a versão para o *deployment*.


.. attention:: Estas novas versões não estão relacionadas, necessariamente, com qualquer versão dos *softwares* que as compõem, ou qualquer *software* que foi utilizado para compor a oferta, versões diferentes podem ser encontradas fora da plataforma do Mangue.io.

====


J. **Rollback**

Esta opção permite ao usuário efetuar a ação de reverter a versão do *deployment* para sua versão imediatamente anterior à existente na Plataforma do Mangue.io.

Esta ação em particular não ativa qualquer tela adicional para confirmação, sua ação é imediata.

.. important:: 	Ao selecionar esta opção, a Plataforma do Mangue.io efetua a ação de reversão da versão de forma imediata, sem solicitação de nenhuma confirmação por parte do usuário.

.. note:: Recomenda-se cautela e atenção, pois esta ação cria algum tipo de baixa performance ao *deployment* em que está sendo efetuada a ação de rollback.

====	

Informações do Deployment
-------------------------

Se o usuário clicar sobre o nome de um *deployment*, a plataforma do Mangue.io apresenta a tela de detalhes do *deployment*, como mostrado na figura abaixo.

O usuário pode notar que esta tela possui diversas seções, cada uma descrita abaixo respectivamente.
  

.. image:: /figuras/fig_mangue/023_mangue_overview_deployment.png
    :alt: Overview do Deployment
    :align: center
=====


A. **Seção: Deployment Overview**

Esta seção exibe três gráficos, sendo dois de desempenho e um de valor:

   * CPU;
   * Memória;
   * Preço nos últimos 30 dias.

Eles mostram o desempenho de CPU (em *milicores*), o desempenho da Memória (em *megabytes*) e o Preço nos últimos 30 dias, tudo referente ao *deployment* selecionado pelo usuário. A linha vermelha do gráfico de preços indica a tendência do gráfico.

Também são exibidos botões de interação para o usuário, eles podem especificar o período dos gráficos de CPU e Memória.
  

.. image:: /figuras/fig_mangue/024_mangue_consumo_deployment.png
    :alt: Overview do consumo do deployment
    :align: center
=====


B. **Seção: ReplicaSet**


A seção **Replicaset** apresenta uma tabela que lista todos os *replicasets* presentes para um *deployment*, nesta lista mostra informações como:

   * Nome;
   * Quantidade de *pods* disponíveis;
   * Quantidade de *pods* totais num dado momento;
   * Imagem juntamente com a sua versão especificada;
   * Tempo (em dias) desde o momento da criação deste *replicaset*;
   * Um botão com a opção de deletá-la, como mostrado na figura abaixo.
  

.. image:: /figuras/fig_mangue/025_mangue_replicaset.png
    :alt: ReplicaSet
    :align: center
=====


Nesta parte, a plataforma do Mangue.io apresenta as seguintes informações:

* **#**: Número sequencial da *replicaset* nesta lista;

* **Nome**: Esta coluna apresenta o nome da *replicaset*, o usuário pode verificar que o ambiente *Kubernetes* gera nomes únicos para cada *replicaset*;

* **Pods disponíveis**: Esta coluna apresenta a quantidade de *pods* para esta *replicaset*;

* **Pods totais**: Esta coluna apresenta a quantidade total de *pods*, configurados para esta *replicaset*;

* **Imagem:** Esta coluna apresenta a informação do arquivo de imagem utilizada para criar este *deployment*;

* **Duração:** Esta coluna apresenta o total de dias que esta *replicaset* existe, desde o momento da sua criação até o presente dia que o usuário visualiza esta lista.

====


C. **Seção: PODs**

Na seção **Pods** há uma tabela com a listagem de todos os *pods* presentes para o *deployment*, cada um detalha suas informações como: 

   * Nome; 
   * 'Nó' em que está sendo rodado;
   * *Status* atual do *pod*; 
   * Imagem juntamente com sua versão e tempo de vida.
  

.. image:: /figuras/fig_mangue/026_mangue_pods.png
    :alt: PODs
    :align: center
=====


Nesta seção, a plataforma do Mangue.io apresenta as seguintes informações:

* **Nome**: Nome do *deployment* que é estabelecido no momento da criação deste;

* **Nó**: Apresenta o nome do *node Kubernetes* que está executando este *deployment*;

* **Status**: Apresenta o status do *deployment* em seu respectivo *node*. O *status* de um *deployment* identifica o estado atual. Podem ser representados por:

     * **Running** identifica que nenhum erro está acontecendo com o *deployment*;

     * **Pending** identifica algum estado de transição no *deployment*. Seja por atualização, inicialização do processo do container ou qualquer atividade que identifique um estado de transição;

     * **!** (ponto de exclamação)   identifica que algo errado aconteceu com o *deployment* e suas
     réplicas. Por exemplo: Ao ser passada a imagem de um container com uma versão que não existe, o *download* desse container é impraticável, torna-se impossível fazê-lo;

* **Imagem**: Esta coluna apresenta a informação da imagem pública utilizada para a criação deste *deployment*. Esta imagem pode ser encontrada em sites públicos que contenham informações técnicas referentes à aplicação em si, um exemplo é o *Docker Hub* (https://hub.docker.com/);

* **Duração**: Apresenta o tempo (em dias) decorridos desde a criação deste *deployment*;

* **Ações**: Esta coluna apresenta o botão ``Ações`` |icone_acao| ao ser clicado apresenta as ações que podem ser efetuadas sobre cada *pod* listado, como mostra a seguinte figura:
  

.. image:: /figuras/fig_mangue/027_mangue_submenu_pods.png
    :alt: submenu PODs 
    :scale: 80 %
    :align: center
=====


Cada uma das opções deste submenu é detalhada e descrita abaixo:


* **Deletar Pod**: Ao clicar na opção deletar, basta aguardar o *feedback* da ação. Ela gera um alerta de 'Sucesso' ou 'Erro' no menu superior direito. Como primeira escolha existe a deleção do *pod* em questão, ao selecioná-la aparece o seguinte modal:
  

.. image:: /figuras/fig_mangue/028_mangue_deletar_pod.png
    :alt: submenu Ações_Deletar_POD 
    :scale: 80 %
    :align: center
=====


* **Gráfico de Performance**: A segunda opção possibilita ao usuário observar os gráficos de performance de CPU e Memória de cada *pod*, uma vez que se clica nesta opção, a tela abaixo é apresentada ao usuário com os gráficos de consumo de CPU e memória do *pod* selecionado.
  

.. image:: /figuras/fig_mangue/029_mangue_performance_pod.png
    :alt: submenu Performance de um POD
    :align: center
=====


* **Log**: Esta terceira opção permite ao usuário visualizar os *logs* de um determinado *pod* de uma forma semelhante ao que se obtém com uma sessão de emulação de console de terminal SSH. O usuário pode filtrar o número de registros (linhas) que ele gostaria de observar (opções são: 10, 20, 50, 100, 300, 500, 1000, all).

Caso o *Pod* tenha mais de um container sendo executado, há um *dropdown* onde é possível selecionar qual container o usuário deseja visualizar os *logs*, como é mostrado na imagem a seguir:
  

.. image:: /figuras/fig_mangue/030_mangue_log_pods.png
    :alt: submenu Ações_LOG diversos PODs
    :align: center
=====

* **Linha de Comando**: A quarta opção oferece ao usuário executar as linhas de comandos no *prompt* do sistema operacional do *pod*, de uma forma semelhante ao que se obtém com uma sessão de emulação de console de terminal SSH. Essa funcionalidade se estende a um ou mais containers que existam dentro do *pod* em questão. 

.. important:: Para habilitar esta função é necessário acessar o menu Integrações e seguir os passos correspondentes ao *Container Execution*. 
    
Caso o *pod* tenha mais de um container sendo executado existe um *dropdown* que possibilita selecionar o container desejado pelo usuário para executar os comandos, como é mostrado na imagem a seguir:
  

.. image:: /figuras/fig_mangue/031_mangue_comando_pod.png
    :alt: submenu Ações_Linha de Comando Outro POD 
    :scale: 80 %
    :align: center
=====

D. **Seção: Volumes e Segredos**

Nesta seção são listados todos os **Volumes** (arquivos que armazenam dados) ou **Segredos** (arquivos, ou definições de autenticação quando necessários), associados ao *deployment* selecionado.


.. image:: /figuras/fig_mangue/032_mangue_volumes_segredos.png
    :alt: Volumes e Segredos
    :align: center
=====

A plataforma do Mangue.io apresenta as seguintes informações nesta seção:

     * **#**: Esta coluna apresenta o número sequencial do volume ou segredo, exibido nesta lista;

     * **Nome**: Esta coluna apresenta o nome do volume ou segredo (arquivo do sistema operacional) exposto nesta lista;

     * **Tipo**: Esta coluna apresenta qual o tipo do item exibido nesta lista, que pode ser um **volume** ou **segredo**.

=====

E. **Seção: Eventos**

Nesta seção, são listados todos os eventos atrelados a um *deployment*. Eventos esses que podem ser: por alteração na quantidade de *Pods*/Réplicas, mudança na versão dos containers do *deployment* ou qualquer outra mudança no estado deste.
  
 
.. image:: /figuras/fig_mangue/033_mangue_eventos.png
    :alt: Eventos de Deployment
    :align: center
=====

A plataforma do Mangue.io apresenta as seguintes informações nesta seção:

   * **#**: Número sequencial do evento na lista apresentada;

   * **Criado há**: Apresenta o número total em dias, até a presente data, decorridos desde o surgimento do evento na plataforma do Mangue.io;

   * **Tipo**: Descreve o tipo do evento ocorrido, e podem ser listados os seguintes tipos de eventos:

     * **Normal**;

     * **Warning**.


   * **Objeto**: Descreve qual objeto configurado na plataforma do Mangue.io que foi a origem do evento listado. A identificação do tipo de objeto, permite ao usuário identificar esta origem para que este possa ter acesso a ele  e atuar na resolução do evento, através da redefinição deste, ou optar por sua remoção. Seus tipos podem ser alguns dos listados abaixo:

     * *Deployments*;
     * *Daemonsets*;
     * *Horizontal Autoscaler*;
     * *Pods*;
     * *Statefulsets*;
     * *Updates*;
     * Serviços;
     * *Ingress*;
     * *StorageClass*;
     * *PersistentVolumes*;
     * *PersistentVolumesClaim*.


   * **Mensagem**: Nesta coluna a plataforma do Mangue.io apresenta uma lista de mensagens que podem ajudar a identificar o sucesso do evento ou a causa raiz de um potencial problema, desta forma permite ao usuário tomar alguma ação para eliminar a causa raiz do problema ou estar seguro do sucesso deste evento.


     * *Pulled*;
     * *Created*;
     * *Started*;
     * *NoPods*;
     * *FailedGetScale*;
     * *ProvisioningFailed*;
     * *FailedBinding*.

=====


F. **Seção: Autoescalador Horizontal de Pods**

A plataforma do Mangue.io permite que o usuário defina as regras para que a performance do *deployment* seja sempre a melhor possível, e a plataforma do Mangue.io pode aumentar o processamento em paralelo do *deployment*, executar diversas instâncias (réplicas) para garantir que os usuários tenham sempre a melhor experiência de uso possível. 

Vale ressaltar que é necessário existir uma instância do *Kubernetes Metrics Server* ativa e operando no cluster, para a execução do *Horizontal Pod Auto Scaler* ocorrer. Por padrão, a instalação do Mangue.io contempla a instalação do serviço de métricas.

Caso o *deployment* não possua nenhum Auto Escalador Horizontal, a tela se apresenta como o exemplo abaixo:
  

.. image:: /figuras/fig_mangue/034_mangue_autoescalador_inexistente.png
    :alt: Nenhum auto escalador horizontal encontrado
    :align: center
=====

Para que o usuário possa criar uma regra de **Escalador**, basta clicar sobre o ícone do sinal de adição ‘+’ a exemplo da imagem acima, para que seja apresentada a interface onde o usuário configura a(s) regra(s) de como a plataforma deve mensurar o consumo de infraestrutura do *deployment*, para iniciar novas réplicas dentro da infraestrutura computacional para que a performance seja atendida.
  

.. image:: /figuras/fig_mangue/035_mangue_criacao_autoescalador.png
    :alt: Auto Escalador Horizontal_Criação
    :align: center
=====

* **Mínimo de Réplicas**: Informar o valor mínimo de réplicas do *deployment* (obrigatório um número inteiro – por exemplo: 1, 2) que a plataforma do Mangue.io deve manter ativas para a aplicação ter a performance mínima necessária, garantir a otimização da experiência do usuário. O valor mínimo para este campo é ‘um’ (1);


* **Máximo de Réplicas**: Informar o valor máximo de réplicas do *deployment* (obrigatório um número inteiro – por exemplo: 1, 2) que a plataforma do Mangue.io deve iniciar para a aplicação suportar o crescimento da demanda de acesso dos usuários e garantir a otimização da experiência do usuário. O valor máximo para este campo é 'quinze' (15);


* **% Máxima de uso de CPU**: O usuário deve clicar sobre o botão verde com o sinal de adição ‘+’ para a plataforma apresentar o campo onde o usuário informa o valor percentual máximo (obrigatório um número inteiro – ex.: 20, 22, 30) a ser utilizado pelo Mangue.io como limite máximo de alocação de **CPU** para executar as réplicas de um *deployment*. Este número é o limite máximo que a plataforma considera para iniciar a criação e execução de uma nova réplica do *deployment*. O valor máximo para este campo é 'cem por cento' (100%);


* **% Máxima de uso de Memória**: O usuário deve clicar sobre o botão verde com o sinal de adição ‘+’ para a que a plataforma apresenta o campo onde o usuário informa o valor percentual máximo (obrigatório um número inteiro – ex.: 20, 22, 30) a ser utilizado pelo Mangue.io como limite máximo de alocação de recurso de **memória** para executar as réplicas de um *deployment*. Este número é o limite máximo que a plataforma do Mangue.io considera para iniciar a criação e execução de uma nova réplica do *deployment*. O valor máximo para este campo é 'cem por cento' (100%).


É importante ressaltar que ao confirmar o evento de criação de um Auto Escalador Horizontal, há um tempo de espera para que ele apareça em tela. Tempo este decorrente da necessidade do escalador coletar as métricas e tornar-se um objeto ativo no *Kubernetes*.

A definição de ‘Regras de Escalabilidade’ controla o incremento/decremento da quantidade de réplicas da aplicação, e por consequência há aumento/diminuição do consumo de recursos computacionais para executar o maior/menor número de réplicas ativas. Portanto há um aumento/diminuição no valor do custo da infraestrutura, durante o tempo em que as várias réplicas são executadas.

Após a definição, ou no caso de uma regra existente, o usuário vê a tela abaixo:
  
 
.. image:: /figuras/fig_mangue/036_mangue_autoescalador_existente.png
    :alt: Auto Escalador Horizontal - Existente
    :align: center
=====


* **#**: Número sequencial do Auto Escalador Horizontal na lista apresentada;

* **Nome**: Identifica o nome do Auto Escalador criado, e normalmente, deve ser o mesmo nome do *deployment*;

* **Min. Réplicas**: Identifica o parâmetro colocado na definição do Auto Escalador e correspondente ao número mínimo de réplicas que esse escalador mantém ativas para garantir a performance ao *deployment*;

* **Máx. Réplicas**: Indica o parâmetro colocado na definição do escalador, corresponde ao número máximo de réplicas mantidas ativas para garantir a performance do *deployment*;    

* **Número de Réplicas**: Identifica a quantidade de réplicas ativas do *deployment* no presente momento.

* **Utilização de CPU**: Apresenta a regra definida ao auto escalador, para os limites mínimos e máximos de utilização de CPU. Esta regra deve ser interpretada da seguinte forma:

     * O primeiro número é o consumo atual do recurso de CPU;

     * O segundo número é o limite máximo de ocupação de CPU, limite ao qual a Plataforma do Mangue.io **comissiona** (ativa) uma nova réplica do *deployment*.

* **Utilização de Memória**: Apresenta a regra definida ao auto escalador, para os limites mínimos e máximos de alocação de memória. Esta regra deve ser interpretada da seguinte forma:

     * O primeiro número é o consumo atual de alocação do recurso Memória;

     * O segundo número é o limite máximo de alocação de memória, limite ao qual a Plataforma do Mangue.io **comissiona** (ativa) uma nova réplica do *deployment*.

* **Ações**: Esta coluna apresenta o botão ``Ações`` |icone_acao| ao ser clicado exibe as ações que podem ser efetuadas sobre o Auto Escalador Horizontal, existem duas opções, são elas:

     * Deletar autoescalador horizontal de pods;
     * Editar autoescalados horizontal de pods.
  

.. image:: /figuras/fig_mangue/037_mangue_acoes_autoescalador.png
    :alt: submenu Ações_Auto escalador horizontal 
    :scale: 80 %
    :align: center
=====

Ao clicar na opção "Deletar" o usuário confirma a remoção das regras de escalabilidade criadas e estas não são mais aplicadas para o *deployment*. 

.. attention:: Um *feedback* de alerta é criado no canto superior direito da tela, informa o sucesso ou erro.

    
A opção “Deletar” do menu de Ações do Horizontal *Autoscalers* apresenta a tela abaixo:
  
 
.. image:: /figuras/fig_mangue/038_mangue_deletar_autoescalador.png
    :alt: submenu Ações_Deletar auto escalador horizontal
    :align: center
=====

Ao clicar sobre a opção “Editar”, a plataforma do Mangue.io apresenta a tela abaixo, onde é possível o usuário alterar os valores existentes do Auto Escalador Horizontal. A imagem seguinte "Auto Escalador Horizontal – Criação" apresenta opções sobre como alterar os valores. 
  

.. image:: /figuras/fig_mangue/039_mangue_criar_autoescalador.png
    :alt: Regras de Auto Escalador Horizontal_Criação
    :align: center
=====

Importante ressaltar que as regras de Auto Escalador Horizontal acima descritos, estão associadas apenas ao *deployment* selecionado pelo usuário.

Através do menu *Workloads*/Autoescalador Horizontal o usuário pode visualizar todas as regras de Auto Escalador Horizontal, configuradas na plataforma do Mangue.io, associadas aos seus respectivos *deployments.*

====


G. **Seção: Preço da Aplicação no último mês**

Esta seção exibe a tela "Preço da aplicação no último mês", nela são listadas as colunas de moeda, preço por memória, preço por CPU e preço total da aplicação, na sequência cada uma das colunas é detalhada:


.. image:: /figuras/fig_mangue/040_mangue_preço_deployment.png
    :alt: Preço da Aplicação (deployment)
    :align: center
=====

* **Moeda**: Apresenta o nome da moeda corrente referente aos valores apresentados nas colunas desta tabela;

* **Preço por Memória**: Apresenta o valor total, do mês corrente, do consumo do recurso de memória RAM para manter o *deployment* sendo executado (consultar a fórmula de cálculo);

* **Preço por CPU**: Apresenta o valor total, do mês corrente, do consumo do recurso de CPU para manter o *deployment* sendo executado (consultar a fórmula de cálculo);

* **Preço total do APP**: Esta coluna apresenta a somatória das duas colunas anteriores (Preço: Memória e CPU). Com esta informação, o usuário pode avaliar o **custo real da infraestrutura** necessária para manter e suportar a execução de um *deployment* ativo e funcional 24 x 7. 

====


Daemonsets
----------

Esta seção apresenta todos os *Daemonsets* de um *cluster* em um determinado *namespace*, na tabela a seguir temos informações como:
  

.. image:: /figuras/fig_mangue/041_mangue_daemonsets.png
    :alt: Listagem de Daemonsets
    :align: center
=====

* **#:** Número sequencial do *daemonset* na lista apresentada;

* **Nome:** É a representação do nome do *Daemonsets*;

* **Labels:** São os identificadores dos *Daemonsets*, usados para ser o elo que liga a um serviço;

* **Instâncias:** Está representada pela quantidade de réplicas operacionais de um *Daemonsets*, e pela quantidade total de réplicas operacionais desejadas para este *Daemonsets*. Estão divididos por uma barra (“/”) onde os valores encontrados antes da barra são as réplicas operacionais, e os valores após a barra representam a quantidade esperada de réplicas operacionais;

* **Status**: O *status* de um *Daemonsets* identifica o estado atual deste. Podem ser presentados por *Running*, *Pending* ou “*!*” (ponto de exclamação):

     * O *status* **Running** identifica que nenhum erro está acontecendo com o *Daemonsets*;

     * O *status* **Pending** identifica algum estado de transição no *Daemonsets*. Seja por atualização, inicialização do processo do container ou qualquer atividade que identifique um estado de transição;

     * O status **“!”** (ponto de exclamação) identifica quando algo errado aconteceu com o *Daemonsets* e suas réplicas. Por exemplo: Ao ser passada a imagem de um container com uma versão que não existe, o *download* desse container é impraticável, torna-se impossível fazê-lo.

* **IP de acesso**: Caso o *Daemonsets* tenha um serviço associado, é nesse campo onde o IP do balanceador de carga pode ser um serviço do tipo *loadbalancer*, porta para acesso ao serviço caso seja um serviço externo (tipo *nodePort*) ou a *string* “Ip interno” caso seja um serviço interno do *cluster* (tipo *ClusterIP*).

* **Imagem e versão**: Caso tenha mais de uma imagem ou versão de um container são listados um abaixo do outro, como no exemplo do 6º *Daemonsets*, listado na imagem da tabela de *Daemonsets*.

* **Duração**: Apresenta o tempo de duração do *Daemonsets*.

* **Ações**: Esta coluna apresenta o botão ``Ações`` |icone_acao| ao ser clicado exibe as seguintes opções:
  
  .. image:: /figuras/fig_mangue/041.1_mangue_acoes_daemonsets.png
    :alt: Editar e deletar Daemonsets 
    :scale: 80 %
    :align: center
=====


     * **Editar DaemonSets**: Esta opção apresenta o *daemonset* em formato JSON, o usuário pode editar o que for necessário e selecionar a opção de editar e esperar o *feedback* da ação pela Plataforma do Mangue.io.

     * **Deletar DaemonSets**: Ao selecionar esta ação, a plataforma do Mangue.io solicita a confirmação do usuário, como mostra a figura abaixo:
  

.. image:: /figuras/fig_mangue/042_mangue_deletar_daemonsets.png
    :alt: Confirmação para deletar Daemonsets
    :align: center
=====


**Informações do DaemonSet**

Caso o usuário clique sobre o nome de algum *Daemonsets* presente na lista, a plataforma do Mangue.io exibe a tela com as informações de um *Daemonset*, conforme o exemplo abaixo:

.. image:: /figuras/fig_mangue/042.1_mangue_overview_daemonsets.png
    :alt: Overview Daemonsets
    :align: center
=====


Autoescalador Horizontal de Pods
--------------------------------

A plataforma do Mangue.io permite que o usuário defina regras para que a performance da aplicação seja sempre a melhor possível e que o *deployment* possa aumentar o processamento paralelo, diversas instâncias do *deployment* (réplicas), para garantir que os usuários tenham sempre a melhor experiência de uso possível.

A definição de ‘Regras de Escalabilidade’ controla o incremento da quantidade de réplicas de um *deployment*, e por consequência há aumento do valor do custo da infraestrutura, durante o tempo em que as várias réplicas estiverem sendo executadas. Na tabela exibe informações como: 
  

.. image:: /figuras/fig_mangue/043_mangue_lista_autoescalador.png
    :alt: Horizontal Autoscaler
    :align: center
=====

* **# ‘coluna acionável’**: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável |uCloud_icone_coluna_acionavel|. Quando o usuário escolhe uma linha ou várias, a plataforma do Mangue.io apresenta o(s) ícone(s) acima desta coluna, eles representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso é apresentado o ícone "Lata de lixo" |icone_lixo_vermelho| que permite ao usuário remover todos os itens indicados com um único comando;

* **Nome:** Identifica o nome do Autoescalador criado, e normalmente deve ser o mesmo nome do *Deployment*;

     * **Min. Réplicas:** Identifica o parâmetro colocado na hora de criação do escalador correspondente ao número mínimo de réplicas que esse escalador garante  para o *Deployment* que ele está associado;

     * **Máx. Réplicas:** Indica o parâmetro colocado na hora de criação do escalador, corresponde ao número máximo de réplicas mantidas ativas para garantir que o *Deployment* está associado;

     * **Número Atual de Réplicas:** Identifica o estado atual da quantidade de réplicas do *Deployment* ao qual o escalador está associado;

* **Ações:** Esta coluna apresenta o botão ``Ações`` |icone_acao| ao ser clicado, exibe as ações que podem ser efetuadas sobre o Auto Escalador Horizontal, existem duas opções:



.. image:: /figuras/fig_mangue/044_mangue_acoes_autoescalador.png
    :alt: submenu Ações_Auto escalador horizontal 
    :scale: 80 %
    :align: center
=====


No menu "Ações" do Horizontal Autoscaler há a opção de deletar, ao selecioná-la é exibido o seguinte modal:


.. image:: /figuras/fig_mangue/045_mangue_deletar_autoescalador.png
    :alt: Deletar Auto Escalador Horizontal
    :align: center
=====

Ao clicar no botão ``Deletar`` o *Horizontal Autoscaler* é excluído, e as regras de escalabilidade criadas não são mais obedecidas pelo *Deployment* anteriormente associado. 

.. attention:: Um *feedback* de alerta é criado no canto superior direito da tela informando o 'sucesso' ou 'erro'.

====


PODs
----

Um **Pod** do *Kubernetes* é um grupo de containers, implantados juntos, no mesmo *host*.

Os *pods* operam em um nível mais alto do que os containers individuais, porque é muito comum ter um grupo de containers trabalhando em conjunto para produzir um artefato ou processar um conjunto de trabalho.

Por exemplo: 

Para ilustrar o que é um *pod*, por analogia, pode-se utilizar a frase *a pod of whales* que significa "um grupo de baleias" neste caso específico, o termo *pods* relaciona-se ao grupo de baleias. 

.. note:: Um *Pod* é um grupo de um ou mais containers, com armazenamento / recursos de rede compartilhados e uma especificação de como executar os containers. 

O conteúdo de um *pod* é sempre colocado e programado conjuntamente, em seguida, executado em um contexto compartilhado. 

.. important:: Um *pod* modela um "*host* lógico" específico do aplicativo. Ele contém um ou mais containeres do aplicativo que são acoplados de forma relativamente forte.

A plataforma do Mangue.io pode ajudá-lo a criar quantos *pods* forem necessários para o seu ambiente *Kubernetes*, a associação do *Deployment* a um *pod* é descrito em outra seção deste manual, juntamente com a descrição do processo de criação de um *pod*.

 
.. image:: /figuras/fig_mangue/046_mangue_listagem_pods.png
    :alt: Listagem de PODs
    :align: center
=====

A imagem acima exibe a listagem dos *pods* criados, a seguir a descrição com o significado de cada uma das sete colunas desta tela:

* **# coluna acionável**: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável |uCloud_icone_coluna_acionavel|. Quando o usuário seleciona uma linha ou várias, a plataforma do Mangue.io apresenta o(s) ícone(s) acima desta coluna, eles representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso é apresentado o ícone "Lata de lixo" |icone_lixo_vermelho| que permite remover todos os itens indicados com um único comando;

* **Nome**: Nome do *Deployment* que é estabelecido no momento da criação deste;

* **Nó**: Apresenta o nome do *node* Kubernetes que está executando este *Deployment*;

* **Status**: Apresenta o *status* do *Deployment* em seu respectivo *node*. O *status* de um *Deployment* identifica o estado atual. Podem ser representados por:

     * **Running** identifica que nenhum erro está acontecendo com o *Deployment*;

     * **Pending** identifica algum estado de transição no Deployment. Seja por atualização, inicialização do processo do container ou qualquer atividade que identifique um estado de transição;

     * **“!”** (ponto de exclamação) identifica que algo errado aconteceu com o *Deployment* e suas réplicas. Por exemplo: Ao ser passada a imagem de um container com uma versão que não existe, logo, o *download* desse container é impraticável, torna-se impossível fazê-lo;

* **Imagem:** Esta coluna apresenta a informação da imagem pública utilizada para a criação deste *Deployment*. Esta imagem pode ser encontrada em sites públicos que contenham informações técnicas referentes à aplicação em si, um exemplo é o *Docker Hub* (https://hub.docker.com/);

* **Duração:** Apresenta o tempo (em dias) decorridos desde a criação deste *Deployment*;

* **Ações:** Esta coluna apresenta o botão ``Ações`` |icone_acao| ao ser clicado, apresentam as ações que podem ser efetuadas sobre cada *Pod* listado, como mostra a figura abaixo:
  

.. image:: /figuras/fig_mangue/027_mangue_submenu_pods.png
    :alt: submenu PODs 
    :scale: 80 %
    :align: center
=====

Cada uma das opções deste submenu está descrita abaixo:

* **Deletar Pod**: Ao clicar na opção **Deletar** basta aguardar o *feedback* da ação. Que vai gerar um alerta de Sucesso ou Erro no menu superior direito. Como primeira opção temos a deleção do *Pod* em questão, ao selecionar esta opção aparece o seguinte modal:
  

.. image:: /figuras/fig_mangue/028_mangue_deletar_pod.png
    :alt: submenu Ações_deletar POD 
    :scale: 80 %
    :align: center
=====

* **Gráfico de Performance**: Na segunda opção, o usuário é capaz de observar os gráficos de performance de CPU e Memória de cada *Pod*, uma vez que se clica nesta opção, a tela abaixo é apresentada ao usuário com os gráficos de consumo de CPU e memória do *Pod* selecionado.
  

.. image:: /figuras/fig_mangue/029_mangue_performance_pod.png
    :alt: submenu Performance de um POD
    :align: center
=====

* **Log**: Na terceira opção, o usuário é capaz de visualizar os *logs* de um determinado *Pod* de uma forma semelhante ao que se obtém com uma sessão de emulação de console de terminal SSH. O usuário é capaz, também, de filtrar o número de registros (linhas) que ele gostaria de observar (opções são: 10, 20, 50, 100, 300, 500, 1000, all). Caso o *Pod* tenha mais de um container sendo executado há um *dropdown* onde é possível selecionar qual container o usuário deseja visualizar os logs, como é mostrado na imagem a seguir:
  

.. image:: /figuras/fig_mangue/030_mangue_log_pods.png
    :alt: submenu Ações_log diversos pods 
    :scale: 80 %
    :align: center
=====

* **Linha de Comando**: Na quarta opção, o usuário é capaz de executar linhas comandos no *prompt* do sistema operacional do *Pod*, de uma forma semelhante ao que se obtém com uma sessão de emulação de console de terminal SSH. Essa funcionalidade se estende a um ou mais containers que existam dentro do Pod em questão. 

.. important:: Para habilitar esta função é necessário acessar o **Menu Integrações** e seguir os passos correspondentes ao *Container Execution*. 

Caso o *Pod* tenha mais de um container sendo executado há um *dropdown* onde é possível selecionar qual container o usuário deseja executar os comandos, como é mostrado na imagem a seguir:
  

.. image:: /figuras/fig_mangue/031_mangue_comando_pod.png
    :alt: submenu Ações_linha de comando outro pod
    :align: center
=====

Statefulsets
------------

Nesta funcionalidade a plataforma do Mangue apresenta todos os *statefulsets* de um *cluster* em um determinado *namespace*, na seguinte imagem são exibidas informações como:
  

.. image:: /figuras/fig_mangue/048_mangue_statefulsets.png
    :alt: Listagem de Statefulsets
    :align: center
=====

* **# coluna acionável**: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável |uCloud_icone_coluna_acionavel|. Quando o usuário seleciona uma linha ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, eles representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso é apresentado o ícone "lata de lixo" |icone_lixo_vermelho| que permite remover todos os itens selecionados com um único comando;

* **Nome**: É a representação do nome do *Statefulsets*;

* **Labels**: São os identificadores dos *Statefulsets*, usados para ser o elo-de-ligação a um serviço;

* **Instâncias**: Os valores apresentados aqui indicam que a quantidade de réplicas de um *Statefulsets* estão divididos por uma barra (“/”) onde os valores encontrados ao lado esquerdo da barra é o valor de réplicas ativas e operacionais, e os valores ao lado direito da barra representa a quantidade máxima de réplicas que podem ser ativadas para manter a performance desejada do *Statefulsets*;

* **Status**: O status de um *Statefulsets* identifica o estado atual de cada *Statefulsets* listado. Pode ser apresentado por **’Running’**, **’Pending’** ou “**!**” (ponto de exclamação).

     * O *status* **’Running’** identifica que nenhum erro está acontecendo com o *Statefulsets*;

     * O *status* **’Pending’** identifica algum estado de transição no *Statefulsets*. Seja por atualização, inicialização do processo do container ou qualquer atividade que identifique um estado de transição; 

     * O *status* **!** (ponto de exclamação) identifica quando algo errado aconteceu com o *Statefulsets* e suas réplicas. Por exemplo: Ao ser passada a imagem de um container com uma versão que não existe, logo, o *download* deste é impraticável, torna-se impossível fazê-lo;

* **IP**: Caso o *Statefulsets* tenha um serviço associado, é nesse campo onde o IP do balanceador de carga pode ser um serviço do tipo *Loadbalancer*, porta para acesso ao serviço caso seja um serviço externo (tipo *nodePort*) ou a *string* "IP interno” caso seja um serviço interno do *cluster* (tipo *ClusterIp*).

* **Imagem e Versão**: Caso tenha mais de uma imagem ou versão de um container são listados um abaixo do outro, como no exemplo do 6º *Statefulsets* listado na imagem da tabela de *Statefulsets*.

* **Duração**: Esta coluna apresenta o tempo decorrido desde o momento de criação do *Statefulsets*.

* **Ações**: Esta coluna apresenta o botão ``Ação`` |icone_acao| ao ser clicado, exibe duas opções como a figura abaixo:
  

.. image:: /figuras/fig_mangue/048.1_mangue_acoes_statefulsets.png
    :alt: Ações editar e deletar statefulsets
    :scale: 80 %
    :align: center
=====



* **Editar Statefulsets**: Esta opção apresenta uma tela com um arquivo JSON com todas as configurações do *Statefulsets* no *Kubernetes*, o usuário pode editar o que for necessário e selecionar a opção de editar e esperar o *feedback* da ação pela Plataforma do Mangue.io. Essa funcionalidade atende aos usuários que tenham conhecimento no formato dos arquivos do *Kubernetes*.
  

.. image:: /figuras/fig_mangue/049_mangue_editar_statefulsets.png
    :alt: Editar 
    :scale: 80 %
    :align: center
=====

* **Deletar Statefulsets**: No menu de ações do *Statefulsets* há a opção de deletar, basta o usuário clicar sobre o botão para confirmar a ação, conforme mostra a tela abaixo:
  

.. image:: /figuras/fig_mangue/050_mangue_deletar_statefulsets.png
    :alt: mensagem confirmação 
    :scale: 80 %
    :align: center
=====



Updates
-------

Um *Update* é considerado um evento de atualização em um *Cluster Kubernetes*, sua funcionalidade tem o intuito de facilitar o controle e a comunicação direta, entre o ambiente *Kubernetes* e a interface do Mangue.io.


.. image:: /figuras/fig_mangue/051_mangue_update.png
    :alt: Update
    :align: center
===== 

A imagem acima exibe a lista de *updates* criados, a seguir a definição de cada uma das oito colunas:

* **#**: Número sequencial do evento na lista apresentada;

* **Deployment Name**: Indica o nome do *Deployment*;

* **Tipo**: Determina o tipo do *update* a ser realizado, existem dois tipos de atualização possível, são eles:

     * **Atualização** - Ocorre quando o usuário determina qual é a próxima versão e o container do Deployment;

     * **Rollback** - É um operação que reverte o evento para a versão anterior;

* **Status**: Existem dois estados possíveis, são eles:

     * *UPDATED* - Este estado corresponde a uma atualização realizada;

     * *OUTDATED* - Refere-se a um estado anterior ou antigo, que aguarda o evento de atualização através da plataforma do Mangue;

* **Namespace**: Corresponde ao *Namespace* da aplicação a ser atualizada que está sendo executada;

* **Novas Imagens**: Corresponde às novas imagens e versões dos containers que são atualizados;

* **Duração**: Corresponde ao tempo que a atualização foi cadastrada/executada;

* **Ações**: Esta coluna apresenta o botão ``Ação`` |icone_acao| ao ser clicado, exibe uma única opção:
  

.. image:: /figuras/fig_mangue/052_mangue_botao_atualizar.png
    :alt: ação atualizar 
    :scale: 80 %
    :align: center
=====

* **Atualizar**: Ao selecionar a opção atualizar no botão de ``Ações`` da tabela, a plataforma do Mangue.io apresenta uma tela de confirmação para a operação:
  

.. image:: /figuras/fig_mangue/053_mangue_mensagem_atualizar.png
    :alt: mensagem atualizar 
    :scale: 80 %
    :align: center
=====

Ao clicar no botão ``Atualizar`` do modal é disparado o evento de atualização para o Deployment correspondente. 

São utilizadas as imagens e versões dos containers que constam no campo de “Novas Imagens”. Um feedback de alerta é criado no canto superior direito da tela informando o sucesso ou erro.

Logo acima da tabela, existem três elementos com os quais o usuário poderá atuar:
  

.. image:: /figuras/fig_mangue/053.1_mangue_pesquisar_atualização.png
    :alt: Pesquisar atualização 
    :scale: 80 %
    :align: center
=====


                     * **A ação de pesquisa**: Caso a lista de apresentada nesta tela seja muito longa (ocupando mais de uma página), existe um campo onde é possível ao usuário efetuar uma pesquisa pelo nome do Update desejado. Basta informar parte do nome e teclar enter ou clicar sobre o ícone da lupa “  ”. Como resultado dessa busca aparecem apenas os Updates que contém a palavra-chave da pesquisa;

                     * **A ação de atualizar**: Basta clicar no ícone “  ” para que o Mangue.io atualize a interface com os valores mais recentes desta tabela de Updates;

                     * **Criar Integração com Updates**: Basta clicar no sinal de adição “+” para que o usuário possa cadastrar uma nova atualização para um Deployment em um determinado Namespace. A plataforma do Mangue.io apresenta a seguinte tela ao usuário:
  

.. image:: /figuras/fig_mangue/054_mangue_criar_integracao.png
    :alt: Criar integração 
    :scale: 80 %
    :align: center
=====

Segue a descrição dos campos desta tela:

                     * **Token**: Este campo é preenchido com uma string de caracteres após o usuário clicar sobre o botão **“Gerar Token”**, neste momento o campo é preenchido com a string de token que é informado para comunicação com a API do Mangue.io. Este token deve ser salvo e deve ser informado para autenticar as versões do CI. Ao gerar  um token, este deve ser enviado via API para o servidor do Mangue.io, pois ele  é responsável por garantir a integridade da requisição enviada.

                     * **Namespace**: Ao clicar neste campo, é apresentada uma lista (drop-down) com todos os Namespaces existentes no cluster que foi selecionado na aba de Seleção de Configuração.

                     * **Deployment**: Ao clicar sobre campo é apresentada uma lista (drop-down) com todos os Deployments associados ao namespace selecionado do campo anterior.

                     * **Criar**: Quando o usuário estiver configurado, todos os campos desta tela, com os critérios corretos para adicionar um evento de atualização (update), basta clicar sobre o botão “Criar” para adicionar o evento de atualização na plataforma do Mangue.io. Este novo evento é adicionado à lista com o status pending. Ao clicar no botão de "Criar” é criada a permissão para que o usuário cadastre atualizações na plataforma através de chamadas à API do mangue. Um feedback de alerta é criado no canto superior direito da tela informando o sucesso ou erro. Caso o evento não apareça listado, imediatamente, o usuário deve clicar sobre o ícone “  ” (update) para atualizar as informações da tela.


Abaixo listamos alguns exemplos dos benefícios para a funcionalidade de Updates:

**Exemplo 1**:

	Um usuário tem um pipeline de CI/CD que é executado e gera algumas versões estáveis por dia. Dado que o usuário tem seu *cluster Kubernetes* gerenciado pelo Mangue.io e suas aplicações instaladas é possível cadastrar atualizações na plataforma através do pipeline de CI/CD, e esperar que o evento de atualização seja disparado pela interface do Mangue.io.


**Exemplo 2**:

	Um usuário tem um pipeline de CI/CD que é executado e gera algumas versões estáveis por dia. Dado que o usuário tem seu *cluster Kubernetes* gerenciado pelo Mangue.io e suas aplicações instaladas é possível atualizar a aplicação direto pelo pipeline de CI/CD.


====	

Catálogo
========

A Plataforma do Mangue.io permite ao usuário criar aplicações (*Deployments*) de duas formas diferentes. A primeira é uma forma simplificada guiando o usuário por intermédio de telas, que depois de todas preenchidas e confirmada pelo usuário, os dados informados serão convertidos em um arquivo com ‘sintaxe YAML’, e esta sintaxe (praticamente sem erros) será utilizada para gerar a aplicação (ex.: *Deployment*).

O objetivo desta primeira abordagem é minimizar os potenciais erros de sintaxe YAML para um ambiente Kubernetes. A criação de código em sintaxe YAML, para o ambiente Kubernetes, demanda um alto grau de especialização e conhecimento do desenvolvedor para que a sintaxe, correta para o ambiente, tenha todas as dependências necessárias para geração do resultado desejado da forma correta e pronta para o uso no ambiente Kubernetes (ex.: uma aplicação / *Deployment*).

A outra forma é permitir ao usuário fazer o upload de um arquivo texto, cujo conteúdo é a codificação da aplicação em sintaxe YAML, já adaptada e preparada para um ambiente Kubernetes. Se o desenvolvedor (usuário) possui prática suficiente para criar seus próprios scripts em sintaxe YAML, pode utilizar seus próprios scripts e trazer estes para a Plataforma do Mangue.io para gerenciar em qual *Cluster*, *Pod*, *Node*, este código/*script* é executado e gerenciado.

Quando o usuário acessar o menu Catálogo, a Plataforma do Mangue.io apresenta a tela abaixo, e iremos descrever cada uma das opções nas páginas abaixo.
  

.. image:: /figuras/fig_mangue/055_mangue_catalogo.png
    :alt: Catálogo  
    :scale: 80 %
    :align: center
=====



Nova Aplicação
--------------

Esta modalidade é a forma que a Plataforma do Mangue.io conduz o usuário através de telas, solicitando as informações na sequência para que, posteriormente, a Plataforma no Mangue.io faça a compilação das informações gerando a aplicação dentro do *Cluster* e *Namespace* selecionados na aba engrenagens “   Seleção de Configuração”.

Abaixo descreveremos as etapas de preenchimento dos formulários das telas que guiam o usuário.

A. Primeiro Passo: Nova Aplicação
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Para a criação de uma nova aplicação *(Deployment)* a plataforma do Mangue.io segmenta o processo em duas etapas, o usuário deve preencher os seguintes campos:


.. image:: /figuras/fig_mangue/056_mangue_criar_deployment.png
    :alt: Criar deployment 
    :scale: 80 %
    :align: center
=====
  

      * **Nome**: Este campo é obrigatório, e o usuário deve informar o nome da aplicação *(Deployment)* com o qual este fica identificado na Plataforma do Mangue.io;

      * **Réplicas**: Este campo é obrigatório, e o usuário deve informar um número (inteiro), que este deseja alocar para executar a aplicação *(Deployment)* assim que criada. Este número é alocado da infraestrutura computacional para que o usuário obtenha a melhor experiência de performance, e a Plataforma do Mangue.io se encarrega de alocação destes recursos computacionais;

      * **Pesquisar Imagem**: Este campo é obrigatório, este campo efetua uma pesquisa da imagem de uma aplicação no servidor de registro de imagens http://hub.docker.com. O usuário pode informar uma sequência de caracteres (mesmo que parcial) de qualquer imagem catalogada no *Hub Docker*, e a Plataforma do Mangue.io efetua a pesquisa e apresenta uma lista que contém a sequência de caracteres. Veja exemplo abaixo, com pesquisa da sequência “wordp”, para buscar a imagem da aplicação *Wordpress*:
            

.. image:: /figuras/fig_mangue/057_mangue_pesquisar_imagem.png
    :alt: Pesquisar imagem 
    :scale: 80 %
    :align: center
=====

* Basta o usuário clicar com o cursor do mouse na linha da imagem desejada para selecionar a melhor imagem disponível.


      * **Nome do Container**: Este campo é obrigatório, neste campo o usuário deve informar o nome com o qual o usuário pretende identificar este dentro da Plataforma do Mangue.io;

      * **Bloquear execução de usuário privilegiado**: Neste campo o usuário pode bloquear os containers do *Deployment* sejam executados de forma privilegiada, com acesso aos recursos e capacidades *Kernel* da máquina *Host*;

      * **Especificar ID de usuário, grupo ou arquivo de sistema**: Neste campo o usuário pode informar o ID de usuário, grupo ou arquivo de sistema que o container é executado.

      * **Tags da Aplicação**: Neste campo o usuário pode informar as Tags da aplicação. Também é possível criar uma Tag para ser associada à aplicação;

      * **Botão Adicionar**: Para a criação de uma nova aplicação *(Deployment)* a plataforma do Mangue.io segmenta o processo em duas etapas; após o usuário confirmar a ação no botão “Adicionar” o usuário vê a seguinte tela:


.. image:: /figuras/fig_mangue/058_mangue_modal_imagem.png
    :alt: Modal imagem 
    :scale: 80 %
    :align: center
=====

               * **Versão da Imagem**: Este campo é obrigatório neste campo o usuário deve informar como a aplicação *(Deployment)* deve ser identificada no ambiente. Este campo pode ser preenchido com números ou caracteres, para atender a demanda do usuário (Ex.: latest, última, 1.xx, 1.20);

               * **ContainerPort**: Este campo é obrigatório neste campo o usuário deve informar porta TCP-IP do container que deve ser utilizada para que a aplicação *(Deployment)* fique disponível para acesso de outros usuários;

                                       * **Máximo Recurso a ser utilizado [CPU em milicores]**: Neste campo o usuário deve informar o máximo de recursos de CPU que devem ser alocados, na infraestrutura computacional do *Cluster* para oferecer o máximo de performance para esta aplicação *(Deployment)*. Esta quantidade deve ser informada com um número inteiro, para suportar e executar a aplicação *(Deployment)*;

                                       * **Mínimo Recurso a ser utilizado [CPU em milicores]**: Neste campo o usuário deve informar o mínimo de recursos de CPU que devem ser alocados, na infraestrutura computacional do Cluster para oferecer a performance mínima aceitável para esta aplicação (Deployment). Esta quantidade deve ser informada com um número inteiro, para suportar e executar a aplicação (Deployment);

                                       * **Máximo Recurso a ser utilizado [Memória em milicores]**: Neste campo o usuário deve informar o máximo de recursos de memória RAM que deve ser alocada, na infraestrutura computacional do Cluster para oferecer o máximo de performance para esta aplicação (Deployment). Esta quantidade deve ser informada com um número inteiro, para suportar e executar o Deployment;

                                       * **Mínimo Recurso a ser utilizado [Memória em milicores]**: Neste campo o usuário deve informar o mínimo de recursos de memória RAM que deve ser alocada, na infraestrutura computacional do Cluster para oferecer a performance mínima aceitável para esta aplicação (Deployment). Esta quantidade deve ser informada com um número inteiro, para suportar e executar a nova aplicação;

                                       * **Permitir execução privilegiada**: Neste campo o usuário deve informar se o container tem acesso aos recursos e capacidades Kernel da máquina Host;

                                       * **Especificar ID de usuário, grupo ou arquivo de sistema**: Neste campo o usuário pode informar o ID de usuário, grupo ou arquivo de sistema que o container é executado;

                                       * **Registry Secret**: Neste campo o usuário deve informar o nome do Secret do servidor de imagens associado a esta imagem. Quando o usuário clicar com o mouse sobre este campo, a Plataforma do Mangue.io apresenta uma lista de arquivos de Secrets disponíveis no servidor de imagem privado. A Plataforma do Mangue.io apresenta apenas os arquivos de Secrets privados que estão presentes na plataforma do Mangue.io.

               * **Botão Próximo**: Quando o usuário clica sobre o botão Próximo a Plataforma do Mangue.io apresenta a tela com campos respectivos de Secrets e Variáveis de Ambiente do container. Veja a tela abaixo:
  

.. image:: /figuras/fig_mangue/059_mangue_secrets_e_variaveis.png
    :alt: Secrets e variáveis do ambiente container 
    :scale: 80 %
    :align: center
=====


      * Variáveis de Ambiente: 

               * Nome da variável de ambiente; 
               * Conteúdo da variável de ambiente; 
               * Botão Adicionar;
               
      * Secrets:

               * Nome do Segredo; 
               * Variável de Ambiente; 
               * Chave do Segredo; 
               * Valor do Segredo; 
               * Botão Adicionar; 
               * Botão Criar Secret; 


      * Botão ``Voltar``;

      * Botão ``Finalizar``.


Após clicar o botão ``Finalizar`` a Plataforma do Mangue.io encerra as sub telas e retorna à primeira etapa do processo de nova aplicação, mas apresenta a configuração desta nova aplicação listada, abaixo segue o exemplo da lista:


.. image:: /figuras/fig_mangue/061_mangue_lista_aplicacao.png
    :alt: Lista aplicação 
    :scale: 80 %
    :align: center
=====


Abaixo descrevemos o conteúdo das colunas apresentadas nesta lista:

      * **#**: Esta coluna apresenta o número sequencial do container na lista apresentada.

      * **Container**: Esta coluna apresenta o nome do container informado nas etapas anteriores, o início do processo de criação de uma nova aplicação (Deployment).

      * **Imagem**: Esta coluna apresenta o nome da imagem da aplicação que foi selecionada do servidor de registro de imagens (ex: http://hub.docker.com).

      * **Versão**: Esta coluna apresenta a informação da versão da aplicação (Deployment) informada nas etapas anteriores.

      * **Ações**: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta um submenu com as seguintes opções:
  

.. image:: /figuras/fig_mangue/062_mangue_acoes_submenu.png
    :alt: Ações submenu 
    :scale: 80 %
    :align: center
=====

               * Adicionar PersistentVolumeClaim: Através desta tela o usuário pode configurar as características do arquivo referente ao PersistentVolumeClaim (PVC). A Plataforma do Mangue.io simplifica o processo de configuração do PVC, oferecendo ao usuário opções na interface gráfica que conduzem as decisões referentes a PVC, abaixo esclarecemos as opções:
  


.. image:: /figuras/fig_mangue/063_mangue_add_pvc.png
    :alt: Adicionar persistentvolume claim 
    :scale: 80 %
    :align: center
=====

      * **Tamanho / 1Gi, 5Gi, 10Gi**: O usuário pode selecionar o tamanho do volume simplesmente clicando com o cursor do mouse sobre o número desejado, selecionando a melhor opção de tamanho para este PVC. As opções estão expressas em Gigabytes (1, 5, ou 10).

      * **Tamanho / Personalizado**: Outra forma de criar um PVC com um volume com um tamanho diferente das opções anteriores, a Plataforma do Mangue.io apresenta uma barra deslizante (slide bar) que permite ao usuário selecionar o tamanho desejado do PVC. Usando o cursor do mouse sobre o indicador laranja, o usuário pode mover este indicador (para esquerda ou direita) para definir o tamanho final desejado. O tamanho mínimo é de 1 gigabyte e o máximo de 100 Gigabytes.

      * **Storage Class**: Este campo é uma lista *(dropdown list)* que é composta apenas por NFS servers configurados na Plataforma do Mangue.io. O usuário deve selecionar o servidor NFS mais adequado para receber o arquivo do PVC.

      * **Modo de Acesso**: Esta coluna apresenta a configuração de acesso a este volume, esses modos de acesso podem ser três, são eles: ReadWriteOnce, ReadOnlyMany, ReadWriteMany.

      * **Mount Path**: Neste campo o usuário deve informar o caminho onde o volume é montado no container. Se a base da aplicação é um ambiente Linux, o caminho de montagem do volume deve utilizar a notação do ambiente do sistema operacional Linux. 

      * **Nome do Volume**: Neste campo o usuário deverá informar no nome do arquivo de volume que será criado no ambiente do sistema operacional do Cluster.


               * **Adicionar ConfigMap**: Um ConfigMap é um objeto API usado para armazenar dados não confidenciais em pares chave-valor. Neste sub tela o usuário pode incluir e configurar o(s) arquivo(s) de *ConfigMap(s)* desejado(s) para o seu ambiente.
  


.. image:: /figuras/fig_mangue/064_mangue_add_configmap.png
    :alt: Adicionar configmap 
    :scale: 80 %
    :align: center
=====


      * **Nome do ConfigMap**: Este campo é obrigatório e o usuário deve informar o nome o qual deseja cadastrar para que a Plataforma do Mangue.io identifique este ConfigMap.

      * **Botão** ``Adicionar`` (“+”): 

      * **Mount Path**: Este campo é obrigatório e o usuário deve informar o caminho onde o volume é montado no container. Se a base da aplicação é um ambiente Linux, o caminho de montagem do volume deve utilizar a notação do ambiente do sistema operacional Linux. 

      * **Nome do Arquivo**: Este campo é obrigatório e o usuário deve informar no nome do arquivo que é criado no sistema operacional da máquina virtual que utilizar o ConfigMap.

      * **Conteúdo do Arquivo**: Este campo é obrigatório e o usuário deve preencher com o conteúdo específico do ConfigMap.

      * **Botão** ``Adicionar ConfigMap``: Após preencher todos os campos anteriores o usuário deve pressionar este botão com o cursor do mouse para que a Plataforma do Mangue.io promova a criação, configuração e gravação do ConfigMap para esta nova aplicação (Deployment).

                * **Editar Container**: Quando selecionada esta opção a Plataforma do Mangue.io apresenta a tela referente ao **Primeiro Passo: Nova Aplicação**, para que o usuário possa editar as configurações deste container.

                * **Excluir Container**: Esta ação é definitiva e quando acionada a Plataforma do Mangue.io remove toda a configuração inicial do container, **não será solicitada uma confirmação desta ação**.


B. Validar Nova Aplicação
~~~~~~~~~~~~~~~~~~~~~~~~~

Se o usuário clicar com o mouse sobre o nome do container a Plataforma do Mangue.io apresenta uma tela com as informações dos Recursos do Container.

A Plataforma do Mangue.io identifica os recursos de *PersistentVolumeClaim*, *ConfigMap*, do container que o usuário configurou para a aplicação e lista estes recursos conforme o exemplo da tela abaixo:
  

.. image:: /figuras/fig_mangue/065_mangue_recurso_container.png
    :alt: Recurso container 
    :scale: 80 %
    :align: center
=====


      * **#**: Esta coluna apresenta o número sequencial do container na lista apresentada.

      * **Nome**: Esta coluna apresenta o nome do recurso informado nas etapas anteriores.

      * **Tipo**: Esta coluna apresenta o tipo do recurso que foi criado nas etapas anteriores.

      * **Mount Path**: Esta coluna apresenta a informação do diretório do sistema operacional conforme foi configurado nas etapas anteriores.

      * **Ações**: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta um submenu com as seguintes opções:
  

.. image:: /figuras/fig_mangue/066_mangue_acoes_recursos.png
    :alt: Ações recursos 
    :scale: 80 %
    :align: center
=====


               * **Atachar a outro container**: Uma facilidade da Plataforma do Mangue.io permite que o usuário possa anexar (atachar) esta aplicação a um container diferente do que foi criado desde o início deste processo. Ao clicar sobre esta opção a Plataforma do Mangue.io apresenta a seguinte tela:
  


.. image:: /figuras/fig_mangue/067_mangue_criar_pcv.png
    :alt: Selecionar container 
    :scale: 80 %
    :align: center
=====

Ao clicar sobre o campo *containers* será apresentado uma lista *(dropdown list)* com os containers disponíveis e configurados na Plataforma do Mangue.io. Basta o usuário selecionar o container desejado e confirmar a ação.

               * **Excluir**: Esta ação é definitiva e quando acionada a Plataforma do Mangue.io remove toda a configuração inicial do container, não será solicitada uma confirmação desta ação.


C. Segundo Passo: Deploy nos Clusters:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta seção da tela a Plataforma do Mangue.io possibilita uma das grandes facilidades desta plataforma; permitir ao usuário criar, lançar e executar esta nova aplicação (Deployment) em mais de um Cluster, simultaneamente. A plataforma possibilita que o usuário selecione um (ou mais) Cluster(s) atualmente configurados no ambiente do Mangue.io. Abaixo descrevemos esta seção:
  

.. image:: /figuras/fig_mangue/068_mangue_deploy_clusters.png
    :alt: Deploy clusters 
    :scale: 80 %
    :align: center
=====


      * **Clusters Disponíveis**: Este campo quando selecionado apresenta a lista *(dropdown list)* com todos os Clusters configurados na plataforma e basta ao usuário selecionar quais deseja lançar e executar a aplicação Deployment que está sendo criado.

      * **Botão Próximo**: O usuário deve clicar neste botão para iniciar a terceira e última etapa para a criação de uma nova aplicação *(Deployment)*.


D. Terceiro Passo: Habilitar Zero Down-time
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Conforme mencionado no início deste tópico, o objetivo desta primeira abordagem – Criação de Nova Aplicação via telas/formulários no Mangue.io – é minimizar os potenciais erros de sintaxe YAML para um ambiente Kubernetes. A criação de código em sintaxe YAML em ambiente Kubernetes demanda um alto grau de especialização e conhecimento do desenvolvedor. Assim a sintaxe correta para o ambiente pode ter  todas as dependências necessárias para gerar o resultado desejado e integrado no uso do ambiente Kubernetes (ex.: uma aplicação / *Deployment*).

O desenvolvimento de um *script* de uma aplicação *(Deployment)* com a sintaxe YAML em um ambiente Kubernetes pode ser muito longo, e as dependências entre seções do *script* e com elementos externos (PVCs, *ConfigMaps*, variáveis de ambiente, entre outros.) pode induzir a criação do *script* com erros ou falhas de ausências de parâmetros, decorrentes da pouca experiência ou tentativa de usar um *script* desenvolvido por outra pessoa.

Um *script* genérico encontrado na internet pode não deixar claro todas as dependências de variáveis de ambiente, arquivos externos (*ConfigMaps*, PVCs, entre outros).

O processo de adaptação de scripts (pouco documentado no ano de 2018) poderia ser uma grande frustração e impedir a popularização do ambiente Kubernetes, portanto a Plataforma do Mangue.io simplifica esse processo guiando o usuário através de telas/formulários.

Após o completo preenchimento desta segunda parte, de todos os campos das telas/formulários referente a criação da aplicação *(Deployment)* a Plataforma do Mangue.io gera o *script YAML* completo e, por consequência, sua compilação sem erros.

Veja abaixo a descrição das próximas telas que fazem parte da última etapa antes da finalização e criação da aplicação *(Deployment)* que é executada e gerenciada pela Plataforma do Mangue.io.
  

.. image:: /figuras/fig_mangue/069_mangue_habilitar_downtime.png
    :alt: Habilitar zero downtime 
    :scale: 80 %
    :align: center
=====


      * **MaxSurge**: Neste campo o usuário deve informar a quantidade máxima de réplicas que deseja manter ativa na Plataforma do Mangue.io. Durante um processo de atualização da versão da aplicação *(Deployment)*, este número é o responsável em manter um mínimo de réplicas para garantir a experiência do usuário durante um processo de atualização.

      * **MaxUnavailable**: Neste campo o usuário deve informar a quantidade máxima de réplicas que deseja manter indisponível na Plataforma do Mangue.io, Durante um processo de atualização da versão da aplicação *(Deployment)*, este número indica para a Plataforma do Mangue.io a quantidade de réplicas que podem ser atualizadas de modo paralelo.

      * **Container**: Este é um cabeçalho de uma seção que indica o nome do container que está sendo criado para esta nova aplicação *(Deployment)*.

      * **Seção ReadinessProbe**: O ambiente Kubernetes usa sondagens de prontidão *(ReadinessProbe)* para saber quando um contêiner está pronto para começar a aceitar tráfego. Um Pod é considerado concluído quando todos os seus contêineres estão prontos. Nos campos abaixo o usuário deve entrar com os valores referentes ao ambiente de *ReadinessProbe*.

               * **SuccessThreshold**: Neste campo o usuário deve informar um número inteiro que define a quantidade mínima de containers que a plataforma do Mangue.io deve manter disponível durante o processo de atualização de forma a garantir a experiência do usuário que está utilizando a aplicação *(Deployment)*.

               * **FailureThreshold**: Neste campo o usuário deve informar um número inteiro que define a quantidade máxima de containers que ficam indisponíveis durante um processo de atualização da versão da aplicação *(Deployment)*. Este número indica para a Plataforma do Mangue.io a quantidade de réplicas que podem ser atualizadas de modo paralelo.

               * **ReadinessPath**: Neste campo o usuário deve informar o caminho do diretório onde é criado um arquivo de registro (log) que armazena os eventos durante o processo de atualização do container.

               * **RequestHeaders**: Nesta subseção o usuário pode configurar o layout do conteúdo do arquivo de registro de eventos da atualização que deve ser criado, adicionando colunas *(headers)* e o conteúdo da coluna;

                    * **Nome do Header**: Neste campo o usuário deve informar o nome da coluna que é criada dentro do arquivo de registro *(log)* de atividades de atualização.

                    * **Valor do Header**: Neste campo o usuário deve informar o valor inicial da coluna que é criada dentro do arquivo de registro *(log)* de atividades de atualização.
                    * Botão ``Adicionar``: Este botão informa para a Plataforma do Mangue.io que o conjunto header/value deve ser configurado no arquivo de registro de atividades *(log)* de atualização. O usuário pode adicionar a quantidade de colunas que se façam necessárias, basta preencher os valores dos campos anteriores e pressionar o botão ``Adicionar``.

      * **LivenessProbe**: O ambiente Kubernetes usa sondagens de atividade *(LivenessProbe)* para saber quando reiniciar um container. Estas sondagens são efetuadas em intervalos de tempo (segundos) definidos pelo usuário e após este período acrescenta uma linha no arquivo de log. Nos campos abaixo o usuário entra com os valores referentes ao ambiente de *LivenessProbe*:

               * **PeriodSeconds**: Neste campo o usuário deve informar um número inteiro que representa o período de segundos referente ao intervalo de sondagem de atividade *(livenessprobe)*.

               * **ReadinessPath**: Neste campo o usuário deve informar o caminho do diretório onde é criado um arquivo de registro *(log)* que armazena os eventos durante o processo de atualização do container.

               * **RequestHeaders**: Nesta subseção o usuário pode configurar o *layout* do conteúdo do arquivo de registro de eventos da atualização que deve ser criado, adicionando colunas *(headers)* e o conteúdo da coluna;

                   * **Nome do Header**: Neste campo o usuário deve informar o nome da coluna que é criada dentro do arquivo de registro *(log)* de atividades de atualização.

                   * **Valor do Header**: Neste campo o usuário deve informar o valor inicial da coluna que é criada dentro do arquivo de registro *(log)* de atividades de atualização.

                     * Botão ``Adicionar``: Este botão informa para a Plataforma do Mangue.io que o conjunto header/value deve ser configurado no arquivo de registro de atividades *(log)* de atualização. O usuário pode adicionar a quantidade de colunas que se façam necessárias, basta preencher os valores dos campos anteriores e pressionar o botão ``Adicionar``.

                     * Botão ``Voltar``: Se o usuário necessitar regressar para uma etapa anterior, ele deve acionar este botão. Importante ressaltar que serão perdidas todas as informações que foram preenchidas nesta tela pelo usuário, e a Plataforma do Mangue.io retorna para a tela anterior.

                     * Botão ``Finalizar``: O usuário deverá pressionar este botão quando houver concluído o preenchimento de todos os campos das telas anteriores e, estando pronto para iniciar a compilação da aplicação *(Deployment)*. A Plataforma do Mangue.io compila todas as informações dos campos e gerar um script YAML; ao compilar este script e gerar a aplicação (e todas suas dependências: PVCs, ConfigMaps, Arquivos de log, entre outros) ela será executada e gerenciada dentro do ambiente da Plataforma do Mangue.io.

Neste ponto a Plataforma do Mangue.io encerra as telas de criação de aplicação *(Deployment)* e o usuário pode encontrar sua nova aplicação listada na tela do menu *Workloads/Deployments*.
O usuário poderá ter uma quantidade maior de informações de sua nova aplicação no menu Informações do *Deployment*.


Deploy via YAML
---------------


Esta é a segunda abordagem que a Plataforma do Mangue.io permite ao usuário fazer o upload de um arquivo texto, cujo conteúdo é a codificação da aplicação em sintaxe YAML, já adaptada e preparada para um ambiente Kubernetes.

O YAML não é uma linguagem de marcação, de acordo com yaml.org, é um padrão de serialização de dados amigável para qualquer linguagem de programação. YAML foi criado na crença que todos os dados podem ser representados adequadamente como combinação de listas, hashes (mapas) e dados escalares (valores simples).

A sintaxe é relativamente simples e foi projetada tendo em conta que é muito legível, mas que também fosse facilmente mapeada para os tipos de dados mais comuns na maioria das linguagens de alto-nível. Além disso, YAML utiliza uma notação baseada em endentação e um conjunto de caracteres distintos dos que são usados pelo XML, fazendo com que as duas linguagens sejam facilmente compostas uma na outra.

Qualquer usuário com conhecimento da sintaxe YAML pode usar a interface do Mangue.io para criar um: Deployment, Service, Statefulsets, Volume ou Ingress.

A plataforma do Mangue.io permite ao usuário experiente em YAML entrar com o seu código de forma livre diretamente através da interface (data-entry), ou carregar um arquivo (upload) em formato texto não formatado (ASCII) de um diretório/folder de seu computador para a plataforma do Mangue.io.

Ao clicar sobre a opção Deploy via Código YAML a plataforma do Mangue.io apresenta a seguinte tela:
  

.. image:: /figuras/fig_mangue/069_mangue_habilitar_downtime.png
    :alt: Deploy em outros clusters 
    :scale: 80 %
    :align: center
=====


Abaixo descrevemos cada objeto acionável desta tela.

A. Clusters Disponíveis
~~~~~~~~~~~~~~~~~~~~~~~

O usuário deve clicar sobre o campo Clusters Disponíveis para abrir uma lista *(dropdown)* de todos os Clusters configurados na plataforma do Mangue.io, e selecionar o Cluster destino no qual o Deployment é criado e executado.

Existe uma mensagem presente na tela que é importante ressaltar para o processo de criação de Deployment via YAML.

.. note::
	Caso nenhum Cluster seja selecionado,  é feito o deploy apenas no Cluster utilizado atualmente.
	

B. Template
~~~~~~~~~~~

Na sequência o usuário deve selecionar uma das opções de modelo (template) de código YAML que estão previamente a configurados na plataforma do Mangue.io, esta funcionalidade agrega produtividade ao usuário; e cada tipo de modelo é uma opção na lista (dropdown):

                                             * Default: Permite ao usuário configurar o código YAML de forma livre. Nesta opção o usuário deve possuir um bom conhecimento da sintaxe YAML para entrar com o código desejado. O usuário deve iniciar clicando com o mouse na área cinza ao lado do número “1”, antes de iniciar a digitação do seu código YAML. A cada nova linha o usuário deve usar a tecla “Enter” para iniciar uma nova linha. O usuário deve utilizar a sua própria experiência de desenvolvimento para estruturar a sintaxe de seu código linha a linha. Através desta opção o usuário pode entrar com um código YAML para criar, para provisionar um novo Pod na plataforma do Mangue.io.
                                             * Deployment: Nesta opção a plataforma do Mangue.io apresenta um modelo de código YAML com a sintaxe inicial para criar um Deployment. O usuário pode usar o mouse para clicar na linha (e no local) desejada para iniciar a digitação dos seus parâmetros específicos do Deployment, dessa forma editando o modelo do código YAML que a plataforma lhe apresenta.
                                             * Serviço: Nesta opção a plataforma do Mangue.io apresenta um modelo de código YAML com a sintaxe inicial para criar um Serviço. O usuário pode usar o mouse para clicar na linha (e no local) desejada para iniciar a digitação dos seus parâmetros específicos do serviço, dessa forma editando o modelo do código YAML que a plataforma lhe apresenta.
                                             * Statefulsets: Nesta opção a plataforma do Mangue.io apresenta um modelo de código YAML com a sintaxe inicial para criar um Statefulsets. O usuário pode usar o mouse para clicar na linha (e no local) desejada para iniciar a digitação dos seus parâmetros específicos para o Statefulsets, dessa forma editando o modelo do código YAML que a plataforma lhe apresenta.
                                             * Volume: Nesta opção a plataforma do Mangue.io apresenta um modelo de código YAML com a sintaxe inicial para criar um Volume. O usuário pode usar o mouse para clicar na linha (e no local) desejada para iniciar a digitação dos seus parâmetros específicos para o Volume, dessa forma editando o modelo do código YAML que a plataforma lhe apresenta.
                                             * Ingress: Nesta opção a plataforma do Mangue.io apresenta um modelo de código YAML com a sintaxe inicial para criar uma definição de Ingress. O usuário pode usar o mouse para clicar na linha (e no local) desejada para iniciar a digitação dos seus parâmetros específicos, dessa forma editando o modelo do código YAML que a plataforma lhe apresenta.
O usuário experiente em YAML vê que o uso de modelos aumenta a produtividade e mantém o código mais bem documentado e estruturado de acordo com as melhores práticas.

C. Browse
~~~~~~~~~

Este botão permite ao usuário carregar (upload) um arquivo tipo texto não formatado (ASCII), com um código YAML previamente criado pelo usuário. O usuário deve clicar sobre o botão “Browse” para que a plataforma do Mangue.io apresente a tela do Explorador de Arquivos (File Explorer) de seu computador para que o usuário possa selecionar o folder/diretório onde se localiza o arquivo de seu código.

A plataforma do Mangue.io está configurada para identificar e apresentar todos os arquivos com extensão “*.yaml e *.yml” presentes no folder/diretório selecionado. Caso o usuário tenha salvo o seu código fonte em um arquivo com extensão diferente, este deve digitar o nome completo do arquivo no campo “Nome” ou selecionar a opção “Todos os arquivos (*.*) / All files (*.*)” para localizar e selecionar o arquivo desejado.
  
.. image:: /figuras/fig_mangue/071_mangue_arquivo_yaml.png
    :alt: Localizar e selecionar arquivo  
    :scale: 80 %
    :align: center
=====


Quando o usuário selecionar o arquivo desejado, basta clicar o botão “Abrir / Open” para que a plataforma do Mangue.io carregue o conteúdo do arquivo selecionado para a interface, e o usuário repara que a plataforma do Mangue.io numera, sequencialmente, todas as linhas do código carregado.

Neste ponto o usuário pode editar o código diretamente através da interface da plataforma do Mangue.io, para personalizar ou corrigir qualquer linha do código YAML presente na tela.

D. Submit
~~~~~~~~~

Quando o usuário estiver satisfeito com o conteúdo de todo código YAML e está seguro de que este código está correto, basta clicar no botão verde “Submit” para que a Plataforma do Mangue.io efetue a carga do código e sua consequente compilação para disponibilizar este código como um Deployment, Serviço, Statefulsets, Volume ou Ingress.

Neste ponto a Plataforma do Mangue.io encerra as telas de criação de aplicação (Deployment) e o usuário pode encontrar sua nova aplicação listada na tela do menu Workloads/Deployments.

O usuário pode ter uma quantidade maior de informações de sua nova aplicação no menu Informações do Deployment.

E. Server VS Code
~~~~~~~~~~~~~~~~~

.. image:: /figuras/fig_mangue/072_mangue_add_vscode.png
    :alt: Adicionar Server VS Code
    :scale: 80 %
    :align: center
=====  

Para criar um Visual Studio Code é necessário clicar no botão de “  ”  e preencher os campos abaixo:

                                             * Nome do Servidor VS Code: Nome do servidor Visual Studio Code a ser criado.
                                             * Tamanho do Servidor VS Code: Tamanho de disco a ser disponibilizado para o Visual Studio Code. A medida do tamanho é definida no campo de Tipo do Tamanho.
                                             * Tipo de Serviço: O usuário pode selecionar o tipo de serviço a ser atribuído ao deployment do Visual Studio Code. As opções disponíveis são: Cluster IP, NodePort, Load Balancer e Ingress
                                             * Porta: O usuário pode selecionar a porta que é utilizada no serviço.
                                             * Tipo do Tamanho: Especifica a unidade de tamanho. As opções disponíveis são: Gi e Mi.
                                             * Ingress Class: Caso o tipo de serviço selecionado seja Ingress é necessário selecionar a Ingress Class a ser utilizada pelo serviço.
                                             * URL do Servidor VS Code: Caso o tipo de serviço selecionado seja Ingress é necessário especificar o caminho da rota do Ingress. Exemplo: /vscode
                                             * Ativar autenticação: O usuário pode atribuir uma senha que é necessária para acessar o Servidor VS Code.
                                             * Senha do Servidor VS Code: Senha a ser utilizada para acessar o Servidor VS Code.

====


ConfigMap
=========

De forma simples, pode-se afirmar que ConfigMap é um conjunto de pares de chave-valor para armazenamento de configurações, que fica armazenado dentro de arquivos que podem ser consumidos através de pods. Ele é muito parecido com Secrets, mas fornece um modo de se trabalhar com strings que não possuem dados confidenciais, como senhas, chaves, tokens e outros dados sigilosos.

Os arquivos de configMap, podem ser tanto arquivos complexos que possuem poucas regras, como também arquivos no formato JSON complexos e cheios de regras.

Vale ressaltar que um arquivo de configmap pode conter, sim, o conteúdo complexo de um JSON, bastando ao usuário preencher o conteúdo deste arquivo obedecendo a sintaxe correta de um arquivo JSON.

Ao selecionar esta opção na barra do menu, a plataforma do Mangue.io apresenta a tela abaixo, que contém uma listagem de todos os configmaps cadastrados na plataforma.
  
.. image:: /figuras/fig_mangue/073_mangue_configmaps.png
    :alt: Configmaps
    :scale: 80 %
    :align: center
=====


Abaixo a descrição de cada coluna desta tabela:

                                             * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                             * Nome: Nesta coluna é apresentado o nome do configmap adicionado pelo usuário. Ao clicar com o mouse sobre o nome,a plataforma do Mangue.io apresenta uma tela com o(s) conteúdo(s) do(s) arquivo(s) de configmap. Por padrão é apresentado somente a visualização de uma linha do conteúdo do arquivo, caso o conteúdo seja maior do que o campo, o usuário pode posicionar o mouse no canto inferior direito, até que o cursor do mouse mude para uma seta diagonal dupla (“  ”), que permite ao usuário redimensionar o tamanho do campo de conteúdo listado, para acomodar o tamanho que for adequado ao usuário, para a melhor visualização deste campo.

.. image:: /figuras/fig_mangue/074_mangue_configmaps_arquivo.png
    :alt: Configmaps arquivo 
    :scale: 80 %
    :align: center
=====  

Importante ressaltar que esta janela não permite a edição do conteúdo listado.

                                                * Duração: Nesta coluna é apresentado o tempo (em dias) desde o momento de criação do configmap.
                                                * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções, assim como a figura abaixo:
  
.. image:: /figuras/fig_mangue/075_mangue_acoes_configmap.png
    :alt: Ações configmap 
    :scale: 80 %
    :align: center
=====


                                                   * Deletar Configmap: Quando o usuário selecionar esta opção a plataforma do Mangue.io irá apresentar a tela abaixo solicitando a confirmação da opção de remoção do configmap.
  
.. image:: /figuras/fig_mangue/076_mangue_deletar_configmap.png
    :alt: Deletar configmap 
    :scale: 80 %
    :align: center
=====


Importante ressaltar que esta ação é definitiva e remove o arquivo do sistema operacional, não sendo possível recuperá-lo, pois serão apagadas todas as referências deste configmap na plataforma do Mangue.io. Será necessário recriar o arquivo desde o início.
                                                   * Editar Configmap: Ao selecionar esta opção a plataforma do Mangue.io apresenta a seguinte tela para que o usuário possa efetuar as alterações necessárias no conteúdo do(s) arquivo(s) de configmap:

.. image:: /figuras/fig_mangue/077_mangue_add_configmap.png
    :alt: Adicionar configmap 
    :scale: 80 %
    :align: center
=====  

Logo acima da tabela, existem três elementos com os quais o usuário poderá atuar:
  
.. image:: /figuras/fig_mangue/078_mangue_pesquisar_atualizacao.png
    :alt: Pesquisar atualização 
    :scale: 80 %
    :align: center
=====


                                                   * A ação de pesquisa: Caso a lista de apresentada nesta tela seja muito longa (ocupando mais de uma página), existe um campo onde será possível ao usuário efetuar uma pesquisa pelo nome do ConfigMaps desejado. Basta informar parte do nome e teclar enter ou clicar sobre o ícone da lupa “  ”. Como resultado dessa busca apenas aparecem os ConfigMaps que contiverem a palavra-chave da pesquisa.
                                                   * A ação de atualizar: Basta clicar no ícone “  ” para que o Mangue.io atualize a interface com os valores mais recentes desta tabela de ConfigMaps.
                                                   * Adicionar um ConfigMaps: Basta clicar no sinal de adição “+” para que o usuário possa cadastrar um novo ConfigMaps em um determinado A plataforma do Mangue.io apresenta a seguinte tela ao usuário:

.. image:: /figuras/fig_mangue/079_mangue_add_configmap.png
    :alt: Adicionar configmap 
    :scale: 80 %
    :align: center
=====
  

Abaixo a descrição dos campos da tela acima:
                                                      * Nome do Configmap: Neste campo o usuário deve digitar o nome do configmap desejado e em seguida clicar sobre o ícone do sinal de adição (“+”), que faz a plataforma do Mangue.io adicionar os campos abaixo.
                                                      * Arquivo “n”: A cada vez que o usuário clicar sobre o sinal de adição (“+”) a Plataforma do Mangue.io adiciona uma linha cinza com o número sequencial do arquivo de Configmap. Caso o usuário necessite remover (apagar) o arquivo configurado no ícone da lata de lixo (“  ”) para optar por remover o arquivo “n” do configmap.
                                                         * Nome do Arquivo: Neste campo o usuário deve informar o nome do arquivo que é criado no sistema operacional destino que dá suporte a execução do deployment. Importante lembrar que este nome, e sua respectiva extensão, devem seguir as regras de nomeação de arquivos do sistema operacional destino, portanto devem conter apenas caracteres ASCII padrão. Atenção: não devem ser utilizadas letras com acentuação (á, é, í, ã, õ, ç, entre outros), pois pode haver erro na criação do arquivo no sistema operacional.
                                                         * Conteúdo do Arquivo: Neste campo o usuário deve digitar com o conteúdo do arquivo nomeado, no campo anterior; conteúdo este que deve ser informado conforme necessidade técnica e o objetivo deste configmap. Por padrão é apresentado somente a visualização de algumas linhas do conteúdo do arquivo, caso o conteúdo seja maior do que o campo, o usuário pode posicionar o mouse no canto inferior direito, até que o curso o mouse mude para uma seta diagonal dupla (“  ”), que permite ao usuário redimensionar o tamanho do campo de conteúdo listado, para acomodar o tamanho que for adequado ao usuário, para a melhor visualização deste campo.
                                                            * Botão “Adicionar Configmap”: Após o usuário informar o(s) arquivo(s) de configmap necessário(s), o usuário deve clicar com o mouse sobre o botão “Adicionar Configmap”, para a Plataforma do Mangue.io efetuar a criação do(s) referido(s) arquivo(s) no ambiente do sistema operacional destino. Após esta ação sobre este botão a plataforma fecha esta janela e retorna para a tela onde é apresentada a lista de configmaps.

====


Cluster Events
==============

Através desta opção de menu, a Plataforma do Mangue.io apresenta todos os eventos que ocorreram no cluster e namespace selecionados na aba engrenagens “   Seleção de Configuração”. A cada seleção de contrato/cluster/namespace a lista de eventos é atualizada automaticamente.

.. image:: /figuras/fig_mangue/080_mangue_cluster_events.png
    :alt: clusters Events 
    :scale: 80 %
    :align: center
=====  

Abaixo a descrição do conteúdo de cada coluna da lista apresentada:
                                                            * #: Número sequencial do evento na lista apresentada;
                                                            * Nome: Nome do evento que a plataforma do Mangue.io gerou para o deployment; 
                                                            * Tipo de Evento: Descreve o tipo do evento ocorrido, e podem ser listados os seguintes tipos de eventos:
                                                            * Normal
                                                            * Warning
                                                            * Tipo de Objeto: Descreve qual objeto configurado na plataforma do Mangue.io que foi a origem do evento listado. A identificação do tipo de objeto, permite ao usuário identificar esta origem para que este possa ter acesso ao objeto e atuar na resolução do evento, através da redefinição do objeto, ou optar por sua remoção. Os tipos de objeto podem ser alguns dos listados abaixo:
                                                            * Deployments;
                                                            * Daemonsets;
                                                            * Horizontal Autoscaler;
                                                            * Pods;
                                                            * Statefulsets;
                                                            * Updates;
                                                            * Serviços;
                                                            * Ingress;
                                                            * StorageClass;
                                                            * PersistentVolumes;
                                                            * PersistentVolumesClaim;
                                                            * Nome do Objeto: Nome do recurso do evento;
                                                            * Mensagem: 
                                                            * Pulled;
                                                            * Created;
                                                            * Started;
                                                            * NoPods;
                                                            * FailedGetScale;
                                                            * ProvisioningFailed;
                                                            * FailedBinding;
                                                            * Executado há: Informa quanto tempo atrás o evento foi executado.


Logo acima da tabela, existem três elementos com os quais o usuário poderá atuar:
  
.. image:: /figuras/fig_mangue/081_mangue_pesquisar_evento.png
    :alt: Pesquisar evento 
    :scale: 80 %
    :align: center
=====


                                                            * A ação de pesquisa: Caso a lista de apresentada nesta tela seja muito longa (ocupando mais de uma página), existe um campo onde será possível ao usuário efetuar uma pesquisa pelo nome do deployment desejado. Basta informar parte do nome do evento e teclar enter ou clicar sobre o ícone da lupa “  ”. Como resultado dessa busca virão apenas os eventos que contiverem a palavra-chave da pesquisa.
                                                            * A ação de atualizar: Basta clicar no ícone “  ” para que o Mangue.io atualize a interface com a lista mais recente de eventos desta tabela.


====

Cron Jobs, Jobs
===============

Nesta opção de menu, o usuário pode visualizar duas funções distintas da plataforma do Mangue.io, são jobs e cron jobs. O usuário vê a lista de todos os jobs e cronjobs, a lista apresenta o que está programado para o contrato, cluster e namespace selecionados na aba engrenagens “   Seleção de Configuração”. A cada seleção de contrato/cluster/namespace a lista é atualizada automaticamente.

A. Cron Jobs
~~~~~~~~~~~~

Os CronJobs são úteis para criar tarefas (jobs) periódicas e recorrentes, como executar backups ou enviar e-mails. Os CronJobs também podem agendar tarefas individuais para um horário específico, como agendar um trabalho para quando seu cluster provavelmente estará ocioso.
A plataforma do Mangue.io lista todos os cronjobs configurados em seu ambiente:

.. image:: /figuras/fig_mangue/082_mangue_cronjobs.png
    :alt: Cron Jobs 
    :scale: 80 %
    :align: center
=====  

Abaixo a descrição do conteúdo de cada coluna da lista apresentada:
                                                               * #: Número sequencial do cronjob na lista apresentada;
                                                               * Nome: Nome do cronjob que a plataforma do Mangue.io gerou para o deployment;
                                                               * Schedule: Apresenta a configuração do agendamento (data e hora) programado para executar este cronjob;
                                                               * Duração: Apresenta o tempo de duração do cronjob;
                                                               * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções assim como a figura abaixo:

.. image:: /figuras/fig_mangue/083_mangue_deletar_cronjobs.png
    :alt: Deletar cron job 
    :scale: 80 %
    :align: center
=====
  

B. Jobs
~~~~~~~

Um job cria um ou mais pods e garante que um número específico deles seja encerrado com êxito. Conforme os pods são concluídos com sucesso, o job rastreia as conclusões bem-sucedidas. Quando um número especificado de conclusões bem-sucedidas é alcançado, a tarefa (ou seja, Job) está concluída. Excluir um job limpará os pods que ele criou.

O usuário também pode configurar um job para que seja executado em vários pods em paralelo.

.. image:: /figuras/fig_mangue/084_mangue_jobs.png
    :alt: Jobs 
    :scale: 80 %
    :align: center
=====  

Abaixo a descrição do conteúdo de cada coluna da lista apresentada:
                                                                  * Nome: Nome do job que a plataforma do Mangue.io gerou para o deployment
                                                                  * Status: Esta coluna apresenta três valores possíveis, “COMPLETED”, “IN PROGRESS” e “FAILED”:
                                                                  * COMPLETED:  Job executado com sucesso.
                                                                  * IN PROGRESS: Job sendo executado.
                                                                  * FAILED: Job falhou na execução.
                                                                  * Paralelismo: Quantidade de Pods para execução em paralelo.
                                                                  * Conclusões: Conclusões bem-sucedidas.
                                                                  * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, exibe a opção de deletar o job, como mostra a figura:
  
.. image:: /figuras/fig_mangue/085_mangue_deletar_job.png
    :alt: Deletar Job 
    :scale: 80 %
    :align: center
=====

Faturamento
===========

Esta opção da plataforma do Mangue.io é uma grande aliada à Governança Financeira das empresas. Poucas ferramentas disponíveis no mercado atualmente apresentam os valores reais de consumo de infraestrutura computacional, para suportar um ambiente serverless baseado em containers (Kubernetes).

O termo serverless pode levar a uma falsa noção de que este ambiente não gera custos de infraestrutura computacional, mas qualquer aplicação de software sempre necessita de um recurso computacional (CPU, memória, disco, sistema operacional - SO). 

Para que este software seja executado cada item carrega seu custo de uso, de armazenamento, de licenciamento (SO e softwares) e deve ser calculado dia a dia, para que atenda a critérios e políticas de Governança de Custos e Governança Financeira.

A plataforma do Mangue.io possui uma base de dados que acumula os valores de consumo de infraestrutura mês-a-mês, desde o momento da sua instalação. Esta base de dados é calculada dia-a-dia e acumula os valores de consumo, de acordo com a fórmula de cálculo apresentada no tópico Cálculo do Valor do Consumo do Cluster.

Ao selecionar esta opção do menu a plataforma do Mangue.io apresenta a seguinte tela:
  
.. image:: /figuras/fig_mangue/086_mangue_faturamento_cluster.png
    :alt: Histórico faturamento cluster 
    :scale: 80 %
    :align: center
=====


A plataforma do Mangue.io apresenta os valores do cluster e namespace selecionados na aba engrenagens “   Seleção de Configuração”. A cada seleção de um novo contrato/cluster/namespace os valores e os gráficos são atualizados automaticamente.

Esta tela está dividida em duas seções diferentes, a seguir o detalhamento de cada seção.

====


Relatório Consolidado
---------------------


Esta tela apresenta informações quanto ao consumo mensal dos clusters, o usuário consegue visualizar o preço de cada cluster no gráfico de pizza presente na imagem acima. Assim como é possível visualizar o consumo por usuário, isso somente ocorre quando o deployment é criado por meio do Mangue.io, uma vez que é guardado no deployment a informação do usuário responsável por sua criação.

.. image:: /figuras/fig_mangue/087_mangue_overview_financeiro.png
    :alt: Overview financeiro 
    :scale: 80 %
    :align: center
=====

Ao selecionar um cluster as informações da tela são recarregadas de acordo com o cluster selecionado, isso inclui tanto os gráficos que informam o preço por cluster e preço por usuário, quanto a tabela com detalhes sobre custo de aplicações.

Por padrão a consulta é realizada considerando todos os namespaces do cluster, mas o usuário pode filtrar por um namespace específico clicando em “Selecione um namespace”, as informações da tela são recarregadas assim como no item anterior, se diferenciando por retornar os valores apenas do namespace selecionado.

Ainda nessa tela é possível visualizar uma lista de detalhes sobre custo das aplicações, como pode ser visto na imagem abaixo:

.. image:: /figuras/fig_mangue/088_mangue_lista_aplicacoes.png
    :alt: Listando aplicação
    :align: center
=====  

                                                                     * Nome: Esta coluna apresenta o nome do deployment, lembrando que para o deployment aparecer aqui ele precisa estar em um cluster com o “bilhetador” habilitado;
                                                                     * Usuário: Esta coluna apresenta o usuário responsável pela criação da aplicação;
                                                                     * Namespace: Esta coluna apresenta o namespace ao qual a aplicação pertence;
                                                                     * Preço de CPU: Esta coluna apresenta o custo por CPU da aplicação correspondente ao mês selecionado;
                                                                     * Preço de Memória: Esta coluna apresenta o custo por Memória da aplicação correspondente ao mês selecionado;
                                                                     * Preço Total: Esta coluna apresenta a soma do preço de CPU e preço de Memória.
Há ainda a possibilidade de exportar as informações correspondente a tabela acima, em formato csv, por meio da funcionalidade “export to csv”  representada pelo seguinte botão   , ao clicar o usuário consegue baixar o arquivo logo em seguida.

====


Histórico
---------  

.. image:: /figuras/fig_mangue/089_mangue_historico_faturamento.png
    :alt: Histórico faturamento mensal cluster
    :scale: 80 %
    :align: center
=====


A. Histórico de Faturamento Mensal do Cluster
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Esta seção apresenta um gráfico com a evolução do valor de consumo dos recursos de CPU e Memória do cluster, para suportar e executar todos os conteúdos do Workloads (Deployments, Statefulsets, Horizontal Autoscaler, Pods).

O usuário pode selecionar o período o qual deseja visualizar os valores, bastando selecionar o mês e ano apresentado logo acima do gráfico:
  
.. image:: /figuras/fig_mangue/090_mangue_mes_ano.png
    :alt: Selecione ano e mês 
    :scale: 80 %
    :align: center
=====


Ao clicar sobre o ícone do calendário, a plataforma do Mangue.io apresenta uma tela de seleção anual, onde o usuário pode escolher qual o ano deseja visualizar:

.. image:: /figuras/fig_mangue/091_mangue_ano.png
    :alt: calendário anual 
    :scale: 80 %
    :align: center
=====  

Assim que o ícone do calendário é clicado, é possível selecionar o ano desejado na plataforma do Mangue.io, conforme a imagem da tela acima. Em seguida, o usuário pode selecionar o mês que deseja visualizar e seus valores acumulados:

.. image:: /figuras/fig_mangue/092_mangue_mes.png
    :alt: calendário mensal 
    :scale: 80 %
    :align: center
=====

Logo que o usuário selecionar o mês, a plataforma do Mangue.io inicia o processo de busca e cálculo dos valores do mês e ano selecionado. Este processo pode demorar alguns segundos e o usuário pode acompanhar a evolução deste processamento, acompanhando uma “linha preta” que aparece da esquerda para a direita no alto da área do browser de internet.

No minuto em que a linha preencher totalmente o topo da área do browser, a plataforma do Mangue.io atualizará o gráfico da tela com os valores diários do mês e ano selecionado.

Importante mencionar que os valores diários apresentados refletem até o dia corrente, em outras palavras, se o usuário deseja consultar os valores do mês, e o mês corrente se encontra (por exemplo) na primeira quinzena, o gráfico representa apenas do dia 1º até o dia 15 do mês corrente.

Este gráfico apresenta uma linha da evolução do valor de consumo de infraestrutura computacional e pode ser compreendido como uma progressão matemática. Em outras palavras, é o valor do consumo do dia anterior somado ao valor de consumo do dia corrente, e, assim, sucessivamente.

A cada início de mês, o valor será “zerado” iniciando um novo ciclo de cálculo de consumo da infraestrutura computacional para o período do mês, até o dia corrente. Desta forma, o valor do primeiro dia do mês pode não ser apresentado imediatamente, pois a plataforma do Mangue.io necessita computar este valor do dia após as 24 horas do primeiro dia – o valor do dia corrente é apresentado após 24 horas.

A linha do gráfico pode apresentar “picos” e “vales” devido a diversos fatores, portanto deve-se levar em consideração o ambiente em sua totalidade. Aumento de consumo pode ser decorrente do lançamento de Autoescaladores Horizontais, Migrações, Updates, CronJobs criação de novas aplicações, deployments entre outros.

Todas as situações acima listadas são potenciais causas de aumento de consumo de infraestrutura computacional e a decorrente evolução dos valores totais deste gráfico.



B. Histórico de Faturamento do Cluster
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Este gráfico apresenta o consumo acumulado mês-a-mês dos últimos quatro (04) meses do período em que se encontra o usuário.

.. image:: /figuras/fig_mangue/093_mangue_historico_cluster.png
    :alt: Histórico faturamento cluster
    :scale: 80 %
    :align: center
=====
  

Na figura acima, pode-se ver o exemplo de como a plataforma do Mangue.io apresenta os valores do consumo de infraestrutura do cluster. Este gráfico exibe os últimos quatro meses do consumo.


O valor acumulado do mês corrente, representa o consumo do primeiro dia do mês até o dia da consulta; desta forma, caso o dia corrente seja na primeira semana do mês, o valor acumulado representa  o consumo da semana. 
Importante mencionar, a plataforma do Mangue.io ZERA todos os valores do mês no primeiro dia de cada mês. E inicia a somatória (progressão matemática) até o último dia do mês (dia 30 ou 31 – com exceção do mês de fevereiro).

No eixo vertical, são apresentados os valores máximos arredondados para o próximo valor acima do máximo, em um período. Para o usuário identificar o valor correto, basta posicionar o ponteiro do mouse sobre a barra do mês desejado, para que a plataforma do Mangue.io possa apresentar o valor detalhado do mês em que o cursor do mouse está posicionado.


C. Por Tags
~~~~~~~~~~~

A plataforma Mangue.io permite que as aplicações Kubernetes possuam Tags, compostas por um conjunto de chave e valor, com o objetivo de agrupar aplicações semelhantes, com o objetivo de visualizar o faturamento delas. As Tags podem ser criadas ou associadas a uma aplicação durante o processo de criação de uma aplicação, conforme demonstrado na seção de Nova Aplicação em Catálogo, ou em uma aplicação já existente, demonstrado na seção de Alterar Tags em Deployments.

A tela de Faturamento por Tags é separada em duas seções: 
        * Histórico de Faturamento Mensal por Tags.
        * Detalhes Tags.

.. image:: /figuras/fig_mangue/094_mangue_historico_tags.png
    :alt: Histórico de tags 
    :scale: 80 %
    :align: center
=====  

Na seção de Histórico de Faturamento Mensal por Tags, o usuário deve primeiramente selecionar um Cluster, para que a plataforma consiga carregar as Tags do Cluster. Após isso, o usuário pode selecionar o período desejado de faturamento e as Tags a serem exibidas em gráfico e na seção de Detalhes de Tags.

.. image:: /figuras/fig_mangue/095_mangue_detalhes_tag.png
    :alt: Detalhes tag
    :scale: 80 %
    :align: center
=====


Na seção de Detalhes de Tags, é exibida uma lista com todas as Tags ou as Tags selecionadas na seção de Histórico de Faturamento Mensal por Tags. No detalhamento da Tag, é apresentada uma lista de aplicações com a Tag e um gráfico com o faturamento da Tag nos últimos 30 dias. 

O usuário pode excluir uma Tag clicando no botão “  ”, no detalhamento da Tag.


D. Alertas
~~~~~~~~~~

Por meio de alertas, é possível ser notificado quando atingir o orçamento estabelecido para um deployment ou conjunto de deployments, quando agrupados em tags, além de conseguir configurar ações que devem ser executadas quando o orçamento para esses recursos for atingido. Isso possibilita ao usuário ter mais controle sobre o custo com cada serviço. A tela de alertas contém duas listas, a lista de alertas e de webhooks, como pode ser visualizado na imagem abaixo:

.. image:: /figuras/fig_mangue/096_mangue_alertas_webhooks.png
    :alt: Alertas webhooks 
    :scale: 80 %
    :align: center
=====



                                                                     * Alertas: Exibe uma lista de alertas, com as seguintes colunas:
                                                                     * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                     * Nome: Esta coluna apresenta o nome do alerta definido no momento de criação do mesmo. Ao selecionar este campo é apresentado na tela informações sobre o alerta, nela o usuário consegue visualizar uma barra de progresso, actions e webhooks selecionados no momento de criação do alerta. Como pode ser visto na imagem abaixo:
  
  .. image:: /figuras/fig_mangue/097_mangue_alert.png
    :alt: Alerta 
    :scale: 80 %
    :align: center
=====

                                                                        * Barra de progresso: Corresponde ao valor atual dos deployments associados ao alerta, tendo como 100% o valor de orçamento do alerta.
                                                                        * Actions: Action que será executada no momento em que os deployments associados a um alerta atingirem o preço de orçamento.
                                                                        * Webhooks: Webhook que será executado no momento em que os deployments associados a um alerta atingirem o preço de orçamento.
                                                                        * Aplicação: Esta coluna apresenta o deployment ou conjunto de deployments selecionados para o alerta correspondente no momento de criação do alerta.
                                                                        * Status: Esta coluna apresenta dois valores possíveis, “DONE” e “PENDING”:
                                                                        * DONE: Indica que o alerta já atingiu o preço do orçamento e que foi executado, disparando os webhooks e actions configurados.
                                                                        * PENDING: Indica que o alerta não foi executado.
                                                                        * Data: Esta coluna apresenta a data de criação do alerta
                                                                        * Cota Alerta: Esta coluna apresenta o preço de orçamento definido para o alerta.
                                                                        * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta uma única opção para “deletar alerta”:
.. image:: /figuras/fig_mangue/098_mangue_deletar_alerta.png
    :alt: Deletar alerta 
    :scale: 80 %
    :align: center
=====
          
                                                                           * Deletar Alerta: Quando o usuário seleciona esta ação a plataforma do Mangue.io irá solicitar confirmação do usuário para remover (apagar) o alerta desejado da base de dados da plataforma do Mangue.io:
  
.. image:: /figuras/fig_mangue/099_mangue_aviso_deletar.png
    :alt: Aviso deletar 
    :scale: 80 %
    :align: center
=====


Nesta seção de alertas é possível visualizar o ícone de adicionar alerta, como no exemplo seguinte “  ”, ao clicar no botão será apresentado um formulário para o usuário com campos que possibilitam a criação de um alerta, seguindo um fluxo de três etapas, detalhes, webhook e actions:
                                                                           * Detalhes: Nesta etapa é solicitado informações voltadas para o alerta especificamente, são solicitadas as seguintes informações:
                                                                           * Nome: Campo correspondente ao nome do alerta
                                                                           * Descrição: Campo correspondente à descrição do alerta
                                                                           * Tipo: Existem dois valores possíveis para o tipo, por Tag para selecionar um conjunto de deployments, e Deployment para selecionar apenas um deployment. Ao selecionar a tag ou deployment ocorre uma busca do valor de custo total correspondente ao deployment ou tag selecionada, esse valor é apresentado no campo de Custo Atual presente na tela.
                                                                           * Prazo: Neste campo pode ser definido um prazo para execução do alerta, alertas mesmo com status pending não serão executados após o prazo definido para o alerta.
                                                                           * Orçamento: Neste campo pode ser informado o preço de orçamento do alerta, quando o custo total da soma dos deployments selecionados atingir o valor informado neste campo o alerta será executado. O Valor de Orçamento precisa ser maior que o valor de Custo Atual
  .. image:: /figuras/fig_mangue/100_mangue_alerta_detalhes.png
    :alt: Alerta detalhes 
    :scale: 80 %
    :align: center
=====

                                                                           * Webhook: Nesta etapa há uma lista de webhooks, o usuário poderá selecionar nenhum ou vários webhooks. Ao selecionar um webhook ele será listado abaixo para que o usuário informe o tipo de retorno que será executado, podendo escolher HTTP ou E-mail.
.. image:: /figuras/fig_mangue/101_mangue_alerta_webhook.png
    :alt: Alerta webhook 
    :scale: 80 %
    :align: center
=====  

                                                                           * Ações: Nesta etapa é possível selecionar uma ação para ser executada no momento de execução do alerta, existem três valores que o usuário poderá selecionar para ação, como no exemplo da imagem abaixo:
  .. image:: /figuras/fig_mangue/102_mangue_alerta_acoes.png
    :alt: Alerta ações 
    :scale: 80 %
    :align: center
=====

                                                                           * Escalonamento da Aplicação: Esta ação permite que o usuário configure a troca da quantidade de réplicas em execução das aplicações selecionadas. No momento em que o alerta for executado, possibilita reduzir/aumentar a quantidade de instâncias de uma aplicação, de forma alinhada ao custo atual da mesma aplicação. Exemplo na imagem a seguir:
  
  .. image:: /figuras/fig_mangue/103_mangue_escalonamento_aplicacao.png
    :alt: Escalonamento aplicação 
    :scale: 80 %
    :align: center
=====

                                                                           * Alterar Request e Limits: Esta ação permite que o usuário altere o request e limite das aplicações selecionadas, a partir do momento em que o alerta for executado. Exemplo na imagem a seguir:
  .. image:: /figuras/fig_mangue/104_mangue_alterar_request_limit.png
    :alt: Alterar request limit 
    :scale: 80 %
    :align: center
=====

                                                                           * Parar Aplicação: Também é possível parar as aplicações selecionadas, a partir do momento em que o alerta for executado. Para isso, é necessário clicar em “Confirmar parada da aplicação”.
  
.. image:: /figuras/fig_mangue/105_mangue_parar_aplicacao.png
    :alt: Parar aplicação 
    :scale: 80 %
    :align: center
=====


Lembrar que ao menos um webhook ou uma ação deve ser informada para possibilitar a criação do alerta.

                                                                           * Webhooks: O webhook é uma forma de envio de informações para algum destino quando um evento acontecer, neste caso quando os deployments relacionados ao alerta atingem o preço de orçamento definido na criação do alerta, o Webhook dispara as informações. O Mangue.io fornece duas formas para o envio das informações, por meio do protocolo HTTP, e/ou por meio de Email.
Um webhook pode conter as duas formas de retorno, no entanto no momento de criar um alerta e associar ao webhook existente é necessário escolher uma das formas (HTTP ou Email) para envio de informações no momento de execução do alerta

.. image:: /figuras/fig_mangue/106_mangue_webhooks.png
    :alt: Webhoooks 
    :scale: 80 %
    :align: center
=====

                                                                           * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                           * Nome: Esta coluna apresenta o nome do webhook definido no momento de criação dele.
                                                                           * Método: Esta coluna apresenta o método HTTP selecionado no momento de criação do webhook, podendo haver os seguintes valores: “GET”, “POST”, “PUT”, “DELETE”, “PATCH”.
                                                                           * Url: Esta coluna apresenta url de destino para envio da mensagem.
                                                                           * Body:Esta coluna apresenta o corpo da requisição HTTP
                                                                           * Email: Esta coluna apresenta o email de destino para envio de mensagem por email.
                                                                           * Alertas: Esta coluna apresenta uma lista de alertas que estão relacionados ao webhook correspondente
                                                                           * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta as opções abaixo:
  
.. image:: /figuras/fig_mangue/107_mangue_acoes_webhook.png
    :alt: 
    :scale: 80 %
    :align: center
=====
        
                                                                              * Deletar Webhook: Quando o usuário seleciona esta ação a plataforma do Mangue.io solicita confirmação do usuário para remover (apagar) o alerta desejado da base de dados da plataforma do Mangue.io:
.. image:: /figuras/fig_mangue/108_mangue_deletar_webhook.png
    :alt: Deletar webhook 
    :scale: 80 %
    :align: center
=====

                                                                              * Editar Webhook: Quando o usuário seleciona esta ação a plataforma do Mangue.io apresenta o formulário presente na imagem abaixo com as informações do webhook, para que o usuário possa editar.
.. image:: /figuras/fig_mangue/109_mangue_editar_webhook.png
    :alt: Editar webhook 
    :scale: 80 %
    :align: center
=====

                                                                              * Nome: Neste campo deve ser informado o nome do webhook
                                                                              * Método: Neste campo pode ser informado o método para requisição HTTP
                                                                              * URL: Neste campo pode ser informado a url para requisição HTTP
                                                                              * Body: Neste campo pode ser informado o body para requisição HTTP
                                                                              * Email: Neste campo pode ser informado o email para envio de mensagens.
                                                                              * Mensagem:  Neste campo pode ser informada a mensagem que é enviada para o email informado no campo anterior.


Nesta seção de webhooks é possível visualizar o ícone de adicionar webhook, como no exemplo seguinte “  ”, ao clicar no botão será apresentado um formulário para adicionar o webhook, é exatamente igual ao formulário apresentado para editar webhook.




Recomendações
=============

A plataforma Mangue.io pode realizar recomendações para otimizar a utilização de CPU e memória das aplicações do Cluster, com o objetivo de evitar desperdício. No Kubernetes realiza a alocação de recursos a uma aplicação utilizando os seguintes conceitos:
                                                                              * Request: Quantidade mínima de recurso alocado à aplicação. Exemplo: uma aplicação com memory request de 256 MB sempre tem alocada essa quantidade de memória, mesmo se aplicação sempre utilizar apenas 20 MB.
                                                                              * Limit: Caso a aplicação precise utilizar mais recursos do que especificado em Request, o Kubernetes tenta alocar mais recursos caso a máquina Nó tenha disponível. É possível limitar a quantidade de recursos que o Kubernetes tenta alocar a aplicação utilizando Limit. Exemplo: uma aplicação com request de 256 MB e limit de 512 MB sempre tem alocada a ela 256 MB, se ela precisar de mais memória ela pode ser alocada até 512 MB e caso isso não seja o suficiente a aplicação fica sem memória, podendo causar lentidão ou instabilidade na aplicação.
A plataforma realiza a otimização analisando as métricas históricas de uso de CPU e memória, assim verificando se uma aplicação está com mais recurso alocado que necessário ou com recursos insuficientes para manter a estabilidade.

.. image:: /figuras/fig_mangue/110_mangue_recomendacoes.png
    :alt: Recomendações 
    :scale: 80 %
    :align: center
=====  

Na página de recomendações é exibida uma lista com as aplicações no namespace e Cluster atual, e, é possível pesquisar recomendações através do nome da aplicação.
Abaixo descrevemos as informações presentes na tabela de tarefas agendadas.
                                                                              * #: Número sequencial da recomendação cadastrada na Plataforma do Mangue.io.
                                                                              * App: Nome da aplicação com a recomendação.
                                                                              * CPU Request Atual/Ideal: Indica o valor atual e recomendado de CPU Request. Caso não haja recomendação nessa coluna é exibido “- / -”.
                                                                              * CPU Limit Atual/Ideal: Indica o valor atual e recomendado de CPU Limit. Caso não haja recomendação nessa coluna será exibido “- / -”.
                                                                              * Memory  Request Atual/Ideal: Indica o valor atual e recomendado de Memory Request. Caso não haja recomendação nessa coluna será exibido “- / -”.
                                                                              * Memory Limit Atual/Ideal: Indica o valor atual e recomendado de Memory Limit. Caso não haja recomendação nessa coluna será exibido “- / -”.
                                                                              * Ações: Esta coluna possui os seguintes elementos: 
                                                                              * um botão de “Aplicar”, que ao ser clicado os valores recomendados na aplicação.
                                                                              * um botão de ação “  ” que ao ser clicado, apresenta as seguinte opção:

.. image:: /figuras/fig_mangue/111_mangue_descartar_recomendacao.png
    :alt: Descartar recomendação 
    :scale: 80 %
    :align: center
===== 

                                                                                 * Descartar recomendação atual: Ao selecionar a opção de descartar a recomendação selecionada é removida, e é exibida uma recomendação anterior caso tenha.
                                                                                 * um botão de “Mais Sugestões”, que ao clicar redireciona para uma página onde será exibido uma lista com  as recomendações geradas anteriormente.
  

.. image:: /figuras/fig_mangue/112_mangue_historico_recomendacao.png
    :alt: Histórico sugestão recomendação 
    :scale: 80 %
    :align: center
=====

Permissões
==========

Todos os pontos descritos neste segmento, estão armazenados na base de dados que suporta a instalação da plataforma do Mangue.io. Esta base de dados, e seu conteúdo, deve ser gerenciado e alterado no prompt do sistema operacional Linux dos servidores (máquinas virtuais) que suportam a infraestrutura da plataforma do Mangue.io.
Durante o processo de implantação padrão da plataforma do Mangue.io, é instalado um gerenciador de base de dados (MariaDB / MySQL) e o conteúdo desta base de dados e seus registros referentes a Clusters, Permissões, Billing, Contratos, ClusterRole, ClusterRoleBinding, Service e ServiceAccount, são populados durante o processo de pós-instalação do software.
Não é objeto deste documento descrever o processo de inclusão de novos registros na base de dados da plataforma do Mangue.io, entre em contato com a área de suporte da Ustore para que você possa ter acesso ao documento “Manual de Instalação do Mangue.io (veja item: Conteúdo Padrão do Banco de Dados)”.
Nas próximas telas descrevemos como a interface da plataforma do Mangue.io apresenta o conteúdo da base de dados através da interface HTML do Mangue.io.


Contrato
--------

Abaixo está a tela que apresenta informações sobre o contrato selecionado no menu de configurações, é possível visualizar informações sobre o contrato e informações sobre os usuários do contrato.

.. image:: /figuras/fig_mangue/113_mangue_informacoes_contrato_user.png
    :alt: Informações contrato user 
    :scale: 80 %
    :align: center
=====  

A. Informações do contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~

É possível visualizar os administradores do contrato, preço por CPU e preço por memória definidos para o contrato.
                                                                                 
B. Informações de usuários
~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta seção são listadas as informações sobre os usuários do contrato, e o nível de permissão de cada usuário. As permissões por usuário refletem o nível de permissão atribuído para um usuário no uCloud, seguindo o exemplo da tabela abaixo:


uCloud
	Mangue.io
	Administrador de contrato
	cluster-admin
	Usuário comum
	edit

.. image:: /figuras/fig_mangue/114_mangue_tabela_ucloud.png
    :alt: Tabela uCloud Mangue.io 
    :scale: 80 %
    :align: center
=====	

Caso tenha ocorrido alguma mudança de permissão em algum dos usuários, seja usuário removido do contrato, usuário adicionado ao contrato, ou até mesmo nível de permissão alterada, há uma rotina para sincronizar as permissões dos usuários com o uCloud, refletindo tais mudanças no Mangue.io. No entanto, caso tenha o interesse de executar a sincronização das permissões naquele exato momento, há um botão ao lado direito, com nome “Sync users”   , ao clicar é executada a mesma função para sincronização de permissões que seria executada pela rotina.

Por meio da lista de usuários é possível extrair as seguintes informações:
                                                                                 * Login: Este campo apresenta o login do usuário que foi provisionado na base de dados da plataforma do Mangue.io.
                                                                                 * Role: Esta coluna apresenta o perfil de autorização (role) do usuário provisionado.
                                                                                 * Service Account: Esta coluna apresenta o service account associado ao usuário
                                                                                 * Cluster Role: Esta coluna apresenta o cluster role associado ao usuário
                                                                                 * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, exibe a seguinte opção como a figura abaixo:
  
.. image:: /figuras/fig_mangue/115_mangue_deletar_permissoes.png
    :alt: Deletar permissões 
    :scale: 80 %
    :align: center
=====
                                                                                    * Deletar Permissões: Quando o usuário selecionar esta ação ele remove as permissões do usuário correspondente a linha selecionada. A plataforma do Mangue.io solicita a confirmação para deletar a permissão do usuário no Mangue.io, conforme imagem abaixo:
  
.. image:: /figuras/fig_mangue/116_mangue_aviso_permissao.png
    :alt: Aviso permissão 
    :scale: 80 %
    :align: center
=====


Roles
-----

O controle de acesso baseado em funções/perfil (Role Based Access Control - RBAC) é um método de regular o acesso a recursos de computador ou rede com base nas funções de usuários individuais em sua organização.
Uma RBAC role (permissão/perfil) ou ClusterRole contém regras que representam um conjunto de permissões.
Uma role sempre define permissões em um namespace específico; ao criar uma role, você deve especificar o namespace ao qual ela pertence.

A. Seção: Roles
~~~~~~~~~~~~~~~

Nesta seção o usuário pode ver a lista de todas as roles existentes no cluster que foi selecionado na aba engrenagens “   Seleção de Configuração”.
  
.. image:: /figuras/fig_mangue/117_mangue_roles.png
    :alt: Roles 
    :scale: 80 %
    :align: center
=====


                                                                                    * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                    * Nome: Nesta coluna é apresentado o nome do role adicionado pelo usuário.
                                                                                    * Labels: Labels são usados para especificar a identificação de atributos de objetos que são significativos e relevantes e presentes na sintaxe yaml da role.
                                                                                    * Duração: Esta coluna apresenta o tempo decorrido em dias desde o momento da aplicação inicial desta role.
                                                                                    * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções assim como a figura abaixo:
  
.. image:: /figuras/fig_mangue/118_mangue_acoes_role.png
    :alt: Ações Role 
    :scale: 80 %
    :align: center
=====


                                                                                       * Deletar Role: Quando o usuário seleciona esta ação ele remove a role do cluster que foi selecionado na aba engrenagens “   Seleção de Configuração”. Vale lembrar que esta ação é irreversível e definitiva. A plataforma do Mangue.io solicita confirmação do usuário para remover (apagar) o grupo desejado da base de dados da plataforma do Mangue.io:
  

.. image:: /figuras/fig_mangue/119_mangue_deletar_role.png
    :alt: Deletar role 
    :scale: 80 %
    :align: center
=====

Caso o usuário tenha executado esta ação por engano, é necessário cadastrar o grupo na base de dados da plataforma do Mangue.io via qualquer ferramenta de SSH; A ação de incluir configurações na base de dados é feita através de linha de comando no sistema operacional Linux da máquina virtual que suporta a execução da plataforma do Mangue.io.


                                                                                          * Editar Role: Recomendamos que somente usuários experientes em sintaxe YAML faça as alterações em uma role, pois a codificação (ou alteração) da sintaxe de forma errônea pode acarretar perda de acesso a todo o ambiente de clusters existentes.
Esta opção abre uma tela de edição da role usando a sintaxe de código YAML, como o exemplo da tela abaixo.
  
.. image:: /figuras/fig_mangue/120_mangue_editar_role.png
    :alt: Editar role 
    :scale: 80 %
    :align: center
=====


O usuário deve iniciar clicando com o mouse na área cinza ao lado do número da linha que deseja editar, antes de iniciar a digitação do seu código YAML. A cada nova linha o usuário deve usar a tecla “Enter” para iniciar uma nova linha. O usuário deve utilizar a sua própria experiência de desenvolvimento para estruturar a sintaxe de seu código linha a linha. Através desta opção o usuário poderá entrar (ou editar) com um código YAML para criar, para editar a role na plataforma do Mangue.io.

Após editar a role o usuário deverá clicar no botão verde “Enviar” para que todo o código seja enviado e aplicado ao cluster que foi selecionado na aba engrenagens “   Seleção de Configuração”.


B. Seção: Role Bindings
~~~~~~~~~~~~~~~~~~~~~~~

Uma vinculação de função/perfil (rolebinding) concede as permissões definidas em uma role a um usuário ou conjunto de usuários. Ele contém uma lista de assuntos (usuários, grupos ou contas de serviço) e uma referência ao role que está sendo concedido. Um RoleBinding concede permissões dentro de um namespace específico, enquanto um ClusterRoleBinding concede esse acesso a todo o cluster.
Um RoleBinding pode fazer referência a qualquer papel no mesmo namespace. Como alternativa, um RoleBinding pode fazer referência a um ClusterRole e vincular um ClusterRole ao namespace do RoleBinding. Se você deseja vincular um ClusterRole a todos os namespaces em seu cluster, use um ClusterRoleBinding.
  
.. image:: /figuras/fig_mangue/121_mangue_bindings.png
    :alt: Bindings 
    :scale: 80 %
    :align: center
=====


                                                                                          * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                          * Nome: Nesta coluna é apresentado o nome da rolebinding adicionado pelo usuário. Ao clicar com o mouse sobre o nome do configmap a plataforma do Mangue.io apresenta uma tela com o(s) conteúdo(s) do(s) arquivo(s) de configmap. Por padrão será apresentado somente a visualização de uma linha do conteúdo do arquivo, caso o conteúdo seja maior do que o campo, o usuário pode posicionar o mouse no canto inferior direito, até que o curso o mouse mude para uma seta diagonal dupla (“  ”), que irá permitir ao usuário redimensionar o tamanho do campo de conteúdo listado, para acomodar o tamanho que for adequado ao usuário, para a melhor visualização deste campo.
                                                                                          * Labels: Labels são usados para especificar a identificação de atributos de objetos que são significativos e relevantes e presentes na sintaxe yaml da role
                                                                                          * Duração: Esta coluna apresenta o tempo decorrido em dias desde o momento da aplicação inicial desta rolebinding
                                                                                          * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções assim como a figura abaixo:
  
.. image:: /figuras/fig_mangue/122_mangue_acoes_bindings.png
    :alt: Ações Bindings 
    :scale: 80 %
    :align: center
=====


                                                                                             * Deletar RoleBinding: Quando o usuário seleciona esta ação ele remove a rolebinding do cluster que foi selecionado na aba engrenagens “   Seleção de Configuração”. Vale lembrar que esta ação é irreversível e definitiva. A plataforma do Mangue.io solicita confirmação do usuário para remover (apagar) a rolebinding desejada da base de dados da plataforma do Mangue.io:
  
.. image:: /figuras/fig_mangue/123_mangue_aviso_bindings.png
    :alt: Aviso bindings
    :scale: 80 %
    :align: center
=====


Caso o usuário tenha executado esta ação por engano, será necessário cadastrar a rolebinding na base de dados da plataforma do Mangue.io via qualquer ferramenta de SSH; A ação de incluir configurações na base de dados é feita através de linha de comando no sistema operacional Linux da máquina virtual que suporta a execução da plataforma do Mangue.io.


                                                                                                * Editar Rolebinding: Recomendamos que somente usuários experientes em sintaxe YAML faça as alterações em uma rolebinding, pois a codificação (ou alteração) da sintaxe de forma errônea pode acarretar perda de acesso a todo o ambiente de clusters existentes.
Esta opção abre uma tela de edição da rolebinding usando a sintaxe de código YAML, como o exemplo da tela abaixo.
  
.. image:: /figuras/fig_mangue/124_mangue_editar_binding.png
    :alt: Editar bindings 
    :scale: 80 %
    :align: center
=====


O usuário deve iniciar clicando com o mouse na área cinza ao lado do número da linha que deseja editar, antes de iniciar a digitação do seu código YAML. A cada nova linha o usuário deve usar a tecla “Enter” para iniciar uma nova linha. O usuário deve utilizar a sua própria experiência de desenvolvimento para estruturar a sintaxe de seu código linha a linha. Através desta opção o usuário poderá entrar (ou editar) com um código YAML para criar, para editar a rolebinding na plataforma do Mangue.io.

Após editar a rolebinding o usuário deve clicar no botão verde “Enviar” para que todo o código seja enviado e aplicado ao cluster que foi selecionado na aba engrenagens “   Seleção de Configuração”.


Service Accounts
----------------

Quando um usuário acessa o cluster, você é autenticado pelo APIServer como uma conta de usuário específica (atualmente, geralmente é admin, a menos que o administrador do cluster tenha personalizado seu cluster). Os processos em containers dentro de PODs também podem entrar em contato com o APIServer. Quando o fazem, eles são autenticados como uma conta de serviço específica (por exemplo, default).
  
.. image:: /figuras/fig_mangue/125_mangue_service_account.png
    :alt: Service account 
    :scale: 80 %
    :align: center
=====


                                                                                                * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                                * Nome: Nesta coluna é apresentado o nome da serviceaccount adicionado pelo usuário. 
                                                                                                * Namespace: Informa o namespace em que o serviceaccount  foi criado.
                                                                                                * Duração: Esta coluna apresenta o tempo decorrido em dias desde o momento da aplicação inicial desta serviceaccount
                                                                                                * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta uma única opção como a figura abaixo:
  



                                                                                                   * Deletar ServiceAccount: Quando o usuário seleciona esta ação ele irá remover a serviceaccount do cluster que foi selecionado na aba engrenagens “   Seleção de Configuração”. Vale lembrar que esta ação é irreversível e definitiva. A plataforma do Mangue.io irá solicitar confirmação do usuário para remover (apagar) a servceaccount desejada da base de dados da plataforma do Mangue.io:
  

.. image:: /figuras/fig_mangue/.png
    :alt: 
    :scale: 80 %
    :align: center
=====

Caso o usuário tenha executado esta ação por engano, é necessário cadastrar a serviceaccount na base de dados da plataforma do Mangue.io via qualquer ferramenta de SSH; A ação de incluir configurações na base de dados é feita através de linha de comando no sistema operacional Linux da máquina virtual que suporta a execução da plataforma do Mangue.io.


Cluster Role
------------

Uma RBAC role ou ClusterRole contém regras que representam um conjunto de permissões.
ClusterRole, por outro lado, é um recurso sem espaço de nomes. Os recursos têm nomes diferentes (Role e ClusterRole) porque um objeto Kubernetes sempre precisa ter namespace ou não; não pode ser ambos.
ClusterRole tem vários usos, você pode usá-lo para:
                                                                                                      * Definir permissões em recursos com namespace e ser concedido dentro de namespaces individuais;
                                                                                                      * Definir permissões em recursos com namespaces e ser concedido em todos os namespaces;
                                                                                                      * Definir permissões em recursos com escopo de cluster;
Se você quiser definir uma função em um namespace, use uma role; se você quiser definir uma role em todo o cluster, use um ClusterRole.
O usuário nota que esta tela possui diversas seções, cada seção está descrita abaixo respectivamente.

A. Seção: Cluster Roles
~~~~~~~~~~~~~~~~~~~~~~~

Nesta tela a plataforma do Mangue.io apresenta a lista de todas as Cluster Roles configuradas e o tempo desde sua criação.
  
.. image:: /figuras/fig_mangue/.png
    :alt: 
    :scale: 80 %
    :align: center
=====


                                                                                                      * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                                      * Nome: Nesta coluna é apresentado o nome da Cluster Roles adicionado pelo usuário. 
                                                                                                      * Labels: Labels são usados para especificar a identificação de atributos de objetos que são significativos e relevantes e presentes na sintaxe yaml da role.
                                                                                                      * Duração: Esta coluna apresenta o tempo decorrido em dias desde o momento da aplicação inicial desta Cluster Roles.
                                                                                                      * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta uma única opção como a figura abaixo:
  
.. image:: /figuras/fig_mangue/.png
    :alt: 
    :scale: 80 %
    :align: center
=====


                                                                                                         * Editar Cluster Role: Recomendamos que somente usuários experientes em sintaxe YAML faça as alterações em uma Cluster Role, pois a codificação (ou alteração) da sintaxe de forma errônea pode acarretar perda de acesso a todo o ambiente de clusters existentes.
Esta opção abre uma tela de edição da Cluster Role usando a sintaxe de código YAML, como o exemplo da tela abaixo. O código de uma Cluster Role pode ser longo, e esta tela ser muito longa, apresentamos aqui apenas algumas linhas da tela.
  
.. image:: /figuras/fig_mangue/.png
    :alt: 
    :scale: 80 %
    :align: center
=====


Ao clicar com o mouse na área cinza ao lado do número da linha que o usuário deseja editar, em seguida pode iniciar a digitação do seu código YAML. 
A cada nova linha o usuário deve clicar “Enter” para abrir outra linha. 
Indica-se ao usuário utilizar a sua própria experiência de desenvolvimento para estruturar a sintaxe de seu código linha a linha. 
Em resumo, a Cluster Role proporciona a opção de criar ou editar o código YAML na plataforma do Mangue.io.
Após editar a Cluster Role o usuário deve clicar no botão verde “Enviar” para que todo o código seja enviado e aplicado ao cluster que foi selecionado na aba engrenagens “   Seleção de Configuração”.




B. Seção: Cluster Role Binding
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nesta tela a plataforma do Mangue.io apresenta a lista de todas as Cluster Role Binding configuradas e o tempo desde sua criação.
  
.. image:: /figuras/fig_mangue/.png
    :alt: 
    :scale: 80 %
    :align: center
=====


                     * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                     * Nome: Nesta coluna é apresentado o nome da Cluster Role Binding adicionado pelo usuário. 
                    * Labels: Labels são usados para especificar a identificação de atributos de objetos que são significativos e relevantes e presentes na sintaxe yaml da role.
                    * Duração: Esta coluna apresenta o tempo decorrido em dias desde o momento da aplicação inicial desta ClusterRole Binding.
                     * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta uma única opção como a figura abaixo:
  
.. image:: /figuras/fig_mangue/.png
    :alt: 
    :scale: 80 %
    :align: center
=====


                                     * Editar Cluster Role Binding: Recomendamos que somente usuários experientes em sintaxe YAML faça as alterações em uma Cluster Role Binding, pois a codificação (ou alteração) da sintaxe de forma errônea pode acarretar perda de acesso a todo o ambiente de clusters existentes.

Esta opção abre uma tela de edição da Cluster Role Binding usando a sintaxe de código YAML, como o exemplo da tela abaixo.
  
.. image:: /figuras/fig_mangue/.png
    :alt: 
    :scale: 80 %
    :align: center
=====


O usuário deve iniciar clicando com o mouse na área cinza ao lado do número da linha que deseja editar, antes de iniciar a digitação do seu código YAML.

A cada nova linha o usuário deve usar a tecla “Enter” para iniciar uma nova linha. O usuário deve utilizar a sua própria experiência de desenvolvimento para estruturar a sintaxe de seu código linha a linha. 

Através desta opção o usuário poderá entrar (ou editar) com um código YAML para criar, para editar a Cluster Role Binding na plataforma do Mangue.io.

Após editar a Cluster Role Binding o usuário deverá clicar no botão verde “Enviar” para que todo o código seja enviado e aplicado ao cluster que foi selecionado na aba engrenagens “   Seleção de Configuração”.


C. Pod Security Policy
~~~~~~~~~~~~~~~~~~~~~~

Pod Security Policy é um recurso do Kubernetes que permite o usuário limitar as aplicações criadas por um ServiceAccount específico, ou todos. Sendo assim possível, por exemplo, proibir que um ServiceAccount crie uma aplicação que utilize o usuário root.
A tela de Pod Security Policy é separada em duas seções: 
                   * Pod Security Policy.
                   * Cluster Role e Role Binding de Pod Security Policy.
  

Na seção de Pod Security Policy é exibido uma lista com os Pod Security Policy do Cluster e é exibido uma barra de pesquisa para pesquisar utilizando o nome.
Abaixo descrevemos as informações presentes na tabela de Pod Security Policy.
                       * #: Número sequencial do Pod Security Policy cadastrado na Plataforma do Mangue.io.
                       * Nome: Nome do Pod Security Policy especificado pelo usuário durante a criação.
                       * Privilegiado: Permite que as aplicações criadas utilizem recursos e capacidades Kernel da máquina Host.
                       * Permite Escalada de Privilégios: Permite que a aplicação criada altere o seu ID de Usuário, possibilitando que processos filhos do container ganhem mais privilégios que o processo pai.
                       * ID Usuário: Faixa de ID de Usuário que as aplicações criadas podem utilizar na execução.
                       * ID Grupo: Faixa de ID de Grupo que as aplicações criadas utilizam na execução.
                       * ID Arquivo de Sistemas: Faixa ID de Arquivo de Sistema que as aplicações criadas utilizam na execução.
                       * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções como a figura abaixo:
  

                                                                                                                                              * Criar Cluster Role: Ao selecionar a opção de criar cluster role é     apresentada a tela abaixo, através da qual o usuário pode criar um Cluster Role para o Pod Security Policy.
                                                                                                                                              * Deletar Pod Security Policy: Ao selecionar a opção de excluir é deletado o Pod Security Policy do Cluster.
  

Para criar um Pod Security Policy é necessário clicar no botão de “  ”, ao clicar é exibido a tela abaixo.
  

Os campos necessários para a criação de Pod Security Policy são os seguintes:
                                                                                                               * Nome do Pod Security Policy: Nome do Pod Security Policy a ser criado.
                                                                                                               * Permitir Containers Privilegiados: Permite a criação de recursos que utilizam containers privilegiados, esses containers podem ter acesso aos recursos e capacidades Kernel da máquina Host.
                                                                                                               * Permitir Escalada de Privilégios: Permite que a aplicação criada altere o seu ID de Usuário, possibilitando que processos filhos do container ganhem mais privilégios que o processo pai.
                                                                                                               * Limitar Usuário: Caso seja selecionado é exibido uma lista (“drop-down list”), com as opções de: 
                                                                                                               * Proibir Root: essa opção permite a criação de aplicação que utilize qualquer ID de usuário, com a exceção do ID do usuário root.
                                                                                                               * Limitar por ID de Usuário, essa opção limita a criação de aplicação para que utilize apenas uma faixa de ID de usuário especificada.
                                                                                                               * Limitar Grupo: Permite apenas aplicações que utilizem a faixa de ID de Grupo especificada.
                                                                                                               * Limitar Arquivo de Sistema: Permite apenas aplicações que utilizem a faixa de ID de Arquivo de Sistema especificada.
Após preencher todos os campos obrigatórios, o botão de “Adicionar Pod Security Policy” está disponível e quando o usuário clicar nele a plataforma cria o Pod Security Policy e exibe uma mensagem de status.
Na seção de Cluster Role e Role Binding de Pod Security Policy é exibido uma lista com os Cluster Role e Role Bindings dos Pod Security Policy e é exibido uma barra de pesquisa para pesquisar utilizando o nome dos recursos.
Abaixo a descrição das informações presentes na tabela de Pod Security Policy.
                                                                                                               * #: Número sequencial do Cluster Role cadastrado na Plataforma do Mangue.io.
                                                                                                               * Cluster Role: Nome do Cluster Role especificado pelo usuário durante a criação.
                                                                                                               * Pod Security Policy: Nome do Pod Security Policy associado ao Cluster Role.
                                                                                                               * Permite Escalada de Privilégios: Permite que a aplicação criada altere o seu ID de Usuário, possibilitando que processos filhos do container ganhem mais privilégios que o processo pai.
                                                                                                               * Role Binding: Nome do Role Binding associado ao Cluster Role.
                                                                                                               * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções como a figura abaixo:
  

                                                                                                                  * Criar Role Binding: Ao selecionar a opção de criar cluster role é apresentada a tela abaixo, através da qual o usuário pode criar um Role Binding associando o Cluster Role a ServiceAccounts.
                                                                                                                  * Deletar Role Binding: Caso tenha um Role Binding associado ao Cluster Role é exibido a opção de deletar o Role Binding, ao selecionar a opção o Role Binding é deletado.
                                                                                                                  * Deletar Cluster Role: Ao selecionar a opção de excluir é deletado o Cluster Role selecionado.
  



Integrações
===========

Através deste menu Integrações, o usuário pode conectar a plataforma do Mangue.io com entidades, serviços e provedores externos. 
Estas integrações permitem ao usuário ampliar a abrangência da plataforma do Mangue.io conectando e integrando a atual infraestrutura, a qual suporta e executa a instalação do Mangue.io com os gerenciadores de containers em provedores públicos. Este menu vem como propósito de tratar outras questões além da simples gestão do Kubernetes, como por exemplo:
                                                                                                                  * Integração via linha de comando nos containers executados no cluster;
                                                                                                                  * Criação de clusters Kubernetes nas nuvens públicas das AWS e Google;
                                                                                                                  * Importar clusters Kubernetes já existentes;
                                                                                                                  * Importar credenciais para que os procedimentos de criação de clusters nas nuvens públicas sejam mais facilmente efetuadas.


1. Clusters
~~~~~~~~~~~

O menu Integrações/Clusters permite ao usuário integrar a plataforma do Mangue.io a um cluster existente, que pode estar ativo em outra infraestrutura computacional, à plataforma do Mangue.io. Além disso, esta tela apresenta uma lista com as informações dos clusters integrados ao Mangue.io
O menu Integrações/Cluster permite fazer todo o gerenciamento e integração dos Clusters Kubernetes gerenciados pela plataforma a partir de um usuário. Neste menu é possível provisionar clusters Kubernetes nas infraestruturas da Amazon e Google (EKS e GKE), lembrando que para provisionar esses clusters é necessário adicionar uma credencial no menu Integrações/Credenciais. 
Também é possível adicionar um cluster Kubernetes que não tenha sido provisionado na plataforma, seja ele no seu ambiente On Premise ou na nuvem. Vale ressaltar que clusters que tiverem as APIS do Kubernetes modificadas, podem não corresponder positivamente às chamadas das APIS do Kubernetes feitas pelo Mangue.io.
  



Na lista pode-se encontrar as informações de cada cluster configurado e integrado a plataforma do Mangue.io:
                                                                                                                  * Nome: Nesta coluna é apresentado o nome que foi utilizado para identificar o Cluster durante o processo de configuração pelo usuário.
                                                                                                                  * IP Público: Esta coluna apresenta a informação do endereço TCP-IP Público do cluster. Este é o endereço pelo qual o cluster pode ser utilizado para acessar as aplicações (deployments) que estão sendo executadas neste cluster.
                                                                                                                  * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta uma única opção como a figura abaixo:
  



                                                                                                                     * Editar Cluster: Nesta opção o usuário pode editar as características de um cluster existente e quando selecionado a plataforma apresenta a tela abaixo:


  



Nome do Cluster: Neste campo o usuário pode alterar o nome de referência com o qual o cluster está configurado.
IP para acesso da API: Neste campo o usuário pode alterar o endereço TCP-IP Público para que o cluster seja possível ser acessado.
Porta para acesso da API: Neste campo o usuário pode alterar a PORTA TCP-IP para que seja possível acessar o cluster.
Cluster Admin Token: Neste campo o usuário pode alterar a cadeia de caracteres (string) que foi gerada pelo provedor público com o objetivo de confirmar e autenticar a identidade (token) da configuração com o cluster. Caso seja necessário alterar esta cadeia de caracteres, é importante consultar o processo de geração da identificação (token) de cada provedor, ou cada ambiente de gerenciamento de container, especificamente.
Confirmar: O usuário deve pressionar este botão após confirmar todos os campos alterados.


                                                                                                                     * Deletar Cluster: Quando o usuário selecionar esta ação ele remove o cluster. A plataforma do Mangue.io irá solicitar confirmação do usuário para remover (apagar) da plataforma do Mangue.io:


  



Caso o usuário tenha executado esta ação por engano, será necessário incluir o cluster novamente na plataforma do Mangue.io. Veja a sequência de inclusão de um novo cluster que está descrito neste documento abaixo.
A plataforma do Mangue.io permite ao usuário tanto integrar com infraestrutura de cluster existente quanto implementar ou criar um cluster novo.
Na sequência o processo de integração é descrito, ele permite ao usuário agregar um cluster existente ou novo à plataforma do Mangue.io.
                                                                                                                     
2. Integrar Cluster
~~~~~~~~~~~~~~~~~~~

Para iniciar o processo de Integrar um Cluster o usuário deve clicar com o mouse sobre o botão do lado esquerdo para que a tela apresente os campos específicos.
  





                                                                                                                     * Nome do Cluster: Neste campo o usuário deve informar o nome de referência com o qual o cluster é identificado na plataforma do Mangue.io.
                                                                                                                     * Contrato: Este campo é uma lista (“drop-down list”) com os contratos do usuário, ao selecionar, o Cluster é associado ao contrato selecionado.
                                                                                                                     * Tipo de Cluster: Este campo é uma lista (“drop-down list”) com as quatro opções disponíveis na plataforma do Mangue.io. Atualmente estão disponíveis os ambientes públicos: Google Kubernetes Engine (GKE), Amazon Elastic Kubernetes System (EKS), Azure Kubernetes Service (AKS) e IBM Cloud (IKS). Quando selecionada cada uma das opções de destino a plataforma do Mangue.io se comporta da forma correta para se comunicar e gerenciar o cluster de forma correta.
                                                                                                                     * IP para acesso da API: Neste campo o usuário deve informar o endereço TCP-IP Público para que o cluster seja possível ser acessado.
                                                                                                                     * Path para acesso da API: Neste campo o usuário deve informar a rota utilizada para acesso a API do Kubernetes, caso tenha.
                                                                                                                     * Porta para acesso da API: Neste campo o usuário deve informar o número da PORTA TCP-IP para que o cluster seja acessado.
                                                                                                                     * Cluster Admin Token: Neste campo o usuário deve informar a cadeia de caracteres (string) que foi gerada pelo provedor público de cluster com o objetivo de conferir e autenticar a identidade (token) da configuração com o cluster. Importante consultar o processo de geração de identificação (token) de cada provedor, ou cada ambiente de gerenciamento de container, especificamente.
                                                                                                                     * Botão Integrar: Ao finalizar o preenchimento dos campos acima, o usuário deve clicar com o mouse no botão verde “Integrar” para que a plataforma do Mangue.io inclua este cluster na lista apresentada nesta tela.
                                                                                                                     * A ação de atualizar: Caso a interface do Mangue.io não apresente na lista, o cluster recém configurado, o usuário deve clicar no ícone “  ” para que a aplicação exiba a lista atualizada desta tabela de clusters.


3. Integrar Múltiplos Clusters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
  

Para iniciar o processo de Integrar Múltiplos Clusters o usuário deve clicar com o mouse sobre o botão do lado direito para que a tela apresente os campos específicos.
Nesta tela o usuário pode integrar vários Clusters existentes nos provedores de nuvens públicas. Deve selecionar as quais deseja procurar, em seguida são exibidos os campos: 
                                                                                                                        * Contrato: Este campo é uma lista (“drop-down list”) com os contratos do usuário, ao selecionar, a plataforma carrega as credenciais do contrato selecionado.
                                                                                                                        * Credencial: O usuário deve selecionar uma das credenciais de acesso cadastradas na plataforma do Mangue.io para confirmar a identidade deste junto ao ambiente contratado com a nuvem pública. Após preencher todos os campos, o usuário deve clicar no botão de “Pesquisar” e a plataforma exibe uma lista (“drop-down list”) dos Clusters já existentes nas plataformas selecionadas. O usuário deve selecionar os Clusters que deseja para serem integrados a plataforma, após selecionar o botão de “Integrar” está disponível para ser clicado.




Integração de Cluster Simplificada – Via Form (GKE, EKS, AKS, IBM Cloud)
------------------------------------------------------------------------

A plataforma do Mangue.io permite simplificar o processo de integração com um cluster existente nos provedores de nuvem pública (Amazon, Google, Azure e IBM) através de um formulário que direciona o usuário para o preenchimento de credenciais e configurações de forma bem clara e simples.
Na tela a seguir o usuário pode ver que abaixo de cada logo de provedor de serviço público existe um botão que apresenta o formulário respectivo de cada provedor:
  



Nas telas abaixo esclarecemos as características do formulário específico de cada provedor.
                                                                                                                        
1. Google Kubernetes Engine – GKE
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para efetuar uma integração (via formulário) com um gerenciador de container existente no provedor Google, o usuário deve clicar com o cursor do mouse na área cinza abaixo do logo do Google Kubernetes Engine e a Plataforma do Mangue.io apresenta a tela abaixo com o formulário GKE:
  



                                                                                                                        * Contrato: O usuário seleciona o contrato para a plataforma carregar as credenciais deste contrato.
                                                                                                                        * Nome do Cluster: Neste campo o usuário deve preencher este campo com o nome de identificação do cluster para a plataforma do Mangue.io.
                                                                                                                        * Credenciais do GKE: O usuário deve selecionar uma das credenciais de acesso cadastradas na plataforma do Mangue.io para confirmar a identidade deste junto ao ambiente contratado com o Google Cloud Platform. Importante ressaltar que deve-se consultar a documentação específica de cada provedor sobre como gerar/criar estas credenciais com permissão ao ambiente de gerenciamento de containers do provedor.
                                                                                                                        * Número de Nodes (por zona): Neste campo o usuário deve informar um número inteiro, que irá definir a quantidade de nós (nodes) desejado para este cluster.
                                                                                                                        * Região: Neste campo o usuário deve selecionar de uma lista (“drop-down”) as regiões disponíveis no provedor específico. Neste caso serão listados apenas as regiões globais específicas da Google Cloud Platform.
                                                                                                                        * Tipo de Máquina: Neste campo o usuário deve selecionar de uma lista (“drop-down”) o tipo de configuração de máquina (CPU, Memória, Disco ou “Template”) disponíveis no provedor. Neste caso serão listados apenas os templates específicos da Google Cloud Platform.
                                                                                                                        * Versão Principal: Neste campo o usuário seleciona a versão do Kubernetes disponível no provedor de nuvem pública.
                                                                                                                        * Criar Cluster: Basta o usuário clicar sobre o botão “Criar Cluster”, quando todas as configurações referentes a todos os nós (nodes) estiverem finalizadas. Para que a plataforma do Mangue.io acrescente novo cluster à infraestrutura interna deve-se inicializar este novo cluster ao ambiente computacional que será executado como mais um ambiente gerenciador de containers (cluster).
                                                                                                                        * A ação de atualizar: A criação do Cluster depende do provedor de nuvem pública, o estado da criação do Cluster pode ser acompanhado em Tarefas.




2. Elastic Kubernetes Service – Amazon EKS
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para efetuar uma integração (via formulário) com um gerenciador de container existente no provedor Amazon AWS, o usuário deve clicar com o cursor na área cinza abaixo do logo do Elastic Kubernetes Service – Amazon EKS e a Plataforma do Mangue.io apresenta a tela abaixo com o formulário EKS:
  



                                                                                                                        * Contrato: O usuário selecionará o contrato para a plataforma carregar as credenciais deste.
                                                                                                                        * Nome do Cluster: Neste campo o usuário deve preencher com o nome de identificação do cluster para a plataforma do Mangue.io.
                                                                                                                        * Credencial: O usuário deve selecionar uma das credenciais de acesso cadastradas na plataforma do Mangue.io para confirmar a identidade deste junto ao ambiente contratado com a Amazon Web Services – AWS. Importante ressaltar que deve-se consultar a documentação específica de cada provedor sobre como gerar/criar estas credenciais com permissão ao ambiente de gerenciamento de containers do provedor.
                                                                                                                        * Região: Neste campo o usuário deve selecionar de uma lista (“drop-down”) as regiões disponíveis no provedor específico. Neste caso serão listados apenas as regiões globais específicas da Amazon Web Services – AWS.
                                                                                                                        * Versão do Kubernetes: Neste campo o usuário seleciona a versão do Kubernetes disponível no provedor de nuvem pública.
                                                                                                                        * Template da Máquina: Neste campo o usuário deve selecionar de uma lista (“drop-down”) o tipo de configuração de máquina (CPU, Memória, Disco ou “Template”) disponíveis no provedor. Neste caso serão listados apenas os templates específicos da AWS.
                                                                                                                        * Quantidade de Nós: Neste campo o usuário deve informar um número inteiro, necessário para a quantidade de nós para a infraestrutura do cluster.
                                                                                                                        * Botão Confirmar: Basta o usuário clicar sobre o botão “Confirmar”, quando todas as configurações referentes a todos os nós (nodes) estiverem finalizadas, para que a plataforma do Mangue.io acrescente novo cluster à infraestrutura interna da plataforma do Mangue.io, inicializar este novo cluster ao ambiente computacional que será executado como mais um ambiente gerenciador de containers (cluster).
                                                                                                                        * A ação de atualizar: A criação do Cluster depende do provedor de nuvem pública, o estado da criação do Cluster pode ser acompanhado em Tarefas.
                                                                                                                        
3. AKS
~~~~~~

Para efetuar uma integração (via formulário) com um gerenciador de container existente no provedor Azure, o usuário deve clicar com o cursor na área cinza abaixo do logo do Azure Kubernetes Service – Azure AKS e a Plataforma do Mangue.io apresenta a tela abaixo com o formulário AKS:
  

                                                                                                                        * Contrato: O usuário seleciona o contrato para a plataforma carregar as credenciais deste contrato.
                                                                                                                        * Nome do Cluster: Neste campo o usuário deve preencher este campo com o nome de identificação do cluster para a plataforma do Mangue.io.
                                                                                                                        * Credencial: O usuário deve selecionar uma das credenciais de acesso cadastradas na plataforma do Mangue.io para confirmar a identidade deste junto ao ambiente contratado com a Azure. Importante ressaltar que cada deve-se consultar a documentação específica de cada provedor para como gerar/criar estas credenciais com permissão ao ambiente de gerenciamento de containers do provedor.
                                                                                                                        * Região: Neste campo o usuário deve selecionar de uma lista (“drop-down”) as regiões disponíveis no provedor específico. Neste caso são listados apenas as regiões globais específicas da Azure.
                                                                                                                        * Versão do Kubernetes: Neste campo o usuário seleciona a versão do Kubernetes disponível no provedor de nuvem pública.
                                                                                                                        * Template da Máquina: Neste campo o usuário deve selecionar de uma lista (“drop-down”) o tipo de configuração de máquina (CPU, Memória, Disco ou “Template”) disponíveis no provedor. Neste caso serão listados apenas os templates específicos da Azure.
                                                                                                                        * Quantidade de Nós: Neste campo o usuário deve informar um número inteiro, necessário para a quantidade de nós para a infraestrutura do cluster.
                                                                                                                        * Botão Confirmar: O usuário deve clicar sobre o botão “Confirmar” quando todas as configurações referentes a todos os nós (nodes) estiverem finalizadas, assim a aplicação acrescenta novo cluster à infraestrutura interna da plataforma do Mangue.io. Ao inicializar este novo cluster ao ambiente computacional ele será executado como mais um ambiente gerenciador de containers (cluster).
                                                                                                                        * A ação de atualizar: A criação do Cluster depende do provedor de nuvem pública, o estado da criação do Cluster pode ser acompanhado em Tarefas.

4. IBM Cloud
~~~~~~~~~~~~

Para efetuar uma integração (via formulário) com um gerenciador de container existente no provedor Azure, o usuário deve clicar com o cursor na área cinza abaixo do logo do IBM Cloud Kubernetes Service – IBM IKS e a Plataforma do Mangue.io apresenta a tela abaixo com o formulário IKS:
  

                                                                                                                        * Contrato: O usuário seleciona o contrato para a plataforma carregar as credenciais deste contrato.
                                                                                                                        * Nome do Cluster: Neste campo o usuário deve preencher este campo com o nome de identificação do cluster para a plataforma do Mangue.io.
                                                                                                                        * Credencial: O usuário deve selecionar uma das credenciais de acesso cadastradas na plataforma do Mangue.io para confirmar a identidade deste junto ao ambiente contratado com a IBM Cloud. Importante ressaltar que deve-se consultar a documentação específica de cada provedor sobre como gerar/criar estas credenciais com permissão ao ambiente de gerenciamento de containers do provedor.
                                                                                                                        * Região: Neste campo o usuário deve selecionar de uma lista (“drop-down”) as regiões disponíveis no provedor específico. Neste caso são listados apenas as regiões globais específicas da IBM Cloud.
                                                                                                                        * Versão do Kubernetes: Neste campo o usuário seleciona a versão do Kubernetes disponível no provedor de nuvem pública.
                                                                                                                        * Template da Máquina: Neste campo o usuário deve selecionar de uma lista (“drop-down”) o tipo de configuração de máquina (CPU, Memória, Disco ou “Template”) disponíveis no provedor. Neste caso serão listados apenas os templates específicos da IBM Cloud.
                                                                                                                        * Quantidade de Nós: Neste campo o usuário deve informar um número inteiro, necessário para a quantidade de nós para a infraestrutura do cluster.
                                                                                                                        * Botão Confirmar: O usuário deve clicar sobre o botão “Confirmar” quando todas as configurações referentes a todos os nós (nodes) estiverem finalizadas, assim a aplicação acrescenta novo cluster à infraestrutura interna da plataforma do Mangue.io. Ao inicializar este novo cluster ao ambiente computacional ele será executado como mais um ambiente gerenciador de containers (cluster).
                                                                                                                        * A ação de atualizar: A criação do Cluster depende do provedor de nuvem pública, o estado da criação do Cluster pode ser acompanhado em Tarefas.


Container Execution
-------------------

O menu Integrações/Container Execution permite configurar uma interface de comunicação com os containers que estão sendo executados em um POD. Para que isso seja possível, é necessário fornecer uma credencial de acesso ao cluster Kubernetes. Esta credencial é chamada de KubeConfig[1] - ou arquivo de configuração do cluster Kubernetes. Neste arquivo de configuração existem informações como: certificados SSL para acesso a API do cluster, endereço da API do cluster e algumas outras informações descritas no link que pode ser encontrado na nota de rodapé desta página.
  

  

o
	É importante salientar que o endereço TCP-IP informado da API do cluster deve ser um endereço que seja alcançável pela infraestrutura computacional da sub-rede onde a Plataforma do Mangue.io foi implantada.
	

Caso já tenha o KubeConfig cadastrado, o usuário pode exibi-lo clicando no ícone “  ”. Também é possível excluir o KubeConfig cadastrado clicando no ícone “  ”.




Performance
-----------

A plataforma do Mangue.io pode utilizar a API do Metric Server para realizar a coleta das métricas do Kubernetes, mas não apenas de métricas de desempenho sobre suas workloads, pods e containers, mas também de eventos e novos eventos gerados por seu cluster.
Esta tela está dividida em duas seções, as quais descrevemos abaixo:
                                                                                                                        1. Seção: Adicionar o Monitoramento
Nesta seção, na parte superior da tela, é apresentado um formulário com os campos necessários para que o usuário preencha:
  



                                                                                                                        * * IP de Monitoramento: Este campo é obrigatório, e deve ser preenchido com o número do endereço TCP-IP do Cluster no qual está instalado o Metric Server.
                                                                                                                        * * Path do Metric Server: Este campo é obrigatório, e deve ser preenchido com a rota utilizada pelo o Metric Server no Cluster
                                                                                                                        * * Porta de Monitoramento: Este campo é obrigatório, e deve ser preenchido com o número da porta TCP-IP do Cluster no qual está instalado o Metric Server.
                                                                                                                        * Token: Neste campo o usuário deve utilizar um Bearer Token (mencionado no tópico abaixo) de um Service Account com a permissão de realizar consultas na API do Metric Server.
                                                                                                                        * Confirmar: O usuário deve pressionar este botão após checar todos os campos anteriores e assim, confirmar as configurações referentes ao servidor de monitoramento.




                                                                                                                        2. Seção: Monitoramentos Disponíveis
Esta seção da tela apresenta uma lista de todos os servidores que estão configurados no ambiente da Plataforma do Mangue.io.
Abaixo a descrição das informações presentes nesta lista.
                                                                                                                        * #: Número sequencial do servidor de monitoramento cadastrado na Plataforma do Mangue.io.
                                                                                                                        * IP de Monitoramento: Nesta coluna é apresentado o número do endereço TCP-IP do servidor de monitoramento.
                                                                                                                        * Porta de Monitoramento: Nesta coluna é apresentado o número da porta TCP-IP do servidor de monitoramento.
                                                                                                                        * Bearer Token: Nesta coluna é apresentado uma parte do Bearer Token utilizado para realizar as consultas no Cluster.
                                                                                                                        * Bilhetagem: Exibe se a bilhetagem está ativada.
                                                                                                                        * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções como a figura abaixo:
  



                                                                                                                           * Ativar/Desativar Bilhetagem: Ao selecionar essa opção é ativado ou desativado a bilhetagem do monitoramento.
                                                                                                                           * Editar: Ao selecionar a opção de editar é apresentada a tela abaixo, através da qual o usuário pode alterar o conteúdo dos campos previamente descritos no item Seção: Adicione o Monitoramento na página anterior.
  



                                                                                                                           * Deletar Monitoramento: Ao selecionar a opção de deletar é solicitada uma confirmação da ação pelo usuário, e em seguida um feedback de alerta é criado no canto superior direito da tela informando o sucesso ou erro.
  



Importante ressaltar que esta ação é definitiva e remove (apaga) esta configuração da Plataforma do Mangue.io, pois são apagadas todas as referências deste servidor de monitoramento na plataforma do Mangue.io.

Helm
----

Helm é uma ferramenta que permite a instalação de aplicações Kubernetes, funcionando como um gerenciador de pacotes para o Kubernetes, as aplicações Helm são definidas no repósitorio de aplicações Helm. Para utilizar a funcionalidade de Helm é necessário ter cadastrado previamente o KubeConfig do Cluster na plataforma Mangue.io.
  

Na tela inicial da página de Helm é exibida uma tabela com os Helms instalados na aplicação. Possibilitando que o usuário realize a pesquisa de Helm através do nome. Na tela inicial, o usuário também pode visualizar os Helms que foram deletados, assim permitindo que sejam reinstalados novamente. 
Abaixo descrevemos as informações presentes na tabela de Helms.
                                                                                                                           * #: Número sequencial do Helm cadastrado na Plataforma do Mangue.io.
                                                                                                                           * Nome: Nome do Helm especificado pelo usuário durante a criação.
                                                                                                                           * Data de Criação: Data em que foi criado a aplicação Helm no Cluster
                                                                                                                           * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções como a figura abaixo:
  

                                                                                                                              * Editar Helm: Ao selecionar a opção de editar é apresentada a tela abaixo, através da qual o usuário pode alterar o nome e argumentos da aplicação Helm
                                                                                                                              * Excluir Helm: Ao selecionar a opção de excluir será desinstalado o Helm selecionado do Cluster.
  

Para criar um Helm é necessário clicar no botão de “  ” é essencial especificar seu nome e selecionar na lista de Helms o nome da aplicação no repositório. Também é possível especificar argumentos para a aplicação, algumas aplicações Helm necessitam de argumentos para realizar a configuração. Após preencher todos os campos necessários, o botão de “Adicionar Helm” está disponível para ser clicado. Ao clicar na plataforma Mangue.io ela realiza a instalação do Helm, após ser instalado exibe uma mensagem de sucesso. 




Server VS Code
--------------

O Visual Studio Code é um Ambiente de Desenvolvimento Integrado (Integrated Development Environment - IDE) para o desenvolvimento de aplicações. Essa IDE pode ser instalada em um Cluster, através de um Deployment, assim permitindo que a IDE seja executada dentro de um navegador do usuário. Para utilizar a funcionalidade de Server VS Code é necessário ter cadastrado previamente o KubeConfig do Cluster na plataforma Mangue.io.
Na tela de Server VS Code será exibida uma lista atualizada, com os Visual Studio Code no Cluster atualmente. Também é possível que o usuário realize a pesquisa dos Visual Studio Code instalados, por meio do nome.
  

Abaixo descrevemos as informações presentes na tabela de VS Codes.
                                                                                                                              * #: Número sequencial do VS Code cadastrado na Plataforma do Mangue.io.
                                                                                                                              * Nome: Nome do VS Code especificado pelo usuário durante a criação.
                                                                                                                              * Usuário: Nome do usuário que criou o Visual Studio Code.
                                                                                                                              * Data de Criação: Data em que foi criado o Visual Studio Code no Cluster
                                                                                                                              * Réplicas: Quantidade de réplicas do deployment disponíveis e desejadas
                                                                                                                              * IP: IP do Visual Studio Code para ser acessado no navegador Web.
                                                                                                                              * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta a opção de excluir VS Code, como mostra a figura:
  

                                                                                                                                 * Excluir  VS Code: Ao selecionar a opção de excluir é removido o VS Code selecionado do Cluster.
  

Para criar um Visual Studio Code é necessário clicar no botão de “  ” e preencher os campos abaixo:
                                                                                                                                 * Nome do Servidor VS Code: Nome do servidor Visual Studio Code a ser criado.
                                                                                                                                 * Tamanho do Servidor VS Code: Tamanho de disco a ser disponibilizado para o Visual Studio Code. A medida do tamanho é definida no campo de Tipo do Tamanho.
                                                                                                                                 * Tipo de Serviço: O usuário pode selecionar o tipo de serviço a ser atribuído ao deployment do Visual Studio Code. As opções disponíveis são: Cluster IP, NodePort, Load Balancer e Ingress
                                                                                                                                 * Porta: O usuário pode selecionar a porta que é utilizada no serviço.
                                                                                                                                 * Tipo do Tamanho: Especifica a unidade de tamanho. As opções disponíveis são: Gi e Mi.
                                                                                                                                 * Ingress Class: Caso o tipo de serviço selecionado seja Ingress é necessário selecionar a Ingress Class a ser utilizada pelo o serviço.
                                                                                                                                 * URL do Servidor VS Code: Caso o tipo de serviço selecionado seja Ingress é necessário especificar a rota do Ingress. Exemplo: /vscode
                                                                                                                                 * Ativar autenticação: O usuário pode atribuir uma senha que é necessária para acessar o Servidor VS Code.
                                                                                                                                 * Senha do Servidor VS Code: Senha a ser utilizada para acessar o Servidor VS Code.

Services, Load Balancing and Networking
=======================================

Os Pods nascem e morrem, e quando morrem, morrem mesmo, não ressuscitam. Os controladores ReplicaSets, em particular, criam e apagam Pods dinamicamente (por exemplo: ao escalar ou reduzir). Embora cada Pod tenha seu próprio endereço TCP-IP, até mesmo estes  não podem ser considerados estáveis ao longo do tempo (ex.: Protocolo de Configuração Dinâmica de Endereços de Rede, em inglês, Dynamic Host Configuration Protocol - DHCP). Isso pode gerar um problema, se algum conjunto de Pods (nomeado de back-end) fornece funcionalidade a outros pods (nomeado de front-end) dentro de um cluster do Mangue.io; Como esses front-ends descobrem e controlam os back-ends que estão neste conjunto? É neste momento que se introduzem os Serviços.
Um Serviço no Mangue.io é uma instância do objeto Service do Kubernetes que, por sua vez, é uma abstração que define um conjunto lógico de Pods e uma política pela qual é possível acessá-los. O conjunto de Pods segmentados por um serviço é, geralmente, determinado por um conjunto de Labels.
O menu Services, Load Balancing and Networking é dividido em dois submenus os quais correspondem por: Serviços, Ingress. Cada submenu tem um propósito específico descrito a seguir.

Serviços
--------

É uma maneira abstrata de expor um aplicativo em execução em um conjunto de pods como um serviço de rede. Com o Kubernetes, o usuário não precisa modificar seu aplicativo para usar um mecanismo de Service Discovery desconhecido. O Kubernetes fornece aos pods seus próprios endereços TCP-IP e um único nome DNS para um conjunto de pods e pode balancear a carga entre eles. Neste submenu serão listados os serviços existentes no namespace o qual o usuário está navegando.
O menu Networking/Serviços apresenta todos os serviços de um cluster em um determinado namespace, na tabela temos informações listadas como na tela abaixo:
  



                                                                                                                                    * Serviço: Representa o nome do serviço criado, é o identificador principal de um serviço na hora de executar uma pesquisa na barra de pesquisa. 
                                                                                                                                    * Protocolo: Responsável por identificar o tipo do protocolo desse serviço, podem ser por exemplo: TCP, UDP. 
                                                                                                                                    * Tipo: Representa o tipo do serviço criado no Kubernetes, existem três tipos de serviço são eles:
                                                                                                                                    * NodePort: São serviços acessíveis externamente através do range de portas de 30000 a 32767.
                                                                                                                                    * ClusterIP: São serviços que só serão possíveis de ser acessados na rede interna do cluster.
                                                                                                                                    * LoadBalancer: É um tipo de serviço existente com o intuito de provisionar um LoadBalancer na 7ª camada, para que seja feita a comunicação com o serviço da 4ª camada criado no cluster Kubernetes.
                                                                                                                                    * Port: São as portas que o serviço está apto a receber requisições.
                                                                                                                                    * Duração: Responsável por identificar a quanto tempo a estrutura do serviço foi criada.
                                                                                                                                    * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta três opções como a figura abaixo:
  

Abaixo segue descrição de cada opção deste submenu:
                                                                                                                                       * Adicionar Ingres: Ingress é um serviço que pode ser configurado para fornecer aos Serviços URLs acessíveis externamente. Um Ingress Controller é responsável por complementar o Ingress, geralmente com um balanceador de carga, embora também possa configurar seu roteador de borda ou front-ends adicionais para ajudar a lidar com o tráfego. Esta tela efetua a criação de um Ingress em duas etapas, inicialmente a criação de um balanceador de carga, e em sequência a criação do Ingress na plataforma do Mangue.io.
  

Nome do Ingress: Neste campo o usuário deve informar um nome que faz este serviço ser configurado na Plataforma do Mangue.io.
Gerar LoadBalancer: Após informar o nome do ingress o usuário deve clicar no botão verde com o ícone de um balanceador de carga (“  ”) para iniciar o processo de criação do balanceador de carga na Plataforma do Mangue.io. O usuário deve esperar um feedback de alerta que é apresentado no canto superior direito da tela informado o sucesso ou erro desta ação.
Adicionar: Após a criação, com sucesso, do balanceador de carga, o usuário deverá clicar no botão Adicionar para efetuar a criação do serviço de ingress na plataforma do Mangue.io.


                                                                                                                                       * Deletar Serviço: Na segunda opção do menu de ações dos serviços existe a opção deletar, ao ser selecionada abre um modal de confirmação, neste pede para confirmar a ação, clicando no botão "Deletar". Na sequência é apresentado o feedback de alerta no canto superior direito da tela informando o sucesso ou erro.
  

Importante ressaltar que esta ação é definitiva e remove (apaga) esta configuração da Plataforma do Mangue.io, pois serão apagadas todas as referências deste servidor de monitoramento na plataforma do Mangue.io.


                                                                                                                                       * Editar Serviço: Esta opção do menu de ações exibe a opção `Editar serviço`. Quando selecionada a Plataforma do Mangue.io apresenta o conteúdo do arquivo em formato JSON com todas as configurações do serviço no Kubernetes. O usuário pode editar o que for necessário neste arquivo e selecionar o botão de “Enviar”. Aguardar o feedback da ação que abre o seguinte modal:
  

Recomendamos que somente usuários experientes em sintaxe YAML ou Kubernetes efetue as alterações no código de um serviço, pois a codificação (ou alteração) da sintaxe de forma errônea pode acarretar perda de acesso a todo o ambiente de clusters existentes. O usuário pode usar o mouse para clicar na linha (e no local) desejada para iniciar a digitação dos seus parâmetros específicos do serviço, dessa forma editando o modelo do código YAML que a plataforma lhe apresenta.


Ingress
-------

O Ingress expõe as rotas HTTP e HTTPS de fora do cluster para serviços dentro do cluster. O roteamento de tráfego é controlado por regras definidas no recurso Ingress. Um Ingress pode ser configurado para fornecer aos Serviços URLs acessíveis externamente, Load Balancing, configuração para SSL / TLS. Um Ingress Controller é responsável por complementar o Ingress, geralmente com um balanceador de carga, embora também possa configurar seu roteador de borda ou front-ends adicionais para ajudar a lidar com o tráfego. Neste submenu, serão listados os Ingress existentes no namespace que foi selecionado na aba engrenagens “   Seleção de Configuração” da plataforma do Mangue.io.
Logo acima da tabela, existem três elementos com os quais o usuário poderá atuar:
  



                                                                                                                                       * A ação de pesquisa: Caso a lista apresentada nesta tela seja muito longa (ocupando mais de uma página), existe um campo que possibilita ao usuário efetuar uma pesquisa pelo nome do Update desejado. Basta informar parte do nome e teclar enter ou clicar sobre o ícone da lupa “  ”. Como resultado desta busca apenas os Updates que contiverem a palavra-chave da pesquisa são recuperados.
                                                                                                                                       * A ação de atualizar: Basta clicar no ícone “  ” para que o Mangue.io atualize a interface com os valores mais recentes desta tabela de Ingress.
  

Abaixo descrevemos as informações da lista apresentada nesta tela:
                                                                                                                                          * #: Número sequencial do servidor de monitoramento cadastrado na Plataforma do Mangue.io.
                                                                                                                                          * Nome: Esta coluna apresenta o nome do Ingress que foi informado durante o processo de cadastramento do Ingress na Plataforma do Mangue.io.
                                                                                                                                          * Host: Esta coluna apresenta a informação do nome do servidor (server name) que está registrado no DNS, ou o número do endereço TCP-IP deste servidor.
                                                                                                                                          * Serviço: Esta coluna apresenta a informação de qual serviço este Ingress está associado.
                                                                                                                                          * Address: Esta coluna apresenta o número do endereço TCP-IP do Ingress que foi configurado na Plataforma do Mangue.io.
                                                                                                                                          * Duração: Esta coluna apresenta tempo em dias decorridos desde a data da criação do Ingress até a presente data que o usuário está consultando esta lista.
                                                                                                                                          * Ações: Esta coluna apresenta um botão de ação para deletar ingress, por meio do ícone de lixeira “  ”, Ao clicar no ícone será solicitado do usuário confirmação para conseguir deletar o ingress, conforme imagem abaixo:
  



No caso de o usuário ter incluído um novo Ingress, recentemente, mas o usuário não encontra o nome na lista, o que o usuário pode fazer é clicar no ícone “  ” para que o Mangue.io possa atualizar a interface com a lista mais recente desta tabela.

Namespaces
==========

O Kubernetes oferece suporte a vários clusters virtuais apoiados por um mesmo cluster físico. Esses clusters virtuais são chamados de “namespaces”. Os namespaces são identificados por um “nome”. Estes podem conter diversos ‘recursos’, e cada recurso deve ter seu nome único. O usuário pode criar o mesmo recurso várias vezes (repetindo o mesmo nome) mas estes recursos devem estar configurados em um namespaces distinto.
Namespaces também dão suporte a definição de quotas, como por exemplo um namespace voltado para um ambiente de Produção e um namespace para o ambiente de Homologação.
De forma clara, o ambiente computacional designado para o namespace Produção deve ter maior capacidade de recursos computacionais do cluster que o namespace configurado para um ambiente de Homologação – afinal este ambiente possui uma carga de uso eventual. As quotas limitam a quantidade de recursos computacionais que um determinado Namespace pode consumir.
O menu Namespaces apresenta uma lista de todos os namespaces de um determinado cluster, na tabela temos informações como: nome do namespace, status e duração do namespace. Os namespaces consistem em diferentes áreas de trabalho que fazem parte de um cluster.
  



Para que o usuário possa criar um namespaces, este deve clicar sobre ícone do sinal de adição ‘+’, para que seja apresentada a tela a seguir onde o usuário pode configurar um novo namespace:
  



A tela acima possui apenas um campo onde o usuário deve preencher o nome que deseja criar para o novo namespaces e clicar com o cursor do mouse no botão “Adicionar Namespaces”, para incluir este na Plataforma do Mangue.io. A Plataforma do Mangue.io apresenta um feedback dessa ação no campo superior direito da tela do browser de internet.
Este novo namespace é criado dentro do cluster que foi selecionado na aba engrenagens “   Seleção de Configuração” da plataforma do Mangue.io.
Após a inclusão de um novo namespace, caso este nome não se apresente na lista, o usuário pode clicar no ícone “  ” para que o Mangue.io possa atualizar a interface com a lista mais recente desta tabela.
Na última coluna da tabela existe a opção de deletar o namespace, quando esta coluna for selecionada ela abre um modal de confirmação. E caso confirmada, há um feedback de criação para o usuário.
  

Abaixo a descrição dos campos da tabela apresentada nesta tela:
                                                                                                                                             * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                                                                             * Nome: Esta coluna apresenta o nome do namespaces que foi informado durante o processo de cadastramento do namespaces na Plataforma do Mangue.io.
                                                                                                                                             * Status: O status de um namespaces identifica o estado atual do namespaces. Podem ser apresentados por Running, Pending ou “!” (ponto de exclamação).
                                                                                                                                                * O status Running identifica que nenhum erro está acontecendo com o namespaces.
                                                                                                                                                * O status Pending identifica algum estado de transição no namespaces. Seja por atualização, inicialização do processo do container ou qualquer atividade que identifique um estado de transição.
                                                                                                                                                * O status “!” (ponto de exclamação) identifica um alarme, em outras palavras, que algo errado aconteceu com o namespaces.
                                                                                                                                                * Cota: Esta coluna apresenta um ícone de um “olho” (“  ”) que irá ficar ativo somente nas linhas de namespaces que possuam alguma cota definida para este. O usuário deve posicionar o cursor do mouse sobre o ícone e a Plataforma do Mangue.io irá apresentar uma janela pop-up com nome e as características da cota definida para este namespace.
  

                                                                                                                                                   * Duração: Esta coluna apresenta tempo em dias decorridos desde a data da criação do namespaces até a presente data que o usuário está consultando esta lista.
                                                                                                                                                   * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta três opções como a figura abaixo:
  

                                                                                                                                                      * Adicionar Labels: Um rótulo (label) permite ao usuário mapear suas próprias estruturas organizacionais em objetos do sistema de uma forma fracamente acoplada, sem impor que os softwares armazenem esses mapeamentos. Rótulos são criados com duas atribuições ‘chave’ e ‘valor’ e são anexados a objetos, como pods. Os rótulos (labels) devem ser usados para especificar a identificação de atributos de objetos que são significativos e relevantes para os usuários. Os rótulos podem ser usados para organizar e selecionar subconjuntos de objetos (informação detalhada no link do rodapé do site de documentação Kubernetes.io[2]).
  



Esta tela possui dois campos e dois botões:
Chave: Neste campo o usuário deve preencher com o nome pelo qual a chave (key) será identificada.
Valor: Neste campo o usuário deve preencher com um número inteiro que será o valor da chave.
Adicionar: O usuário deve clicar com o cursor do mouse sobre este botão para adicionar a chave e seu valor na plataforma do Mangue.io. Ao clicar sobre este botão a Plataforma do Mangue.io limpa ambos os campos e cria uma lista logo abaixo. Caso o usuário tenha adicionado uma chave/valor de forma errada, basta clicar no botão “Remover”, que o respectivo par de informação é removido, e o usuário pode cadastrar um novo par (chave/valor) com o conteúdo correto.
  

Confirmar: O usuário deve clicar no botão “Confirmar” quando houver completado de informar a(s) chave(s)/valor(es) necessária(s) ao namespaces. Ao clicar no botão, a Plataforma do Mangue.io irá configurar estas informações e fechar esta tela, apresenta o feedback da ação no canto superior direito da tela do browser de internet.


                                                                                                                                                      * Adicionar Cota de Recurso: Esta tela permite ao usuário estabelecer a quantidade ideal de recursos computacionais que o namespace consome para manter a sua performance ideal, bem como estabelecer o seu limite máximo de consumo de recursos computacionais.
A definição de uma cota pode impactar em outros serviços (workloads) cadastrados na Plataforma o Mangue.io. Quando o usuário define um limite de CPU e Memória para um namespaces caso um deployment possua vários pods, réplicas ou Autoescalador Horizontal, estes nunca ultrapassam o limite de recurso computacional estabelecido na cota. 
Por exemplo: se um deployment necessita iniciar uma nova réplica definida no Auto Escalador Horizontal, e o limite de CPU e Memória já houver sido alcançado, a Plataforma do Mangue.io não inicia a nova réplica, mesmo que os valores definidos no Autoescalador Horizontal sejam alcançados, mas o limite da cota não permite haver recursos computacionais disponíveis para esta nova réplica.
  



Nome da Cota: Informar o nome com o qual a cota será identificada para o namespaces na Plataforma do Mangue.io.
CPU Request: Neste campo o usuário deve preencher com um número inteiro que é o valor inicial de quantidade de CPU que o namespace deve requerer para manter a performance ideal.
Memory Request: Neste campo o usuário deve preencher com um número inteiro que é o valor inicial de quantidade de Memória que o namespace deve requerer para manter a performance ideal.
CPU Limit: Neste campo o usuário deve preencher com um número inteiro que é o valor do limite máximo de quantidade de CPU que o namespace deve restringir para não exaurir os recursos computacionais do cluster.
Memory Limit: Neste campo o usuário deve preencher com um número inteiro que é o valor do limite máximo de quantidade de Memória que o namespace deve restringir para não exaurir os recursos computacionais do cluster.
Confirmar: Quando o usuário preencher todos os campos deste formulário ele deve clicar no botão “Confirmar” para que a plataforma do Mangue.io configure e inclua as cotas de recursos ao namespaces selecionado.


                                                                                                                                                      * Deletar: A terceira opção deste submenu permite que o usuário possa apagar (deletar) um namespace definitivamente do cluster que foi selecionado na ‘aba’ Configurações; e ao ser clicado abrirá a seguinte tela de interface solicitando a confirmação por parte do usuário:
  



 Warning 


Atenção
	Essa é uma ação extremamente destrutiva, pois ao deletar um namespace será deletado também TODOS os recursos e serviços presentes no mesmo.
	

Nodes
=====

O menu Nodes apresenta todos os nodes (Máquinas virtuais) de um determinado cluster. Em Overview Nodes é possível visualizar graficamente o consumo dos recursos (CPU e memória) de todos os Nodes de um Cluster em um determinado período. 
O consumo de CPU é medido em MilliCores e o de memória em MegaBytes, ambos em função do tempo, conforme podemos verificar na figura abaixo. 
É permitido ao usuário selecionar o período desejado clicando sobre os botões localizados acima dos gráficos. As opções disponíveis para o usuário estão entre os últimos 30, 15, 7 e 1 dia(s) e, nas últimas 12 horas. Para os períodos de 30, 15 e 7 dias, as aferições em função do tempo são diárias e para os períodos de 1 dia e 12 horas, são por hora. 
Destacado na cor azul do gráfico de barras, são apresentadas as quantidades de recursos utilizados naquele período selecionado, seja ele por dia ou por hora, conforme escolhido pelo usuário, enquanto a cor verde mensura a quantidade total de recursos, ou seja, que permanecem ociosos naquele período. 
A quantidade total de recursos dos Nodes de um Cluster, tanto para CPU quanto para memória, é representada pela soma dessas duas medidas.  


  





  

Logo acima da tabela, existe um elemento com o qual o usuário pode atuar:
                                                                                                                                                      * Exibir Nós por Contrato: Selecionando esta opção, aparece um campo, onde o usuário pode informar o nome do contrato pelo qual deseja realizar sua busca.


Abaixo a descrição das colunas desta tabela:
                                                                                                                                                      * Nome: Nome do node.
                                                                                                                                                      * Status: Corresponde ao estado atual do node.
                                                                                                                                                      * Running: Indica que o node está “saudável”.
                                                                                                                                                      * Failure: Indica que algum erro aconteceu com o node, ou no presente momento este se encontra indisponível.
                                                                                                                                                      * CPU Utilizada: Representa o consumo atual do recurso de CPU da máquina virtual (node). Este valor está expresso com uma fração de número inteiro (decimais) da quantidade de CPU existente na infraestrutura que compõe a máquina virtual. A infraestrutura computacional existente da máquina virtual suporta e executa micro serviços (ex.: deployment), os quais consomem apenas uma pequena parte do total de recurso de CPU. Assim, a aplicação apresenta a quantidade decimal do total de CPU consumido pela máquina virtual.
                                                                                                                                                      * Memória Utilizada: O consumo atual do recurso de Memória RAM da máquina virtual. Este valor está expresso em Gigabytes, da quantidade total Megabytes de memória RAM existente na infraestrutura que compõe a máquina virtual (node). A infraestrutura computacional existente da máquina virtual (node) para suportar e executar micro serviços (ex.: deployment), desta forma um micro serviço consome apenas uma pequena parte do total de recurso de Megabytes de Memória RAM de um node.


Para o usuário conhecer detalhes de todos os pods de um node específico, basta clicar com o cursor do mouse sobre o nome do node para que a Plataforma do Mangue.io apresente a seção com uma lista de todos os pod que estão em execução no node selecionado.
  

A seção “Pods” apresenta uma tabela que lista todos os pods em execução neste node. Exibe informações detalhadas como nome, nó em que está sendo rodado, status atual do pod, imagem, juntamente com sua versão e tempo de vida (veja a descrição completa dos campos desta tabela no item Seção: PODs).
Caso seja necessário o usuário consultar os logs, ou ter acesso ao prompt do sistema operacional de um pod específico, na coluna Ações o usuário deve clicar com o cursor do mouse sobre o ícone “  ” para que a Plataforma do Mangue.io apresente um submenu com a opção de acesso ao log e a linha de comando do pod selecionado.
Logo acima da tabela, existem três elementos com os quais o usuário pode atuar:
  



                                                                                                                                                      * A ação de pesquisa: Caso a lista apresentada nesta tela seja muito longa (ocupando mais de uma página), existe um campo onde será possível ao usuário efetuar uma pesquisa pelo nome do Update desejado. Basta informar parte do nome do update e teclar enter ou clicar sobre o ícone da lupa “  ”. Como resultado dessa busca virão apenas os nodes que contiverem a palavra-chave da pesquisa.
                                                                                                                                                      * A ação de atualizar: Basta clicar no ícone “  ” para que o Mangue.io possa atualizar a interface com os lista de nomes de nodes configurados na Plataforma do Mangue.io.
                                                                                                                                                      * Adicionar Labels: Caso o usuário necessite adicionar um (ou mais) label ao node o usuário deve clicar com o cursor do mouse no ícone de rótulos (labels - “  ”) para que a plataforma do Mangue.io apresentar a seguinte tela:
  



                                                                                                                                                         * Selecionar Nós: Ao clicar sobre campo é apresentada uma lista (drop-down) com todos os nodes configurados na Plataforma do Mangue.io. Basta o usuário clicar com cursor do mouse sobre o nome do node desejado para selecionar.
                                                                                                                                                         * Nome da Label: Neste campo o usuário deve preencher com o nome pelo qual a label (key) é identificada.
                                                                                                                                                         * Valor da Label: Neste campo o usuário deve preencher com um número inteiro que é o valor da chave.
                                                                                                                                                         * Adicionar: O usuário deve clicar com o cursor do mouse sobre este botão para adicionar a label e seu valor na plataforma do Mangue.io. Ao clicar sobre este botão a Plataforma do Mangue.io limpa ambos os campos e cria uma lista logo abaixo. Caso o usuário tenha adicionado um label/valor de forma errada, basta clicar no botão “Remover”, que o respectivo par de informação é removido, e o usuário pode cadastrar um novo par (chave/valor) com o conteúdo correto.
                                                                                                                                                         * Obs: Adicionar labels aos nodes pode ser importante para os usuários que desejam fazer configurações de Node Affinity aos seus Deployments.
                                                                                                                                                         * Finalizar: Este botão permite adicionar (o)s label(s) selecionados na plataforma do Mangue.io. Na sequência é exibido o feedback desta ação.  


Migração de Cluster
===================

O Mangue.io é uma plataforma de Gestão de Ambientes de Múltiplos Orquestradores de Container, que permite a orquestração, a implantação (localização e agendamento) e a operacionalização (execução) de containers de aplicações dentro de um cluster computacional (público ou privado) ou entre clusters computacionais (público e/ou privado).
A plataforma opera em um modelo de multicloud híbrido e, dessa forma, permite às empresas total controle, suporte para a sustentação de cópias de segurança (backup), replicação e migração de ambientes.
O menu Migrações de Cluster é responsável por realizar a migração de múltiplos recursos entre clusters – de público e/ou privado para público e/ou privado.
Através da Plataforma do Mangue.io o usuário pode migrar o conteúdo completo de um cluster – com todos seus diversos tipos de workloads – para outro cluster.
A praticidade de migração de todos os tipos de workloads entre clusters facilita a criação de um ambiente de Múltiplos Orquestradores de Contêineres preparado para cenários de Disaster Recovery.
A Plataforma do Mangue.io é agnóstica a provedores de serviços (privados, públicos) e através da funcionalidade do menu Migrações o usuário pode manter, gerenciar e operar diversas cópias de seu clusters em múltiplos orquestradores de containers, de forma simultânea e centralizada.


Processo de Migração de Workloads:
---------------------------------

O usuário pode notar que esta tela é segmentada em duas seções: Migração entre Clusters e Workloads, e o processo de migração é simples e o usuário é guiado de forma intuitiva para completar o processo de preenchimento da tela da Plataforma do Mangue.io.


Abaixo apresentamos o processo para o correto preenchimento da tela de migração:


  

                                                                                                                                                         1. Selecionar o Cluster Origem (Seção Migração)
                                                                                                                                                         * Este campo é um “drop-down list” e são listados apenas os clusters configurados no item Integrar Cluster.


                                                                                                                                                         2. Selecionar o Cluster Destino (Seção Migração)
                                                                                                                                                         * Este campo é um “drop-down list” e são listados apenas os clusters  configurados no item Integrar Cluster.


                                                                                                                                                         3. Selecionar Namespace (Seção Workloads)
                                                                                                                                                         * Este campo é um “drop-down list” e são listados apenas os namespaces configurados no item Namespaces.
                                                                                                                                                         * Se caso a linha abaixo deste campo estiver pontilhada, significa que não existe nenhum namepaces configurados e disponível para migração no cluster de origem informado no passo 1. Veja exemplo na tela abaixo:
  
  



                                                                                                                                                         * Quando existem namespaces configurados a Plataforma do Mangue.io apresenta uma linha contínua abaixo deste campo, veja exemplo abaixo:
  
  



                                                                                                                                                         4. Selecionar o Tipo de Workload (Seção Workloads)
                                                                                                                                                         * Este campo é um “drop-down list” e nele apresenta-se a lista de todos os tipos de workloads configurados no item Workloads.
                                                                                                                                                         * Ao clicar neste campo, a Plataforma do Mangue.io apresenta uma relação de workloads que são passíveis de serem migrados de um cluster para outro (Configmaps, Deployments, Daemonsets, Statefulsets, Ingresses, Services).
                                                                                                                                                         * No Kubernetes, não existe um objeto, componente ou qualquer tipo de construção chamada “workload”. No entanto, o termo é frequentemente usado como uma categoria geral para tarefas e serviços que o usuário deseja executar em seu cluster.
                                                                                                                                                         5. Selecionar o Nome do Workload (Seção Workloads)
                                                                                                                                                         * Este campo é um “drop-down list” e são listados apenas os nomes de workloads que fazem parte do mesmo tipo de workload selecionado no campo anterior.
                                                                                                                                                         * Quando o usuário preenche todos os campos anteriores (namespace, Tipo de workload) a Plataforma do Mangue.io apresenta a lista de nomes disponíveis e o usuário pode selecionar um dos nomes pois cada linha está representada por um ícone selecionável (“  ”). Assim que o usuário selecionar um dos nomes, este é adicionado na lista de migração, conforme o exemplo abaixo:
  



                                                                                                                                                            * A Plataforma do Mangue.io permite adicionar diversos tipos de workloads para que a migração de diversos workloads possa ser efetuada de uma única etapa, conforme o exemplo da tela abaixo:
  



                                                                                                                                                            6. Confirmar: Após selecionados, os recursos são exibidos na tabela contendo informações como: Nome do recurso, Tipo do recurso, Namespace, Cluster de Origem e Cluster destino. A Plataforma do Mangue.io inicia a movimentação dos workloads entre os clusters selecionados, e logo em seguida, há um feedback dessa ação que é apresentada no canto superior direito da tela do browser.
Após confirmar este procedimento a Plataforma do Mangue.io efetua a migração de todas as workloads selecionadas entre os clusters indicados, uma mensagem de feedback é apresentada no canto superior direito da tela do browser de internet. 


Migração de Namespace
---------------------

Este menu é responsável por realizar a migração de múltiplos recursos entre namespaces do mesmo Cluster.
Esta tela é segmentada em duas seções, como a tela de Migração de Cluster: Migração entre Namespaces e Workloads, e o processo de migração é simples e o usuário é guiado de forma intuitiva para completar o processo de preenchimento da tela da Plataforma do Mangue.io.
Abaixo apresentamos o processo para o correto preenchimento da tela de migração:


  

                                                                                                                                                            1. Selecionar o Namespace Origem (Seção Migração)
                                                                                                                                                            * Este campo é um “drop-down list” e são listados os namespaces do Cluster.
                                                                                                                                                            2. Selecionar o Namespace Destino (Seção Migração)
                                                                                                                                                            * Este campo é um “drop-down list” e são listados os namespaces do Cluster.
                                                                                                                                                            3. Selecionar o Tipo de Workload (Seção Workloads)
                                                                                                                                                            * Este campo é um “drop-down list” ele lista todos os tipos de recursos disponíveis para migração.
                                                                                                                                                            4. Selecionar o Nome do Workload (Seção Workloads)
                                                                                                                                                            * Este campo é um “drop-down list” e serão listados apenas os nomes dos recursos que fazem parte do mesmo tipo de workload selecionado no campo anterior.
                                                                                                                                                            * Quando o usuário preenche todos os campos anteriores (namespace, Tipo de workload) a Plataforma do Mangue.io apresenta a lista de nomes disponíveis e o usuário pode selecionar um dos nomes pois cada linha está representada por um ícone selecionável (“  ”). Assim que o usuário selecionar um dos nomes, este será adicionado na lista de migração, conforme o exemplo abaixo:
  



                                                                                                                                                               * A Plataforma do Mangue.io permite adicionar diversos tipos de workloads para que a migração de diversos workloads possa ser efetuada de uma única etapa, conforme o exemplo da tela abaixo:
  



                                                                                                                                                               5. Confirmar: Após selecionados, os recursos são exibidos na tabela contendo  informações como: Nome do recurso, Tipo do recurso, Namespace, Namespace de Origem e Namespace destino. A Plataforma do Mangue.io inicia a movimentação dos workloads entre os namespaces selecionados, e logo em seguida, há um feedback dessa ação que será apresentada no canto superior direito da tela do browser.
Após confirmar este procedimento a Plataforma do Mangue.io efetua a migração de todas as workloads selecionadas entre os namespaces indicados, um uma mensagem de feedback será apresentada no canto superior direito da tela do browser de internet.


Registry
========

O menu Registry apresenta todos os Docker Registries integrados à plataforma. O Docker Registry provê um serviço para hospedagem de imagens do Docker análogo ao que está disponível no hub.docker.com, porém com a possibilidade de uso e hospedagem em uma rede interna. Os Registries podem e devem ser utilizados como alternativa para armazenamento de imagens docker dos servidores e aplicações de uma organização. 
No menu Registry é possível conectar a um registry privado, ou seja, um servidor de registro de imagem privado da organização. Ou um serviço de registro de imagem público, como o http://hub.docker.com.
Há nesta seção uma tabela contendo as informações dos Registries adicionados ao Kubernetes, lembrando que os registries são segredos (veja o item Secrets) criados por namespace.
Logo acima da tabela, existem dois elementos com os quais o usuário poderá atuar:
  



                                                                                                                                                               * A ação de pesquisa: Caso a lista apresentada nesta tela seja muito longa (ocupando mais de uma página), existe um campo onde será possível ao usuário efetuar uma pesquisa pelo nome do Registry desejado. Basta informar parte do nome do update e teclar enter ou clicar sobre o ícone da lupa “  ”. Como resultado dessa busca virão apenas os Registry que contiverem a palavra-chave da pesquisa.
                                                                                                                                                               * Adicionar um Registry: Basta clicar no sinal de adição “+” para que o usuário possa cadastrar um novo Registry na plataforma. Na sequência é exibida a tela abaixo:
  



                                                                                                                                                                  * Nome do Servidor: Este campo é obrigatório e o usuário deve informar o nome do servidor de Registry que deseja configurar na Plataforma do Mangue.io.
                                                                                                                                                                  * Username: Este campo é obrigatório e o usuário deve informar o login de usuário provisionado no sistema operacional do servidor de registry existente;
                                                                                                                                                                  * Email: Este campo é obrigatório e o usuário deve informar o e-mail do usuário que é utilizado para fazer autenticação no servidor de registry;
                                                                                                                                                                  * Senha: Este campo é obrigatório e o usuário deve informar a senha do login de usuário, provisionado no sistema operacional do servidor, que será utilizado para fazer autenticação deste usuário no servidor de registry
                                                                                                                                                                  * Nome Secret: Nome do Secret a ser criado para os dados do Registry.
                                                                                                                                                                  * Botão Confirmar: Após o usuário alterar todos os campos anteriores, ele deve clicar com o cursor do mouse sobre este botão para confirmar as alterações informadas para a Plataforma do Mangue.io.


Abaixo é descrito as colunas apresentadas nesta lista de registries:
  



                                                                                                                                                                  * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                                                                                                  * Nome: Esta coluna apresenta o nome do servidor de Registro de imagem criado;
                                                                                                                                                                  * Username: Esta coluna apresenta o nome do usuário que é utilizado para fazer autenticação no servidor de registro de imagem;
                                                                                                                                                                  * Email: Esta coluna apresenta o e-mail do usuário que é utilizado para fazer autenticação no servidor de registro de imagem;
                                                                                                                                                                  * Senha: Esta coluna apresenta a senha do usuário que é utilizado para fazer autenticação no servidor de registro de imagem
                                                                                                                                                                  * URL do Servidor: Esta coluna apresenta a url que o usuário utiliza para se autenticar e baixar as imagens do servidor de registro de imagem;
                                                                                                                                                                  * Duração: Esta coluna indica a quanto tempo aquela credencial para acesso ao servidor de registro de imagem está criada na plataforma;
                                                                                                                                                                  * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta duas opções como a figura abaixo:
  

                                                                                                                                                                     * Deletar Registry: Ação responsável por apagar a credencial de acesso ao servidor de registro de imagem. Ao selecionar este botão a Plataforma do Mangue.io solicita confirmar a operação de remoção da credencial. Lembrando que esta ação ao ser confirmada é irreversível. Caso alguma aplicação do Cluster utilize esta credencial para baixar o container docker, após a deleção esta ação de baixar o container docker  falha, já que a credencial foi apagada.
  

                                                                                                                                                                     * Editar Registry: Ação responsável por fornecer um mecanismo para atualizar as informações de uma credencial de acesso a um servidor de registro de imagem. Ao selecionar a ação “Editar Registry” aparece uma tela com as informações adicionadas anteriormente para a credencial em questão, podendo alterar os campos desejados e ao clicar no botão "Confirmar” a credencial é atualizada. Um alerta com feedback para a ação de atualizar é gerado no canto superior direito da tela do browser de internet.
  

Nome do Servidor: Neste campo o usuário pode alterar o nome do servidor de Registry existente.
Username: Neste campo o usuário pode alterar o nome do usuário que é utilizado para fazer autenticação no servidor de registry de imagem;
Email: Neste campo o usuário pode alterar o e-mail do usuário que é utilizado para fazer autenticação no servidor de registry;
Senha: Neste campo o usuário pode alterar a senha do usuário que é utilizado para fazer autenticação no servidor de registry
Botão Confirmar: Após o usuário alterar todos os campos anteriores, ele deve clicar com o cursor do mouse sobre este botão para confirmar as alterações informadas para a Plataforma do Mangue.io.




Secrets
=======

Secrets (segredos) permitem armazenar e gerenciar informações consideradas confidenciais ou sensíveis, tais como: senhas, tokens, OAuth e chaves SSH. Empregar essa informação através de um Secret é a forma mais segura e flexível do que ‘expor’ a informação, em uma definição de ciclo de vida do Pod ou em uma imagem de contêiner. Os valores de um segredo são salvos em BASE64[3] . O que não significa que há uma certa “camada” de criptografia nas informações, adicionalmente, esta é a abordagem mais recomendada para armazenamento de informações sensíveis.
Ao selecionar este menu será apresentado uma lista de todos os secrets presentes no cluster que foi selecionado na aba engrenagens “   Seleção de Configuração” da plataforma do Mangue.io.


  

O menu de Segredo contém uma tabela com as seguintes informações:
                                                                                                                                                                     * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                                                                                                     * Nome: Esta coluna apresenta o nome do Secret que foi utilizado no momento de sua configuração.
                                                                                                                                                                     * Tipo: Tipo do segredo.
                                                                                                                                                                     * Duração: Esta coluna apresenta o tempo (em dias) decorridos desde a criação deste secret.
                                                                                                                                                                     * Ações: Esta coluna apresenta um botão de ação, que é uma lata de lixo “  ” que ao ser clicado, remove o secret da mesma linha. Ao selecionar a ação “Deletar Secret” a Plataforma do Mangue.io solicita confirmação da ação pelo usuário.
  



Importante ressaltar que esta ação ao ser confirmada é irreversível. Qualquer workload do cluster que esteja associado, ou utilize, este secret pode apresentar um erro fatal (crash) em sua execução.


Se o usuário necessita conhecer os conteúdos armazenados de um Secret, este  deve clicar sobre o nome do Secret para que a Plataforma do Mangue.io apresente as informações específicas configuradas para o Secret em uma seção abaixo da lista.
Esta nova seção da tela apresenta a lista de todos os componentes de um secret.
Para cada componente do secret a Plataforma do Mangue.io apresenta um ícone de visualização do conteúdo do componente do Secret. Este ícone é representado com “olho” (“  ”), quando o usuário clicar sobre o ícone a Plataforma do Mangue.io  apresenta o conteúdo do componente como o exemplo abaixo:
  



Quando o usuário clicar sobre o ícone de visualização, novamente, a Plataforma do Mangue.io fecha a apresentação do conteúdo do Secret da tela.


Schedule Task
=============

A plataforma Mangue.io pode agendar tarefas para serem realizadas em uma data posterior, tarefas como: 
                                                                                                                                                                        * Atualizar Deployment.
                                                                                                                                                                        * Escalar Deployment.
                                                                                                                                                                        * Atualizar ConfigMap.
  

Na página de Schedule Task é exibida uma lista com as tarefas agendadas na plataforma, também é possível pesquisar as tarefas agendadas através do nome do recurso.
Abaixo é descrito as informações presentes na tabela de tarefas agendadas.
                                                                                                                                                                        * #: Número sequencial do VS Code cadastrado na Plataforma do Mangue.io.
                                                                                                                                                                        * Data Agendada: Data para qual a tarefa foi agendada.
                                                                                                                                                                        * Tipo: Tipo de tarefa a ser realizada.
                                                                                                                                                                        * Detalhes: Detalhes sobre a tarefa a ser realizada.
                                                                                                                                                                        * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta as seguintes opções:
  

                                                                                                                                                                           * Editar Agendamento: Ao selecionar a opção de editar será apresentada a tela com as informações do agendamento, sendo possível editá-las.
                                                                                                                                                                           * Cancelar Agendamento: Ao selecionar a opção de cancelar agendamento, a data desejada será excluída da plataforma.


  

Para criar uma tarefa agendada é necessário clicar no botão de “  ” e é necessário preencher os campos abaixo:
                                                                                                                                                                           * Data Atualização: Data e horário em que a tarefa será executada.
                                                                                                                                                                           * Tipo de Tarefa: Tipo de tarefa a ser executada, as opções são:
                                                                                                                                                                           * Atualizar Deployment.
                                                                                                                                                                           * Escalar Deployment.
                                                                                                                                                                           * Atualizar ConfigMap.


  

Caso seja selecionada a opção de “Atualizar Deployment” será necessário preencher os novos campos, conforme a figura acima, de: 
                                                                                                                                                                           * Deployment: O usuário deve selecionar o deployment a ser atualizado,
                                                                                                                                                                           * Nome do Container: O nome do container a ser atualizado.
                                                                                                                                                                           * Versão do Container: Versão para qual o Container será atualizado.


  

Caso seja selecionada a opção de “Escalar Deployment”, é essencial preencher os novos campos, conforme a figura acima, de: 
                                                                                                                                                                           * Deployment: O usuário deve selecionar o deployment a ser atualizado,
                                                                                                                                                                           * Réplicas: Quantidade de réplicas a qual o Deployment será escalado.
  

Caso seja selecionado a opção de “Atualizar ConfigMap” é necessário preencher os novos campos, conforme a figura acima, de: 
                                                                                                                                                                           * ConfigMap: O usuário deve selecionar o ConfigMap que será atualizado.
                                                                                                                                                                           * Nome do ConfigMap: O usuário deve preencher com o nome do ConfigMap desejado.
É possível adicionar ou remover arquivos clicando nos ícones de “  ” e “  ” respectivamente.
Os campos de um arquivo de ConfigMap são:
                                                                                                                                                                           * Nome do Arquivo: O usuário deverá informar no nome do arquivo que será criado no sistema operacional da máquina virtual que utilizar o ConfigMap.
                                                                                                                                                                           * Conteúdo do Arquivo: O usuário deverá preencher com o conteúdo específico do arquivo a ser criado.


Storage
=======

Lidar com aplicações em contêineres tem alguns desafios, e um destes desafio é como interagir com arquivos em disco. Os arquivos em disco de um container são efêmeros, isto representa alguns problemas para aplicações não triviais empacotadas em containers. Primeiro, quando um container falha, o Mangue.io tenta reiniciá-lo, mas com isso os arquivos em disco serão perdidos, logo, o container começa sempre com um estado limpo. Em segundo lugar, ao executar containers juntos em um Pod, geralmente é necessário compartilhar arquivos entre esses contêineres. A abstração de Volume do Kubernetes utilizada no Mangue.io resolve esses dois problemas (para o ambiente Docker é diferente[4]).
Por outro lado, um volume do Kubernetes (utilizado pelo Mangue.io) tem uma vida útil explícita – o mesmo que o Pod que o contém. Consequentemente, um volume ultrapassa todos os contêineres que são executados no Pod e os dados são preservados nas reinicializações deste mesmo contêiner. Naturalmente, quando um Pod deixa de existir, o volume deixa de existir também. Talvez mais importante do que isso, como o Kubernetes suporta muitos tipos de volumes, e um Pod pode usar qualquer número deles simultaneamente, a Plataforma do Mangue.io também herdou essa capacidade. 
Em sua essência, um Volume é apenas um diretório, possivelmente com alguns dados, que são acessíveis aos contêineres em um Pod. O diretório é o “local”, e seu “conteúdo” é determinado pelo tipo de volume específico utilizado.
Na sessão de Storage o usuário encontra os menus relacionados a estrutura de armazenamento de dados persistentes em Kubernetes. É possível por navegar por três estruturas diferentes:
                                                                                                                                                                           * StorageClass
                                                                                                                                                                           * Persistent Volumes
                                                                                                                                                                           * Persistent Volume Claims


StorageClass
------------

Os StorageClass são responsáveis por criar classes de storage de diferentes tipos, pode-se encarar como exemplo o seguinte cenário:
                                                                                                                                                                           1. Um usuário tem dois tipos de discos montados em dois NFS servers diferentes e deseja utilizar o disco com maior potencial de leitura e escrita para um tipo de aplicação e o disco com menor potencial de leitura e escrita para as demais aplicações.
                                                                                                                                                                           2. Desta forma o usuário deverá criar dois StorageClass diferentes, cada um representa um servidor de NFS: um para o disco que tem potencial de leitura e escrita mais rápido e outro para o disco que tem potencial de leitura e escrita mais baixo.
Quando o usuário selecionar o menu Storage/StorageClass a plataforma do Mangue.io apresentará a lista de todos os StorageClass que existem configurados no cluster que foi selecionado na aba engrenagens “   Seleção de Configuração” da plataforma do Mangue.io. 
  



Abaixo são descritos as colunas desta lista:
                                                                                                                                                                           * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                                                                                                           * Nome: Nome do StorageClass.
                                                                                                                                                                           * Provisioner: Nome do provisionador do StorageClass.
                                                                                                                                                                           * Duração: Descreve há quanto tempo atrás o recurso foi criado.
                                                                                                                                                                           * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta a opção de apagar StorageClass selecionado:
  

                                                                                                                                                                              * Ao selecionar a ação “Deletar StorageClass” a Plataforma do Mangue.io solicita confirmação da ação pelo usuário.
  



                                                                                                                                                                              * Importante ressaltar que esta ação ao ser confirmada é irreversível. Qualquer workload do cluster que esteja associado, ou utilize, este StorageClass pode apresentar um erro fatal (crash) em sua execução.




PersistentVolume
----------------

Os PersistentVolumes (PV) são uma parte do armazenamento no cluster que foi provido por um administrador ou provisionado dinamicamente usando StorageClass. É um recurso do cluster, assim como um node. PVs são plugins de volume como o recurso Volumes, mas têm um ciclo de vida independente de qualquer Pod individual que usa o PV.
Quando o usuário selecionar o menu Storage/PersistentVolume a plataforma do Mangue.io apresenta a lista de todos os PersistentVolumes que existem configurados no cluster que foi selecionado na aba engrenagens “   Seleção de Configuração” da plataforma do Mangue.io. 
  

                                                                                                                                                                              * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                                                                                                              * Capacity: Esta coluna apresenta o tamanho/capacidade do PersistentVolume em Gigabytes.
                                                                                                                                                                              * Access Modes: Esta coluna apresenta a configuração de acesso a este volume, esses modos de acesso podem ser três, são eles:
                                                                                                                                                                                 * ReadWriteOnce: O volume será montado e poderá receber instruções de leitura e escrita apenas de um único node.
                                                                                                                                                                                 * ReadOnlyMany: O volume será montado e tem permissão apenas de leitura, mas de diferentes nodes simultaneamente, não sendo permitido escrita.
                                                                                                                                                                                 * ReadWriteMany: O volume será montado e poderá receber instruções de leitura e escrita simultaneamente, mas de diferentes nodes.
                                                                                                                                                                                 * Reclaim Policy: Quando um usuário conclui seu volume, ele pode excluir os objetos do Persistent Volumes Claim da API que permite a recuperação (reclaim) do recurso. A política de recuperação para um PersistentVolume informa ao cluster o que fazer com o volume depois que ele for liberado da sua reivindicação. Existem atualmente três políticas de recuperação:
                                                                                                                                                                                 * Retain: A política (retain) permite a recuperação manual do recurso. Quando o PersistentVolumeClaim é excluído, o PersistentVolume ainda existe e o volume é considerado "liberado". Mas ainda não está disponível para outra reclamação porque os dados do reclamante anterior permanecem no volume.
                                                                                                                                                                                 * Delete: Para volumes que oferecem suporte à política de recuperação de exclusão, esta remove o objeto PersistentVolume do Kubernetes, bem como o arquivo de armazenamento associado na infraestrutura externa (por ex.: um volume AWS EBS, GCP PD ou Disco do Azure).
                                                                                                                                                                                 * Recycle: Nesta última opção a política de recuperação para um PersistentVolume permite ao cluster fazer uma limpeza básica. 
                                                                                                                                                                                 * Status: Esta coluna apresenta a situação atual (status) da solicitação do volume, existem dois status que podem ser apresentados:
                                                                                                                                                                                 * Bound: Quando as vinculações (binding) do tamanho volume correspondem ao espaço designado no ambiente computacional do node.
                                                                                                                                                                                 * Unbound: Quando as vinculações (binding) do tamanho do volume não correspondem ao espaço designado no ambiente computacional do  node.
                                                                                                                                                                                 * StorageClass: Esta coluna apresenta o nome do StorageClass ao qual o PersistentVolume está associado.
                                                                                                                                                                                 * Age: Esta coluna apresenta o tempo (em dias) decorridos desde a criação deste PersistentVolume.
                                                                                                                                                                                 * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta a opção de apagar o volume selecionado:
  

                                                                                                                                                                                    * Ao selecionar a ação “Deletar Volume” a Plataforma do Mangue.io solicita confirmação da ação pelo usuário.
  



                                                                                                                                                                                    * Importante ressaltar que esta ação ao ser confirmada é irreversível. Qualquer workload do cluster que esteja associado, ou utilize, este PersistentVolume poderá apresentar um erro fatal (crash) em sua execução.


PersistentVolumeClaims
----------------------

Os PersistentVolumeClaims (PVC) são uma solicitação de armazenamento por um usuário. É semelhante a um pod. Os pods consomem recursos do node e os PVCs consomem recursos PV. Os pods podem solicitar níveis específicos de recursos (CPU e memória). Os PVCs podem solicitar tamanhos específicos de armazenamento e modos de acesso (por exemplo, eles podem ser montados ReadWriteOnce, ReadOnlyMany ou ReadWriteMany).
O menu Storage/Persistent Volume Claims apresenta todos os PVCs presentes em um determinado namespace do cluster, a tabela exibe informações como:
  



                                                                                                                                                                                    * # ‘coluna acionável’: Esta coluna apresenta uma forma alternativa de remover (apagar) várias linhas com um único comando. Cada linha está representada por um ícone selecionável (“   - check mark”). Quando o usuário seleciona uma linha, ou várias, a plataforma do Mangue.io apresenta ícone(s) acima desta coluna, e que representam ações ao usuário para serem executadas de uma única vez para todas as linhas selecionadas. Neste caso será apresentado um ícone de lata de lixo (“  ”) que permite ao usuário remover todos os itens selecionados com um único comando.
                                                                                                                                                                                    * Nome: Responsável por identificar o nome do PVC
                                                                                                                                                                                    * Capacidade: Esta coluna apresenta o tamanho/capacidade do PersistentVolumeClaim em Gigabytes.
                                                                                                                                                                                    * Status: Responsável por identificar o estado do PVC, geralmente podem ser os seguintes estados:
                                                                                                                                                                                       * Bound: Quando o PVC foi criado com sucesso.
                                                                                                                                                                                       * Pending: Quando está no aguardo de alguma instrução para que seja criado com sucesso.
                                                                                                                                                                                       * Terminating: Quando está no aguardo de alguma instrução para que seja deletado com sucesso.
                                                                                                                                                                                       * Provisioner: Responsável por identificar qual StorageClass aquele PVC está utilizando.
                                                                                                                                                                                       * Duração: Esta coluna apresenta o tempo (em dias) decorridos desde a criação deste PersistentVolume.
                                                                                                                                                                                       * Ações: Esta coluna apresenta um botão de ação “  ” que ao ser clicado, apresenta a opção de apagar o PVC selecionado:
  

                                                                                                                                                                                          * Ao selecionar a ação “Deletar Volume” a Plataforma do Mangue.io solicita confirmação da ação pelo usuário.
  



                                                                                                                                                                                          * Importante ressaltar que esta ação ao ser confirmada é irreversível. Qualquer workload do cluster que esteja associado, ou utilize, este PersistentVolumeClaim pode apresentar um erro fatal (crash) em sua execução.


Tarefas
=======

A Plataforma do Mangue.io é um ambiente que se comunica com o gerenciador de container Kubernetes via API-Restful, desta forma sempre que o usuário adiciona, ou re-configura algum recurso através da interface do Mangue.io, a plataforma envia uma ‘tarefa’ via API-Restful para o cluster Kubernetes para que esta tarefa seja executada.
Ao final do processamento da tarefa, a plataforma do Mangue.io recebe uma mensagem de retorno/resposta do Gerenciador de Kubernetes e apresenta-a para o usuário na tabela da interface. Abaixo a tela Tarefas exibe um exemplo:


  

Na lista podemos encontrar o status das tarefas referentes ao cluster que foi selecionado na aba engrenagens “   Seleção de Configuração” da plataforma do Mangue.io:
                                                                                                                                                                                          * Operação: Nesta coluna é apresentado uma descrição sucinta da tarefa que foi executada pelo usuário através da interface do Mangue.io.
                                                                                                                                                                                          * Cluster: Nesta coluna é apresentado a identificação do cluster em que a tarefa ocorreu.
                                                                                                                                                                                          * Usuário: Nesta coluna é apresentado a identificação do usuário que efetuou o login na plataforma e solicitou a ação na interface do Mangue.io.
                                                                                                                                                                                          * Detalhes: Nesta coluna é apresentado um ícone de uma letra “i”, nas linhas em que a coluna ‘status’ esteja com o status “Failed” a plataforma do Mangue.io apresenta um pop-up com detalhes do resultado da tarefa. O usuário deve posicionar o cursor do mouse sobre a letra “i” e a plataforma do Mangue.io apresenta uma tela de pop-up com o conteúdo da mensagem de erro retornado pelo Kubernetes para a plataforma do Mangue.io. Veja um exemplo abaixo:
  

                                                                                                                                                                                          * Data de Início: Esta coluna apresenta a data e hora em que a tarefa foi criada na plataforma do Mangue.io. O formato de data a apresentação é de: dia/mês/ano (padrão brasileiro – DD/MM/AAA), para o formato de hora é de: hora, minuto e segundo (formato 24 horas – HH:MM:SS).
                                                                                                                                                                                          * Criado em: Esta coluna apresenta a quantidade de dias decorridos desde a data de início da tarefa (coluna anterior)
                                                                                                                                                                                          * Status: Esta coluna apresenta o conteúdo da mensagem de retorno/resposta do Gerenciador de Kubernetes e apresenta esta resposta para o usuário em três status diferentes:
                                                                                                                                                                                          * SUCCESS: Tarefa enviada para o Kubernetes e foi processada com sucesso;
                                                                                                                                                                                          * PENDING: Tarefa enviada para o Kubernetes e está sendo processada, até o presente momento não foi encerrada;
                                                                                                                                                                                          * FAILED: Tarefa enviada para o Kubernetes e seu processamento gerou erro/falha durante a tentativa de sua execução.


Logo acima da tabela, existem três elementos com os quais o usuário pode atuar:
  



                                                                                                                                                                                          * A ação de pesquisa: Caso a lista de apresentada nesta tela seja muito longa (ocupando mais de uma página), existe um campo onde será possível ao usuário efetuar uma pesquisa por alguma parte do texto presente na coluna “Operação”. Basta informar parte do nome da operação e teclar enter, ou clicar sobre o ícone da lupa “  ”. Como resultado dessa busca virão apenas as linhas que contiverem a palavra-chave da pesquisa.
Esta pesquisa é sensível ao caso das letras (maiúsculas / minúsculas), portanto, o resultado da busca pela palavra “Deletar” será diferente do resultado da busca pela palavra “deletar”.
Caso a busca não retorne nenhuma incidência, a lista fica em branco. Para voltar a lista inicial, o usuário deve apagar qualquer conteúdo/string deste campo, e clicar sobre o ícone da lupa “  ” (busca por campo em ‘branco’) e a plataforma do Mangue.io apresenta o conteúdo completo da lista antes de qualquer busca.
                                                                                                                                                                                             * A ação de atualizar: Basta clicar no ícone “  ” para que o Mangue.io atualize a interface com os status mais recentes desta tabela de tarefas.


Clusters Workloads
==================

Esta opção de menu lista todas as cargas de trabalho (workloads) existentes em todos os clusters integrados à Plataforma do Mangue.io.
Inicialmente, é relevante esclarecer o que é exatamente uma carga de trabalho (workload). No Kubernetes, não há objeto, componente e qualquer tipo de construção chamada “carga de trabalho”. No entanto, o termo é frequentemente usado como uma categoria geral para tarefas e serviços que o usuário deseja executar em seu cluster. Pode ser sinônimo de microsserviços, aplicativos, containers ou processos. As cargas de trabalho, geralmente, são processos de longa duração, mas também podem ser de curta duração sob demanda ou jobs em lote.
A Plataforma do Mangue.io pode gerenciar diversos componentes que o Kubernetes oferece para gerenciar e configurar suas cargas de trabalho. Pode-se listar pods e para os componentes que encapsulam pods, como ReplicaSets, Deployments, DaemonSets e StatefulSets. Em seguida, detalhamento sobre os componentes periféricos, como Serviços, EndPoints e Ingress.
Por se tratar de uma quantidade muito grande de componentes, esta lista pode ser extensa. Abaixo está apresentado um exemplo de um destes componentes que são listados na tela:
  



                                                                                                                                                                                                * # ‘coluna acionável’: Esta coluna apresenta o número sequencial da workload na lista exibida.
                                                                                                                                                                                                * Nome: Esta coluna apresenta o nome do workload que foi criado durante o processo de inclusão deste componente na plataforma do Mangue.io.
                                                                                                                                                                                                * Tipo: Esta coluna apresenta o tipo específico do(s) componente(s) workload(s).
                                                                                                                                                                                                * Deployments
                                                                                                                                                                                                * Daemonsets
                                                                                                                                                                                                * Horizontal Autoscaler
                                                                                                                                                                                                * Pods
                                                                                                                                                                                                * Statefulsets
                                                                                                                                                                                                * Updates
                                                                                                                                                                                                * Réplicas: Esta coluna apresenta a quantidade de réplicas ativas que este componente possui no presente momento da consulta.
                                                                                                                                                                                                * Cluster: Esta coluna apresenta o nome do cluster o qual o componente está associado. A Plataforma do Mangue.io exibe todos os clusters com os quais possui configuração de integração.
                                                                                                                                                                                                * Namespace: Esta coluna apresenta o nome do namespace que o componente está associado.
Caso o usuário necessite visualizar todas as informações detalhadas de um componente presente na lista, basta clicar com o cursor do mouse sobre o nome do componente e a Plataforma do Mangue.io apresenta as mesmas informações presentes no menu Workloads (exemplo de informações de um deployment abaixo):
  



________________


Conclusão
=========


Este documento conclui a apresentação e descrição do Mangue.io, uma Plataforma de Gestão de Ambientes de Múltiplos Orquestradores de Container que entrega de forma contínua, ágil, segura e produtiva, as aplicações direcionadas a implantação, testes e atualizações com downtime zero e rollback de deployments.


====

Equipe Ustore
Manual de Uso do Mangue.IO. 4ª Edição. Versão 1.



.. |icone_engrenagem| image:: /figuras/fig_mangue/icone_engrenagem.png

.. |icone_lata_lixo_preta| image:: /figuras/fig_mangue/icone_lixo.png

.. |icone_lupa_vermelha| image:: /figuras/fig_mangue/icone_lupa_vermelha.png

.. |icone_sinal_menor| image:: /figuras/fig_mangue/icone_sinal_menor.png

.. |uCloud_icone_coluna_acionavel| image:: /figuras/uCloud_icone_coluna_acionavel.png

.. |icone_reversao| image:: /figuras/fig_mangue/icone_reversao.png

.. |icone_escalar| image:: /figuras/fig_mangue/icone_escalar.png

.. |icone_lixo_vermelho| image:: /figuras/fig_mangue/icone_lixo_vermelho.png

.. |icone_alterar_versao| image:: /figuras/fig_mangue/icone_alterar_versao.png

.. |icone_adicionar| image:: /figuras/fig_mangue/icone_adicionar.png

.. |icone_acao| image:: /figuras/fig_mangue/icone_acao.png









