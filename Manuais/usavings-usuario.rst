uSavings - Manual do Usuário
++++++++++++++++++++++++++++


.. image:: /figuras/uSavings-logo-gde.png
    :alt: logo usavings
    :align: center
======


INTRODUÇÃO Visão Geral
=========================

Este documento descreve a aplicação uSavings, a visão e o posicionamento do produto,.
Importa esclarecer que ele se encontra em constante desenvolvimento e evolução, por isto, as telas apresentadas neste documento podem sofrer alterações a qualquer momento, por conta da evolução do software.

O que é uSavings?
-----------------

O uSavings é uma ferramenta que analisa em tempo real o consumo da infraestrutura dos recursos computacionais (das máquinas virtuais, abreviado como VMs) nas diferentes nuvens, é por meio desta análise que a aplicação recomenda modificações, no caso de a organização acolher ou apoiar esta sugestão, tal decisão poderá permitir gerar o máximo de economia financeira e otimização dos recursos criados e/ou executados. A aplicação uSavings é um “cost advisor", ou seja, um consultor de custos que permite aconselhar o usuário como reduzir os custos da sua infraestrutura, bilhetada pela Plataforma uCloud, nos diversos provedores de serviços de nuvem - AWS, Azure, Google, IBM e VMWare.

Como funciona?
--------------

A plataforma do uSavings obtém e extrai a informação dos dados históricos da própria Virtual Machine, ou seja, da máquina virtual e da bilhetagem de cada provedor de nuvem pública – a coleta destes dados é iniciada com a integração à Plataforma do uCloud. A aplicação apresenta um painel consolidado e sugestões dos gastos do cliente em cada provedor de nuvem, entregando assim, informações precisas para a melhor tomada de decisão sobre os custos alocados dos recursos de infraestrutura da organização.

- [ ] inserir *Figura1 Organograma funcionamento uSavings*

Esta imagem, a **Figura 1**, representa o organograma de funcionamento do uSavings: nele a máquina virtual do uCloud ou ‘VM’, é um dos elementos principais neste fluxo, conforme demonstrado no diagrama acima. O seguinte elemento apresentado é o Flavor, ele possibilita saber o quanto de memória, vCPU entre outros recursos são utilizados pela máquina. Logo, é a partir do Flavor que se sabe o quanto determinada máquina custará no final do mês. Com estes dados, é possível para a plataforma do uSavings sugerir ao cliente economia de recursos na fatura mensal.

- [ ] inserir *Figura2 Recorte organograma*

O recorte no organograma, **Figura 2**, destaca a parte pertinente no diagrama, ela representa a forma sugestiva da aplicação do uSavings. Existem duas maneiras para recomendar as melhorias para uma determinada Virtual Machine: (i) por Flavor e (ii) por Billing.

* (i) Por Flavor* 
(i)	**Por Flavor**, o uSavings checa o Flavor alocado na máquina, e sugere uma possibilidade de melhoria – esta melhoria se relaciona ao custo beneficio – a aplicação publica os resultados em diversos formatos (gráficos ou porcentagem) e mostra qual será a melhor cloud a ser utilizada para economizar recursos, para a VM. Este parâmetro, por dedução, entende que a máquina fica ligada o tempo todo.

* (ii) Por Billing*
(ii)	**Por Billing**, A bilhetagem do banco de dados do uCloud suporta diversas nuvens, ela difere do alcance da aplicação do uSavings. O banco de dados do uCloud pode comportar todos os tipos de billing disponíveis. Já na regra de negócio do uSavings, só é possível fazer uma sugestão assertiva com o billing para a AWS e AZURE, como mostra o diagrama, na **Figura 2**.

1.3 Como economizar recursos?
-----------------------------

A vantagem da implantação do uSavings nas organizações é a possibilidade de receber informação sobre recursos ociosos que foram criados, e até executados anteriormente, atualmente não utilizados. Informação que pode possibilitar a economia de recursos.

Pelo fato da aplicação do uSavings ser uma ferramenta que analisa em tempo real o consumo da infraestrutura dos recursos computacionais nas diferentes nuvens, a aplicação uSavings exibe os recursos ociosos criados. 

A ferramenta é relevante para a tomada de decisão nas organizações, pois ao analisar a informação obtida pela aplicação entrega resultados reais. Isto contribui para uma decisão organizacional capaz de gerar economia financeira e otimização dos recursos criados e/ou executados.

A aplicação uSavings pode referenciar sugestões de redução da configuração – ‘rightsizing’ de máquinas virtuais, caso tenham sido previamente criadas com ‘super configurações’ e/ou apresentarem um baixo consumo no histórico de performance. **Direciona** a possibilidade de ampliar a relação custo-consumo, **não a executa**. O objetivo da implantação da plataforma uSavings é indicar à organização a possibilidade e/ou caminho para aumentar a economia dos seus custos, no próximo período de cobrança do provedor de serviço de nuvem.

| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
|  ATENÇÃO   |  A organização munida das informações, entregues pela aplicação uSavings, deve entrar em contato com o provedor do serviço de nuvem sobre ‘rightsizing’.  |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |

+--------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| ".."   | atenção "::" A organização munida das informações, entregues pela aplicação uSavings, deve entrar em contato com o provedor do serviço de nuvem sobre ‘rightsizing’. |
+--------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Ao adquirir a plataforma uSavings, as organizações podem ter em mãos uma valiosa ferramenta estratégica e de inteligência de negócio (BI) que indica o melhor caminho para ampliar a relação “custo-benefício” das suas infraestruturas virtuais e, também, a melhor forma de maximizar os recursos das máquinas virtuais criadas nos provedores de serviços de nuvem.

1.4 Otimizações recomendadas após o monitoramento
-------------------------------------------------

As otimizações a seguir podem ser propostas com base em sugestões de:

a) Rightsizing:
~~~~~~~~~~~~~~~

Consiste na sugestão da melhor combinação de CPU e memória, com o objetivo de minimizar os custos e maximizar o desempenho. A ferramenta coleta métricas de desempenho para determinar o consumo médio e máximo de recursos de uma instância em um período configurável e recomenda uma modificação para um tipo de configuração de máquina virtual ‘VM’ de menor configuração ou de configuração apropriada para o projeto.

b) Custos Comparativos:
~~~~~~~~~~~~~~~~~~~~~~~

Apresenta ao usuário a relação atual das suas máquinas virtuais ‘VMs’ e uma sugestão do que seria a ‘melhor configuração’ em cada provedor de nuvem. Permite ao usuário avaliar qual provedor está com o menor custo em determinada máquina virtual ‘VM’ , na data que foi obtido o valor deste custo.

c) Monitoramento de Recursos Ociosos:
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

O monitoramento de recursos ociosos permite checar se os recursos estão em uso. É possível monitorar os recursos criados e não utilizados.

d) Instâncias Reservadas:
~~~~~~~~~~~~~~~~~~~~~~~~~

Sobre a instância reservada, a aplicação uSavings consegue mostrar ao cliente-usuário que no caso da alteração de uma máquina *on-demand* para uma máquina reservada – a instância reservada consegue exibir o quanto é possível economizar em relação a atual máquina.

**Por exemplo**

Ao utilizar o provedor AWS, as instâncias reservadas (*Reserved Instances - RIs*) da Amazon EC2 são uma das formas mais óbvias de controlar os custos de computação, permitindo ao usuário reservar capacidade de computação EC2 em troca de taxas horárias com descontos significativos.

É importante observar e reforçar ao cliente/usuário que as instâncias reservadas (AWS, AZURE ou instância preemptiva Google) não são instâncias que o usuário possa criar e executar por um preço menor do que as instâncias normais. E, deve ser considerado que não há garantia de que estes serviços computacionais sejam dedicados ao cliente ou estejam disponíveis e acessíveis durante os 365 dias do ano. 

Caso o provedor de serviços de nuvem necessite ter acesso a estes recursos computacionais, para outro tipo de tarefa, o provedor pode encerrar estas instâncias a qualquer momento (ou seja, forçar a interrupção destas VMs) sem obrigação da prévia comunicação.


2. INTERFACE e MENU
===================

A interface inicial apresentada ao usuário é um painel de controle (*Dashboard*) que exibe um resumo da atual infraestrutura, endereçável e acessível por meio da plataforma do uCloud. Ao efetuar o acesso à interface do uSavings, o usuário se conecta automaticamente com a sua atual infraestrutura de máquina virtual ‘VMs’. Desta forma, o usuário visualiza os custos atuais das máquinas virtuais ‘VMs’ existentes, pode comparar os custos das suas máquinas virtuais entre os diversos provedores de serviços públicos de infraestrutura de nuvem.

O uSavings permite criar manualmente uma lista de máquinas virtuais ‘VMs’ com configurações específicas (uma configuração privada e/ou ‘imaginária’), para o caso do usuário que deseja obter a relação completa das suas máquinas virtuais e prefere conectar-se de forma manual.

2.1 Como acessar a plataforma uSavings
--------------------------------------

O acesso à plataforma uSavings é realizado pela web, podendo ser utilizado qualquer um dos navegadores: **Firefox**, **Google Chrome** ou **Microsoft Edge**, em diversos sistemas operacionais, a exemplo do **Microsoft Windows** 10 ou 11.

Para o acesso inicial é necessário solicitar as credenciais ao administrador - ao receber o link com o endereço e as credenciais de acesso, o usuário deve utilizar seu navegador de preferência para acessar a web e conectar-se. Outra forma de acesso à plataforma do uSavings é direto da plataforma do uCloud, pelo seu menu lateral esquerdo. 

Para o caso de o acesso ser realizado direto na web a Figura 3 abaixo será mostrada ao usuário. Neste momento, ele deve inserir as credenciais recebidas.

- [ ] inserir *Figura3 Tela de acesso inicial*

O usuário deve preencher os campos **‘login’** e **‘senha’**, com as credenciais recebidas do administrador da plataforma. Clicar em **‘Entrar’**. Após este procedimento, a tela inicial do Dashboard será apresentada. 

Se a tela de Dashboard não for apresentada, isto significa que algum dos campos estão preenchidos com informações inconsistentes, ou seja, ‘login’ ou ‘senha’ inexistentes e/ou pode ter havido um erro na digitação das informações. É importante checar e repetir a operação.

- [ ] inserir *Figura4 Tela de problema no acesso*

No caso de insucesso ao logar, será apresentada ao usuário a **Figura 4** acima, com a seguinte orientação: **(i)** checar as credenciais e **(ii)** repetir a operação.

3. VISÃO GERAL do MENU SUPERIOR
===============================

De início, antes de adentrar na sessão do **Dashboard** é relevante entender o impacto de algumas ferramentas existentes no menu superior.

- [ ] inserir *Figura5 recorte Menu superior*

No recorte do menu superior, acima demonstrado na **Figura 5**, são exibidos componentes relevantes, a seguir descritos em detalhe, Na ordem: da esquerda para a direita:

3.1 Ícone de Troca de Contrato
------------------------------

Este ícone 

- [ ] inserir ícone

  é um ponto relevante a fazer uma ressalva, ao partir da premissa de que há a possibilidade de um usuário cadastrado na plataforma do uCloud fazer parte **de mais de um grupo** de usuários. Logo ele pode fazer parte de mais de um contrato. E, existe a possibilidade de selecionar um outro contrato, este contrato selecionado pode conter outros recursos atrelados a este contrato. 

  = [ ] inserir *Figura6 ícone troca de contrato*

Este ícone de troca de contrato apresenta todos os contratos nos quais o usuário logado na plataforma uSavings participa. Assim, é permitido ao usuário trocar entre eles livremente. A troca de contrato pode implicar na troca dos recursos que serão apresentados ao usuário, pois cada contrato pode ter uma determinada característica, na sequência deste manual de uso do uSavings estas minucias serão descritas.

3.2 Ícone de Configuração de Clouds
-----------------------------------

Como introdução sobre a usabilidade deste recorte da tela:

- [ ] inserir ícone

Pode-se afirmar que o termo *Clouds* é empregado para abstrair um agrupamento de *Flavors* de uma determinada Cloud, sendo este agrupamento tanto de *Flavors* reais quanto imaginários. 

- [ ] inserir *Figura7 Configurações de Clouds*

No menu de configurações existe a parte de criação de *Clouds*, alteração da atividade das *Clouds* e a área de criação de novas *Clouds*.

- [ ] inserir *Figura8 Configuração alteração de atividade*

3.3 Ícone Lista de troca de idiomas
-----------------------------------

Este ícone

- [ ] inserir ícone

  permite trocar o idioma na plataforma uSavings, a plataforma originalmente está em português e pode ser alternada para o Espanhol e para o Inglês, basta apenas clicar no ícone com as bandeiras:

  - [ ] inserir ícone das bandeiras

3.4 Ícone Nome do usuário logado
--------------------------------

Este ícone

- [ ] inserir ícone ucloud

   apresenta o nome do usuário que está logado na plataforma uSavings.

3.5 Ícone de LogOut
-------------------

Este ícone

- [ ] inserir ícone 

  desloga o usuário da plataforma.

4. VISÃO GERAL do *DASHBOARD*
=============================

A interface inicial do uSavings exibida ao usuário é um painel de controle *(Dashboard)*.

- [ ] inserir *Figura9 Menu de entrada Dashboard*

Este painel, **Figura 7**, exibe alguns dados na tela que retratam um resumo da atual infraestrutura endereçável e acessível pela plataforma, estes dados são compostos de segmentações denominadas *Cards*.

- [ ] inserir *Figura 10 Tela inicial: Dashboard e Funcionalidades*

Na primeira parte da tela inicial, **Figura 8**, **são espelhados somente os serviços de nuvem** que a organização **possui na plataforma do uCloud**, e, **autoriza a integração**, o acesso pela aplicação uSavings.

- [ ] inserir *Figura11 Container conectado na plataforma uCloud*

Neste caso, a **Figura 11** apresenta a relação dos containers que participam do contrato no qual o usuário está conectado. Esta autorização de acesso funciona a partir do Contrato, conforme o exemplo a seguir:

'''
Quando um determinado container da plataforma do uCloud, está contido no Virtual Datacenter, que por sua vez faz parte de um contrato em que o usuário logado na plataforma do uSavings participa. 
'''

Desta forma, existe o acesso aos dados do container, sendo somente após este acesso e análise dos dados que a plataforma do uSavings pode sugerir as melhorias de performance de uso.

O *Dashboard* permite a visualização rápida sobre cada uma das nuvens conectadas ao uCloud, as quais são refletidas na aplicação uSavings. No caso de a nuvem do usuário estar ausente do uSavings, isto significa que a nuvem não foi conectada na plataforma do uCloud.

A seguir, neste documento, os quatro *cards* exibidos na tela do Dashboard são descritos em detalhes.

4.1 Latest Months
-----------------

O primeiro *card* **Latest Months**, apresenta a bilhetagem ocorrida no período relacionado aos últimos seis (6) meses, ou seja, serão listados todos os valores investidos em determinada conta, por um período relacionado aos últimos 6 meses.

- [ ] inserir *Figura12 Latest months*

Tal valor é coletado a partir de valores gerados pelo *job* do uSavings, responsável por sumarizar o Billing da plataforma do uCloud.

- [ ] Inserir *Figura13 Gráfico de investimentos em Real x 6 últimos meses*

O gráfico constante na **Figura 13** apresenta o valor do custo em Dólar *versus* o período requerido dos últimos 6 meses.

4.2 Consolidated cost
---------------------

O segundo *card* **Consolidated Cost** exibe algumas sugestões na tela do Dashboard, estas sugestões são relacionadas ao que a máquina virtual “VM” selecionada contêm, é relevante mencionar que todos os valores são apresentados em dólar. O card mostra o *Flavor* e as regiões habilitadas para a máquina, a reunião destas informações permite sugerir melhorias para otimizar o uso.

Neste *card* são detalhadas as informações a respeito do percentual de economia, diferença de custo, custo corrente despendido, custo otimizado e *Flavors* utilizados e/ou sugeridos pela aplicação. Valores apresentados em dólar.

- [ ] inserir *Figura14 Custos Consolidados*

Ao observar a **Figura 14**, o percentual de 65,25% no campo *Saving* representa o percentual de economia que a aplicação uSavings entrega como resultado, baseado na sugestão de mudança de *Flavor* dentro da própria nuvem. Ou seja, o usuário está realizando uma pesquisa na nuvem AWS, a economia exibida de 65,25% é possível implementar ao trocar de *Flavor* dentro da própria nuvem. 

As informações detalhadas, neste *Card* de custos consolidados, apresentam uma riqueza de detalhes para o entendimento entre a melhor combinação de CPU, memória e disco, com foco na redução dos custos:

* **Saving** – Mostra o percentual de economia (na cor verde) ou dispêndio (na cor vermelha) baseia-se no consumo atual e compara com as otimizações sugeridas;

* **Difference Cost** – Representa o mesmo cálculo usado pelo *Saving* sendo que revela a diferença em Real (R$);

* **Current Cost** – Apresenta o valor que está sendo despendido, em referência ao período que a análise foi coletada.

* **Otimized Cost** – Indica o valor futuro, caso as mudanças sugeridas sejam aceitas e implementadas.

  * **Obs:** Todos os valores exibidos podem sofrer mudanças no decorrer do período, a depender do consumo trafegado nas nuvens.

4.3 Actual Flavor
-----------------

Este terceiro *Card* apresenta o *Flavor* das máquinas selecionadas deste container, caso seja modificado, ele carrega as novas informações. A exibição das porcentagens utilizadas pelo *Flavor* é apresentada pelo gráfico de pizza e sua representatividade ocorre por tipo, no conjunto total da infraestrutura.

Todos os valores são exibidos em dólar, sem tributação de impostos. Os preços têm origem na tabela importada diretamente do provedor de nuvem e inserida no banco de dados desta aplicação. O preço é calculado a partir da quantidade de horas que compõem o mês.

- [ ] inserir *Figura15 Gráfico Actual Flavors*

As informações contidas na **Figura 15**, acima, se referem ao ambiente AWS, onde cada item difere em relação ao tamanho da memória, vCPU, preço e sistema operacional e, ao final, é apresentado o valor total do custo dos *Flavors* atualmente utilizados.

4.4 Sugested Flavors
--------------------

Este *Card* apresenta um outro tipo de gráfico, a partir do *card Actual Flavors* ele demonstra quanto seria a diferença a partir da sugestão de economia referenciada. Ou seja, o quanto é possível salvar do recurso criado que está ocioso, ao apresentar as informações do consumo atual e a sugestão de consumo num gráfico de colunas. 

A coluna azul representa o gasto atual, a coluna verde sugere a economia que pode ser gerada, no caso da aplicação das sugestões de melhoria de consumo dos recursos apresentadas pela plataforma do uSavings.

- [ ] inserir *Figura16 Sugested Flavors*

Os gráficos e as informações apresentadas são uma **análise inicial** da economia potencial dos valores que a organização pode se beneficiar ao adotar as recomendações sugeridas pela plataforma uSavings. 

Os valores apresentados se referem ao período da coleta de dados (o período mínimo inicial é de quinze dias). Quanto mais longo for o período da coleta de informações, mais confiável será a estimativa da economia calculada.

- [ ] inserir *Figura17 Tela entrada Dashboard (parte 1/2)*

Esta análise inicial é calculada com base no uso, ou seja, na ocupação dos recursos computacionais das máquinas virtuais ‘VMs’ dentro do período armazenado na base de dados da plataforma uSavings.

- [ ] inserir *Figura18 Tela entrada Dashboard (parte 2/2)*

O resultado desta análise é a sugestão da melhor combinação de CPU e memória. Sugestão que objetiva a redução dos custos e a maximização do desempenho *(rightsizing)*. A análise não faz o cálculo comparativo entre os valores de configuração das máquinas virtuais ‘VMs’ em outros provedores.

5. MENU LATERAL de Funcionalidades
==================================

No lado esquerdo do menu de entrada da plataforma do uSavings são listados os menus de funcionalidades, são eles: *Virtual Machines*, *Compare Clouds*, *Imaginary Cloud*, *Container Hint* e o menu de acesso à plataforma uCloud.

- [ ] inserir *Figura19 Submenu das Funcionalidades*

5.1 Virtual Machines
--------------------

No menu Virtual Machines são apresentadas todas as máquinas virtuais da infraestrutura do usuário (ou seja, o inventário de todas as máquinas virtuais ‘VMs’ das contas pertencentes à organização).

- [ ] inserir *Figura20 Virtual Machines*

Esta exibição permite a seleção do container específico para a análise de custos e sugestão de mudança de *flavor* na mesma cloud das máquinas virtuais listadas. Todas a informações apresentadas podem ser exportadas em relatório formato .csv.

- [ ] inserir *Figura21 Menu Virtual Machines*

É relevante ressaltar que o container apontado deve estar contido no uCloud, ou seja, o container a ser analisado deve estar conectado e sincronizado na plataforma uCloud.

- [ ] inserir *Figura22 Selecionar Container*

Após selecionar o container, as informações são apresentadas em colunas, seguindo a ordem da 1ª até a 6ª coluna: 

* (i) o nome da máquina virtual;
* (ii) o flavor utilizado;
* (iii) o custo atual da máquina é atribuído se ela estiver ligada durante o mês inteiro;
* (iv) o flavor sugerido para otimização;
* (v) o custo mensal do flavor sugerido; 
* (vi) o valor anual da máquina virtual.

- [ ] inserir *Figura23 Informações Container*

As sugestões exibidas *(Rightsizing)* são baseadas no consumo de CPU das máquinas virtuais, do período que ela foi criada até o presente momento. As métricas são coletadas e o cálculo é baseado nas médias de consumo, logo em seguida, a sugestão é apresentada. 

A análise do consumo de memória pode fazer parte do cálculo, caso o provedor ou as instâncias estejam prontas para fornecer as métricas necessárias. Caso a informação não esteja disponível será assumida a memória definida pelo *flavor* da instância *deployada*.

a) *Rightsizing* - sugestão de mudança de *Flavor*
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Para receber o resultado de sugestão de mudança de *Flavor*, o usuário deve selecionar o container desejado, **Figura 24**. A aplicação uSavings gera a listagem e o comparativo de preços. Basta clicar e aguardar.

- [ ] inserir *Figura24 Container selecionado*

Como resultado desta operação será exibida a **Figura 25**, a qual apresenta em blocos as diversas informações, como: o *Flavor* e o Custo atual, a sugestão de *Flavor* e o custo estimado deste novo *Flavor*. Por último, exibe o custo da reserva do *Flavor* sugerido e estimado para 1 ano.

- [ ] inserir *Figura25 Resultado estimado na seleção* 

b) Caso de uso
~~~~~~~~~~~~~~

Para iniciar o passo a passo deste caso de uso, é relevante lembrar que as máquinas virtuais listadas são provenientes da plataforma do uCloud, portanto, as nuvens conectadas no uCloud devem conter as máquinas virtuais. 

No caso da inexistência das máquinas virtuais, consultar o Manual do uCloud, no tópico: Como conectar e importar *Virtual Machine*. 

**1º Passo** 
Selecionar a nuvem (container) que deseja analisar.

- [ ] inserir *Figura26 Selecionar nuvem na VM*

**2º Passo** 
Escolher a região que roda a *Virtual Machine* selecionada.

- [ ] inserir *Figura27 Selecionar a região VM*

**3º Passo** 
O resultado da seleção é exibido conforme a **Figura 25**, a lista de todas as *Virtual Machines*. Nesta mesma tela, no canto superior direito, é permitido exportar a lista de resultado em formato **.CSV**, basta clicar no botão **Export CSV**.

**4º Passo**
Exportar o relatório para visualização em planilha excel, na máquina do usuário, o resultado será semelhante a **Figura 26** abaixo:

- [ ] inserir *Figura28 Relatório exportado ao excel*

**5º Passo**
Existe a opção de analisar as informações de performance, na coluna Performance, conforme grifado na *Figura 29*. Logo após a coluna Nome, a coluna Performance apresenta um ícone com símbolo de * (asterisco).

- [ ] inserir *Figura 29 Coluna Performance*

**6º Passo** 
Ao clicar no ícone * **(asterisco)**, o relatório de performance é exibido:

- [ ] inserir *Figura 30 Performance das máquinas*

O relatório de performance proporciona a visualização do gráfico com a média do consumo de CPU e da memória da virtual máquina selecionada, num período de aproximadamente 15 a 20 dias.

5.2 Compare Clouds
------------------

Na aplicação do uSavings, a funcionalidade “Compare Clouds” permite realizar análise comparativa **Por Billing** ou **Por Container** dos custos entre a nuvem utilizada e as nuvens escolhidas para comparar.

- [ ] inserir *Figura 31 Submenu de funcionalidades*

Para que as unidades se tornem disponíveis é necessário a integração com a plataforma uCloud, neste caso, as contas precisam estar conectadas e sincronizadas, respeitando as definições de regras de segurança. 

O Compare Clouds permite realizar a análise comparativa entre a própria nuvem, assim como comparar com outras nuvens. Bem como comparar com as nuvens públicas que não estejam conectadas à plataforma do uCloud, como por exemplo: IBM, AZURE, Google, AWS. 

Existem duas maneiras de realizar esta análise comparativa, comparar por Billing ou por Container.

- [ ] inserir *Figura 32Tela inicial Compare Cloud*

Nesta **Figura 32** são apresentadas duas barras com a possibilidade de realizar a análise comparativa: **Comparar por Bilhetagem** e **Comparar por Container**. Ao clicar na barra pretendida ela assume a cor laranja, conforme a *Figura 33* a seguir:

- [ ] inserir *Figura 33 Seleção Compare by Billing ou Compare by Container* 

Reforçando, para que as unidades estejam disponíveis, **é imprescindível** integrar com a plataforma do uCloud.

a) Comparar por Billing
~~~~~~~~~~~~~~~~~~~~~~~

Para que seja possível fazer a análise comparativa por Billing (Bilhetagem), é necessário que o bilhetador tenha sido executado no determinado container. Atualmente, suportamos, a análise comparativa por Billing para as nuvens AWS e Azure, **Figura 33**.

Antes de selecionar o container ou a nuvem que se deseja comparar, é necessário checar se a plataforma do uCloud está bilhetada. Pelo menos um (1) container deve estar bilhetado e conectado à plataforma uCloud.

+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
|                                                                                                                               |
| **Significado** de *Estar bilhetado*  Significa que existe a fatura de consumo em determinado período, pelo menos um (1) mês. |
|                                                                                                                               |
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

**PASSO A PASSO**

**1º Passo** 
Para realizar a análise comparativa, inicialmente, clicar no botão **Compare by Billing**. Checar se a plataforma do uCloud está bilhetada, ao menos um container deve estar bilhetado e conectado à plataforma.

**2º Passo**
Selecionar a nuvem contendo todos os seus containers, *Figura 34*. Clicar em **AWS** ou **AZURE**, em seguida clicar em **NEXT**.

- [ ] inserir *Figura 34 Recorte Compare by Billing*

Neste caso, a nuvem **AWS** está selecionada. Ao clicar em **NEXT**, a aplicação do uSavings apresenta a próxima tela com a pergunta: “Que nuvens participarão deste comparativo?” E solicita, ao usuário, selecionar as nuvens que deseja realizar a análise comparativa dos valores. 

**3º Passo**
Ao selecionar a nuvem, o usuário deve preencher no calendário o período correspondente a análise. 

- [ ] inserir *Figura 35 Seleção período bilhetagem e nuvem a ser comparada*

O período é importante, pois os valores da nuvem podem sofrer alteração devido o provedor de nuvem. Por esta razão é possível escolher um determinado intervalo de tempo. Este intervalo será calculado com base no Billing gerado pelo uCloud.

**4º Passo**
Selecionar as nuvens que participarão da análise comparativa de valores. O que inclui nuvens que o usuário não tem necessariamente conectada à plataforma do uCloud, como por exemplo, as nuvens IBM e GOOGLE, conforme *Figura 36*.

- [ ] inserir *Figura 36 Selecionar as nuvens para a análise comparativa dos valores*

**5º Passo**
Neste caso, ao selecionar qualquer uma das nuvens públicas relacionadas, a próxima tela destina-se a escolha da região. Importa saber que esta região corresponde ao *Flavor* cadastrado na base de dados.

- [ ] inserir *Figura 37 Escolher a Região por nuvem*

**6º Passo**
Após selecionar a região por nuvem, a aplicação uSavings apresenta a Figura 38 com o resultado por extenso da região selecionada. E um botão que permite apagar a região, para a possibilidade de erro e escolha de outra região.

- [ ] inserir *Figura 38 Resultado após escolha da Região*

Para que seja possível fazer a análise comparativa por Billing (Bilhetagem), é necessário que o bilhetador tenha sido executado no determinado container. Atualmente, suportamos, a análise comparativa por Billing para as nuvens AWS e Azure. E, para que as **unidades se tornem disponíveis é necessário a integração com a plataforma uCloud**. Neste caso, as contas precisam estar conectadas e sincronizadas, respeitando as definições de regras de segurança.

b) Comparar por Container
~~~~~~~~~~~~~~~~~~~~~~~~~

O segundo comparativo oferecido pela aplicação uSavings é a análise por Container. É necessário selecionar e avançar a sequência do processo para obter o resultado pretendido que é a análise comparativa por container. Para o processo acontecer é primordial selecionar uma outra nuvem, além da nuvem inicial escolhida. 

- [ ] inserir *Figura 39 Seleção do Comparativo por Container*

**PASSO A PASSO**

**1º Passo**

Para realizar a análise comparativa, inicialmente, clicar no botão **Compare by Container**.

- [ ] inserir *Figura 40 Selecionar container e nuvem a comparar*

**2º Passo**

Selecionar o container **Figura 41**, a ser comparado com a nuvem apresentada na **Figura 40**, ver imagem anterior, o recorte localizado no lado esquerdo.

- [ ] inserir *Figura 41 Selecionar container ou nuvem*

**3º Passo**

Selecionar a região e clicar em Next para finalizar a operação e obter o resultado.

- [ ] inserir *Figura 42 Tela de escolha de região por cloud*

- [ ] inserir *Figura 43 Comparativo por Container versus nuvem*

O resultado será apresentado e assim o usuário chega no último step.

Após a análise comparativa ser executada e o resultado apresentado, este documento segue com a descrição do próximo passo, momento que existem os dados comparativos em tela.


c) Analisar e Exportar as informações coletadas
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A plataforma uSavings permite ao usuário navegar em cada uma destas unidades de informação e selecioná-las de acordo com a necessidade de informação.

**4º Passo**

Análise e exportação das informações coletadas.

A **Figura 44** exibe alguns cards demonstrando valores sobre as sugestões na mesma nuvem e nas nuvens escolhidas. Os resultados podem ser visualizados direto na aplicação uSavings, ou exportados para um relatório em formato .csv.

- [ ] inserir *Figura 44 Cards de preços consolidados*

A plataforma uSavings permite ao usuário navegar em cada uma destas unidades de informação e selecioná-las de acordo com a necessidade de informação. Este comparativo de nuvem possibilita perceber que há dois tipos de comparativo: ON DEMAND e RESERVED.

- [ ] inserir *Figura 45 Representação gráfica dos preços das nuvens*

A coluna verde é a análise que exibe o menor valor, pois ela representa o menor custo, este custo é a sugestão de troca de *Flavor* dentro da própria nuvem. As colunas centrais representam as estimativas das outras nuvens, em relação a coluna da direita (cor azul) que representa a nuvem atual com o valor atual de custo do contrato.

Ao baixar a tela, a segunda parte do comparativo dos *Flavors* **versus** as nuvens, é apresentada a combinação entre CPU, memória e o respectivo custo.

- [ ] inserir *Figura 46 Tela de resultado*

Nesta tela, é possível ver o comparativo dos *flavors* e nuvens. Além disso, ao passar o mouse sobre os diferentes *flavors*, será exibida a combinação de CPU, memória e seu respectivo custo. Nesta tabela também é possível alterar as sugestões feitas pelo uSavings, caso não se adeque ao uso do usuário e da organização.

A **Figura 46** exibe o detalhamento por cada *Virtual Machine* e os custos por nuvem, o usuário pode passar o mouse e visualizar o custo do *Flavor* na nuvem distinta. 
Ao clicar nesta informação, será aberto um menu que permite ao usuário alterar o *Flavor* sugerido na nuvem.

No caso de selecionar outro *Flavor* a aplicação do uSavings perguntará se deseja alterá-lo para outros semelhantes ou iguais. No caso afirmativo, todas as VMs g1-small serão calculadas como e2-small. Consultar no relatório exportado no formato .CSV Figura abaixo:

- [ ] inserir *Figura 47 Relatório exportado em .csv*

Tal procedimento não altera o *Flavor* das *Virtual Machines* nas nuvens, apenas calcula as estimativas de alteração de *Flavor* que deve ser realizada no console das nuvens ou na plataforma do uCloud.


5.3 Imaginary Cloud
-------------------

A penúltima funcionalidade do submenu uSavings está nomeada *Imaginary Cloud*.

- [ ] inserir *Figura 48 Submenu de funcionalidades*

O submenu *Imaginary Cloud* permite criar um ambiente imaginário, na intenção de prever o custo da infraestrutura do usuário/cliente ao utilizar as diferentes nuvens públicas.

- [ ] inserir *Figura 49 Tela inicial Imaginary Cloud*

Na tela inicial do *Imaginary Cloud* podem ser visualizados os Containers criados e é possível Deletar Container. Assim como, visualizar as *Virtual Machines*. *Load Balancer*, *Storage*, *IP* e *Database*. A seguir, o detalhamento das telas e a descrição das colunas destes 5 itens:

- [ ] inserir *Figura 50 Tela Imaginary VM*

Na tela *Imaginary Virtual Machine*, as dez informações apresentadas da esquerda para direita: 

**(i)** deletar máquina virtual; **(ii)** nome; **(iii)** memória; **(iv)** vCPU; **(v)** preço atual em dólar; **(vi)** sistema operacional; **(vii)** IBM; **(viii)** Google; **(ix)** Azure; **(x)** AWS.

- [ ] inserir *Figura 51 Tela Imaginary Load Balancers*

A tela *Imaginary Load Balancers* apresenta oito informações na tela, da esquerda para a direita: 

**(i)** deletar load balancer; **(ii)** nome; **(iii)** instâncias; **(iv)** Regras; **(v)** Dados por mês; **(vi)** AZURE; **(vii)** GCP; **(viii)** AWS.

- [ ] inserir *Figura 52 Tela Imaginary Storage*

A tela *Imaginary Storage* apresenta seis informações na tela, da esquerda para a direita:

**(i)** deletar storage; **(ii)** nome; **(iii)** quantidade de IP; **(iv)** GCP; **(v)** AZURE; **(vi)** AWS.

- [ ] inserir *Figura 53 Tela Imaginary IP*

A tela *Imaginary IP* apresenta seis informações na tela, da esquerda para a direita: 

**(i)** deletar IP; **(ii)** nome; **(iii)** quantidade de IP; **(iv)** GCP; **(v)** AZURE; **(vi)** AWS.

- [ ] inserir *Figura 54 Tela Imaginary Database*

Na tela *Imaginary Database*, as dez informações apresentadas da esquerda para direita: 

**(i)** deletar Database; **(ii)** nome; **(iii)** vCPUs; **(iv)** memória; **(v)** storage; **(vi)** banco de dados; **(vii)** Multi-Zone; **(viii)** AWS; **(ix)** AZURE; **(x)** GCP.

- [ ] inserir *Figura 55 Imaginary Clouds tela Containers*

A partir deste ambiente é permitido ao usuário criar ambiente imaginário (container) e deletar os containers criados.

- [ ] inserir *Figura 56 Tela Criar ambiente imaginário - Container*

- [ ] inserir *Figura 57 Tela Deletar ambiente imaginário - Container*

O ambiente *Imaginary Cloud* possibilita a criação de máquinas, importe de arquivo .csv com o inventário da infraestrutura, permite a criação de container e apresentação de uma tela com o custo das diferentes nuvens.

Estas telas de ambiente imaginário são resultado da intenção de prever o custo da infraestrutura do usuário/cliente ao utilizar as diferentes nuvens públicas. E, cada uma destas colunas representa o custo do que seria realizado, incluindo o custo da migração.

Após toda esta imaginação de cenários, a aplicação fornece documentação em formato .CSV, pronto para importação e uso em reuniões de tomada de decisão.

- [ ] inserir *Figura 58 Criar container Imaginário*

Após a criação do container imaginário, podemos seguir criando outros recursos e comparar seus preços para as diferentes nuvens, mostrando também qual seria a nuvem que provêm o menor preço para os dados desejados.

- [ ] inserir *Figura 59 Criar Virtual Machine*

Começando com a criação da *Virtual Machine*, temos uma série de inputs que devem ser preenchidos, começando pelo campo Nome até outras opções como vCPU, memória e sistema operacional desejado, além disso, deve-se estipular o quanto de orçamento existiria para “pagar” por essa *Virtual Machine*.

- [ ] inserir *Figura 60 Import e Export CSV*

Após a sua criação, são apresentados os resultados na tela, em dois formatos: **(i)** os gráficos relacionando as VMs com os Flavors desejados para cada uma das clouds que o produto cobre; **(ii)** uma tabela .CSV que pode ser exportada para a necessidade do usuário de outras informações além das apresentadas no gráfico, caso o gráfico não seja suficiente ou satisfatório.

- [ ] inserir *Figura 61 Comparativo ao Criar Load Balancer*

Temos a opção de criar um *Load Balancer* imaginário da mesma forma, com 4 *inputs* essa criação também necessita de um nome – O *input* Nome será necessário para todas as opções de criação - e de 3 novos *inputs*: instâncias, Regras de transferência e dados por mês em GB. 

Os resultados são apresentados em formato de tabela, a qual mostra o preço do serviço desejado para cada *Cloud*. Vale ressaltar que neste exemplo de criação de *Load Balancer*, a nuvem AZURE apresenta o menor valor, em segundo lugar a nuvem AWS e, por último, o maior custo neste exemplo será a nuvem GCP. É assim que a aplicação uSavings sugere a economia dos recursos contratados para a tomada de decisão na organização.

- inserir *Figura 62 Criar Storage no Imaginary Cloud*

Seguindo o processo, criar um *Storage* imaginário da mesma forma, com 4 *inputs* que consistem nos *inputs*: nome, instâncias, quantidade de transações e tamanho em GB.

- [ ] inserir *Figura 63 Criar Storage*

Após a criação de um *Storage*, a tela de apresentação será semelhante a exibição do *Load Balancer*.

- [ ] inserir *Figura 64 Resultado da criação do Storage*

Para a penúltima opção de criação temos o IP, que segue a mesma lógica, necessitando somente de 2 *Inputs*: Nome e quantidade de IPs.

- [ ] inserir *Figura 65 Criar IP*

O formato de apresentação da tela do IP será semelhante aos itens já explicados acima nesse manual. A última opção a ser descrita para criação imaginária é o Database.

- [ ] inserir *Figura 66 Criar Database no Imaginary Cloud*

Para que a operação seja bem-sucedida precisaremos preencher Nome, vCPUs, memória em GB, Storage em GB, engine que será utilizada e, se deve ser multi zona, ou não.

- [ ] inserir *Figura 67 Criar Database no Imaginary Cloud*

Após a criação também receberemos uma tabela com os dados que foram criados e os preços existentes de mercado.

Caso o usuário considere necessário deletar o *Imaginary Cloud*, após a criação de todos esses itens, temos a opção de apagar qualquer um deles a qualquer momento, no caso de apagar os itens dentro do container deve-se clicar no símbolo de lixeira a esquerda da tabela. Para apagar o container deve-se clicar nele e preencher um modal com o nome do item que se deseja deletar.

5.4 Container Hint
------------------

A última funcionalidade do menu uSavings é o *Container Hint*, ela apresenta os recursos que aparentemente não estão sendo utilizados ou estão gerando custos supostamente desnecessários. 

- [ ] inserir *Figura 68 Menu Container Hint*

A funcionalidade está disponível para as contas conectadas e integradas com a plataforma do uCloud.

- [ ] inserir *Figura 69 Seleção por tipo de nuvem ou container*

Ao conectar a conta da nuvem pública na plataforma do uCloud será listada a imagem acima. Nesta **Figura 69** podem ser selecionados os tipos de provedores de nuvens: **(i)** GCP; **(ii)** AWS; **(iii)** AZURE; **(iv)** VMWare ou selecionar um container.

- inserir *Figura 70 Tela de recursos não utilizados*

O usuário deve selecionar uma das quatro nuvens que deseja pesquisar para descobrir quais recursos aparentemente não estão sendo utilizados ou estão gerando custos supostamente desnecessários.

Após selecionar a nuvem desejada, a tela apresenta uma lista que possibilita pesquisar nos seguintes recursos:

* **Disks** - Lista os discos que foram criados e não estão associados a nenhuma máquina virtual;

* **Public IP** - Lista os IPs públicos que foram solicitados em algum momento que geram custos e não estão associados a nenhuma máquina virtual;

* **Disk Snapshot** - Lista todos os discos snapshots criados, mão não distingue quais deles devem ou não ser apagados;

* **VM Snapshot** - Lista todos os snapshots das máquinas virtuais criados, mão não distingue quais deles devem ou não ser apagados.

* **Load Balancer** - Lista todos os Load Balancer criados, mas não distingue quais deles devem ou não ser apagados.

* **Virtual Machine** - Lista todas as máquinas virtuais criadas.

Assim, o usuário pode realizar a pesquisa e descobrir quais recursos não são utilizados ou geram custos desnecessários para a organização.


6. uCLOUD
=========

Ao clicar neste menu a aplicação uSavings encaminha o usuário à plataforma do uCloud.


CONCLUSÃO
=========

Assim, este documento conclui a descrição geral dos procedimentos necessários para o uso. A leitura deste manual de utilização permitirá ao usuário da aplicação utilizar as suas funcionalidades de maneira adequada. 

Equipe Ustore



uSavings Manual de uso
Edição 2 v.7
20/05/2022
















