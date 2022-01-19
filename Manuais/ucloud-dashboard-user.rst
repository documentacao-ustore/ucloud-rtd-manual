Dashboard
=========

Após informar o usuário e senha, será possível ver a tela principal do portal uCloud, conforme apresentado na tela abaixo, a mesma possui um menu na lateral esquerda com uma lista de opções, sendo que cada opção representa uma tela de administração do uCloud, algumas telas só estarão disponíveis de acordo com o nível de acesso do usuário.

O usuário pode notar que a tela do Dashboard está dividida em seções, a seguir descritas:

Seção Containers
----------------

Nesta seção são apresentados todos os provedores de nuvem (público e/ou privado) onde cada container está representado com um “botão” na interface, conforme o exemplo abaixo:

**imagem_dashboard**  

A cada busca de uma informação do container que o usuário tiver interesse, basta selecionar com o mouse o “botão” que representa o container. 

Assim, para que o usuário possa checar suas cotas e alocação de recursos, basta selecionar o container escolhido na seção de Gráficos de Uso dos Recursos. Então, ao finalizar a seleção a imagem da tela será alterada e apresentará como resultado a representação da respectiva alocação referente o container selecionado.

Dado que a Plataforma do uCloud é um ambiente híbrido multi-nuvem, serão apresentados quantos botões forem necessários para representar todas as nuvens (público e/ou privado) que tenham sido configuradas no ambiente do uCloud.

No caso de existir apenas um botão, isto significa que o cliente possui um único provedor de serviço de nuvem configurado em seu ambiente.

Ver o ítem Containers para entender os processos de como configurar um provedor de serviço de nuvem (público e/ou privado) na Plataforma do uCloud.

Seção Gráficos de uso dos recursos
----------------------------------

Nesta seção o usuário pode verificar a quantidade de recursos computacionais disponíveis (cota limite) e o valores totais que já foram utilizados/consumidos por ele:

**imagem_secao001**

Estes limites (cotas) foram definidos e/ou alocados para o usuário, eles seguem os padrões e regras de negócio da organização, os quais foram associados a este usuário no momento do provisionamento das suas credenciais na Plataforma do uCloud.

Consultar os ítens Grupos e Usuários para configurar ou alterar os limites (cotas) de recursos computacionais ou recursos financeiros, tanto para grupos quanto para limite individual destinado a um usuário específico.

Seção Últimas Tarefas
---------------------

A Plataforma do uCloud é um ambiente que se comunica com os consoles dos provedores de nuvem ou com o hypervisor utilizado internamente no Data Center de sua organização através da API Rest. Desta forma, todas as ações - atividades - funções solicitadas através da Plataforma do uCloud são ‘encapsuladas’ como se fossem uma mensagem e são enviadas para o console destino para que este console execute as tarefas enviadas.
  
**imagem_secao002**

Por consequência, a seção Tarefas apresenta a lista mais recente das ações - atividades - funções solicitadas pelo usuário que está registrado e ativo (login) na Plataforma do uCloud.

Nesta seção será apresentada uma lista de algumas tarefas, as quais demonstram o percentual executado e o(s) respectivo(s) resultado(s) dessa(s) ação(ões), tanto para ações completas com sucesso ou não completas, devido algum erro recebido de resposta do console destino (pública e/ou privada).
Veja outros detalhes no item Tarefas.

Seção Máquinas Virtuais 
-----------------------

Nesta seção serão listadas aqui as máquinas virtuais que sofreram interações ou alterações recentes através da interface da Plataforma do uCloud.

**imagem_secao003**

Importante ressaltar um ponto: qualquer máquina virtual que o usuário tenha alterado alguma das suas características através do console do provedor de serviço de nuvem (público e/ou privado) esta máquina virtual não fará parte desta lista. A Plataforma do uCloud lista apenas as máquinas virtuais as quais foram alteradas por usuários registrados e ativos (login) na Plataforma do uCloud.

Consultar o item Menu de Usuário para entender as funcionalidades de cada opção do menu.

Seção Atalhos para os principais menus
--------------------------------------

Nesta seção são apresentados atalhos para as mais frequentes funcionalidades da Plataforma do uCloud de forma mais acessível e direta.
  
**imagem_secao004**

Todos os atalhos até aqui apresentados podem ser acessados através das suas respectivas funções no Menu do Usuário, que está posicionado na barra ao lado esquerdo na interface da Plataforma do uCloud.

Importante ressaltar que o usuário ativo (login) pode possuir restrições a determinadas opções do menu, em função do perfil associado a este usuário, determinado pela organização a qual o usuário está associado. Desta forma, serão listados os atalhos correspondentes ao perfil do usuário que terá permissão de acessar.

Solicitação de Nova Senha
=========================

Caso o usuário não lembre dos seus dados para efetuar o login na Plataforma do uCloud, ela permite recuperar a senha de acesso durante o processo do login ou caso o usuário receba a mensagem no canto superior da tela com um aviso pop-up  “Usuário ou senha incorretos” conforme a figura abaixo:

**sugestão_de_imagem**

O usuário deverá clicar com o cursor do mouse sobre a opção “Esqueceu sua Senha?” conforme o detalhe na figura abaixo:

**sugestão_de_imagem**

Figura 1 Acesso ao portal Intercloud

Caso as informações de login do usuário existam, mas se o mesmo necessitar inserir nova senha, a Plataforma do uCloud apresentará ao usuário o formulário para alteração.

No primeiro campo, o usuário informa o endereço de e-mail que está registrado e no segundo campo ele deve preencher com a informação de login do usuário que foi provisionado na Plataforma do uCloud.
Após informar uma conta de e-mail e usuário válidos para acesso, o usuário deve clicar com o cursor do mouse no botão verde Editar, a interface apresentará a mensagem a seguir:

**sugestão_de_imagem**

O usuário deverá verificar o recebimento de uma mensagem em sua caixa postal de e-mail com as instruções para redefinição da senha. O usuário deverá proceder como descrito no e-mail e redefinir a sua senha de acesso.
  
É necessário checar se o domínio “@ucloud.usto.re” está bloqueado na sua lista de mensagens indesejadas (spam) para permitir o recebimento dela.
Quando o usuário clicar com o cursor do mouse sobre o link/url presente no seu e-mail, este será levado para uma sessão do seu navegador (browser) de Internet conectado na Plataforma do uCloud, a tela abaixo será apresentada:
  
**sugestão_de_imagem**

Após o usuário informar a nova sequência de caracteres no campo Nova Senha, o mesmo deverá informá-la novamente no campo seguinte Confirmar Senha igual a informada no campo anterior.
Após confirmar a nova senha o usuário deve clicar com o cursor do mouse no botão Salvar, a interface apresentará a seguinte mensagem:
  
**sugestão_de_imagem**

Após este procedimento o usuário poderá efetuar o processo de login utilizando as informações de usuário e a nova senha. A nova senha estará disponível de forma imediata, não sendo necessário aguardar nenhum período para a efetivação dela.

Usuário não provisionado
------------------------

Caso a informação de login do usuário não tenha sido previamente cadastrada ou a combinação de e-mail e dados de login, a Plataforma do uCloud apresentará uma mensagem pop-up - no canto superior direito da tela - com a informação de que os dados informados para alteração da senha não existam na Plataforma do uCloud.
  
**sugestão_de_imagem**

Neste caso, basta entrar em contato com o Administrador da Plataforma do uCloud da sua organização para que ele possa efetuar o provisionamento dos seus dados para o login.
Somente um usuário devidamente provisionado terá seu acesso efetivado.