Acesso a plataforma uCloud
==========================

Para o usuário utilizar a Plataforma do uCloud, seu acesso é feito através de um endereço de Internet, o usuário deve utilizar um navegador de Internet (*Internet browser*) e inserir o endereço da ``URL/link``, assim o usuário visualiza a tela inicial de apresentação. Os navegadores de Internet compatíveis com a Plataforma do uCloud são: Microsoft Edge versão 86.x, Google Chrome versão 85.x, Firefox verão 80.x ou Opera versão 71.x.

.. warning:
	*Importante ressaltar que a Plataforma do uCloud não é compatível com o Microsoft Internet Explorer (IE) em qualquer versão, pois as tecnologias deste navegador se encontram desatualizadas e não suportam a evolução das atuais páginas HTML.*

Após iniciar uma sessão de Internet browser, o endereço/caminho para o acesso a aplicação deve ser preenchido conforme exemplo abaixo, da seguinte forma:
  ``http://<ucloudserverTCP_IP_Address>:80``
  ``http://ucloud_Server_Name.com/``

As credenciais para o login e senha devem ter sido provisionadas previamente na Plataforma do uCloud, por um usuário com perfil de Administrador (ou outro usuário com esta permissão).
O usuário deverá informar nos campos os seus dados de login e senha e clicar com o cursor do mouse sobre o botão Entrar.
Caso as credenciais de acesso não tenham sido provisionadas, não existam ou em último caso, o usuário não se recorde das corretas informações das suas credenciais, não terá acesso a plataforma. Ver o item Solicitação de Nova Senha, no caso de o usuário esquecer algum tipo de informação para proceder com o login de acesso à Plataforma do uCloud.
Após inserir suas credenciais de acesso (nome do usuário e senha), efetuar o procedimento de login, ao usuário será apresentada a tela inicial (*Dashboard*).

Dashboard
---------



Seção Containers
----------------
Seção Gráficos de uso dos recursos
----------------------------------
Seção Últimas Tarefas
~~~~~~~~~~~~~~~~~~~~~
Seção Máquinas Virtuais
~~~~~~~~~~~~~~~~~~~~~~~
Seção Atalhos para os principais menus
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Solicitação de Nova Senha
=========================
Usuário não provisionado
------------------------


2. Acesso a plataforma uCloud
O acesso à plataforma é feito através de um endereço de Internet, o usuário deve utilizar um navegador de Internet (Internet browser) e inserir o endereço da URL/link, assim o usuário visualiza a tela inicial de apresentação. Os navegadores de Internet compatíveis com a Plataforma do uCloud são: Microsoft Edge versão 86.x, Google Chrome versão 85.x, Firefox verão 80.x ou Opera versão 71.x.


☝
Atenção
	Importante ressaltar que a Plataforma do uCloud não é compatível com o Microsoft Internet Explorer (IE) em qualquer versão, pois as tecnologias deste navegador se encontram desatualizadas e não suportam a evolução das atuais páginas HTML.
	

Após iniciar uma sessão de Internet browser, o endereço/caminho para o acesso a aplicação deve ser preenchido conforme exemplo abaixo, da seguinte forma:
http://<ucloudserverTCP_IP_Address>:80
http://ucloud_Server_Name.com/
Após entrar com o endereço corretamente, a tela do usuário será similar a figura abaixo:
  



As credenciais para o login e senha devem ter sido provisionadas previamente na Plataforma do uCloud, por um usuário com perfil de Administrador (ou outro usuário com esta permissão).
O usuário deverá informar nos campos os seus dados de login e senha e clicar com o cursor do mouse sobre o botão Entrar.
Caso as credenciais de acesso não tenham sido provisionadas, não existam ou em último caso, o usuário não se recorde das corretas informações das suas credenciais, não terá acesso a plataforma. Ver o item Solicitação de Nova Senha, no caso de o usuário esquecer algum tipo de informação para proceder com o login de acesso à Plataforma do uCloud.
Após inserir suas credenciais de acesso (nome do usuário e senha), efetuar o procedimento de login, ao usuário será apresentada a tela abaixo:
 Graphical user interface, application

Description automatically generated 



A seguir, a descrição detalhada das características da tela inicial (Dashboard) da Plataforma do uCloud.
   1. Dashboard
Após informar o usuário e senha, será possível ver a tela principal do portal uCloud, conforme apresentado na tela abaixo, a mesma possui um menu na lateral esquerda com uma lista de opções, sendo que cada opção representa uma tela de administração do uCloud, algumas telas só estarão disponíveis de acordo com o nível de acesso do usuário.
O usuário pode notar que a tela do Dashboard está dividida em seções, a seguir descritas:
1. Seção Containers
Nesta seção são apresentados todos os provedores de nuvem (público e/ou privado) onde cada container está representado com um “botão” na interface, conforme o exemplo abaixo:
  
  
  
  
  
  

A cada busca de uma informação do container que o usuário tiver interesse, basta selecionar com o mouse o “botão” que representa o container. 
Assim, para que o usuário possa checar suas cotas e alocação de recursos, basta selecionar o container escolhido na seção de Gráficos de Uso dos Recursos. Então, ao finalizar a seleção a imagem da tela será alterada e apresentará como resultado a representação da respectiva alocação referente o container selecionado.
Dado que a Plataforma do uCloud é um ambiente híbrido multi-nuvem, serão apresentados quantos botões forem necessários para representar todas as nuvens (público e/ou privado) que tenham sido configuradas no ambiente do uCloud.
No caso de existir apenas um botão, isto significa que o cliente possui um único provedor de serviço de nuvem configurado em seu ambiente.
Ver o ítem Containers para entender os processos de como configurar um provedor de serviço de nuvem (público e/ou privado) na Plataforma do uCloud.
2. Seção Gráficos de uso dos recursos
Nesta seção o usuário pode verificar a quantidade de recursos computacionais disponíveis (cota limite) e o valores totais que já foram utilizados/consumidos por ele:
  



Estes limites (cotas) foram definidos e/ou alocados para o usuário, eles seguem os padrões e regras de negócio da organização, os quais foram associados a este usuário no momento do provisionamento das suas credenciais na Plataforma do uCloud.
Consultar os ítens Grupos e Usuários para configurar ou alterar os limites (cotas) de recursos computacionais ou recursos financeiros, tanto para grupos quanto para limite individual destinado a um usuário específico.
3. Seção Últimas Tarefas
A Plataforma do uCloud é um ambiente que se comunica com os consoles dos provedores de nuvem ou com o hypervisor utilizado internamente no Data Center de sua organização através da API Rest. Desta forma, todas as ações - atividades - funções solicitadas através da Plataforma do uCloud são ‘encapsuladas’ como se fossem uma mensagem e são enviadas para o console destino para que este console execute as tarefas enviadas.
  

Por consequência, a seção Tarefas apresenta a lista mais recente das ações - atividades - funções solicitadas pelo usuário que está registrado e ativo (login) na Plataforma do uCloud.
Nesta seção será apresentada uma lista de algumas tarefas, as quais demonstram o percentual executado e o(s) respectivo(s) resultado(s) dessa(s) ação(ões), tanto para ações completas com sucesso ou não completas, devido algum erro recebido de resposta do console destino (pública e/ou privada).
Veja outros detalhes no item Tarefas.
4. Seção Máquinas Virtuais 
Nesta seção serão listadas aqui as máquinas virtuais que sofreram interações ou alterações recentes através da interface da Plataforma do uCloud.
  

Importante ressaltar um ponto: qualquer máquina virtual que o usuário tenha alterado alguma das suas características através do console do provedor de serviço de nuvem (público e/ou privado) esta máquina virtual não fará parte desta lista. A Plataforma do uCloud lista apenas as máquinas virtuais as quais foram alteradas por usuários registrados e ativos (login) na Plataforma do uCloud.
Consultar o item Menu de Usuário para entender as funcionalidades de cada opção do menu.
5. Seção Atalhos para os principais menus
Nesta seção são apresentados atalhos para as mais frequentes funcionalidades da Plataforma do uCloud de forma mais acessível e direta.
  



Todos os atalhos até aqui apresentados podem ser acessados através das suas respectivas funções no Menu do Usuário, que está posicionado na barra ao lado esquerdo na interface da Plataforma do uCloud.
Importante ressaltar que o usuário ativo (login) pode possuir restrições a determinadas opções do menu, em função do perfil associado a este usuário, determinado pela organização a qual o usuário está associado. Desta forma, serão listados os atalhos correspondentes ao perfil do usuário que terá permissão de acessar.


   2. Solicitação de Nova Senha
Caso o usuário não lembre dos seus dados para efetuar o login na Plataforma do uCloud, ela permite recuperar a senha de acesso durante o processo do login ou caso o usuário receba a mensagem no canto superior da tela com um aviso pop-up  “Usuário ou senha incorretos” conforme a figura abaixo:
  

Usuário ou senha incorretos


O usuário deverá clicar com o cursor do mouse sobre a opção “Esqueceu sua Senha?” conforme o detalhe na figura abaixo:
  
  

Figura 1 Acesso ao portal Intercloud


Caso as informações de login do usuário existam, mas se o mesmo necessitar inserir nova senha, a Plataforma do uCloud apresentará ao usuário o formulário para alteração.
  



No primeiro campo, o usuário informa o endereço de e-mail que está registrado e no segundo campo ele deve preencher com a informação de login do usuário que foi provisionado na Plataforma do uCloud.
Após informar uma conta de e-mail e usuário válidos para acesso, o usuário deve clicar com o cursor do mouse no botão verde Editar, a interface apresentará a mensagem a seguir:
  

Alterar senha
O usuário deverá verificar o recebimento de uma mensagem em sua caixa postal de e-mail com as instruções para redefinição da senha. O usuário deverá proceder como descrito no e-mail e redefinir a sua senha de acesso.
  

É necessário checar se o domínio “@ucloud.usto.re” está bloqueado na sua lista de mensagens indesejadas (spam) para permitir o recebimento dela.
Quando o usuário clicar com o cursor do mouse sobre o link/url presente no seu e-mail, este será levado para uma sessão do seu navegador (browser) de Internet conectado na Plataforma do uCloud, a tela abaixo será apresentada:
  



Após o usuário informar a nova sequência de caracteres no campo Nova Senha, o mesmo deverá informá-la novamente no campo seguinte Confirmar Senha igual a informada no campo anterior.
Após confirmar a nova senha o usuário deve clicar com o cursor do mouse no botão Salvar, a interface apresentará a seguinte mensagem:
  

Alterar senha
Após este procedimento o usuário poderá efetuar o processo de login utilizando as informações de usuário e a nova senha. A nova senha estará disponível de forma imediata, não sendo necessário aguardar nenhum período para a efetivação dela.
   3. Usuário não provisionado
Caso a informação de login do usuário não tenha sido previamente cadastrada ou a combinação de e-mail e dados de login, a Plataforma do uCloud apresentará uma mensagem pop-up - no canto superior direito da tela - com a informação de que os dados informados para alteração da senha não existam na Plataforma do uCloud.
  



Neste caso, basta entrar em contato com o Administrador da Plataforma do uCloud da sua organização para que ele possa efetuar o provisionamento dos seus dados para o login.
Somente um usuário devidamente provisionado terá seu acesso efetivado.

