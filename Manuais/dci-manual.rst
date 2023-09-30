
.. image:: /figuras/index/_ustore_pequena.png
    :alt: logo ustore
    :align: center
======

.. centered:: Português     -     Español_     -     English_

.. _Español: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuales/dci.spa.html

.. _English: https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/MEnglish/dci.eng.html

====

Manual de funcionalidades 
=========================

Soluções em tecnologia da informação que viabilizam implementar uma arquitetura computacional escalável, sólida e confiável em nuvem híbrida.

====


Introdução
----------


Este documento consiste em um manual com a descrição breve das principais funcionalidades contidas no produto **Data Center Interconnect - DCI** da plataforma uCloud.

----

Apresentação
-------------

**Data Center Interconnect -  DCI** é uma solução de conectividade cuja rede é definida por *software*. 

A rede definida por *software* (SDN) é uma arquitetura que permite um gerenciamento e controle mais eficiente dos recursos de rede, ela delimita o plano de controle do plano de dados. 

Em termos descomplicados, comunicação entre datacenters significa que as funções de controle e dados da rede estão separadas, o que permite maior flexibilidade e automação no gerenciamento de rede.


----

Como logar no DCI
-----------------


Para ter acesso à plataforma é necessário ter realizado uma "Primeira compra" no Painel do Cliente. 

Após essa compra o usuário recebe as suas credenciais de acesso, enviadas diretamente ao seu e-mail registrado. 


.. image:: /figuras/fig_dci/001_log_in.png
    :alt: login
    :scale: 100 %
    :align: center
======

O usuário deve preencher os campos ``login`` e ``senha``, com as credenciais recebidas do administrador da plataforma. 

Clicar no botão ``Entrar``. 

Após este procedimento, a tela inicial do portal é apresentada.

----


Visão Geral
-----------


Neste primeiro contato é importante entender o impacto de algumas ferramentas existentes no menu superior direito, exibido ao usuário após seu login no DCI. 
  

A imagem seguinte é um recorte do menu superior direito, apresentado em todas as telas disponíveis ao usuário. Este menu demonstra componentes relevantes como nome, e-mail, configurações de conta, acesso a este manual de funcionalidades e logout, cada um descrito em detalhe a seguir.


  * Nome; 
  * E-mail;
  * Configurações de conta;
  * Acesso a este manual de funcionalidades;
  * Logout.


.. image:: /figuras/fig_dci/002_nome_config_manual_logout.png
    :alt: visão geral
    :align: center
======

 
**Ícone de notificação**  |icone_tarefas|: Este ícone é um ponto relevante para a visualização de todas as atividades que são realizadas no portal. Através deste é possível observar as ações mais recentes, refletidas em forma de notificação na tela "Tarefas".

**Nome**: Exibe o nome do usuário logado e seu endereço de e-mail.
  
**Configuração de conta**: Possibilita acessar os detalhes da conta criada, na qual é possível alterar o e-mail, o telefone de contato e gerenciar os usuários em seu contrato. Este botão direciona ao menu **Administração**.

**Manual de funcionalidades**: Direciona o usuário ao documento “manual de funcionalidades” armazenado no ambiente de documentação online da Ustore Brasil.

**Logout**: sair ou deslogar da aplicação.

----


Menu **Administração**
----------------------

Para a completa visualização dos serviços do DCI existem alguns menus na lateral esquerda da plataforma, neste é possível encontrar informações valiosas ao produto.
  
Ao acessar este menu de Administração é possível o usuário operacionalizar os submenus: 

  * Usuários;
  * Grupos;
  * Contratos.

.. image:: /figuras/fig_dci/003_menu_admin.png
    :alt: menu administração
    :scale: 80 % 
    :align: center
======

.. hyperlink

.. https://ustore-software-e-servicos-ltda-manuais.readthedocs-hosted.com/pt/latest/Manuais/usr-manual.html#menu-administracao


Menu **DCI**
------------

Este menu contém três submenus que possibilitam visualizar:

  * Portas;
  * Circuitos;
  * Excursionamentos. 

Na sequência cada um destes submenus é detalhado.

.. image:: /figuras/fig_dci/004_menu_dci.png
    :alt: menu dci
    :scale: 80 % 
    :align: center
======


Submenu Portas
~~~~~~~~~~~~~~


Este submenu possibilita visualizar os recursos de portas, além disso, pode-se observar as ações disponbilizadas como incluir recursos desabilitados ao listar, buscar uma informação, atualizar a tela após modificação e seis colunas que categorizam cada uma das portas. As portas ligam-se por intermédio dos Circuitos, elas podem ou não ter circuitos, todas as portas estão dentro do Datacenter, ao comprar a porta, o cliente recebe a LOA (carta de autorização) ela é necessária para o fluxo do processo.


.. image:: /figuras/fig_dci/005_menu_portas.png
    :alt: Menu Portas 
    :align: center
======


Três funcionalidades são apresentadas: 

  * O botão para ``Incluir recursos desabilitados``: Ao clicar neste botão o usuário pode visualizar os recursos que estão desabilitados; 
  * A ação de ``Procurar``: sinalizado pela lupa que indica ao usuário a possibilidade de busca;
  * O botão para atualização da página ao clicar em ``Refresh``.

As informações das portas, são divididas em seis colunas e apresentadas, conforme mencionadas abaixo:

  * Designação;
  * *Status*;
  * Banda;
  * Tipo;
  * *Data Center*;
  * *Golden Jumper*.



Ao selecionar uma porta, é possível visualizar os detalhes de forma completa, esta nova página apresenta em seu cabeçalho algumas opções acionadas pelos botões de ``Voltar`` ,  ``Baixar LOA``, ``Reenviar LOA`` e  ``Confirmado``, no corpo da tela estão distribuídos os *cards* descritos na sequência. 

.. image:: /figuras/fig_dci/006_menu_porta_spo.png
    :alt: Menu porta spo 
    :align: center
======

O submenu Portas exibe três *cards* categorizando relevantes informações: 

  * Geral;
  * Vlans;
  * Histórico.

----

*Card* Geral
""""""""""""

Este *card* está contido no submenu Portas, menu DCI. Ele apresenta as principais informações desta Porta.

.. image:: /figuras/fig_dci/006_a_portas_card_geral.png
    :alt: card geral 
    :align: center
======

 Após preenchidos os catorze elementos, listados na sequência, eles devem exibir um panorama geral ao usuário, inclusive a data de criação e alocação desta porta, como mostra o exemplo acima: 

  * Usuário;
  * Nome da empresa;
  * CPF/CNPJ;
  * Designação;
  * Banda;
  * Roteador;
  * Roteador porta;
  * Posição do DGO;
  * *Status*;
  * Datacenter;
  * Cidade;
  * Tipo de porta;
  * Data de criação;
  * Data de alocação.

----
 
*Card* Vlans
""""""""""""

O segundo *card* mostrado neste submenu Portas, localizado no lado direito da tela, além das informações contém um botão de ação de coloração verde. 


.. image:: /figuras/fig_dci/006_b_portas_card_vlans.png
    :alt: card vlans 
    :align: center
======


O *card* Vlans exibe no lado direito superior uma funcionalidade de atualização da página que pode ser acionada pelo botão ``Refresh``, em seguida as informações são divididas em quatro colunas: 

  * Vlans em Uso;
  * Circuitos;
  * Banda;
  * Banda Base.

As informações sobre as Vlans são exibidas em blocos de 10, 25, 50 ou 100 linhas.

----

.. *Card* Histórico
.. """"""""""""""""

.. .. image:: /figuras/fig_dci/009_circuito_card_histórico.png
    :alt: Circuito card historico
    :align: center
.. ======

.. .. note:: conteúdo em elaboração.

.. ----

Submenu Circuitos
~~~~~~~~~~~~~~~~~~


Esta tela permite visualizar a lista de Circuitos, possibilitando observar as ações a serem tomadas com cada item, distribuídos nos botões e colunas. 


.. image:: /figuras/fig_dci/007_menu_circuitos.png
    :alt: Menu Circuitos 
    :align: center
======

Nesta tela, inicialmente pode-se observar as ações disponibilizadas pela aplicação, como incluir recursos desabilitados, buscar uma informação, atualizar a tela após proceder alteração e oito colunas que categorizam as informações sobre cada um dos circuitos.

Três funcionalidades são apresentadas:
  
  * Botão ``Incluir recursos desabilitados``: Ao clicar neste botão o usuário pode visualizar os recursos que estão desabilitados;
  * A ação de ``Procurar``: o sinal da lupa indica ao usuário a ação de buscar algo;
  * Botão ``Refresh``: indica que ao clicar neste botão a página é atualizada.

Na sequência, a tela circuitos exibe separadamente as oito colunas informativas, listadas abaixo:


  * Designação;
  * Tipo;
  * Banda Base;
  * Banda Atual;
  * *Port - Vlan ID*;
  * *Port - Vlan ID*;
  * *Status*;
  * *Golden Jumper*.



Ao clicar em cada circuito individualmente, é possível visualizar detalhes das informações, iniciando pelo botão com a ação de ``Voltar``, o *card* Geral, *card* Configurações, *card* Excursionamentos e por último, o *card* Histórico. 

.. image:: /figuras/fig_dci/008_menu_circuito_spo.png
    :alt: Menu Circuito spo 
    :align: center
======

Neste detalhamento do circuito listado, o usuário visualiza quatro *cards* que categorizam informações distintas:

  * Geral;
  * Configurações;
  * Excursionamentos:
  * Histórico.

----

*Card* Geral
""""""""""""
Este *card* está contido no submenu Circuito, apresenta as principais informações deste.

.. image:: /figuras/fig_dci/008_a_menu_circuito_card_geral.png
    :alt: circuito card geral
    :align: center
======

Composto de oito elementos como mostra o exemplo acima, eles refletem o panorama geral do circuito ao usuário, inclusive as portas que ligam-se através do circuito, listados na sequência:

  * Usuário;
  * Nome da empresa;
  * CPF/CNPJ;
  * Designação;
  * Data da criação;
  * Data da ativação;
  * Porta origem;
  * Porta destino.

----

*Card* Configurações
""""""""""""""""""""

O segundo *card* do submenu Circuito, apresenta as principais informações deste.

.. image:: /figuras/fig_dci/008_b_menu_circuito_card_configurações.png
    :alt: circuito card configurações
    :align: center
======

O *card* Configurações disponibiliza no seu lado superior direito a funcionalidade de atualizar a página, ela pode ser acionada pelo botão ``Refresh``. Este *card* disponibiliza algumas informações como:

  * Status: “Ativado” e na sequência o botão ``Bloquear``;
  * O motivo do bloqueio:
         * Tipo e na sequência o botão ``Alterar tipo``;
         * Banda atual;
         * Vlan porta origem e na sequência o botão ``Alterar vlans``;
         * Vlan porta destino.

----

*Card* Excursionamentos
"""""""""""""""""""""""

O terceiro *card* do submenu Circuito, apresenta as principais informações deste.

.. image:: /figuras/fig_dci/008_c_menu_circuito_card_excursionamentos.png
    :alt: circuito card excursionamentos
    :align: center
======

Ao visualizar o *card* Excursionamentos neste é permitido utilizar os dois botões localizados à direita, são eles: ``+Criar excursionamento`` e ```Refresh``. Este *card* exibe sete colunas contendo informações como:

  * Banda;
  * Data de início estimada;
         * Data final estimada;
         * Data de início;
         * Data final;
         * Status;
         * Ação.

----

*Card* Histórico
""""""""""""""""
O último *card* do submenu Circuito, apresenta as seguintes informações sobre o histórico de ações realizadas: 

.. image:: /figuras/fig_dci/009_circuito_card_histórico.png
    :alt: Circuito card historico
    :align: center
======

  * Operação:
  * Autor;
  * Data e Hora. 

Ao final é exibido um bloco com a opção de selecionar as informações em blocos de 10, 25, 50 ou 100 linhas.

----

Submenu Excursionamentos
~~~~~~~~~~~~~~~~~~~~~~~~

*Card* Geral
""""""""""""

Este submenu possibilita a visualização dos Excursionamentos: finalizados, interrompidos, pendentes, agendados ou ativados do usuário, nele é possível verificar além dos status do excursionamento, a quantidade de banda a ser expandida no circuito e a banda base do mesmo, tendo-se as datas de começo e finalização estimadas e as datas em que o excursionamento realmente aconteceu ou finalizou, as portas e suas Vlans também estão disponíveis para visualização.

Nesta tela são exibidas as opções para duas funcionalidades:

  * Botão ``Refresh``: indica que ao clicar neste botão a página é atualizada;
  * Botão de ação ``+ Criar Excursionamento``: o sinal de mais indica ao usuário que ao clicar pode criar algo.


.. image:: /figuras/fig_dci/013_menu_excursionamentos.png
    :alt: excursionamentos
    :align: center
======

Para agendar um excursionamento é necessário clicar no botão ``+ Criar Excursionamento`` e preencher os campos no modal apresentado.


.. image:: /figuras/fig_dci/013_submenu_criar_excursionamento_circuito.png
    :alt: criar excursionamento circuito
    :align: center
======

Ao visualizar este novo modal para criar excursionamento o usuário observa os seguintes campos:

  * Data de início;
  * Data final e horário;
  * Circuito.

No campo "data de início" o usuário seleciona a data pretendida para o agendamento do começo deste excursionamento e a data desejada para o término deste. Além de informar no espaço seguinte sobre qual circuito esse excursionamento deve ser executado.  

Após o preenchimento desses dados é exibido ao usuário a capacidade base do circuito selecionado, além da capacidade máxima possível para aquele circuito e o campo "Banda" que permite selecionar a banda estimada, de acordo com a imagem seguinte: 


.. image:: /figuras/fig_dci/013_submenu_criar_excursionamento_banda.png
    :alt: criar excursionamento banda
    :align: center
======

Ao finalizar o preenchimento com os dados necessários, o usuário pode clicar no botão ``Criar excursionamento`` e seguir à próxima etapa deste fluxo. 

.. note:: O botão ``Cancelar`` pode ser acionado a qualquer momento, no caso da desistência desta criação.

Após criado o excursionamento, a operação está completa. Ela possibilita ao usuário verificar o mesmo no submenu "Excursionamento" com todas as suas informações, juntamente com a opção de cancelar tal excursionamento.  

----


Menu **Tarefas**
----------------

Na aba de tarefas é possível acompanhar todas as operações realizadas dentro da plataforma.

----

Painel de Tarefas
~~~~~~~~~~~~~~~~~


Como supracitado, a tela de tarefas é importante para acompanhar o andamento dos pedidos realizados na plataforma. 

.. image:: /figuras/fig_dci/010_menu_tarefas.png
    :alt: Menu Tarefas 
    :align: center
======

Este menu possibilita visualizar quaisquer casos de erro, acompanhar o *status* dos pedidos e cancelar algumas operações. 


.. image:: /figuras/fig_dci/011_recorte_menu_tarefas.png
    :alt: Cabeçalho Tarefas 
    :align: center
======

A tela acima apresenta na parte superior direita o símbolo de tarefas, o nome do usuário logado, em seguida as funcionalidades:

  * Botão ``Pesquisa``: Campo que facilita encontrar as informações com agilidade. 
  * Botão ``Refresh``: Permite atualizar a página com apenas um clique.



As tarefas são apresentadas em formato de lista, categorizadas em abas contendo as informações sobre: 

       * Tarefas;
       * Aprovações pendentes;
       * Tarefas agendadas.
 
.. image:: /figuras/fig_dci/012_menu_tarefas_abas_listas.png
    :alt: Lista de tarefas 
    :align: center
======

A aba "Tarefas" exibe onze tipos de informações divididas em colunas: 

  * Operação;
  * ID do pedido;
  * Designação;
  * Razão social;
  * Autor;
  * *Erro*;
  * Progresso em porcentagem;
  * Data de início;
  * Duração;
  * *Status*;
  * Ação.


Detalhando a coluna *status* que mostra três estados distintos:

 * São eles ``Sucesso``, ``Falha`` ou ``Aprovada``.

O objetivo deste estado é direcionar a ação de acompanhamento, de acordo com o seguinte:

  
**Status de Sucesso** - exibido na coloração verde, significa que a operação foi concluída com sucesso.
 
  
**Status de Falha** - apresentado na coloração vermelha, significa que ocorreu algum problema durante a operação. Na própria tarefa falhada é possível constatar qual é o motivo da irregularidade, através da coluna de "Erro".

  
**Status de Aprovada** - mostrada na coloração verde, significa que a operação ocorreu com sucesso. Porém depende de alguma ação do usuário, seja ele o "admin" ou "user": 

    * Para casos como "Primeira Venda", fica pendente ao usuário a confirmação do *Golden Jumper* de ambas as portas. 

    * Para os casos de venda subsequente de portas, fica pendente o *Golden Jumper* da porta em questão.


====


Conclusão
---------

Este documento apresentou a descrição das funcionalidades contidas no produto **Data Center Interconnect - DCI**, desenvolvido pela Ustore.


====

**Equipe Ustore**

DCI Manual de funcionalidades - v.5 - Atualização 25/07 Revisão 03/08/2023 - Criado em 08/02/2023.



.. |icone_tarefas| image:: /figuras/ucloud_icone_sino.png 
