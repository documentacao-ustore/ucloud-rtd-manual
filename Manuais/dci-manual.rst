
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

Em termos descomplicados, significa que as funções de controle e dados da rede estão separadas, o que permite maior flexibilidade e automação no gerenciamento de rede.


----

Como logar no DCI
-----------------


Para ter acesso à plataforma é necessário ter realizado uma primeira compra no Painel do Cliente. 

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


Neste primeiro contato é importante entender o impacto de algumas ferramentas existentes no menu superior direito, exibido ao usuário no acesso, após seu login no DCI. 
  

A imagem seguinte é um recorte do menu superior direito, ele demonstra componentes relevantes ao usuário, detalhados a seguir como:


  * Nome; 
  * E-mail;
  * Configurações de conta;
  * Acesso a este manual de funcionalidades;
  * Logout.


.. image:: /figuras/fig_dci/002_nome_config_manual_logout.png
    :alt: visão geral
    :align: center
======

 
**Ícone de notificação**  |icone_tarefas|: Este ícone é um ponto relevante para a visualização de todas as atividades que são realizadas no Portal. Através deste é possível observar as ações mais recentes, refletidas em forma de notificação na tela de Tarefas.

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
    :scale: 100 % 
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
    :scale: 100 % 
    :align: center
======


Submenu Portas
~~~~~~~~~~~~~~


Este submenu possibilita visualizar os recursos de portas, além disso, pode-se observar as ações disponbilizadas como incluir recursos desabilitados, buscar uma informação, atualizar a tela após modificação e seis colunas que categorizam as informações sobre cada uma das portas. 


.. image:: /figuras/fig_dci/005_menu_portas.png
    :alt: Menu Portas 
    :align: center
======

Três funcionalidades são apresentadas: 

  * O botão para ``Incluir recursos desabilitados``; 
  * A ação de ``Procurar``;
  * O botão para atualização da página ``Refresh``.

As informações das portas, são divididas em seis colunas e apresentadas, conforme mencionadas abaixo:

  * Designação;
  * *Status*;
  * Banda;
  * Tipo;
  * *Data Center*;
  * *Golden Jumper*.



Ao selecionar uma porta, é possível visualizar os detalhes de forma completa, esta nova página apresenta em seu cabeçalho algumas opções acionadas pelos botões de ``Voltar`` ,  ``Baixar LOA``, ``Reenviar LOA`` e  ``Confirmado``, no corpo da tela estão distribuídos os *cards* a seguir descritos. 

.. image:: /figuras/fig_dci/006_menu_porta_spo.png
    :alt: Menu porta spo 
    :align: center
======

O submenu Portas exibe alguns *cards* categorizados com as informações: 

  * Geral;
  * Vlans;
  * Histórico.

----

*Card* Geral
""""""""""""

Os elementos deste *card* “Geral” são divididos em catorze tipos:

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

A funcionalidade de atualização da página ``Refresh`` é apresentada, e as informações são divididas em quatro colunas: 

  * Vlans em Uso;
  * Circuitos;
  * Banda;
  * Banda Base.

As informações sobre as Vlans são exibidas em blocos de 10, 25, 50 ou 100 linhas.

----

Submenu Circuitos
~~~~~~~~~~~~~~~~~~


Esta tela permite visualizar seus recursos de circuitos, possibilitando observar as ações a serem tomadas com cada item. 


.. image:: /figuras/fig_dci/007_menu_circuitos.png
    :alt: Menu Circuitos 
    :align: center
======

Nesta tela, inicialmente três funcionalidades são apresentadas em formato de botão, são elas:
  
  * Botão ``Exibir recursos desabilitados``;
  * A ação de ``Procurar``: o sinal da lupa indica ao usuário a ação de buscar algo;
  * Botão ``Refresh``: indica que ao clicar neste botão a página é atualizada.

Na sequência, a tela circuitos exibe separadamente em oito colunas informativas, listadas abaixo:


  * Designação;
  * Tipo;
  * Banda Base;
  * Banda Atual;
  * *Port - Vlan ID*;
  * *Port - Vlan ID*;
  * *Status*;
  * *Golden Jumper*.

.. image:: /figuras/fig_dci/008_menu_circuito_spo.png
    :alt: Menu Circuito spo 
    :align: center
======

Ao clicar em cada circuito individualmente, é possível visualizar as informações de histórico de ações realizadas e seu histórico de excursionamento nesse circuito. 


.. image:: /figuras/fig_dci/009_circuito_cardhistorico.png
    :alt: Circuito card historico
    :align: center
======


Além disso, é permitido realizar algumas operações dentro do circuito, como por exemplo, a alteração de VLAN ou a mudança de tipo. 

----


Menu Tarefas
------------

Na aba de tarefas é possível acompanhar todas as operações realizadas dentro da plataforma.

.. image:: /figuras/fig_dci/010_menu_tarefas.png
    :alt: Menu Tarefas 
    :align: center
======


Painel de Tarefas
~~~~~~~~~~~~~~~~~


Como supracitado, a tela de tarefas é importante para acompanhar o andamento dos pedidos realizados na plataforma. 

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
       * Aprovações Pendentes;
       * Tarefas Agendadas.
 
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

Este documento apresentou uma descrição breve das funcionalidades contidas no produto Data Center Interconnnect - DCI, desenvolvido pela Ustore.


====

**Equipe Ustore**

DCI Manual de funcionalidades - v.4 - Revisão 25/07/2023 - Criado em 08/02/2023.



.. |icone_tarefas| image:: /figuras/ucloud_icone_sino.png 
