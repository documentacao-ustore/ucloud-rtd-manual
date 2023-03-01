
.. image:: /figuras/index/_ustore_pequena.png
    :alt: logo ustore
    :align: center
======



DCI - Manual de Funcionalidades  
===============================

Soluções em tecnologia da informação que viabilizam implementar uma arquitetura computacional escalável, sólida e confiável em nuvem híbrida.

====


Introdução
----------


Este documento consiste em um manual com a descrição breve das principais funcionalidades contidas no produto DCI da plataforma Ustore.


Login
-----


Para ter acesso à plataforma é necessário,  ter realizado uma primeira compra no Painel do Cliente. 

Após essa compra o usuário recebe suas credenciais de acesso, enviadas diretamente ao seu e-mail registrado. 


.. image:: /figuras/fig_dci/01_log_in.png
    :alt: login
    :align: center
======

O usuário deve preencher os campos ``login`` e ``senha``, com as credenciais recebidas do administrador da plataforma. 

Clicar no botão ``Entrar``. 

Após este procedimento, a tela inicial do Portal é apresentada.


Visão Geral
-----------


De início, é importante entender o impacto de algumas ferramentas existentes no menu superior direito. 
  

Para isto, o recorte do menu superior demonstrado na imagem seguinte, exibe componentes relevantes, descritos detalhadamente na sequência.



.. image:: /figuras/fig_dci/02_qa_config_logout.png
    :alt: visão geral
    :align: center
======

 
**Ícone de notificação**  |icone_tarefas|: Este ícone é um ponto relevante para a visualização de todas as atividades que são realizadas no Portal. Através dele é possível observar as ações mais recentes, refletindo em forma de notificação a tela de Tarefas.


  
**Configuração de conta**: Possibilita acessar os detalhes da conta criada, onde é possível alterar o e-mail, o telefone de contato e gerenciar usuários em seu Contrato. Este botão direciona para o menu de **Administração**.

Menu Administração
------------------

Para a completa visualização dos serviços do DCI existem alguns menus na lateral da plataforma, nestes é possível encontrar informações valiosas ao produto.
  


.. image:: /figuras/fig_dci/03_menu_adm.png
    :alt: menu administração 
    :align: center
======



**DCI**
~~~~~~~

Este menu contém submenus que possibilitam visualizar Portas, Circuitos e Excursionamentos. 


**Tarefas**
~~~~~~~~~~~~

Na aba de tarefas é possível acompanhar todas as operações realizadas dentro da plataforma.



Painel de Tarefas
-----------------


Como supracitado, a tela de tarefas é importante para acompanhar o andamento dos pedidos realizados na plataforma. 

.. image:: /figuras/fig_dci/04_menu_tarefas.png
    :alt: Menu Tarefas 
    :align: center
======

Este menu possibilita visualizar quaisquer casos de erro, acompanhar o *status* dos pedidos e cancelar algumas operações. 


.. image:: /figuras/fig_dci/04_head_tarefas.png
    :alt: Cabeçalho Tarefas 
    :align: center
======

A tela acima apresenta o símbolo do menu tarefas, o nome do usuário logado, em seguida as funcionalidades:

  * Pesquisa 
  * Refresh




As tarefas são apresentadas em formato de lista, categorizadas em abas contendo as informações sobre 

       * Tarefas
       * Aprovações Pendentes
       * Tarefas Agendadas
 
.. image:: /figuras/fig_dci/04_lista_tarefas.png
    :alt: Lista de tarefas 
    :align: center
======

A aba "Tarefas" exibe onze tipos de informações divididas em colunas: 

  * Operação
  * ID do pedido
  * Designação
  * Razão social
  * Autor
  * Erro
  * Progresso em porcentagem
  * Data de início
  * Duração
  * Status
  * Ação


Detalhando a coluna *status* que mostra três estados distintos:
 * São eles ``Sucesso``, ``Falha`` ou ``Aprovada``.

O objetivo deste estado é direcionar a ação de acompanhamento, de acordo com o seguinte:

  
**Status de Sucesso** - exibido na coloração verde, significa que a operação foi concluída com sucesso.
 
  
**Status de Falha** - apresentado na coloração vermelha, significa que ocorreu algum problema durante a operação. Na própria tarefa falhada é possível constatar qual é o motivo da irregularidade, através da coluna de "Erro".

  
**Status de Aprovada** - mostrada na coloração verde, significa que a operação ocorreu com sucesso. Porém depende de alguma ação do usuário, seja ele o "admin" ou "user": 

    * Para casos como "Primeira Venda", fica pendente ao usuário a confirmação do *Golden Jumper* de ambas as portas. 

    * Para os casos de venda subsequente de portas, fica pendente o *Golden Jumper* da porta em questão.





Tela de Portas
--------------


Nesta tela é possível visualizar seus recursos de portas, além disso, pode-se observar as ações a serem tomadas com cada item. 


.. image:: /figuras/fig_dci/05_menu_portas.png
    :alt: Menu Portas 
    :align: center
======

Três funcionalidades são apresentadas: o botão para ``Exibir recursos desabilitados``, a ação de ``Procurar`` e a de atualização da página ``Refresh``.

As informações das portas, são divididas em seis colunas, que são apresentadas, conforme mencionadas abaixo:

  * Designação
  * Status
  * Banda
  * Tipo
  * Data Center
  * Golden Jumper

Ao selecionar uma porta, é possível visualizar os detalhes de forma completa. A nova página apresenta três funcionalidades para ``Baixar LOA``, ``Reenviar LOA`` e o botão de ``Confirmado``.

.. image:: /figuras/fig_dci/06_menu_porta_bre.png
    :alt: Menu porta bre 
    :align: center
======

São exibidos também dois *cards* de informações: Geral e Vlans. 

No *card* de Vlans, a funcionalidade de atualização da página ``Refresh`` é apresentada, e as informações são divididas em quatro colunas: 

  * Vlans em Uso
  * Circuits
  * Banda
  * Banda Base

As informações sobre as Vlans são exibidas em blocos de 10, 25, 50 ou 100.




Tela Circuitos
--------------


Esta tela permite visualizar seus recursos de circuitos, possibilitando observar as ações a serem tomadas com cada item. 


.. image:: /figuras/fig_dci/07_menu_circuitos.png
    :alt: Menu Circuitos 
    :align: center
======

Ao clicar em cada circuito individualmente, é possível visualizar as informações de histórico de ações realizadas e seu histórico de excursionamento nesse circuito. 

.. image:: /figuras/fig_dci/08_menu_circuito_04.png
    :alt: Menu Circuitos 
    :align: center
======

Além disso, é permitido realizar algumas operações dentro do circuito, como por exemplo, a alteração de VLAN ou a mudança de tipo. 



====

Conclusão
---------

Este documento apresentou uma descrição breve das funcionalidades contidas no produto DCI da plataforma Ustore.


====

**Equipe Ustore**

DCI Manual de funcionalidades - 08/02/2023.



.. |icone_tarefas| image:: /figuras/ucloud_icone_sino.png 
