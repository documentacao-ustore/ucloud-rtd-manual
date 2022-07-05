uSavings - Manual do Usuário
++++++++++++++++++++++++++++


.. image:: /figuras/uSavings-logo-gde.png
    :alt: logo usavings
    :align: center
======

Soluções em tecnologia da informação que viabilizam implementar uma arquitetura computacional escalável, sólida e confiável em nuvem híbrida.

----


Apresentação
============

Este documento tem como objetivo apresentar as principais características e funcionalidades relacionadas a aplicação *uSavings*. 

Neste Manual são apresentados os conceitos, as telas, as funcionalidades e os comandos para uso deste produto.

----


Visão e posicionamento
======================

Este documento descreve a aplicação uSavings, a visão e o posicionamento do produto.
Importa esclarecer que ele se encontra em constante desenvolvimento e evolução, por isto, as telas apresentadas neste documento podem sofrer alterações a qualquer momento, por conta da evolução do software.

A presente tendência, a cada momento mais forte, da migração de recursos computacionais das nuvens privadas ou ambientes de *co-location*, para o ambiente  dos provedores de nuvem pública, representa um dos grandes desafios das organizações que é a Governança de Custos decorrentes do alto uso destes recursos computacionais e, consequentemente, as empresas não conseguem obter as devidas visualizações destes custos no futuro.

Atualmente, a quase totalidade de plataformas de *Cloud Service Broker (CSB)* podem apresentar sugestões de redução de custos, porém, a obtenção de alguns valores são dependentes de um serviço (ou ação) humana, para obter tais valores.

Os provedores de serviço de nuvem pública, continua e initerruptamente, disponibilizam novas configurações de hardware (*flavors*) com características similares, mas valores, por vezes, muito diferentes. Neste momento, fica a critério de um especialista de arquitetura efetuar uma busca por configurações de hardware possíveis e compatíveis.

A Plataforma uSavings preenche estas atividades de forma automatizada para que as comparações de configurações de hardware e/ou custos recorrentes possam ser apresentados de forma mais clara para o usuário desta plataforma.

A Plataforma uSavings, obtém o inventário de todos os recursos computacionais de nuvem pública através da sua integração com a Plataforma uCloud. Portanto, a relação de recursos computacionais de servidores apresentado na interface da Plataforma uSavings é a representação fiel do seu ambiente encontrado no provedor de serviço de nuvem pública, desta forma, a realidade existente em seu ambiente.

Todas as opções de alternativas de configuração de hardware são informadas como **sugestões**, pois fica a critério do usuário efetuar a troca (reconfiguração) do hardware do recurso computacional (*flavor*) no melhor momento para o seu ambiente.

Importante ressaltar que a Plataforma uSaving apresentará somente **sugestões**, pois qualquer troca de configuração de hardware (*flavor*) somente pode ser efetuada com a infraestrutura desligada (**à frio**), desta forma, o usuário deve gerenciar o melhor momento (dia e hora) para atuar nesta mudança de configuração.

A integração com a Plataforma uCloud, permite ao usuário visualizar as sugestões apresentadas na interface da Plataforma uSavings, para que possa identificar corretamente o recurso computacional, e, através da Plataforma uCloud executar a tarefa da troca de configuração de hardware (*flavor*) diretamente no ambiente do provedor de serviço de nuvem pública, sem a necessidade do usuário estar conectado no console do provedor de nuvem pública.

O que é uSavings ?
------------------

O uSavings é uma ferramenta que analisa em tempo real o consumo da infraestrutura dos recursos computacionais (das máquinas virtuais, abreviado como VMs) nas diferentes nuvens, é por meio desta análise que a aplicação recomenda modificações. No caso de a organização acolher ou apoiar esta sugestão, tal decisão poderá permitir gerar o máximo de economia financeira e otimização dos recursos criados e/ou executados. A aplicação uSavings é um “cost advisor", ou seja, um consultor de custos que permite aconselhar o usuário como reduzir os custos da sua infraestrutura, bilhetada pela Plataforma uCloud, nos diversos provedores de serviços de nuvem - AWS, Azure, Google, IBM e VMWare.

Como funciona ?
---------------

A plataforma do uSavings além de obter dados das diversas nuvens, extrai a informação dos dados históricos da própria Virtual Machine (máquina virtual) e da bilhetagem de cada provedor de nuvem pública – a coleta destes dados é iniciada com a integração à Plataforma do uCloud. A aplicação apresenta um painel consolidado e sugestões dos gastos do cliente em cada provedor de nuvem, entregando assim, informações precisas para a melhor tomada de decisão sobre os custos alocados dos recursos de infraestrutura da organização.

.. image:: /figuras/fig_usavings/organograma_funcionamento_usavings001.png
    :alt: organograma de funcionamento do usavings
    :align: center
====


A imagem acima representa o organograma de funcionamento do uSavings: nele a máquina virtual do uCloud (VM), é um dos elementos principais neste fluxo, conforme demonstrado no diagrama acima. O seguinte elemento apresentado é o *Flavor*, ele possibilita saber o quanto de memória, vCPU entre outros recursos são utilizados pela máquina. Logo, é a partir do *Flavor* que se sabe o quanto determinada máquina custará no final do mês. Com estes dados, é possível para a plataforma do uSavings sugerir ao cliente economia de recursos na fatura mensal.

.. image:: /figuras/fig_usavings/002_recorte_organograma.png 
    :alt: recorte do organograma do usavings
    :align: center
====


O recorte no organograma, destaca a parte pertinente no diagrama, ela representa a forma sugestiva da aplicação do uSavings. Existem duas maneiras para recomendar as melhorias para uma determinada Virtual Machine: (i) por Flavor e (ii) por Billing.

* **Por Flavor** - O uSavings checa o *Flavor* alocado na máquina, e sugere uma possibilidade de melhoria – esta melhoria se relaciona ao custo beneficio – a aplicação publica os resultados em diversos formatos (gráficos ou porcentagem) e mostra qual será a melhor cloud a ser utilizada para economizar recursos, para a VM. Este parâmetro, por dedução, entende que a máquina fica ligada o tempo todo.

* **Por Billing** - A bilhetagem do banco de dados do uCloud suporta diversas nuvens, ela difere do alcance da aplicação do uSavings. O banco de dados do uCloud pode comportar todos os tipos de billing disponíveis. Já na regra de negócio do uSavings, só é possível fazer uma sugestão assertiva com o billing para a AWS e AZURE, como mostra o diagrama, na figura recorte do organograma, apresentada acima deste parágrafo.

Como economizar recursos ?
--------------------------

A vantagem da implantação do uSavings nas organizações é a possibilidade de receber informação sobre recursos ociosos que foram criados, e até, executados anteriormente, atualmente não utilizados. Informação que pode possibilitar a economia de recursos.

Pelo fato da aplicação do uSavings ser uma ferramenta que analisa em tempo real o consumo da infraestrutura dos recursos computacionais nas diferentes nuvens, a aplicação uSavings exibe os recursos ociosos criados. 

A ferramenta é relevante para a tomada de decisão nas organizações, pois ao analisar a informação obtida pela aplicação entrega resultados reais. Isto contribui para uma decisão organizacional capaz de gerar economia financeira e otimização dos recursos criados e/ou executados.

A aplicação uSavings pode referenciar sugestões de redução da configuração – ‘rightsizing’ de máquinas virtuais, caso tenham sido previamente criadas com ‘super configurações’ e/ou apresentarem um baixo consumo no histórico de performance. **Direciona** a possibilidade de ampliar a relação custo-consumo, a aplicaçãoout **não a executa**. O objetivo da implantação da plataforma uSavings é indicar à organização a possibilidade e/ou caminho para aumentar a economia dos seus custos, no próximo período de cobrança do provedor de serviço de nuvem.

.. attention:: A organização munida das informações, entregues pela aplicação uSavings, deve entrar em contato com o provedor do serviço de nuvem sobre ‘rightsizing’.

Ao adquirir a plataforma uSavings, as organizações podem ter em mãos uma valiosa ferramenta estratégica e de inteligência de negócio (BI) que indica o melhor caminho para ampliar a relação “custo-benefício” das suas infraestruturas virtuais e, também, a melhor forma de maximizar os recursos das máquinas virtuais criadas nos provedores de serviços de nuvem.

Otimizações recomendadas após o monitoramento
---------------------------------------------

As quatro otimizações, a seguir, podem ser propostas com base em sugestões de:

Rightsizing :
~~~~~~~~~~~

Consiste na sugestão da melhor combinação de CPU e memória, com o objetivo de minimizar os custos e maximizar o desempenho. A ferramenta coleta métricas de desempenho para determinar o consumo médio e máximo de recursos de uma instância em um período configurável e recomenda uma modificação para um tipo de configuração de máquina virtual ‘VM’ de menor configuração ou de configuração apropriada para o projeto.

Custos Comparativos :
~~~~~~~~~~~~~~~~~~~

Apresenta ao usuário a relação atual das suas máquinas virtuais ‘VMs’ e uma sugestão do que seria a ‘melhor configuração’ em cada provedor de nuvem. Permite ao usuário avaliar qual provedor está com o menor custo em determinada máquina virtual ‘VM’ , na data que foi obtido o valor deste custo.

Monitoramento de Recursos Ociosos :
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O monitoramento de recursos ociosos permite checar se os recursos estão em uso. É possível monitorar os recursos criados e não utilizados.

Instâncias Reservadas :
~~~~~~~~~~~~~~~~~~~~~

Sobre a instância reservada, a aplicação uSavings consegue mostrar ao cliente-usuário que no caso da alteração de uma máquina *on-demand* para uma máquina reservada – a instância reservada consegue exibir o quanto é possível economizar em relação a atual máquina.

**Por exemplo:**

Ao utilizar o provedor AWS, as instâncias reservadas (*Reserved Instances - RIs*) da Amazon EC2 são uma das formas mais óbvias de controlar os custos de computação, permitindo ao usuário reservar capacidade de computação EC2 em troca de taxas horárias com descontos significativos.

É importante observar e reforçar ao cliente/usuário que as instâncias reservadas (AWS, AZURE ou instância preemptiva Google) não são instâncias que o usuário possa criar e executar por um preço menor do que as instâncias normais. E, deve ser considerado que não há garantia de que estes serviços computacionais sejam dedicados ao cliente ou estejam disponíveis e acessíveis durante os 365 dias do ano. 

Caso o provedor de serviços de nuvem necessite ter acesso a estes recursos computacionais, para outro tipo de tarefa, o provedor pode encerrar estas instâncias a qualquer momento (ou seja, forçar a interrupção destas VMs) sem obrigação da prévia comunicação.

----


Menu inicial
============

A interface inicial apresentada ao usuário é um painel de controle (*Dashboard*) que exibe um resumo da atual infraestrutura, endereçável e acessível por meio da plataforma do uCloud. Ao efetuar o acesso à interface do uSavings, o usuário se conecta automaticamente com a sua atual infraestrutura de máquina virtual ‘VMs’. Desta forma, o usuário visualiza os custos atuais das máquinas virtuais ‘VMs’ existentes, pode comparar os custos das suas máquinas virtuais entre os diversos provedores de serviços públicos de infraestrutura de nuvem.

O uSavings permite criar manualmente uma lista de máquinas virtuais ‘VMs’ com configurações específicas (uma configuração privada e/ou ‘imaginária’), para o caso do usuário que deseja obter a relação completa das suas máquinas virtuais e prefere conectar-se de forma manual.

Como acessar a plataforma uSavings
----------------------------------

O acesso à plataforma uSavings é realizado pela web, podendo ser utilizado qualquer um dos navegadores: **Firefox**, **Google Chrome** ou **Microsoft Edge**, em diversos sistemas operacionais, a exemplo do **Microsoft Windows** 10 ou 11.

.. attention::
    *Importante ressaltar que a Plataforma uCloud não é compatível com o Microsoft Internet Explorer (IE) em qualquer versão, pois as tecnologias deste navegador se encontram desatualizadas e não suportam a evolução das atuais páginas HTML.*

Para o acesso inicial é necessário solicitar as credenciais ao administrador - ao receber o link com o endereço e as credenciais de acesso, o usuário deve utilizar seu navegador de preferência para acessar a web e conectar-se. Outra forma de acesso à plataforma do uSavings é direto da plataforma do uCloud, pelo seu menu lateral esquerdo. 

Para o caso de o acesso ser realizado direto na web, a imagem abaixo será mostrada ao usuário. Neste momento, ele deve inserir as credenciais recebidas.

.. image:: /figuras/fig_usavings/003_tela_acesso_inicial.png 
    :alt: tela de acesso inicial
    :align: center
====

O usuário deve preencher os campos **‘login’** e **‘senha’**, com as credenciais recebidas do administrador da plataforma. Clicar em **‘Entrar’**. Após este procedimento, a tela inicial do Dashboard será apresentada. 

Se a tela de Dashboard não for apresentada, isto significa que algum dos campos estão preenchidos com informações inconsistentes, ou seja, ‘login’ ou ‘senha’ inexistentes e/ou pode ter havido um erro na digitação das informações. É importante checar e repetir a operação.

.. image:: /figuras/fig_usavings/004_tela_problema_acesso.png 
    :alt: tela de problema no acesso 
    :align: center
----

No caso de insucesso ao logar, será apresentada ao usuário a imagem acima, com a seguinte orientação: **(i)** checar as credenciais e **(ii)** repetir a operação.



Visão geral
===========

De início, antes de adentrar na sessão do **Dashboard** é relevante entender o impacto de algumas ferramentas existentes no menu superior.

.. image:: /figuras/fig_usavings/005_recorte_menu_superior.png 
    :alt: recorte do menu superior
    :align: center
----

Para isso, o recorte do menu superior demonstrado na imagem acima, exibe componentes relevantes, a seguir descritos em detalhe, seguindo a ordem: da esquerda para a direita.

Ícone de Troca de Contrato
--------------------------

Este ícone |icone_ustore| é um ponto relevante a fazer uma ressalva, ao partir da premissa de que há a possibilidade de um usuário cadastrado na plataforma do uCloud fazer parte **de mais de um grupo** de usuários. Logo ele pode fazer parte de mais de um contrato. E, existe a possibilidade de selecionar um outro contrato, este contrato selecionado pode conter outros recursos atrelados a este contrato. 

.. image:: /figuras/fig_usavings/006_troca_contrato.png 
    :alt: troca de contrato
    :align: center
----

Este ícone de troca de contrato apresenta todos os contratos nos quais o usuário logado na plataforma uSavings participa. Assim, é permitido ao usuário trocar entre eles livremente. A troca de contrato pode implicar na troca dos recursos que serão apresentados ao usuário, pois cada contrato pode ter uma determinada característica, na sequência deste manual de uso do uSavings estas minucias serão descritas.

Ícone de Configuração de Clouds
-------------------------------

Como introdução sobre a usabilidade deste recorte da tela: |icone_configuracao|

Pode-se afirmar que o termo *Clouds* é empregado para abstrair um agrupamento de *Flavors* de uma determinada Cloud, sendo este agrupamento tanto de *Flavors* reais quanto imaginários.

.. image:: /figuras/fig_usavings/007_configuracoes_clouds.png 
    :alt: configuracoes de clouds
    :align: center
----

No menu de configurações existe a parte de criação de *Clouds*, alteração da atividade das *Clouds* e a área de criação de novas *Clouds*.

.. image:: /figuras/fig_usavings/008_configuracao_alteracao_atividade.png 
    :alt: configuracao de alteracao de atividade
    :align: center
----

Ícone Lista de Troca de Idiomas
-------------------------------

Este ícone |icone_lista_troca_idioma| permite trocar o idioma na plataforma uSavings, a plataforma originalmente está em português e pode ser alternada para o Espanhol e para o Inglês, basta apenas clicar no ícone com as bandeiras: |icone_bandeira_troca_idioma|

.. |icone_bandeira_troca_idioma| image:: /figuras/fig_usavings/icone_bandeira_troca_idioma.png

Ícone Nome do Usuário Logado
----------------------------

Este ícone |icone_nome_usuario_logado| apresenta o nome do usuário que está logado na plataforma uSavings.

Ícone de LogOut
---------------

Este ícone |icone_logout| desloga o usuário da plataforma.


Painel de controle *Dashboard*
==============================

A interface inicial do uSavings exibida ao usuário é um painel de controle *(Dashboard)*.

.. image:: /figuras/fig_usavings/009_menu_entrada_dashboard.png
    :alt: menu de entrada do dashboard
    :align: center
----

Este painel, imagem apresentada acima, exibe alguns dados na tela que retratam um resumo da atual infraestrutura endereçável e acessível pela plataforma, estes dados são compostos de segmentações denominadas *Cards*.

.. image:: /figuras/fig_usavings/010_tela_inicial_dashboard_funcionalidades.png 
    :alt: tela inicial: dashboard e funcionalidades
    :align: center
----

Na primeira parte da tela inicial, apresentada na imagem acima, **são espelhados somente os serviços de nuvem** que a organização **possui na plataforma do uCloud** e **autoriza a integração**, sendo o acesso pela aplicação uSavings.

.. image:: /figuras/fig_usavings/011_container_conectado_plataforma_ucloud.png 
    :alt: container conectado na plataforma uCloud
    :align: center
----

Neste caso, a imagem do container conectado na plataforma uCloud apresenta a relação dos containers que participam do contrato no qual o usuário está conectado. Esta autorização de acesso funciona a partir do Contrato, conforme o exemplo a seguir:

.. note:: Quando um determinado container da plataforma do uCloud, está contido no Virtual Datacenter, que por sua vez faz parte de um contrato em que o usuário logado na plataforma do uSavings participa. 

Desta forma, existe o acesso aos dados do container, sendo somente após este acesso e análise dos dados que a plataforma do uSavings pode sugerir as melhorias de performance de uso.

O *Dashboard* permite a visualização rápida sobre cada uma das nuvens conectadas ao uCloud, as quais são refletidas na aplicação uSavings. No caso de a nuvem do usuário estar ausente do uSavings, isto significa que a nuvem não foi conectada na plataforma do uCloud.

A seguir, neste documento, os quatro *cards* exibidos na tela do Dashboard são descritos em detalhes.

Latest Months
-------------

O primeiro *card* **Latest Months**, apresenta a bilhetagem ocorrida no período relacionado aos últimos seis (6) meses, ou seja, serão listados todos os valores investidos em determinada conta, por um período relacionado aos últimos 6 meses.

.. image:: /figuras/fig_usavings/012_latest_months.png 
    :alt: Latest months
    :align: center
----

Tal valor é coletado a partir de valores gerados pelo *job* do uSavings, responsável por sumarizar o Billing da plataforma do uCloud.

.. image:: /figuras/fig_usavings/013_grafico_investimentos_real_versus_meses.png 
    :alt: grafico de investimentos em real x 6 ultimos meses 
    :align: center
----

O gráfico constante na imagem acima apresenta o valor do custo em Dólar *versus* o período requerido dos últimos 6 meses.

Consolidated Cost
-----------------

O segundo *card* **Consolidated Cost** exibe algumas sugestões na tela do Dashboard, estas sugestões são relacionadas ao que a máquina virtual “VM” selecionada contêm, é relevante mencionar que todos os valores são apresentados em dólar. O card mostra o *Flavor* e as regiões habilitadas para a máquina, a reunião destas informações permite sugerir melhorias para otimizar o uso.

Neste *card* são detalhadas as informações a respeito do percentual de economia, diferença de custo, custo corrente despendido, custo otimizado e *Flavors* utilizados e/ou sugeridos pela aplicação. Valores apresentados em dólar.

.. image:: /figuras/fig_usavings/014_custos_consolidados.png 
    :alt: custos consolidados 
    :align: center
----

Na imagem acima, observa-se que o percentual de 65,25% no campo *Saving* representa o percentual de economia que a aplicação uSavings entrega como resultado, baseado na sugestão de mudança de *Flavor* dentro da própria nuvem. Ou seja, o usuário está realizando uma pesquisa na nuvem AWS, a economia exibida de 65,25% é possível implementar ao trocar de *Flavor* dentro da própria nuvem. 

As informações detalhadas, neste *Card* de custos consolidados, apresentam uma riqueza de detalhes para o entendimento entre a melhor combinação de CPU, memória e disco, com foco na redução dos custos:

  * **Saving** – Mostra o percentual de economia (na cor verde) ou dispêndio (na cor vermelha) baseia-se no consumo atual e compara com as otimizações sugeridas;

  * **Difference Cost** – Representa o mesmo cálculo usado pelo *Saving* sendo que revela a diferença em Real (R$);

  * **Current Cost** – Apresenta o valor que está sendo despendido, em referência ao período que a análise foi coletada.

  * **Otimized Cost** – Indica o valor futuro, caso as mudanças sugeridas sejam aceitas e implementadas.

    * **Obs:** Todos os valores exibidos podem sofrer mudanças no decorrer do período, a depender do consumo trafegado nas nuvens.

Actual Flavor
-------------

Este terceiro *Card* apresenta o *Flavor* das máquinas selecionadas deste container, caso seja modificado, ele carrega as novas informações. A exibição das porcentagens utilizadas pelo *Flavor* é apresentada pelo gráfico de pizza e sua representatividade ocorre por tipo, no conjunto total da infraestrutura.

Todos os valores são exibidos em dólar, sem tributação de impostos. Os preços têm origem na tabela importada diretamente do provedor de nuvem e inserida no banco de dados desta aplicação. O preço é calculado a partir da quantidade de horas que compõem o mês.

.. image:: /figuras/fig_usavings/015_grafico_actual_flavors.png 
    :alt: gráfico actual flavors 
    :align: center
----

As informações contidas na imagem acima, se referem ao ambiente AWS, onde cada item difere em relação ao tamanho da memória, vCPU, preço e sistema operacional e, ao final, é apresentado o valor total do custo dos *Flavors* atualmente utilizados.

Sugested Flavors
----------------

Este *Card* apresenta um outro tipo de gráfico, a partir do *card Actual Flavors* ele demonstra quanto seria a diferença a partir da sugestão de economia referenciada. Ou seja, o quanto é possível salvar do recurso criado que está ocioso, ao apresentar as informações do consumo atual e a sugestão de consumo num gráfico de colunas. 

A coluna azul representa o gasto atual, a coluna verde sugere a economia que pode ser gerada, no caso da aplicação das sugestões de melhoria de consumo dos recursos apresentadas pela plataforma do uSavings.

.. image:: /figuras/fig_usavings/016_sugested_flavors.png 
    :alt: sugested flavors
    :align: center
----

Os gráficos e as informações apresentadas são uma **análise inicial** da economia potencial dos valores que a organização pode se beneficiar ao adotar as recomendações sugeridas pela plataforma uSavings. 

Os valores apresentados se referem ao período da coleta de dados (o período mínimo inicial é de quinze dias). Quanto mais longo for o período da coleta de informações, mais confiável será a estimativa da economia calculada.

.. image:: /figuras/fig_usavings/017_tela_entrada_dashboard_1.2.png 
    :alt: tela entrada dashboard (parte 1/2)
    :align: center
----

Esta análise inicial é calculada com base no uso, ou seja, na ocupação dos recursos computacionais das máquinas virtuais ‘VMs’ dentro do período armazenado na base de dados da plataforma uSavings.

.. image:: /figuras/fig_usavings/018_tela_entrada_dashboard_2.2.png 
    :alt: tela entrada dashboard (parte 2/2)
    :align: center
----

O resultado desta análise é a sugestão da melhor combinação de CPU e memória. Sugestão que objetiva a redução dos custos e a maximização do desempenho *(rightsizing)*. A análise não faz o cálculo comparativo entre os valores de configuração das máquinas virtuais ‘VMs’ em outros provedores.

----


Menu Funcionalidades
====================

No lado esquerdo do menu de entrada da plataforma do uSavings são listados os menus de funcionalidades, são eles: *Virtual Machines*, *Compare Clouds*, *Imaginary Cloud*, *Container Hint* e o menu de acesso à plataforma uCloud.

.. image:: /figuras/fig_usavings/019_submenu_funcionalidades.png
    :alt: submenu funcionalidades
    :align: center
----

Virtual Machines
----------------

No menu Virtual Machines são apresentadas todas as máquinas virtuais da infraestrutura do usuário (ou seja, o inventário de todas as máquinas virtuais ‘VMs’ das contas pertencentes à organização).

.. image:: /figuras/fig_usavings/020_virtual_machines.png 
    :alt: virtual machines
    :align: center
----

Esta exibição permite a seleção do container específico para a análise de custos e sugestão de mudança de *flavor* na mesma cloud das máquinas virtuais listadas. Todas a informações apresentadas podem ser exportadas em relatório formato .csv.

.. image:: /figuras/fig_usavings/021_menu_virtual_machines.png 
    :alt: menu virtual machines
    :align: center
----

É relevante ressaltar que o container apontado deve estar contido no uCloud, ou seja, o container a ser analisado deve estar conectado e sincronizado na plataforma uCloud.

.. image:: /figuras/fig_usavings/022_selecionar_container.png
    :alt: selecionar container
    :align: center
----

Após selecionar o container, as informações são apresentadas em colunas, seguindo a ordem da 1ª até a 6ª coluna: 

  * 1. o nome da máquina virtual;
  * 2. o flavor utilizado;
  * 3. o custo atual da máquina é atribuído se ela estiver ligada durante o mês inteiro;
  * 4. o flavor sugerido para otimização;
  * 5. o custo mensal do flavor sugerido; 
  * 6. o valor anual da máquina virtual.

.. image:: /figuras/fig_usavings/023_informacoes_container.png 
    :alt: informações container
    :align: center
----

As sugestões exibidas *(Rightsizing)* são baseadas no consumo de CPU das máquinas virtuais, do período que ela foi criada até o presente momento. As métricas são coletadas e o cálculo é baseado nas médias de consumo, logo em seguida, a sugestão é apresentada. 

A análise do consumo de memória pode fazer parte do cálculo, caso o provedor ou as instâncias estejam prontas para fornecer as métricas necessárias. Caso a informação não esteja disponível será assumida a memória definida pelo *flavor* da instância *deployada*.

*Rightsizing* - sugestão de mudança de *Flavor*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para receber o resultado de sugestão de mudança de *Flavor*, o usuário deve selecionar o container desejado, conforme a imagem apresentada a seguir. A aplicação uSavings gera a listagem e o comparativo de preços. Basta clicar e aguardar.

.. image:: /figuras/fig_usavings/024_container_selecionado.png 
    :alt: container selecionado
    :align: center
----

Como resultado para esta operação será exibida a imagem abaixo, a qual apresenta em blocos as diversas informações, como: o *Flavor* e o Custo atual, a sugestão de *Flavor* e o custo estimado deste novo *Flavor*. Por último, exibe o custo da reserva do *Flavor* sugerido e estimado para 1 ano.

.. image:: /figuras/fig_usavings/025_resultado_estimado_selecao.png 
    :alt: resultado estimado selecao 
    :align: center
----

Caso de uso
~~~~~~~~~~~

Para iniciar o passo a passo deste caso de uso, é relevante lembrar que as máquinas virtuais listadas são provenientes da plataforma do uCloud, portanto, as nuvens conectadas no uCloud devem conter as máquinas virtuais. 

No caso da inexistência das máquinas virtuais, consultar o Manual do uCloud, no tópico: Como conectar e importar *Virtual Machine*. 

**1º Passo :** 

Selecionar a nuvem *(container)* que deseja analisar.

.. image:: /figuras/fig_usavings/026_selecionar_nuvem_vm.png 
    :alt: selecionar nuvem na vm 
    :align: center
----

**2º Passo :** 

Escolher a região que roda a *Virtual Machine* selecionada.

.. image:: /figuras/fig_usavings/027_selecionar_regiao_vm.png 
    :alt: selecionar a regiao vm 
    :align: center
----

**3º Passo :** 

O resultado da seleção é exibido conforme a imagem *Resultado estimado da seleção* posicionada acima do tópico Caso de uso, que é a lista de todas as *Virtual Machines*. Nesta mesma tela, no canto superior direito, é permitido exportar a lista de resultado em formato **.csv**. Basta clicar no botão **Export .csv**.

**4º Passo :**

Exportar o relatório para visualização em planilha excel, na máquina do usuário. O resultado será semelhante a imagem *Relatório exportado ao excel* apresentado abaixo:

.. image:: /figuras/fig_usavings/028_relatorio_exportado_excel.png 
    :alt: relatorio exportado ao excel 
    :align: center
----

**5º Passo :**

Existe a opção de analisar as informações de performance, na coluna Performance, conforme grifado na imagem a seguir. Logo após a coluna Nome, a coluna Performance apresenta um ícone com símbolo de * (asterisco).

.. image:: /figuras/fig_usavings/029_coluna_performance.png 
    :alt: coluna performance 
    :align: center
----

**6º Passo :** 

Ao clicar no ícone * **(asterisco)**, o relatório de performance é exibido:

.. image:: /figuras/fig_usavings/030_performance_maquinas.png 
    :alt: performance das maquinas
    :align: center
----

O relatório de performance proporciona a visualização do gráfico com a média do consumo de CPU e da memória da virtual máquina selecionada, num período de aproximadamente 15 a 20 dias.


Compare Clouds
--------------

Na aplicação do uSavings, a funcionalidade “Compare Clouds” permite realizar análise comparativa **Por Billing** ou **Por Container** dos custos entre a nuvem utilizada e as nuvens escolhidas para comparar.

.. image:: /figuras/fig_usavings/031_submenu_funcionalidades.png 
    :alt: submenu de funcionalidades 
    :align: center
----

Para que as unidades se tornem disponíveis é necessário a integração com a plataforma uCloud, neste caso, as contas precisam estar conectadas e sincronizadas, respeitando as definições de regras de segurança. 

O *Compare Clouds* permite realizar a análise comparativa entre a própria nuvem, assim como comparar com outras nuvens. Bem como comparar com as nuvens públicas que não estejam conectadas à plataforma do uCloud, como por exemplo: IBM, AZURE, Google, AWS. 

Existem duas maneiras de realizar esta análise comparativa, comparar **por Billing** ou **por Container**.

.. image:: /figuras/fig_usavings/032_tela_inicial_compare_clouds.png 
    :alt: tela inicial compare clouds 
    :align: center
----

Na imagem acima são apresentadas duas barras com a possibilidade de realizar a análise comparativa: 

  * **Comparar por Bilhetagem** 
  e 
  * **Comparar por Container**. 
  
Ao clicar na barra pretendida ela assume a cor laranja, conforme a imagem a seguir:

.. image:: /figuras/fig_usavings/033_selecao_compare_billing_compare_container.png 
    :alt: selecao compare billing compare container
    :align: center
----

Reforçando, para que as unidades estejam disponíveis, **é imprescindível** integrar com a plataforma do uCloud.

Comparar por Billing
~~~~~~~~~~~~~~~~~~~~

Para que seja possível fazer a análise comparativa por Billing (Bilhetagem), é necessário que o bilhetador tenha sido executado no determinado container. Atualmente, suportamos, a análise comparativa por Billing para as nuvens AWS e Azure, ver a imagem acima.

Antes de selecionar o container ou a nuvem que se deseja comparar, é necessário checar se a plataforma do uCloud está bilhetada. Pelo menos um (1) container deve estar bilhetado e conectado à plataforma uCloud.


.. note:: **Significado** do termo *estar bilhetado*: é a existência da fatura de consumo em determinado período, período mínimo de pelo menos um mês.                                                                                                                


**Etapas do passo a passo**

**1º Passo :** 

Para realizar a análise comparativa, inicialmente, clicar no botão **Compare by Billing**. Checar se a plataforma do uCloud está bilhetada, ao menos um container deve estar bilhetado e conectado à plataforma.

**2º Passo :**

Selecionar a nuvem contendo todos os seus containers, *Figura 34*. Clicar em **AWS** ou **AZURE**, em seguida clicar em **NEXT**.

.. image:: /figuras/fig_usavings/034_recorte_compare_billing.png 
    :alt: recorte compare by billing
    :align: center
----

Neste caso, a nuvem **AWS** está selecionada. Ao clicar em **NEXT**, a aplicação do uSavings apresenta a próxima tela com a pergunta: “Que nuvens participarão deste comparativo?” E solicita, ao usuário, selecionar as nuvens que deseja realizar a análise comparativa dos valores. 

**3º Passo :**

Ao selecionar a nuvem, o usuário deve preencher no calendário o período correspondente a análise.

.. image:: /figuras/fig_usavings/035_selecao_periodo_bilhetagem_nuvem_comparada.png 
    :alt: selecao periodo bilhetagem e nuvem a ser comparada 
    :align: center
----

O período é importante, pois os valores da nuvem podem sofrer alteração devido o provedor de nuvem. Por esta razão é possível escolher um determinado intervalo de tempo. Este intervalo será calculado com base no Billing gerado pelo uCloud.

**4º Passo :**

Selecionar as nuvens que participarão da análise comparativa de valores. O que inclui nuvens que o usuário não tem necessariamente conectada à plataforma do uCloud, como por exemplo, as nuvens IBM e GOOGLE, conforme a seguir.

.. image:: /figuras/fig_usavings/036_selecionar_nuvens_analise_comparar_valores.png 
    :alt: selecionar as nuvens para a analise comparativa dos valores 
    :align: center
----

**5º Passo :**

Neste caso, ao selecionar qualquer uma das nuvens públicas relacionadas, a próxima tela destina-se a escolha da região. Importa saber que esta região corresponde ao *Flavor* cadastrado na base de dados.

.. image:: /figuras/fig_usavings/037_escolher_regiao_nuvem_1.png 
    :alt: escolher a regiao por nuvem 1 
    :align: center
----

.. image:: /figuras/fig_usavings/037_escolher_regiao_nuvem_2.png 
    :alt: escolher a regiao por nuvem 2 
    :align: center
----

**6º Passo :**

Após selecionar a região por nuvem, a aplicação uSavings apresenta a imagem *Resultado após a escolha da região* com o resultado por extenso da região selecionada. E um botão que permite apagar a região, para a possibilidade de erro e escolha de outra região.

.. image:: /figuras/fig_usavings/038_resultado_escolha_regiao.png 
    :alt: resultado apos a escolha da regiao 
    :align: center
----

Para que seja possível fazer a análise comparativa por Billing (Bilhetagem), é necessário que o bilhetador tenha sido executado no determinado container. 

Atualmente, suportamos, a análise comparativa por Billing para as nuvens AWS e Azure. E, para que as **unidades se tornem disponíveis é necessário a integração com a plataforma uCloud**. Neste caso, as contas precisam estar conectadas e sincronizadas, respeitando as definições de regras de segurança.

Comparar por Container
~~~~~~~~~~~~~~~~~~~~~~

O segundo comparativo oferecido pela aplicação uSavings é a análise por Container. É necessário selecionar e avançar a sequência do processo para obter o resultado pretendido que é a análise comparativa por container. Para o processo acontecer é primordial selecionar uma outra nuvem, além da nuvem inicial escolhida. 

.. image:: /figuras/fig_usavings/039_selecao_comparativo_container.png 
    :alt: selecao do comparativo por container 
    :align: center
----

**Etapas do passo a passo**

**1º Passo :**

Para realizar a análise comparativa, inicialmente, clicar no botão **Compare by Container**.

.. image:: /figuras/fig_usavings/040_selecionar_container_nuvem_compara.png 
    :alt: selecionar container e nuvem a comparar
    :align: center
----

**2º Passo :**

Selecionar o container conforme a imagem apresentada abaixo. Este container será comparado com a nuvem selecionada anteriormente, ver imagem anterior, localizar o campo ondem estão todas as nuvens, no lado esquerdo da imagem anterior.

.. image:: /figuras/fig_usavings/041_selecionar_container_nuvem.png 
    :alt: selecionar container ou nuvem 
    :align: center
----

**3º Passo :**

Selecionar a região e clicar em Next para finalizar a operação e obter o resultado.

.. image:: /figuras/fig_usavings/042_tela_escolha_regiao_cloud.png 
    :alt: tela de escolha de regiao por cloud
    :align: center
----

.. image:: /figuras/fig_usavings/043_comparativo_container_nuvem.png 
    :alt: comparativo por container versus nuvem
    :align: center
----

O resultado será apresentado e assim o usuário chega no último step.

Após a análise comparativa ser executada e o resultado apresentado, este documento segue com a descrição do próximo passo, momento que existem os dados comparativos em tela.


Analisar e Exportar as informações coletadas
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A plataforma uSavings permite ao usuário navegar em cada uma destas unidades de informação e selecioná-las de acordo com a necessidade de informação.

**4º Passo :**

Análise e exportação das informações coletadas.

A imagem abaixo exibe alguns cards demonstrando valores sobre as sugestões na mesma nuvem e nas nuvens escolhidas. Os resultados podem ser visualizados direto na aplicação uSavings, ou exportados para um relatório em formato .csv.

.. image:: /figuras/fig_usavings/044_cards_precos_consolidados.png 
    :alt: cards de precos consolidados
    :align: center
----

A plataforma uSavings permite ao usuário navegar em cada uma destas unidades de informação e selecioná-las de acordo com a necessidade de informação. Este comparativo de nuvem possibilita perceber que há dois tipos de comparativo: ON DEMAND e RESERVED.

.. image:: /figuras/fig_usavings/045_representacao_grafica_preco_nuvem.png 
    :alt: representacao grafica dos precos das nuvens
    :align: center
----

A coluna verde espelha a análise que exibe o menor valor, pois ela representa o menor custo, este custo é a sugestão de troca de *Flavor* dentro da própria nuvem. As colunas centrais representam as estimativas das outras nuvens, em relação a coluna da direita (cor azul) que representa a nuvem atual com o valor atual de custo do contrato.

Ao baixar a tela, a segunda parte do comparativo dos *Flavors* **versus** as nuvens, é apresentada a combinação entre CPU, memória e o respectivo custo.

.. image:: /figuras/fig_usavings/046_tela_resultado.png 
    :alt: tela de resultado
    :align: center
----

Nesta tela, é possível ver o comparativo dos *flavors* e nuvens. Além disso, ao passar o mouse sobre os diferentes *flavors*, será exibida a combinação de CPU, memória e seu respectivo custo. Nesta tabela também é possível alterar as sugestões feitas pelo uSavings, caso não se adeque ao uso do usuário e da organização.

A imagem acima, *tela de resultado* exibe o detalhamento por cada *Virtual Machine* e os custos por nuvem, o usuário pode passar o mouse e visualizar o custo do *Flavor* na nuvem distinta.

Ao clicar nesta informação, será aberto um menu que permite ao usuário alterar o *Flavor* sugerido na nuvem.

No caso de selecionar outro *Flavor* a aplicação do uSavings perguntará se deseja alterá-lo para outros semelhantes ou iguais. No caso afirmativo, todas as VMs *g1-small* serão calculadas como *e2-small*. Consultar na figura abaixo que apresenta o relatório exportado no formato .csv:

.. image:: /figuras/fig_usavings/047_relatorio_exportado_csv.png 
    :alt: relatorio exportado em csv
    :align: center
----

Tal procedimento não altera o *Flavor* das *Virtual Machines* nas nuvens, apenas calcula as estimativas de alteração de *Flavor* que deve ser realizada no console das nuvens ou na plataforma do uCloud.


Imaginary Cloud
---------------

A penúltima funcionalidade do submenu uSavings está nomeada como *Imaginary Cloud*.

.. image:: /figuras/fig_usavings/048_submenu_funcionalidade.png 
    :alt: submenu de funcionalidades
    :align: center
----

O submenu *Imaginary Cloud* permite criar um ambiente imaginário, na intenção de prever o custo da infraestrutura do usuário/cliente ao utilizar as diferentes nuvens públicas.

.. image:: /figuras/fig_usavings/049_tela_inicial_imaginary_cloud.png 
    :alt: tela inicial imaginary cloud
    :align: center
----

Na tela inicial do *Imaginary Cloud* podem ser visualizados os Containers criados e é possível Deletar Container. Assim como, visualizar as *Virtual Machines*. *Load Balancer*, *Storage*, *IP* e *Database*. A seguir, o detalhamento das telas e a descrição das colunas destes 5 itens:

.. image:: /figuras/fig_usavings/050_tela_imaginary_vm.png 
    :alt: tela imaginary vm
    :align: center
---- 

Na tela *Imaginary Virtual Machine*, as dez informações apresentadas da esquerda para direita: 

  * **(i)** deletar máquina virtual; 
  * **(ii)** Nome; 
  * **(iii)** Memória; 
  * **(iv)** vCPU; 
  * **(v)** Preço atual em dólar; 
  * **(vi)** Sistema operacional; 
  * **(vii)** IBM; 
  * **(viii)** Google; 
  * **(ix)** Azure; 
  * **(x)** AWS.

.. image:: /figuras/fig_usavings/051_tela_imaginary_load_balancer.png 
    :alt: tela imaginary load balancers
    :align: center
----

A tela *Imaginary Load Balancers* apresenta oito informações na tela, da esquerda para a direita: 

  * **(i)** Deletar load balancer; 
  * **(ii)** Nome; 
  * **(iii)** Instâncias; 
  * **(iv)** Regras; 
  * **(v)** Dados por mês; 
  * **(vi)** AZURE; 
  * **(vii)** GCP; 
  * **(viii)** AWS.

.. image:: /figuras/fig_usavings/052_tela_imaginary_storage.png 
    :alt: tela imaginary storage
    :align: center
----

A tela *Imaginary Storage* apresenta seis informações na tela, da esquerda para a direita:

  * **(i)** Deletar storage; 
  * **(ii)** Nome; 
  * **(iii)** Quantidade de IP; 
  * **(iv)** GCP; 
  * **(v)** AZURE; 
  * **(vi)** AWS.

.. image:: /figuras/fig_usavings/053_tela_imaginary_ip.png 
    :alt: tela imaginary ip
    :align: center
----

A tela *Imaginary IP* apresenta seis informações na tela, da esquerda para a direita: 

  * **(i)** Deletar IP; 
  * **(ii)** Nome; 
  * **(iii)** Quantidade de IP; 
  * **(iv)** GCP; 
  * **(v)** AZURE; 
  * **(vi)** AWS.

.. image:: /figuras/fig_usavings/054_tela_imaginary_database.png 
    :alt: tela imaginary database
    :align: center
----

Na tela *Imaginary Database*, as dez informações apresentadas da esquerda para direita: 

  * **(i)** Deletar Database; 
  * **(ii)** Nome; 
  * **(iii)** vCPUs; 
  * **(iv)** Memória; 
  * **(v)** Storage; 
  * **(vi)** Banco de dados; 
  * **(vii)** Multi-Zone; 
  * **(viii)** AWS; 
  * **(ix)** AZURE; 
  * **(x)** GCP.

.. image:: /figuras/fig_usavings/055_imaginary_clouds_containers.png 
    :alt: imaginary clouds tela containers
    :align: center
----

A partir deste ambiente é permitido ao usuário criar ambiente imaginário (container) e deletar os containers criados.

.. image:: /figuras/fig_usavings/056_criar_ambiente_imaginario.png 
    :alt: criar ambiente imaginario container
    :align: center
----

.. image:: /figuras/fig_usavings/057_tela_deletar_ambiente_imaginario_container.png 
    :alt: tela deletar ambiente imaginario container
    :align: center
----

O ambiente *Imaginary Cloud* possibilita a criação de máquinas, importe de arquivo .csv com o inventário da infraestrutura, permite a criação de container e apresentação de uma tela com o custo das diferentes nuvens.

Estas telas de ambiente imaginário são resultado da intenção de prever o custo da infraestrutura do usuário/cliente ao utilizar as diferentes nuvens públicas. Cada uma destas colunas representa o custo do que seria realizado, incluindo o custo da migração.

Após toda esta imaginação de cenários, a aplicação fornece documentação em formato .csv, pronto para importação e uso em reuniões de tomada de decisão.

.. image:: /figuras/fig_usavings/058_criar_container_imaginario.png 
    :alt: criar container imaginario
    :align: center
----

Após a criação do container imaginário, podemos seguir criando outros recursos e comparar seus preços para as diferentes nuvens, mostrando também qual seria a nuvem que provêm o menor preço para os dados desejados.

.. image:: /figuras/fig_usavings/059_criar_virtual_machine.png 
    :alt: criar virtual machine
    :align: center
----

Começando com a criação da *Virtual Machine*, temos uma série de *inputs* que devem ser preenchidos, começando pelo campo Nome até outras opções como vCPU, memória e sistema operacional desejado, além disso, deve-se estipular o quanto de orçamento existiria para *“pagar”* por essa *Virtual Machine*.

.. image:: /figuras/fig_usavings/060_import_export_csv.png
    :alt: import e export csv
    :align: center
----

Após a sua criação, são apresentados os resultados na tela, em dois formatos: 
 * **(i)** os gráficos relacionando as VMs com os Flavors desejados para cada uma das *clouds* que o produto cobre; 
 * **(ii)** uma tabela .csv que pode ser exportada para a necessidade do usuário de outras informações além das apresentadas no gráfico, caso o gráfico não seja suficiente ou satisfatório.

.. image:: /figuras/fig_usavings/061_comparativo_criar_load_balancer.png 
    :alt: comparativo ao criar load balancer
    :align: center
----

Temos a opção de criar um *Load Balancer* imaginário da mesma forma, com 4 *inputs* essa criação também necessita de um nome – O *input* Nome será necessário para todas as opções de criação - e de 3 novos *inputs*: instâncias, Regras de transferência e dados por mês em GB. 

Os resultados são apresentados em formato de tabela, a qual mostra o preço do serviço desejado para cada *Cloud*. Vale ressaltar que neste exemplo de criação de *Load Balancer*, a nuvem AZURE apresenta o menor valor, em segundo lugar a nuvem AWS e, por último, o maior custo neste exemplo será a nuvem GCP. É assim que a aplicação uSavings sugere a economia dos recursos contratados para a tomada de decisão na organização.

.. image:: /figuras/fig_usavings/062_criar_storage_imaginary_cloud.png 
    :alt: criar storage imaginary cloud
    :align: center
----

Seguindo o processo, criar um *Storage* imaginário da mesma forma, com 4 *inputs* que consistem nos *inputs*: nome, instâncias, quantidade de transações e tamanho em GB.

.. image:: /figuras/fig_usavings/063_criar_storage.png 
    :alt: criar storage
    :align: center
----

Após a criação de um *Storage*, a tela de apresentação será semelhante a exibição do *Load Balancer*.

.. image:: /figuras/fig_usavings/064_resultado_criacao_storage.png 
    :alt: resultado da criacao do storage
    :lign: center
----

Para a penúltima opção de criação temos o IP, que segue a mesma lógica, necessitando somente de 2 *Inputs*: Nome e quantidade de IPs.

.. image:: /figuras/fig_usavings/065_criar_ip.png 
    :alt: criar ip
    :align: center
----

O formato de apresentação da tela do IP será semelhante aos itens já explicados acima nesse manual. A última opção a ser descrita para criação imaginária é o Database.

.. image:: /figuras/fig_usavings/066_criar_database_imaginary_cloud.png 
    :alt: criar database no imaginary cloud
    :align: center
----

Para que a operação seja bem-sucedida precisaremos preencher Nome, vCPUs, memória em GB, Storage em GB, engine que será utilizada e, se deve ser multizona, ou não.

.. image:: /figuras/fig_usavings/067_criar_database_imaginary_cloud_2.png 
    :alt: criar database imaginary cloud
    :align: center
----

Após a criação será recebida uma tabela com os dados que foram criados e os preços existentes de mercado.

Caso o usuário considere necessário deletar o *Imaginary Cloud*, após a criação de todos esses itens, temos a opção de apagar qualquer um deles a qualquer momento, no caso de apagar os itens dentro do container deve-se clicar no símbolo de lixeira a esquerda da tabela. Para apagar o container deve-se clicar nele e preencher um modal com o nome do item que se deseja deletar.

Container Hint
--------------

A última funcionalidade do menu uSavings é o *Container Hint*, ela apresenta os recursos que aparentemente não estão sendo utilizados ou estão gerando custos supostamente desnecessários. 

.. image:: /figuras/fig_usavings/068_container_hint.png 
    :alt: menu container_hint
    :align: center
----

A funcionalidade está disponível para as contas conectadas e integradas com a plataforma do uCloud.

.. image:: /figuras/fig_usavings/069_selecao_tipo_nuvem_container.png 
    :alt: selecao por tipo de nuvem ou container
    :align: center
----

Ao conectar a conta da nuvem pública na plataforma do uCloud será listada a imagem acima. Nesta imagem de seleção por tipo de nuvem ou container, podem ser selecionados os tipos de provedores de nuvens: 

  * **(i)** GCP; 
  * **(ii)** AWS; 
  * **(iii)** AZURE; 
  * **(iv)** VMware ou selecionar um container.

.. image:: /figuras/fig_usavings/070_tela_recursos_nao_utilizados.png 
    :alt: tela de recursos nao utilizados
    :align: center
----

O usuário deve selecionar uma das quatro nuvens que deseja pesquisar para descobrir quais recursos aparentemente não estão sendo utilizados ou estão gerando custos supostamente desnecessários.

Após selecionar a nuvem desejada, a tela apresenta uma lista que possibilita pesquisar nos seguintes recursos:

  * **Disks** - Lista os discos que foram criados e não estão associados a nenhuma máquina virtual;

  * **Public IP** - Lista os IPs públicos que foram solicitados em algum momento que geram custos e não estão associados a nenhuma máquina virtual;

  * **Disk Snapshot** - Lista todos os discos snapshots criados, mão não distingue quais deles devem ou não ser apagados;

  * **VM Snapshot** - Lista todos os snapshots das máquinas virtuais criados, mão não distingue quais deles devem ou não ser apagados.

  * **Load Balancer** - Lista todos os Load Balancer criados, mas não distingue quais deles devem ou não ser apagados.

  * **Virtual Machine** - Lista todas as máquinas virtuais criadas.

Assim, o usuário pode realizar a pesquisa e descobrir quais recursos não são utilizados ou geram custos desnecessários para a organização.

----

uCloud
======

O último menu de funcionalidade apresenta a possibilidade de ir à plataforma uCloud, apenas clicando sobre este menu a aplicação uSavings encaminha o usuário à plataforma do uCloud.

----

Conclusão
=========

Assim, este documento conclui a descrição geral dos procedimentos necessários para o uso. A leitura deste manual de utilização permitirá ao usuário da aplicação utilizar as suas funcionalidades de maneira adequada. 

**Equipe Ustore**



uSavings Manual de uso
Edição 2 v.7
20/05/2022



.. |icone_ustore| image:: /figuras/fig_usavings/icone_ustore.png 

.. |icone_configuracao| image:: /figuras/fig_usavings/icone_configuracao.png

.. |icone_lista_troca_idioma| image:: /figuras/fig_usavings/icone_lista_troca_idioma.png

.. |icone_bandeira_troca_idioma| image:: /figuras/fig_usavings/icone_bandeira_troca_idioma.png

.. |icone_nome_usuario_logado| image:: /figuras/fig_usavings/icone_nome_usuario_logado.png

.. |icone_logout| image:: /figuras/fig_usavings/icone_logout.png














