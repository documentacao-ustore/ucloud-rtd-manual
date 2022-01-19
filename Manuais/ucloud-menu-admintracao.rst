Menu Administração 
==================

Ao apresentar alguns conceitos sobre o ambiente de administração do uCloud, é importante esclarecer alguns pontos sobre a Plataforma do uCloud, nos conceitos existem três termos que serão amplamente utilizados no ambiente do uCloud:

* **Contrato**: é a forma com o qual se define a relação ‘comercial’ entre o provedor e a empresa que o contratou. No contrato são definidos os custos, a margem financeira, taxa de conversão de moeda, custos de recursos (opcional) e a cota (limite) global que pode ser uma cota financeira ou uma cota de recursos computacionais.

* **Grupo**: é uma forma lógica definida unicamente dentro da Plataforma do uCloud que pode definir um grupo de usuários (ex.: DevOps), um departamento (ex.: vendas), uma iniciativa (ex.: VDI), ao qual vários usuários estão associados sendo parte integrante deste grupo. Estes ‘grupos’ não existem nos provedores de nuvem (público e/ou privado) existem somente dentro da Plataforma do uCloud.

* **Usuário**: Um usuário é a entidade que possui acesso identificado à Plataforma do uCloud para efetuar ações nos recursos computacionais dos provedores (público e/ou privado).

A figura abaixo exemplifica, em uma imagem, a relação entre estes três termos e é primordial que o usuário utilize esta figura como referência para entender as relações::
  
**imagem_arquitetura_contrato**

É importante entender que um **Contrato** pode possuir vários grupos e cada *Grupo* pode conter vários *Usuários*. Entretanto, a Plataforma do uCloud permite somente que um Usuário faça parte de apenas um grupo e um único Grupo esteja vinculado a exclusivamente um contrato.

A seguir, neste documento, será descrito que ao configurar as cotas (limites financeiros ou de recursos) do contrato, estes limites serão compartilhados/divididos por cada um dos grupos existentes e, por consequência, os usuários estão limitados às cotas do grupo ao qual estão incluídos.

É possível notar, na figura anterior, o termo Virtual Data Center (VDC) este termo é uma alocação lógica de máquinas virtuais que permite às organizações definir um (ou mais) grupo(s) de servidor(es) que faz(em) parte de uma nuvem. Um VDC pode representar um departamento, uma subsidiária ou um grupo de usuários. Veja mais informações no item Virtual Data Center.

A opção Administração apresenta campos que variam de acordo com o perfil do usuário que está acessando o sistema naquele momento. O uCloud possui cinco perfis diferentes.

#. **Usuários do sistema**: são os usuários regulares que acessam o sistema para consumir os recursos.
#. Usuários do sistema, com perfil apenas de leitura: usuários regulares que podem apenas acessar o sistema para visualizar as informações. 
#. **Usuários Administradores de Contrato**: são os usuários que estão associados a um contrato e sobre este contrato podem definir regras de bilhetagem, provisionar e alterar outros usuários na plataforma.
#. **Usuários Administradores de Grupo**: são usuários que estão associados a um grupo de usuários, eles podem provisionar e alterar outros usuários na plataforma.
#. **Usuários Gestores Financeiros**: usuários com perfil para acessar as informações financeiras do uCloud.
#. **Usuários Administradores**: São usuários com perfil de acesso total e podem efetuar intervenções globais nas configurações da plataforma. Este perfil de usuário é exclusivo da Ustore ou de um único perfil de usuário da organização que efetuou a aquisição das licenças da Plataforma do uCloud. Este usuário administrador possui permissão para gerenciar todas as funcionalidades e recursos globais ofertados pela plataforma.

.. note::
  *O Perfil Administrador não será coberto neste documento. Entre em contato com seu ponto focal na Ustore para obter o documento específico: Manual do Administrador da Plataforma uCloud.
  Por segurança, melhores práticas e por padrão, existe apenas um (01) usuário provisionado com este tipo de perfil*.
	
Menu Administração / Usuários
-----------------------------

A Plataforma do uCloud possui bancos de dados próprios que armazenam as informações dos usuários como login e senha de forma segura e criptografada. A tela inicial do Menu Administração apresenta a lista de usuários provisionados, a informação de login de um usuário, o grupo ao qual o usuário está associado e o tipo do seu perfil deste login.

De acordo com o tipo de perfil do usuário que está acessando o sistema, a Plataforma do uCloud apresentará somente a relação de usuários que o perfil que está registrado e ativo pode gerenciar ou administrar.

**lista_de_usuários_imagem**

Para proceder com o acesso à Plataforma do uCloud deve-se provisionar (cadastrar) um usuário com seu respectivo login e senha de acesso.

Abaixo estão descritas as colunas apresentadas nesta lista de usuários:

* **Botão Criar Usuário** “  " Quando selecionado este botão, o processo está descrito no item Criando Novo Usuário, veja na página 41.
* **Login**: Esta coluna apresenta as credenciais de login do usuário. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de login de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Nome**: Esta coluna apresenta o nome do usuário que foi informado durante o processo do seu provisionamento na Plataforma do uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de nomes de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Grupo**: Esta coluna apresenta o grupo principal do usuário que foi informado durante o processo do seu provisionamento na Plataforma do uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Perfil**: Esta coluna apresenta o perfil do usuário que foi informado durante o processo do seu provisionamento na Plataforma do uCloud. Como forma de simplificar a visualização, se clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de perfis de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Busca Rápida**: O usuário poderá observar que logo abaixo do nome de cada coluna existe um campo em ‘branco’, este campo permite efetuar uma busca rápida no conteúdo da listagem para reduzir e estreitar a quantidade de incidências desta lista de eventos de login. Basta preencher o campo em ‘branco’ com uma sequência de caracteres que possam ser relevantes e a Plataforma do uCloud atualizará a tela de forma a representar este padrão de busca.
   * **Coluna Perfil**: O campo de busca rápida, na coluna Perfil, possui um controle avançado em forma de um "*dropdownlist*" que permite aplicar um **filtro** de ‘tipo perfil’ para que a lista apresentada fique restrita somente à opção que foi selecionada. Para isto, basta clicar com o cursor do mouse neste campo, a Plataforma do uCloud apresenta as opções de filtragem.

**coluna_perfil_imagem**  

Um usuário, provisionado, deve estar vinculado a apenas um dos seis **Tipos de Perfil** disponíveis, e esta definição decorre de qual função este usuário pode estar associado. Destes seis tipos, apenas *dois (02)* perfis (perfil *Usuário* e *Auditor*) são utilizados no dia a dia das operações na Plataforma do uCloud.

O perfil **Auditor** tem uma função muito restrita, mas muito importante no controle e gerenciamento de custos do ambiente de recursos computacionais em nuvem (público e/ou privado).

O perfil **Usuário** é o mais fundamental e mais flexível, pois este pode assumir diferentes níveis de permissões e funções de operação, gerenciamento e administração do ambiente empresarial no uCloud.

Abaixo descrevemos os quatro tipos básicos de perfil de usuários na Plataforma do uCloud, são eles:

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

**usuário_listagem-imagem**

* **Seção Geral**: A primeira seção desta tela apresenta os dados gerais do perfil do usuário provisionado na Plataforma do uCloud. Por meio desta tela será possível alterar alguns campos referentes ao usuário.
   * **Botão de Excluir Usuário**: Este botão pode ser usado para remover o usuário provisionado na Plataforma do uCloud de forma definitiva e irreversível. Basta o usuário clicar com o cursor do mouse sobre o botão, e será apresentada a tela solicitando a confirmação da ação, conforme a tela abaixo:
  
   **imagem_confirma_exclusão**

   Após a confirmação da Exclusão do usuário, este usuário e suas credenciais de acesso ficam indisponíveis imediatamente de forma irreversível, não sendo possível recuperar as informações deste usuário. Se a exclusão for acidental, este usuário deverá ser provisionado novamente, ver o item Criando Novo Usuário na página 41. 
   * **Ícone de Edição Ativo**: Todos os campos que possuem o ícone de edição ativo são passíveis de terem seu conteúdo altera
   * **Ícone de Edição Inativo**: Todos os campos que possuem o ícone de edição inativo ou não são passíveis de terem seu conteúdo alterado através desta tela (ex.: valores das cotas de grupo) ou o perfil do usuário que está registrado e acessando esta tela, não possui permissão para alterar o conteúdo do(s) campo(s).
   * **Ícone de Confirmação**: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma do uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma do uCloud.
   * **Ícone de Cancelamento**: Caso o usuário tenha clicado sobre o ícone de edição por engano ou não deseja que a alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna para os valores iniciais, antes de proceder qualquer preenchimento ou alteração.
   * **Barra de Rolagem**: Esta seção possui um grande conjunto de campos, para a completa visualização de todos o usuário deve utilizar a barra de rolagem ao lado direito desta seção. Se o usuário rolar o mouse, a tela desce e apresenta os campos que não estavam sendo visualizados, conforme a tela abaixo:
   * **Apenas Leitura**: Este campo configura um usuário que não tem permissão de efetuar nenhuma ação através da Plataforma do uCloud, mas seu login está ativo e ele possui a capacidade de visualizar todas as telas, as quais ele tenha permissão.
   Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o seu perfil permita proceder a alteração. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.
  
   * **Autenticação Multifator**: Este campo indica se este usuário terá seu processo de autenticação na plataforma (login) sendo verificado duplamente, antes de aprovar que este usuário tenha acesso a Plataforma do uCloud. Para isto ocorrer, será enviada uma mensagem no número de serviço móvel do celular cadastrado.
      * Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o seu perfil permita proceder a alteração. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.
  
   * **Ativar Cota de Faturamento**: Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o perfil permita alterar. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.
   * **Aprovação do Administrador**: Este campo configura que todas as ações e solicitações efetuadas na interface da Plataforma do uCloud, deste usuário, deverão ser aprovadas por um usuário Administrador do Grupo. Esta é uma funcionalidade para aumentar o controle de governança de custos e operações.
   * Este é um campo tipo “check box” que o usuário pode atuar para alternar o seu modo atual, desde que o perfil permita alterar. Se o ícone estiver na cor vermelha, basta clicar com o cursor do mouse e o campo será ativado para a cor verde. Caso o ícone esteja na cor verde, basta clicar com o mouse e o campo será desativado ficando na cor vermelha.


* **Seção Permissões do Usuário**: Quando o usuário é criado ele herda/recebe todas as permissões definidas no Grupo ao qual ele pertence (ver próxima seção), bem como as permissões estabelecidas no Contrato. Esta tabela é opcional, mas permite adicionar, ou revogar, as permissões que este usuário possui para efetuar ações, ou acessar menus, na Plataforma do uCloud.
   * **Botão Editar**: Para acrescentar ou revogar permissões para o usuário, o Administrador (ou usuário com autorização) deve clicar neste botão para que a Plataforma do uCloud possa apresentar a tela que seja possível realizar o procedimento de adicionar ou excluir permissões específicas para este usuário. Veja exemplo abaixo:
   * Esta tela possui duas colunas distintas:
       * À esquerda são as permissões previamente adicionadas ao usuário. Ao lado de cada permissão existe um campo do tipo “check box” que ao ser selecionado exclui (revoga) a respectiva permissão deste usuário.
       * À direita estão as permissões disponíveis na Plataforma do uCloud que podem ser adicionadas ao perfil individual deste usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, adiciona a respectiva permissão deste usuário.
       * **Utilizar as permissões padrões**: Ao selecionar este campo “check box”, e confirmar a ação, o usuário receberá todas as permissões de usuário disponíveis na Plataforma do uCloud.
       * **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o mouse no botão Aplicar para confirmar as alterações - de forma definitiva e imediata - para o usuário que está visualizando/alterando. Terminada esta ação a Plataforma do uCloud fechará esta tela e retorna à tela anterior, com seu conteúdo atualizado, apresentando a nova relação de permissões do usuário.

* **Seção Políticas de Permissionamento do Usuário (eventual)**: Esta seção somente será apresentada para usuários que foram provisionados na Plataforma uCloud com o "checkbox" Criar Usuário na Nuvem habilitado. Esta seção apresenta todas as políticas de permissionamento únicas e específicas do ambiente do provedor de serviço de nuvem pública. Estas políticas são ‘importadas’ durante o processo de sincronização do container, e permitem um alto nível de controle granular das capacidades (permissões) que o usuário pode efetuar dentro do ambiente do provedor de serviço de nuvem. Quando o usuário é recém provisionado, este pode estar associado a nenhuma política de permissionamento, será necessário configurar manualmente as permissões.  
   * Botão Editar “  " Este botão permite ao usuário Administrador (ou usuário com autorização) acrescentar ou revogar políticas de permissionamento do ambiente do provedor de serviço de nuvem. Para isto, ele deve clicar no botão ‘Editar’ a partir daí será permitido ao usuário administrador adicionar ou excluir permissões específicas para o usuário desejado. Veja exemplo abaixo:
   * Esta tela possui duas colunas distintas:
      * À esquerda são as políticas de permissionamento previamente adicionadas ao usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, exclui (revoga) a respectiva permissão deste usuário.
      * À direita estão as políticas de permissionamento disponíveis do ambiente do provedor de serviço de nuvem pública que podem ser adicionadas ao perfil individual deste usuário. Ao lado de cada permissão existe um campo do tipo “check box” que, quando selecionado, adiciona a respectiva permissão deste usuário.
      * **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação, a Plataforma do uCloud fechará esta tela e retornará à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.
   
* **Seção Permissões do Grupo**: Esta seção somente apresenta as permissões que foram definidas nas configurações do Grupo ao qual este usuário está vinculado. A Plataforma do uCloud não permite que as permissões listadas aqui possam ser alteradas através desta tela. Para ter contato e conhecer as permissões definidas no grupo, veja o item Administração / Grupos. Se forem necessárias alterações de qualquer permissão listadas aqui, estas alterações devem ser efetuadas nas configurações do Grupo.

* **Seção Grupos Secundários**: Nesta seção é possível associar um usuário a mais de um grupo na Plataforma do uCloud. Na seção Geral, é possível verificar o Grupo principal ao qual o usuário está vinculado.
   * **Botão Editar**: Para vincular este usuário a um grupo secundário, ou desvincular este usuário de um grupo secundário, o Administrador (ou usuário com autorização) deve clicar neste botão Editar para que a Plataforma do uCloud possa apresentar a tela que permite desvincular o usuário de grupos secundários. Veja exemplo abaixo:
   * À direita estão listados os grupos que estão vinculados ao contrato do grupo principal ao qual este usuário foi provisionado originalmente. A Plataforma do uCloud lista somente os grupos que estão vinculados ao contrato vigente. Ao lado de cada grupo existe um campo do tipo “check box” que, quando selecionado, vincula o grupo selecionado a este usuário.
   * À esquerda estão listados os grupos secundários que este usuário está vinculado. Ao lado de cada grupo existe um campo do tipo “check box” que, quando selecionado, desvincula o grupo selecionado deste usuário.
   * **Botão Aplicar**: Após certificar que todas as vinculações, ou remoção, foram configuradas, o usuário deve clicar no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

* **Seção Perfis de Visualização**: Esta seção permite que o administrador do contrato possa selecionar quais opções do Menu do Usuário, este usuário poderá visualizar. Através desta funcionalidade, o administrador pode personalizar como este usuário interage com a Plataforma do uCloud. É possível acompanhar o processo de definição destes perfis no item Configurações / Perfis de Visualização. Esta configuração retira ou adiciona as opções da barra de Menu de Usuário, de forma que para o usuário não há como saber que tal função existe. A possibilidade de saber, seria acompanhar outro usuário utilizando a plataforma com outras opções de Menu de Usuário visíveis.
   * **Botão Adicionar**: Para adicionar este usuário a um perfil de visualização, ou desvincular este usuário de um grupo secundário, o Administrador (ou usuário com autorização) deve clicar neste botão Adicionar para que a Plataforma do uCloud possa apresentar a tela que possibilita associar o usuário a um dos perfis de visualização configurados na plataforma. Veja exemplo abaixo:
   * Pode-se informar parte do nome de um grupo e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud apresente uma lista com todos os grupos que possuem a mesma sequência de caracteres informados. Este campo é sensível a maiúsculas e/ou minúsculas, somente irá listar os Perfis de Visualização que combinam exatamente com a parte do texto que foi digitado (se nada for listado, digitar o texto com outra combinação de maiúsculas e ou minúsculas.

.. note:: *Importante ressaltar que os perfis listados na tela exemplo não existem e foram criados apenas para fins ilustrativos.*

   * **Botão Salvar**: Após certificar que vinculou o usuário ao Perfil de Visualização correto, o usuário deve clicar com o botão do mouse no botão Salvar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está visualizando/alterando. Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

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

A seguir a descrição do correto preenchimento dos campos desta tela, para provisionar um usuário na Plataforma do uCloud, são eles:

* *Grupo*: Este campo é obrigatório e o usuário deve informar um grupo previamente provisionado na Plataforma do uCloud, pois não será possível continuar o cadastramento de um usuário sem vincular este novo usuário a um grupo existente.
   * Pode-se informar parte do nome de um grupo e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo:
   * Quando encontrado o Grupo ao qual este novo usuário deverá estar vinculado, basta selecioná-lo e o campo se preencherá com o grupo específico.
   * *Importante ressaltar que será possível associar este usuário a mais de um grupo, caso seja necessário. Mas estes grupos devem estar vinculados a somente um único Contrato.*

* **Nome**: Este campo é obrigatório e deve ser preenchido com o nome do usuário que se está provisionando.
* **Login**: Este campo é obrigatório e deve ser preenchido com a sequência de caracteres que será utilizada para identificar o usuário durante o processo de login no uCloud.
* **Senha**: Este campo é obrigatório e deve ser preenchido com a sequência de caracteres da senha do usuário. Importante ressaltar que esta sequência deve ser maior do que quatro (04) caracteres alfanuméricos. Deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”, conforme a documentação encontrada no site da Azure. A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres e deve conter caracteres de três das seguintes categorias:
   * Letras maiúsculas e minúsculas (A a Z)
   * Números de base 10 (de 0 a 9)
   * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' <>,.? /) – Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política.

* **Confirmar Senha**: Este campo é obrigatório e deve ser preenchido com a mesma sequência de caracteres informados no campo anterior. Caso a sequência informada neste campo seja diferente da anterior, será apresentado um pop-up com uma mensagem de erro na tela.
* **Email**: Este campo é obrigatório, nele deve ser informado um endereço de correio eletrônico (e-mail) válido. Este endereço de correio eletrônico será fundamental durante o processo de redefinição de senha pelo usuário, pois a Plataforma do uCloud utiliza este e-mail para o envio de uma mensagem que permite ao usuário criar uma senha, para ele, de forma automática.

.. attention::
    A Plataforma do uCloud **não efetua** qualquer validação prévia referente a existência do e-mail informado ou seu efetivo funcionamento. No caso de inexistência do e-mail destino, ou erro em sua digitação, o usuário ficará impossibilitado de executar a redefinição da sua senha de acesso. Neste caso deverá contactar o administrador do seu grupo/contrato.

* **Telefone**: Este campo é obrigatório, e deve ser preenchido com um número de telefone de serviço móvel celular, utilizar o seguinte formato:
   * **Dois (02)** números que identificam o código de área do número de telefone de serviço móvel celular (XX). Não é necessário informar o número ‘zero (0)’ que antecede ao código de área no padrão brasileiro.
   * **nove (09)** números que identificam o número de telefone do serviço móvel celular do usuário. Não é necessário informar qualquer outro caractere para separação dos grupos de números de telefone serviço móvel celular.
   * Exemplo de preenchimento: ``11999991234``

* **Cargo**: Este campo é obrigatório, mas é meramente informativo para identificar o cargo do usuário que se deseja provisionar.
* **Empresa**: Este campo é obrigatório, mas é meramente informativo para identificar a organização a qual este usuário está associado.
* **Tipo de Cota**: Este campo é obrigatório, trata-se de um campo do tipo “drop down list”, quando o usuário clicar sobre este será apresentada a lista das opções de tipos de cota disponíveis para provisionar um usuário, veja as opções abaixo:
   * **Cota de Grupo**: Quando selecionada esta opção o usuário compartilha dos limites (cotas) financeiros ou de recursos computacionais que estão definidos nas configurações do Grupo. Usuários com cota de grupo devem ficar atentos nas informações apresentadas na tela inicial (dashboard – veja item Dashboard) uma vez que a Plataforma do uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites disponíveis no grupo ao qual o usuário está vinculado.
   * **Cota de Usuário**: Quando selecionada esta opção pelo usuário, a Plataforma do uCloud solicita que sejam informados os limites (cotas) financeiros ou de recursos computacionais específicos e individuais para este usuário, conforme a tela abaixo:
      * **Cota de CPU**: Este campo é obrigatório e deve ser informado um número inteiro que representa o limite máximo de consumo do recurso computacional de CPUs para todas as máquinas virtuais criadas nos provedores de serviço de nuvem (público e/ou privado), por este usuário.
      * **Cota de Faturamento**: Este campo é opcional e deve ser informado um número inteiro que será estabelecido como limite máximo referente aos valores financeiros dos custos de consumo dos recursos computacionais para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado).
      * **Cota de Memória**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Memória para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado). Pode ser selecionado o limite em Gigabytes ou um limite em Terabytes.
      * **Cota de Disco**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Disco para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado). Pode ser selecionado o limite em Gigabytes ou um limite em Terabytes.
      * **Cota de IPs Públicos**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de IPs Públicos para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado).
      * Em outras palavras, os usuários sem cota individual podem consumir a cota definida no Grupo; quando definida uma cota para um usuário, uma parte da cota do Grupo é alocada para o usuário, esta parte da cota do Grupo não será acessível a outros usuários do Grupo.
      * Quando um usuário se registra, ele deve observar as informações apresentadas na tela inicial (dashboard – veja item Dashboard na página ) pois a Plataforma do uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites definidos para este usuário.      

.. note:: *Importante ressaltar que os usuários com cotas individuais: esta cota individual será subtraída (retirada) da cota do Grupo ao qual este usuário está vinculado.* 

* **Habilitar Primeiro Acesso**: Este campo é um campo opcional do tipo de seleção  “check box”, que permite que o usuário possa alterar sua senha de acesso no primeiro acesso deste usuário a Plataforma do uCloud. Quando selecionado, a Plataforma do uCloud irá apresentar um ‘pop-up’ solicitando ao usuário informar uma nova senha, para substituir a senha inicialmente provisionada para este usuário,

.. warning:: Importante ressaltar que esta etapa é mandatória, e a Plataforma do uCloud não irá permitir que o usuário inicie uma sessão ativa sem antes o usuário substituir a senha originalmente informada. Após o usuário informar a nova senha, será armazenada de forma encriptada nas bases de dados internas, neste momento a sessão do usuário se torna ativa para iniciar a o uso da Plataforma do uCloud normalmente.

* **Ativar Autenticação Multifator**: Este campo é um campo de seleção “check box” que indica se este usuário terá seu processo de autenticação na plataforma (login) sendo verificado duplamente antes de aprovar que este usuário tenha acesso a Plataforma do uCloud. Será enviada uma mensagem para o correio eletrônico informado no campo **e-mail** com um link/url para o usuário confirmar a segunda etapa de autenticação.
* **Ativar cota de Faturamento**: Este campo é um campo de seleção “check box” que indica se este usuário terá seu faturamento computado constantemente na relação de consumo de Faturamento (ver item Financeiro).
* **Administrador precisa aprovar a realização de atividades**: Este campo é um campo de seleção "checkbox" que indica todas as ações e solicitações efetuadas na interface da Plataforma do uCloud, elas devem ser aprovadas por um usuário Administrador do Grupo. Esta é uma funcionalidade destinada a aumentar o controle de governança de custos e operações.
   Na prática, qualquer novo recurso computacional (uma nova máquina virtual) que este usuário solicitar através da interface do uCloud: a solicitação não será enviada para o provedor de serviço de nuvem (público e/ou privado) de forma imediata, a solicitação ocorrerá em 2 tempos. No primeiro momento, ela aguarda a aprovação do Administrador do Grupo. No segundo tempo, após a aprovação do administrador do grupo (se aprovada) a solicitação segue no processo de criação/alteração solicitada por este usuário.
* **Criar Usuário na Nuvem**: Este campo é um campo de seleção "checkbox" que indica as credenciais de login e senha deste usuário (informadas acima), elas serão enviadas ao provedor de serviço de nuvem pública para que seja provisionado um usuário com as mesmas credenciais de acesso no provedor de serviço de nuvem pública selecionado abaixo.
   * **Containers**: Este campo é obrigatório e do tipo “Dropdown” quando o usuário clica com o cursor do mouse, a Plataforma do uCloud lista todos os containers configurados na Plataforma do uCloud. O usuário deve selecionar um provedor da lista.
* **Permissões**: O usuário recebe/herda todas as permissões definidas no Grupo ao qual ele pertence, bem como as permissões estabelecidas no Contrato e por último as permissões específicas deste usuário. Esta tabela é opcional, ela permite adicionar ou revogar as permissões que este usuário recebe, o que permite efetuar ações ou acessar menus na Plataforma do uCloud. São cento e trinta e duas (132) permissões disponíveis que podem ser associadas ao usuário (todas ou apenas uma parte). Qualquer alteração efetuada nas permissões disponíveis (inclusão ou revogação) será aplicada de forma imediata no login deste usuário após a confirmação. Veja o item Configurações / Perfis de Permissionamento para uma forma alternativa de criar grupos de permissões customizados para sua empresa
   * **Botão Criar**: Após todos os campos obrigatórios e opcionais para provisionar o novo usuário estarem preenchidos o usuário pode clicar com o cursor do mouse no botão verde Criar, assim a Plataforma do uCloud provisiona o novo usuário em suas bases de dados internas. Caso o botão Criar não seja apresentado na cor verde, significa que algum campo obrigatório permanece sem preenchimento (o usuário deve checar e corrigir) ou a sequência de caracteres da senha do login deve ser inferior a quatro (04) caracteres.

Administração / Grupos
----------------------

Na Plataforma uCloud, o termo Grupo estabelece um conceito que permite alocar uma determinada quantidade de recursos computacionais, ou recursos financeiros, que poderão ser consumidos por todos os usuários que estão vinculados ao grupo, criando assim uma pequena ‘célula’ de governança financeira. A Plataforma do uCloud pode conter diversos Grupos para que a governança financeira fique mais próxima do cenário real da organização.

Importante ressaltar que o conceito de ''Grupos" existe somente para a Plataforma do uCloud e não existe nada similar nos provedores de serviço de nuvem pública ou privada.

Um Grupo de usuários pode ser um Departamento, uma Unidade de Negócio, um Centro de Custos, uma Filial. Quando se define um limite de quantidade de recursos computacionais ou um limite financeiro para um grupo, significa que a Plataforma do uCloud registra este limite. 

Se este recurso ultrapassar os limites estabelecidos para o grupo, da parte de qualquer usuário vinculado a este grupo, a Plataforma do uCloud nega (bloqueia) a criação ou alteração de determinada quantidade de recurso computacional, uma vez que este novo recurso computacional não poderá ultrapassar estes limites.

Estes limites podem ser ajustados a qualquer momento (aumento ou redução) da parte dos usuários com perfil de Administrador de Grupo ou Administrador de Contrato, apenas eles estão habilitados para alterar os valores limites (cotas) estabelecidos no grupo.

A seguir a descrição das colunas apresentadas nesta lista de grupos:
* **Botão Criar Grupo “  ”**: Quando selecionado este botão o processo está descrito no item.
* **Nome**: Esta coluna apresenta o nome do Grupo. Como forma de simplificar a visualização, é possível clicar com o botão do mouse no título desta coluna, o resultado apresentado na Plataforma do uCloud apresenta a classificação da lista de grupos de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Contrato**: Esta coluna apresenta o nome do Contrato ao qual este grupo está associado. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no nome do contrato de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Admin**: Esta coluna apresenta o nome do login de usuário que foi associado no campo de Administrador do Grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no nome do login de usuário de forma alfabética crescente (a – z) ou decrescente (z – a).
* **Cota de CPU**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de CPU que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor da quantidade de CPU de forma crescente ou decrescente.
* **Cota de Memória**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Memória que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor da quantidade de memória de forma crescente ou decrescente.
* **Cota de Disco**: Esta coluna apresenta o número inteiro que representa o limite (cota) valor total de Disco de Armazenamento que foi definido para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor total do Disco de Armazenamento de forma crescente ou decrescente.

Visualizando Grupo
------------------

Estando na listagem de grupos é possível visualizar algumas informações de um grupo, para isto, basta clicar com o mouse sobre a linha à qual um grupo faz parte e a Plataforma do uCloud apresentará a tela com todas as informações de um grupo provisionado na plataforma. Através desta tela é possível adicionar novas configurações ao perfil de um usuário.

A tela de visualização de detalhes de um usuário está dividida em seções, descrita abaixo:

* **Botão de Excluir Grupo**: Este botão pode ser usado para remover o grupo provisionado na Plataforma do uCloud de forma definitiva e irreversível. Basta o usuário clicar com o cursor do mouse sobre o botão, e será apresentada uma tela solicitando a confirmação da ação, conforme a tela abaixo:
     * Após a confirmação da Exclusão do grupo, este grupo e as configurações associadas a este estarão indisponíveis imediatamente de forma irreversível, não sendo possível recuperar as informações deste grupo. Se a exclusão for acidental, este usuário deverá ser provisionado novamente, ver o item  na página.

.. warning:: A Plataforma do uCloud não permite remover um grupo quando existem ainda usuários vinculados ao grupo. Antes de excluir um grupo da plataforma certifique que todos seus usuários foram desvinculados do referido grupo para que seja possível a remoção do grupo seja definitiva.
	
* **Seção Geral**: Esta seção da tela apresenta as informações sobre o grupo que está provisionado e os campos apresentados nesta seção podem ter seu conteúdo alterado através desta tela. O que define a condição de alteração está relacionado com o ícone de edição a seguir:
   * **Ícone de Edição Ativo**: Todos os campos que possuem o ícone de edição ativo são passíveis de ter seu conteúdo alterado.
   * **Ícone de Edição Inativo**: Todos os campos que possuem o ícone de edição inativo ou não são passíveis de terem seu conteúdo alterado através desta tela (ex.: valores das cotas de grupo) ou o perfil do usuário que está registrado e acessando esta tela, não possui permissão para alterar o conteúdo do(s) campo(s).
   * **Ícone de Confirmação**: Quando o usuário confirma a intenção de alterar o conteúdo do campo desejado, a Plataforma do uCloud apresenta um ícone de confirmação. Após ter finalizado a alteração do conteúdo do campo o usuário deve clicar com o cursor do mouse no botão verde para confirmar a alteração. Após esta ação a informação do campo será alterada permanentemente nas bases de dados da Plataforma do uCloud.
   * **Ícone de Cancelamento**: Caso o usuário tenha clicado sobre o ícone de edição por engano, ou não deseja que as alteração seja armazenada (gravada) permanentemente, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho, para cancelar as alterações e o conteúdo do campo irá retornar para os valores iniciais, antes de qualquer preenchimento ou alteração.
* **Seção Permissões**: O Grupo recebe (herda) todas as permissões definidas no Contrato ao qual este grupo está vinculado. Esta tabela é opcional, mas permite adicionar ou revogar as permissões que este grupo possui para efetuar ações ou acessar menus na Plataforma do uCloud.
   * **Botão Editar**: Para acrescentar ou revogar permissões para o usuário Administrador do Grupo (ou usuário autorizado com perfil semelhante ao administrador), basta clicar neste botão para que a Plataforma do uCloud apresente a tela para adicionar ou excluir permissões específicas para este grupo.
   * Esta tela possui duas colunas distintas, à esquerda são as permissões definidas no Contrato que são repassadas para o Grupo vinculado ao contrato. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, exclui (revoga) a respectiva permissão deste usuário.
   * À direita estão as permissões disponíveis na Plataforma do uCloud que podem ser adicionadas ao grupo. Ao lado de cada permissão existe um campo do tipo “checkbox” que, quando selecionado, adiciona a respectiva permissão deste usuário.
   * **Utilizar as permissões padrões**: Ao selecionar este campo “checkbox”, e confirmar a ação, o Grupo receberá todas as permissões disponíveis na Plataforma do uCloud.
   * **Botão Aplicar**: Após o usuário certificar-se de que todas as alterações necessárias foram configuradas (inclusões ou exclusões),ele deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o grupo que se está alterando. Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.

* **Seção Políticas de Permissionamento**: Seção Virtual Data Center: Nesta seção são listados todos os Virtual Data Centers (VDC) associados a este grupo. Um Virtual Data Center é um agrupamento ‘lógico’ de determinados recursos computacionais de nuvem (templates, flavors, redes, regiões globais, storage e máquinas virtuais) que possibilita um controle de governança financeira para a empresa. O usuário vinculado a este grupo, que possui um (ou mais) Virtual Data Center, somente poderá consumir os recursos computacionais disponíveis neste Virtual Data Center. Para mais informações veja no item Menu Virtual Data Center.
   * **Botão Editar**: Para vincular um Grupo a um Virtual Data Center, o usuário Administrador do Grupo (ou usuário com autorização) deve clicar neste botão para que a Plataforma do uCloud possa apresentar a tela para adicionar ou excluir um Virtual Data Center vinculado a este grupo.
   * Esta tela possui duas colunas distintas, à esquerda estão apresentados os Virtual Data Centers (VDCs) que foram vinculados a este Grupo (no momento do seu provisionamento). Ao lado de cada VDC existe um campo do tipo “checkbox” , ao selecioná-lo a Plataforma do uCloud exclui (desvincula) o VDC deste grupo.
   * À direita estão apresentados os Virtual Data Centers (VDCs) que estão vinculados ao contrato deste, ao qual este grupo pertence e que permite ser vinculado a este Grupo. Ao lado de cada VDC existe um campo do tipo “checkbox” , quando selecionado, vincula o VDC ao Grupo.
   * **Botão Aplicar**: Após certificar que todas as alterações necessárias foram configuradas (inclusões ou exclusões), o usuário deve clicar com o botão do mouse no botão Aplicar para configurar as alterações, de forma definitiva e imediata, para o grupo que se está alterando. Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando a nova relação de permissões do usuário.
   * **Coluna Ações / Botão Kick-Off**: Este botão permite desvincular o Virtual Data Center do Grupo em uma ação. Basta o usuário clicar com o mouse no botão Kick-Off para que o VDC seja desvinculado do Grupo, de forma definitiva e imediata, para o grupo que se está alterando. Importante ressaltar que esta ação não solicita validação para o usuário.

* **Seção Usuários**: Esta seção da tela apresenta a lista de todos os usuários que estão vinculados ao grupo e o respectivo consumo individual de recursos computacionais. Através desta tela o usuário com perfil de Administrador do Grupo, pode acompanhar qual(is) usuário(s) consome(m) mais recursos computacionais nos provedores de nuvem (público e/ou privado)
   * **Botão Criar Usuário**: Este botão permite provisionar um novo usuário na Plataforma do uCloud já vinculando este novo usuário ao grupo que se está visualizando. Esta é a metodologia recomendada pela Ustore para provisionar novos usuários para acessar o ambiente. Quando clicar com o botão do Mouse sobre este botão, a Plataforma do uCloud apresenta a tela de Criando Novo Usuário.
   * **Botão Adicionar Usuário Existente**: Este botão permite vincular um usuário existente a este grupo. Quando o usuário clicar com o cursor do mouse neste botão será apresentada uma tela.
   * É necessário preencher o campo desta tela com alguns caracteres do login do usuário que se deseja associar e a Plataforma do uCloud apresenta uma lista com os logins de usuário que possuam os caracteres informados em sua identificação de login. Selecionar o usuário desejado com o botão do mouse e depois confirmar a ação através do botão verde OK. Esta tela será encerrada e a lista de usuários do grupo será atualizada - como resultado apresenta este usuário, neste grupo.

Esta seção da tela possui uma lista com colunas, descritas a seguir:
* **Login**: Esta coluna apresenta as credenciais de login do usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de login de usuários de forma alfabética crescente (a – z) ou decrescente (z – a).

* **Cota de CPU**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de CPU que foi definida para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor da quantidade de CPU de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (0).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de Faturamento**: Esta coluna apresenta o número que representa o limite (cota) do valor financeiro que foi definido para o usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor financeiro de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (‘0’).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.

* **Cota de Memória**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Memória que for definida para este usuário. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor da quantidade de memória de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (‘0’).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.
* **Cota de Disco**: Esta coluna apresenta o número inteiro que representa o limite (cota) valor total de Disco de Armazenamento que for definido para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor total do Disco de Armazenamento de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (‘0’).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.
* **Cota de IPs Públicos**: Esta coluna apresenta o número inteiro que representa o limite (cota) da quantidade de Endereços TCP-IP Públicos que foram definidos para este grupo. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de grupos com base no valor da quantidade de IPs Públicos de forma crescente ou decrescente.
   * Se o usuário for provisionado para consumir cota do grupo o valor desta coluna será zero (‘0’).
   * Se o usuário for provisionado com limites (cotas) individuais, esta coluna apresenta o valor específico deste usuário.
* **Uso da CPU**: Esta coluna apresenta a quantidade consumida do recurso computacional CPU por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor total de consumo do recurso CPU de forma crescente ou decrescente.
* **Uso da Memória**: Esta coluna apresenta a quantidade consumida do recurso computacional de Memória por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor total de consumo do recurso Memória de forma crescente ou decrescente.
* **Uso do Disco**: Esta coluna apresenta a quantidade consumida do recurso computacional Disco de Armazenamento por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista dos usuários com base no valor total de consumo do recurso Disco de Armazenamento, de forma crescente ou decrescente.
* **Uso de IP**: Esta coluna apresenta a quantidade consumida do recurso computacional Endereços TCP-IP Público por este usuário específico. Como forma de simplificar a visualização, ao clicar com o botão do mouse no título desta coluna, a Plataforma do uCloud classifica a lista de usuários com base no valor total de consumo do recurso Endereço IP, de forma crescente ou decrescente.
* **Ações**: Esta coluna apresenta ícones que demonstram se o usuário está provisionado consumindo as cotas do Grupo ou possui cota individual. Para usuários com cotas individuais, existe um botão para editar os limites (cotas) dos recursos computacionais ou financeiros de um usuário com cotas individuais.
   * **Ícone de Cota de Grupo**: Este ícone será apresentado nas linhas de usuários que estão associados a cota de grupo.
   * **Ícone de Cota de Usuário**: Este ícone será apresentado nas linhas de usuários que estão associados a cota individual.
   * **Botão Editar Cotas**: Este botão é apresentado somente nas linhas de usuários que estão associados às cotas individuais. Exclusivamente estará ativo se o perfil do usuário que está registrado e acessando esta tela for um administrador de grupo ou de contrato e possuir a permissão para alterar o conteúdo do(s) campo(s). Quando for pressionado o botão 'Editar Cotas' a Plataforma do uCloud apresenta a tela abaixo:
      * **Cota de CPU**: Alterar, se necessário, o novo valor de limite de quantidade do recurso computacional das CPUs.
      * **Cota de Memória**: Alterar, se necessário, o novo valor de limite de quantidade do recurso computacional de Memória.
      * **Cota de Disco**: Alterar, se necessário, o novo valor de limite de quantidade do recurso computacional do Disco de Armazenamento.
      * **Cota de IPs Públicos**: Alterar, se necessário, o novo valor de limite de quantidade do recurso computacional de Endereços TCP-IP Público.
      * **Cota de Faturamento**: Alterar, se necessário, o novo valor do limite (cota) do valor financeiro que for definido para o usuário.
      * **Botão Editar**: Após checagem de que todas as alterações necessárias foram configuradas, o usuário deve clicar com o botão do mouse no botão Editar para configurar as alterações, de forma definitiva e imediata, para o usuário que se está alterando.
      * Após esta ação a Plataforma do uCloud fecha esta tela e retorna à tela anterior com seu conteúdo apresentando as novas cotas do usuário.


Criando Novo Grupo
------------------

O conceito de Grupos criado unicamente para a Plataforma do uCloud,  não existe nada semelhante em qualquer provedor de recursos computacionais de nuvem (público e/ou privado).
Para a Plataforma do uCloud um “Grupo” tem duas atribuições básicas que são:
#. Permite organizar usuários de forma a identificar um departamento, um centro de custo, uma iniciativa, apenas para citar alguns pontos.
#. Pode estabelecer um limite (cotas de recursos ou financeiro) para os usuários vinculados ao grupo, de como será possível consumir os recursos computacionais de nuvem (público e/ou privado).
Para criar um grupo é preciso provisionar, previamente, um Contrato na Plataforma do uCloud, e vincular o grupo a um contrato existente.
Importante ressaltar que somente os usuários com perfil de Administrador de Contrato, ou Administrador de Grupo estão habilitados para provisionar um grupo na Plataforma do uCloud.
Abaixo se apresenta a tela para provisionar um grupo na Plataforma do uCloud

* **Nome**: Este campo é obrigatório e deve ser preenchido com o nome do grupo.
* **Contrato**: Este campo é obrigatório e deve ser informado o nome do contrato, ao qual o grupo está vinculado. Pode-se informar parte do nome de um contrato e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo:
   * Serão listados apenas os contratos aos quais o perfil do usuário tem a permissão de visualizar. Assim que selecionado o grupo ficará vinculado ao contrato.
   * Assim que um contrato é selecionado, a Plataforma do uCloud apresenta, na coluna à direita desta tela, o grupo de Permissões que foram definidas no Contrato.

* Todos os usuários que pertencem ao grupo recebem as mesmas permissões. Existem duas formas diferentes que podem ser utilizadas neste momento para repassar as permissões do contrato para o grupo.
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

Somente usuários com perfil de Administrador de Contrato têm a permissão de visualizar esta lista de contratos da empresa. Este usuário terá acesso apenas aos contratos os quais o seu login de usuário está vinculado no campo de Administrador de Contrato.
  

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

Seção Geral
-----------

Quando um contrato é provisionado no sistema, o usuário com perfil de Administrador informa os dados cadastrais básicos da organização, informações gerais para um contrato, tais como Identificação do contrato, nome da empresa, o código CNPJ para empresas (ou CPF no caso de pessoa física), a forma padrão de faturamento das máquinas deste contrato (este padrão de faturamento fica válido somente no caso de não existir regras de bilhetagem no restante do contrato).

Deve ser informadas as credenciais de login de um usuário no campo Administrador, neste momento este usuário (simples) fica associado ao perfil de Administrador do Contrato. Veja a seção (card) abaixo:

Abaixo detalhamento dos campos não mencionados:
* **Public Gateway**: Este botão é válido apenas para ambientes em que o contrato está associado a um ambiente de um Data Center privado, no qual o ambiente de virtualização (hypervisor) é de controle da organização (on-premises). Para que este botão seja válido é necessário ao usuário, com perfil de Administrador da Plataforma uCloud, ter provisionado um Gateway SDN (Software Defined Network). Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração de um Gateway SDN.
* **Experimental**: Durante o aprovisionamento do contrato o Administrador do Contrato informa os limites (cotas) financeiros e/ou dos recursos computacionais. Em seguida, pode-se acessar a configuração de contrato Experimental. 
Através desta configuração é possível estabelecer a data de validade (expiração) do contrato, bem como um limite percentual, que ao ser atingido envia uma mensagem de ‘alerta’ de custo do contrato ou de consumo dos recursos computacionais. Adicionalmente, o usuário pode definir para quem o e-mail de alerta deve ser enviado (Administrador da Plataforma, Administrador do Contrato ou todos os usuários vinculados ao contrato). Veja o exemplo na tela abaixo:
  

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração do campo Experimental.
                                                            1. Seção Regras de Faturamento
Nesta seção o Administrador do Contrato pode personalizar as regras de como os valores dos custos do contrato podem ser convertidos para moeda local, também personaliza, se para o cálculo de conversão de moeda aplicará no fator de conversão: um valor fixo ou um valor variável. Para o valor variável, a Plataforma do uCloud está configurada para obter a taxa do valor de conversão diretamente do site do Banco Central do Brasil, local onde pode extrair a taxa PTAX do último dia útil do mês. 
Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração do campo Experimental.
  



                                                            * Quantidade de Casas Decimais: Este campo define a quantidade de casas decimais e é muito útil quando o Contrato possui valor em moeda estrangeira.
                                                            * Perfil de Tagueamento: Ver opção de Menu Configurações / Tagueamento de Recursos USN.


                                                            3. Seção Categorias de Preço
Nesta seção é possível provisionar as categorias de preço utilizadas para agrupar os preços do contrato, quando este contrato está associado a uma empresa do Governo municipal, estadual ou federal em que os valores a serem apresentados referente ao consumo dos recursos computacionais de nuvem deverão ser convertidos para a métrica de Unidade de Serviço de Nuvem (USN).
A Unidade de Serviço de Nuvem (USN) é um modelo de precificação dos serviços, divididos em categorias: os serviços de IaaS, PaaS e serviços técnicos. Visa estabelecer-se como método previsível, linear e flexível para obtenção de uma quantidade objetivamente definida a ser cobrada pelos serviços de computação em nuvem. A métrica de USN consiste no estabelecimento de um valor de referência específico para cada tipo de serviço de nuvem, conforme métrica individual associada ao consumo dos recursos.
  



Conforme esclarecido acima, o Administrador do Contrato, deverá efetuar o provisionamento de Categorias de Preço somente no caso deste contrato controlar algum órgão do Governo Brasileiro no âmbito municipal, estadual ou federal, única e somente este deve ser regido pela métrica de USN.
Importante ressaltar que se deve ignorar provisionar qualquer Categorias de Preço quando o seu contrato for controlar os recursos computacionais de nuvem de uma organização privada.


                                                            4. Seção Políticas de Alertas
A Plataforma do uCloud possibilita, ao usuário com perfil de Administrador do Contrato, definir Políticas de Alertas de consumo individual de recursos computacionais de nuvem. Quando a condição da regra for atingida a Plataforma do uCloud envia um e-mail para o Administrador de Contrato. Veja o exemplo da tela abaixo:
  



Abaixo descrevemos as colunas desta seção da tela de contratos:
                                                            * Nome: Esta coluna apresenta o nome de identificação da política de alerta definido durante seu provisionamento.
                                                            * Recurso: Essa coluna apresenta o tipo de recurso definido para que a Plataforma do uCloud monitore o consumo.
                                                            * Política: Essa coluna apresenta a forma definida que estabelece o limite do alerta.
                                                            * Valor: Essa coluna apresenta o valor de limite superior definido para que a Plataforma do uCloud possa comparar e enviar o alerta para o usuário Administrador do Contrato.
                                                            * Ações: Esta coluna apresenta dois ícones para que o usuário possa interagir com a política definida:
                                                            * Botão Lata de Lixo “  ”: Basta clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud remova esta Política de Alarme de forma imediata e definitiva.
                                                            * Botão Habilitar/Desabilitar “  ”: Este botão é um tipo “checkbox” que o usuário pode atuar para alternar o seu modo atual. A cor verde indica que a política está HABILITADA. A cor vermelha indica que a política está DESABILITADA.
Para alternar entre os estados basta clicar com o cursor do mouse e o campo será ativado, apresentando a cor verde. Se estiver na cor verde, basta clicar com o mouse e o campo será desativado, apresentando a cor vermelha.
Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração de uma Política de Alerta.
                                                               5. Seção Preço dos Recursos
Esta seção permite que o Administrador do Contrato possa redefinir os valores dos recursos que estão sendo consumidos dentro deste contrato. Através desta tela é possível definir preços diferentes para os recursos cobrados pelo provedor de serviço de nuvem. Estes novos valores devem ser informados manual e individualmente, não sendo necessário que todos sejam informados.
Apenas os valores dos recursos que foram informados serão recalculados pela Plataforma do uCloud, apresentados nos relatórios do menu Financeiro.
Os recursos com valor igual a zero (0), terão o seu valor original cobrado pelo provedor de serviço de nuvem sem ser recalculado.
  

Recomendamos fortemente que, qualquer alteração nos Valores dos Recursos altere os valores originalmente cobrados pelo provedor de serviços de nuvem.
☝
Atenção
	Lembramos ao usuário: ao informar qualquer novo valor, este ‘novo valor’ altera o valor da fatura mensal a ser cobrada pelo provedor, e qualquer diferença, multa ou penalidade contratual advindas destas alterações não são responsabilidade da Ustore ou da Plataforma do uCloud, pois a plataforma está desempenhando o função pela qual foi desenhada a efetuar.
	

                                                               6. Seção Cota do Contrato
A tela abaixo apresenta um exemplo da seção (card) de um contrato, o contrato apresenta os limites financeiros e os limites definidos para a quantidade dos recursos definidos para o contrato, pela organização.
  

Abaixo segue o detalhamento dos valores da tela acima:
                                                               * Cota de Faturamento / Alocada: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite financeiro (cota) do contrato. O primeiro número é a definição do limite superior do contrato, e o segundo número, representa o valor que já foi “alocado” para um (ou vários) grupo(s) que estão vinculados a este contrato. Neste exemplo: o contrato tem um limite de cem mil reais (R$100.000,00) e foi alocado para um (ou mais) grupo(s) um montante de três mil reais (R$3.000,00).
Importante mencionar: Outros grupos que venham a ser criados não podem ter locado valor acima deste limite financeiro.
O valor informado aqui é uma referência, não impede qualquer usuário na criação de novos recursos computacionais ultrapassar este valor. O número informado aqui, será utilizado como base de referência para a definição de “Alerta de Consumo” conforme descrito na seção acima.
                                                               * Cota de IPs Públicos / Alocada: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite numérico (cota) da quantidade de recurso de Endereços TCP-IP do contrato. O primeiro número é a definição do limite superior do contrato, e o segundo número, representa o valor que já foi “alocado” para um (ou vários) grupo(s) que estão vinculados a este contrato. Neste exemplo: o contrato tem um limite de duzentos (200) recursos e já foi alocado para um (ou mais) grupo(s) um total de dez (10) Endereços TCP-IP.
                                                               * Cota de CPU / Alocada: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite numérico (cota) da quantidade de recurso de CPUs do contrato. Neste exemplo: o contrato tem um limite de trezentos e sessenta (360) CPUs e já foram alocadas para um (ou mais) grupo(s) um total de duzentas (200) CPUs.
                                                               * Cota de Memória / Alocada: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite numérico (cota) da quantidade de recurso de Memória do contrato. Neste exemplo: o contrato tem um limite de seiscentos e dez Gigabytes (610GB) e já foram alocadas para um (ou mais) grupo(s) um total de quinhentos Gigabytes (500GB).
                                                               * Cota do Disco / Alocada: Neste campo o usuário com perfil de Administrador do Contrato cliente pode definir o limite numérico (cota) da quantidade de recurso de espaço em disco para armazenamento do contrato. Neste exemplo: o contrato tem um limite de cinquenta (50) Terabytes e já foram alocadas para um (ou mais) grupo(s) um total de trinta e nove (39) Terabytes.
Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de configuração de Cotas do Contrato.


                                                               7. Seção Contato Primário
Esta seção possibilita ao Administrador do Contrato informar os dados de contato de um responsável Financeiro, Fiscal ou Contábil referente a este contrato.
  

Esta seção não é obrigatória, e o não preenchimento desta seção não impede, ou bloqueia, nenhuma funcionalidade do perfeito uso da Plataforma do uCloud. 
Recomendamos o preenchimento destas informações para que a Plataforma do uCloud possa enviar informações automaticamente para o gestor do contrato.


                                                               8. Seção Administradores
Esta seção apresenta a relação de usuários (e/ou Grupos de Usuários), que possuem permissão de alterar qualquer um dos dados que compõem um contrato.
  



                                                               9. Seção Dados da Empresa
Esta seção possibilita ao Administrador do Contrato informar os dados genéricos da empresa associada a este contrato.
  

Esta seção não é obrigatória. No caso desta seção deixar de ser preenchida, isto não impede ou bloqueia as funcionalidades e o perfeito uso da Plataforma do uCloud.
                                                               10. Seção Virtual Datacenters Concedidos
Nesta seção o usuário Administrador do Contrato vincula o Virtual Data Center (VDC) ao contrato. Esta é uma das alternativas de Governança de Custos permitida pela Plataforma do uCloud – veja mais informações acima no item Administração de Contrato na página 58.
Quando ocorre a vinculação de um VDC a um contrato, significa que o usuário administrador do contrato estabelece para a Plataforma do uCloud a concessão deste VDC ao contrato. Assim, para o usuário - com permissão de administrador do contrato - serão listados apenas os VDCs deste contrato. Em outras palavras, todas as telas da Plataforma do uCloud onde um VDC pode ser ofertado (solicitado) ao usuário selecionar, o usuário pode visualizar/solicitar apenas os VDCs listados nesta seção.
  

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como vincular um VDC a um contrato.


                                                               11. Seção Usuários
Nesta seção (card) estão listados todos os usuários que estão vinculados, indiretamente, ao contrato. A associação do usuário ao contrato é estabelecida, pela inclusão do usuário a um Grupo e a vinculação do Grupo ao Contrato. Desta forma, o usuário fica vinculado a um contrato, ele compartilha e consome os limites financeiros e os limites (cotas) dos recursos computacionais de nuvem.
Nesta seção é possível verificar as cotas de cada usuário e o consumo dos recursos até o presente momento.
  





                                                               12. Seção Grupos
Esta seção apresenta todos os Grupos vinculados ao Contrato. A Plataforma do uCloud mostra ou lista as cotas que foram alocadas para cada Grupo vinculado ao Contrato. É possível verificar as cotas de cada grupo e o consumo dos recursos, dentro do grupo, até o momento da pesquisa.
  



                                                               * Botão “+Adicionar Grupo Existente”: Através deste botão, o usuário com perfil de Administrador de Grupo, poderá vincular um grupo - previamente provisionado na Plataforma do uCloud - ao contrato que se está visualizando. Quando o usuário clicar com o cursor do mouse sobre este botão, será apresentada a seguinte tela:
  



                                                               * Grupo: Neste campo o usuário precisa informar parte do nome de um grupo existente, como resultado a Plataforma do uCloud apresenta uma lista de todos os grupos que possuem parte dos caracteres informados. Basta o usuário selecionar o grupo desejado, o resultado é apresentado da seguinte forma:
  



                                                               * Botão “Adicionar Grupo (  ): Neste momento, o usuário deve clicar com o cursor do mouse sobre este botão para que a Plataforma do uCloud efetive a vinculação do grupo selecionado ao contrato que se está visualizando.
                                                               * Botão Ok: Ao clicar com o cursor do mouse sobre este botão, a Plataforma do uCloud encerra esta tela e retorna à visualização do Contrato, e a relação de grupos vinculados ao contrato, atualizada com o novo grupo.
                                                                  * Botão “+Criar Grupo”: Através deste botão o usuário, com perfil de Administrador de Grupo, poderá provisionar um novo grupo na Plataforma do uCloud. Mediante este botão, o novo grupo ficará obrigatoriamente vinculado ao contrato que se está visualizando. Veja a descrição de todo o processo de provisionamento de um grupo na Plataforma do uCloud no item Criando Novo Grupo na página 55 .


                                                                  13. Seção Dados de Faturamento
Nesta seção são apresentadas as informações de Faturamento de um Contrato. Estas informações, geralmente, são necessárias para integrações automatizadas com sistemas de CRM, showback e chargeback.
  

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos para informar os dados de Faturamento do Contrato.


                                                                  14. Seção Perfis de Permissionamento
Esta seção (card) se aplica ao usuário Administrador da Plataforma uCloud (perfil diferente do Administrador do Contrato), que tiver provisionado antecipadamente Perfis de Permissões através do menu Configurações / Perfis de Permissionamento. Somente um usuário com o perfil Administrador da Plataforma é responsável pela gerência de todos e dos demais grupos e permissões.
Quando um Perfil de Permissionamento é vinculado ao Contrato, isto implica que todos seus Grupos e Usuários recebem as mesmas permissões para acessar os menus da plataforma definidas neste perfil, de forma a permitir aos usuários vinculados a este contrato acesso às funcionalidades da Plataforma do uCloud definidas neste perfil de permissionamento.
  

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como provisionar um Perfil de Permissionamento e vincular um VDC a um contrato.


                                                                  15. Seção Produtos
Um produto pode ser visto como recurso, um software, o valor de uma licença específica, um serviço recorrente ou qualquer coisa que se seja necessário incluir em um Contrato. Importante ressaltar que o produto sempre será algo que não existe ou que não pode ser criado e gerenciado pela Plataforma do uCloud, diretamente no console dos provedores de nuvem pública e/ou privada. É indicado configurar um Produto quando a oferta é o Virtual Data Center como um todo, no caso de serviços, ofertas específicas para máquinas virtuais, é recomendado optar pelas assinaturas.
  

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como adicionar um Produto a um contrato.


                                                                  16. Seção Permissões Concedidas
Esta seção (card) permite personalizar as permissões concedidas aos usuários com acesso às funcionalidades na Plataforma do uCloud, de forma global. Estas permissões básicas, definidas e vinculadas ao Contrato, implicam que todos seus Grupos e Usuários recebam as mesmas permissões de acesso às funcionalidades definidas nesta seção. Diferente do Perfil de Permissionamento, esta configuração permite que o usuário com perfil de Administrador de Contrato adicione ou remova, permissões não previstas no Perfil de Permissionamento. Permite também, remover/excluir permissões do Contrato.
  

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como provisionar ou excluir Permissões vinculadas a um contrato.


                                                                  17. Seção Perfil de Faturamento de Container
Esta seção apresenta todos os dados relacionados ao perfil de faturamento de um contrato por tipo de container a ser utilizado. A Plataforma do uCloud permite vincular um Contrato a um Container. O termo container representa um hypervisor ou conexão com uma nuvem pública, sendo assim é possível que existam perfis de preços distintos de acordo com o container que um usuário possa vincular a um contrato. 
Através desta configuração é possível que sejam definidos preços distintos por perfil de faturamento (preço fixo, recurso alocado ou recurso efetivamente utilizado) por tipo de container.
  

Favor consultar o documento: Manual do Administrador da Plataforma do uCloud, para conhecer os procedimentos de como provisionar um contrato.


                                                                  8. Provisionando Contrato
É relevante ressaltar que não é objetivo deste documento descrever o processo de provisionamento de um contrato, pois apenas os usuários com perfil de Administrador da Plataforma uCloud têm permissão para isto. Veja o documento Manual do Administrador da Plataforma do uCloud onde descrevemos o processo como provisionar um contrato.
