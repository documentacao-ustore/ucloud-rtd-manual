uCloud - Manual do Adminstrador
+++++++++++++++++++++++++++++++

Passo a passo provisionamento de Novos Clientes na Plataforma uCloud.

Apresentamos as melhores Práticas para o correto provisionamento de Usuários, Grupos, Contratos, VDCs, Container, Billing Settings e Casos de Uso.

Este documento tem como objetivo explicar as tarefas associadas ao perfil de Administrador da Plataforma “uCloud”, uma plataforma de *Cloud Service Broker* (broker de serviços em nuvem) que permite gerenciar múltiplos provedores de serviços de nuvem, tanto privados quanto provedores de nuvem pública.

Neste documento são apresentados as ações e configurações que são específicas do usuário com perfil  ”Administrador da Plataforma - Administrador do Sistema”. Este perfil possui capacidades de provisionamento diferentes de todos os outros perfis de usuários.

.. important::
  Importante ressaltar que algumas das ações descritas neste manual serão efetuadas somente uma única vez, e a correção de algum parâmetro pode gerar erros em algumas (ou todas) ações executadas pelo usuário final na Plataforma do uCloud.

Apreciamos seu *feedback* com o relato de sua experiência de uso da nossa aplicação, se tiver algo a nos sugerir, favor enviar correio eletrônico na caixa de correio: manual@usto.re.



Introdução
==========

Neste documento seguem as atividades iniciais que devem ser executadas por profissionais (funcionários) do integrador (Embratel, Claro Brasil, Telmex, etc) quando houver a necessidade de provisionar um novo *cliente/empresa* que irá necessitar conectar em três diferentes provedores denuvem pública (por ex.: AWS, Azure, Google).

As atividades para todas as etapas, devem ser efetuadas por um usuário da organização do integrador, e que tenha o perfil de Administrador (apenas como exemplo perfil: “Admin/Admin). Este deve iniciar uma sessão na Plataforma do uCloud e provisionar um novo usuário. Na tela de inclusão de usuários deve selecionar no campo **Perfil de Usuários** a opção **Administrador**, para representar este novo cliente, ou empresa, ao qual o novo usuário ficará vinculado e será utilizado para todas as configurações referentes ao(s) provedor(es) de serviço de nuvem pública.


Primeira Etapa: Criação do Usuário (perfil Administrador)
---------------------------------------------------------
Criar usuário com perfil *Administrador* que será responsável por conectar os containers e configurar *Billing Settings (Bucket)*, criar Grupo, VDC e Contrato.

Esse usuário não será um usuário normal que deve ser utilizado para provisionar recursos computacionais na(s) nuvem(ns) do(s) provedores de serviço, pois ele é uma abstração das nuvens conectadas.

Importante colocar nome de identificação da nuvem e deixar claro que esse é o usuário de conexão (abstrato).

Seguido o seguinte formato: *Nome_do_ClienteAdminSistema[Provedor]*.

Abaixo listamos exemplos de padronização para a criação de usuários na Plataforma do uCloud, e ressaltamos que são meros exemplos  ilustrativos, mas usaremos estes exemplos para ilustrar os todas os processos de cada etapa deste docuento.

- No caso **AWS** Exemplo de usuário: *Cliente1AdminSistemaAWS*.
- No caso **Azure** Exemplo de usuário: *Cliente1AdminSistemaAzure*.
- No caso **Google** Exemplo de usuário: *Cliente1AdminSistemaGCP*.
- No caso **Huawei** Exemplo de usuário: *Cliente1AdminSistemaHuawei*.


* **Perfil do Usuário**: *Este campo é obrigatório*, trata-se de um campo do tipo “drop down list”, quando o usuário clicar sobre este será apresentada a lista com três opções:
  
  * Selecionar opção: **Administrador**.
  
* **Grupo**: *Este campo é obrigatório* e o usuário deve informar um grupo previamente provisionado na Plataforma do uCloud, pois não será possível continuar o cadastramento de um usuário sem vincular este novo usuário a um grupo existente.
  * Pode-se informar parte do nome de um grupo e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo:

.. note:: Importante ressaltar que esta etapa é temporária, posteriormente este novo usuário será vinculado a outro Grupo, portanto informar e selecionar o Grupo **Admins**.

* **Nome**: *Este campo é obrigatório* e deve ser preenchido com o nome do usuário que se está provisionando.

* **Login**: *Este campo é obrigatório* e deve ser preenchido com a sequência de caracteres que será utilizada para identificar o usuário durante o processo de login no uCloud. O usuário do integrador deverá seguir a padronização e uniformização citada acima:

  * **Login para AWS Informar**: Cliente1AdminSistemaAWS
  * **Login para Azure Informar**: Cliente1AdminSistemaAzure
  * **Login para GCP Informar**: Cliente1AdminSistemaGCP
  * **Login para Huaewi Informar**: Cliente1AdminSistema**Huawei

* **Senha**: Este campo é obrigatório e deve ser preenchido com a sequência de caracteres da senha do usuário. Esta sequência de caracteres deve ser maior do que quatro (04) caracteres alfanuméricos. Deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”. A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres e deve conter caracteres de três das seguintes categorias:

  * Letras maiúsculas e minúsculas (A a Z) somente ASCII básico NÃO USAR caracteres acentuados!
  * Números de base 10 (de 0 a 9)
  * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' &lt;>,.? /) – *Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política.*

* **Confirmar Senha**: *Este campo é obrigatório* e deve ser preenchido com a mesma sequência de caracteres informados no campo anterior. Caso a sequência informada neste campo seja diferente da anterior, será apresentado um ``pop-up`` com uma mensagem de erro na tela.

* **Email**: *Este campo é obrigatório*, nele deve ser informado um endereço de correio eletrônico (e-mail) válido. Este endereço de correio eletrônico será fundamental durante o processo de redefinição de senha pelo usuário, pois a Plataforma do uCloud utiliza este e-mail para o envio de uma mensagem que permite ao usuário criar uma senha, para ele, de forma automática.

.. attention:: Importante ressaltar que a Plataforma do uCloud não efetua qualquer validação prévia referente a existência do e-mail informado ou seu efetivo funcionamento. No caso de inexistência do e-mail destino, ou erro em sua digitação, o usuário ficará impossibilitado de executar a redefinição da sua senha de acesso. Neste caso deverá contactar o administrador do seu grupo/contrato.

* **Telefone**: *Este campo é obrigatório*, e deve ser preenchido com um número de telefone de serviço móvel celular, utilizar o seguinte formato:

  * **dois (02)** números que identificam o código de área do número de telefone de serviço móvel celular (XX). *Não é necessário informar o número ``zero (0)`` que antecede ao código de área no padrão brasileiro*.
  * **nove (09)** números que identificam o número de telefone do serviço móvel celular do usuário. Não é necessário informar qualquer outro caractere para separação dos grupos de números de telefone serviço móvel celular.
  * Exemplo de preenchimento: ``11999991234``

* **Cargo**: *Este campo é obrigatório*, mas é meramente informativo para identificar o cargo do usuário que se deseja provisionar.
* **Empresa**: *Este campo é obrigatório*, mas é meramente informativo para identificar a organização a qual este usuário está associado.
* **Tipo de Cota**: *Este campo é obrigatório*, trata-se de um campo do tipo “_drop down list_”, quando o usuário clicar sobre este será apresentada a lista das opções de tipos de cota disponíveis para provisionar um usuário, veja as opções abaixo:
  
  * **Cota de Grupo**: Quando selecionada esta opção o usuário compartilha dos limites (cotas) financeiros ou de recursos computacionais que estão definidos nas configurações do Grupo. Usuários com cota de grupo devem ficar atentos nas informações apresentadas na tela inicial (**Dashboard**) uma vez que a Plataforma do uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites disponíveis no grupo ao qual o usuário está vinculado.
  
    * Selecionar: **Cota de Grupo**

  * **Cota de Usuário**: Quando selecionada esta opção pelo usuário, a Plataforma do uCloud solicita que sejam informados os limites (cotas) financeiros ou de recursos computacionais específicos e individuais para este usuário, conforme a tela abaixo:
  
  * **Cota de CPU**: *Este campo é obrigatório* e deve ser informado um número inteiro que representa o limite máximo de consumo do recurso computacional de CPUs para todas as máquinas virtuais criadas nos provedores de serviço de nuvem (público e/ou privado), por este usuário.
  
  * **Cota de Faturamento**: Este campo é opcional e deve ser informado um número inteiro que será estabelecido como limite máximo referente aos valores financeiros dos custos de consumo dos recursos computacionais para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado).
  
  * **Cota de Memória**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Memória para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado). Pode ser selecionado o limite em **Gigabytes** ou um limite em **Terabytes**.
  
  * **Cota de Disco**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Disco para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado). Pode ser selecionado o limite em **Gigabytes** ou um limite em **Terabytes**.
  
  * **Cota de IPs Públicos**: Este campo é obrigatório e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de IPs Públicos para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado).
    
.. note:: Para usuários com cotas individuais: esta cota individual será subtraída (retirada) da cota do Grupo ao qual este usuário está vinculado. Em outras palavras, os usuários sem cota individual podem consumir a cota definida no Grupo; quando definida uma cota para um usuário, uma parte da cota do Grupo é alocada para o usuário, esta parte da cota do Grupo não será acessível a outros usuários do Grupo.

Quando um usuário se registra, ele deve observar as informações apresentadas na tela inicial (**Dashboard**) pois a Plataforma do uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites definidos para este usuário.

* **Ativar Autenticação Multifator**: Este campo é um campo de seleção “*check box*” que indica se este usuário terá seu processo de autenticação na plataforma (login) sendo verificado duplamente antes de aprovar que este usuário tenha acesso a Plataforma do uCloud. Será enviada uma mensagem para o número de telefone do serviço móvel de celular.

  * **Não selecionar este “check box” - Manter em BRANCO**
  
* **Ativar cota de Faturamento**: Este campo é um campo de seleção “*check box*” que indica se este usuário terá seu faturamento computado constantemente na relação de consumo de Faturamento (ver item Financeiro).

  * **Não selecionar este “check box” - Manter em BRANCO**

* **Administrador precisa aprovar a realização de atividades**: Este campo é um campo de seleção "*check box*" que indica todas as ações e solicitações efetuadas na interface da Plataforma do uCloud, elas devem ser aprovadas por um usuário Administrador do Grupo. Esta é uma funcionalidade destinada a aumentar o controle de governança de custos e operações.

  * **Não selecionar este “check box” - Manter em BRANCO**

* **Criar Usuário na Nuvem**: Este campo é um campo de seleção "_checkbox_" que indica as credenciais de login e senha deste usuário (informadas acima), elas serão enviadas ao provedor de serviço de nuvem pública para que seja provisionado um usuário com as mesmas credenciais de acesso no provedor de serviço de nuvem pública selecionado abaixo.

  * **Não selecionar este “check box” - Manter em BRANCO**

* **Permissões**: O usuário recebe/herda todas as permissões definidas no Grupo ao qual ele pertence, bem como as permissões estabelecidas no Contrato e por último as permissões específicas deste usuário. Esta tabela é opcional, ela permite adicionar ou revogar as permissões que este usuário recebe, o que permite efetuar ações ou acessar menus na Plataforma do uCloud. São cento e trinta e duas (132) permissões disponíveis que podem ser associadas ao usuário (todas ou apenas uma parte). Qualquer alteração efetuada nas permissões disponíveis (inclusão ou revogação) será aplicada de forma imediata no login deste usuário após a confirmação. Veja o item Configurações / Perfis de Permissionamento para uma forma alternativa de criar grupos de permissões customizados para sua empresa.

* **Botão Cancelar**: O usuário pode usar este botão para cancelar o processo de criação de um Usuário. A Plataforma do uCloud encerra a tela e retorna à tela anterior.

* **Botão Criar**: Após todos os campos obrigatórios e opcionais para provisionar o novo usuário estarem preenchidos o usuário pode clicar com o cursor do mouse no botão verde **Criar,** assim a Plataforma do uCloud provisiona o novo usuário em suas bases de dados internas. Caso o botão **Criar** não seja apresentado na cor verde, significa que algum campo obrigatório permanece sem preenchimento (o usuário deve checar e corrigir) ou a sequência de caracteres da senha do login deve ser inferior a quatro (04) caracteres.

Após o provisionamento do(s) usuário(s) para o novo cliente, o profissional do integrador deve encerrar a sessão com a sua credencial na Plataforma do uCloud, e efetuar o login de uma nova sessão com as credenciais recém criadas acima e seguir as etapas abaixo.

Após a criação do(s) usuário(s) acima, o operador deve encerrar a sessão com o seu login e senha do integrador.

Neste ponto o usuário do integrador deve iniciar uma nova sessão na Plataforma do uCloud, mas utilizando as informações de login/senha das novas credenciais criadas (usuário e senha) definidos para a credencial (exemplo ``Cliente1AdminSistemaAWS``). 

Importante ressaltar que o usuário do integrador deverá efetuar todos os procedimentos descritos nas etapas abaixo, com uma sessão ativa com a credencial acima criada.


Segunda Etapa: Conectar Container de Provedor de Nuvem Pública
--------------------------------------------------------------

Neste ponto é fundamental que o profissional do integrador deva ter em mãos a informação referente a credencial de acesso de usuário programático (Programmatic User/Access) que contenha as informações específicas de cada provedor -- Entre em contato com a equipe técnica da Ustore para obter o documento que descreve o passo a passo para criação de usuário programático para cada provedor de serviço de nuvem pública.

Apenas como exemplo ilustrativo, iremos iniciar a descrição dos procedimentos de um novo cliente com as informações referentes ao provedor de serviço AWS (Amazon Web Service).

Caso o cliente em questão deseja adicionar mais de um ambiente de provedor de serviço de nuvem pública, deve-se repetir os passos conforme descritos ao final deste documento

O profissional do integrador deve acessar o menu Container,  selecionar o botão “Conectar Container”, clicar com o cursor do mouse sobre o campo Tipo de Container e selecionar a opção AWS. Preencher os dados conforme os campos da tela abaixo:
* Tipo de Container: Este campo é obrigatório, trata-se de um campo do tipo “drop down list”, quando o usuário clicar sobre este será apresentada a lista das opções de tipos provedores (públicos e privados) que são suportados pela Plataforma do uCloud.
   * Selecionar a opção: **AWS**

* Nome do Container: Este campo é obrigatório e deve ser informado o nome com o qual deseja identificar este container :
   * Informar (*como exemplo*): **Cliente1AWS**

* Access Key: Este campo é obrigatório e deve ser preenchido com a informação específica referente a credencial de acesso programático que foi criada diretamente na console da AWS para esta finalidade. Importante ressaltar que o conjunto de Access Key, só pode ser utilizado uma única tentativa, em caso de erro de digitação o conjunto de informações ficará invalidado e outra credencial de acesso programático deverá ser provisionada na console da AWS.

* Secret Key: Este campo é obrigatório e deve ser preenchido com a informação específica referente a credencial de acesso programático que foi criada diretamente na console da AWS para esta finalidade. Importante ressaltar que o conjunto de Secret Key, só pode ser utilizado uma única tentativa, em caso de erro de digitação o conjunto de informações ficará invalidado e outra credencial de acesso programático deverá ser provisionada na console da AWS.

* Importar sem recursos: Este botão é opcional e alternar este botão para o modo ATIVO indica para a Plataforma do uCloud que o processo de conexão a esta credencial da AWS deve sincronizar e importar o inventário completo de todos os recursos computacionais existentes no ambiente da AWS.
Manter este botão no modo NÃO ATIVO significa que a Plataforma do uCloud irá somente se conectar aos dados de faturamento e billing desta credencial. Significa que a empresa optou por não efetuar a operação dos recursos computacionais existentes na AWS através da interface da Plataforma do uCloud.
   * Não selecionar este “check box” - Manter em BRANCO

.. important:
	Importante esclarecer que devem ser concedidas/vinculadas certas permissões de acesso aos recursos computacionais ao usuário programático utilizado neste processo. de acesso de forma que seja possível ‘importar’ todos os recursos computacionais existentes no provedor (ex.: AWS). Se este usuário programático, não possuir estas permissões, a Plataforma do uCloud não irá apresentar nenhum recurso computacional existente neste provedor de serviço de nuvem pública (ex.: AWS). Entre em contato com a equipe técnica da Ustore para obter o documento que descreve o passo a passo para criação de usuário programático para cada provedor de serviço de nuvem pública.

	   * Atrelar Container ao VDC: Este botão é opcional e alternar este botão para o modo ATIVO indica para a Plataforma do uCloud que o processo de conexão a esta credencial da AWS vincular este ambiente a um Virtual Datacenter (VDC) previamente provisionado no ambiente da Plataforma do uCloud.
   * Não selecionar este “check box” - Manter em BRANCO
   * Botão Baixar Demo JSON: Este botão é opcional, e pode ser utilizado para efetuar o download de um arquivo JSON de demonstração, com suas informações em branco, e pode ser utilizado como um exemplo para automatizar o processo de criação de outras credenciais da AWS.
   * Botão Importar JSON: Este botão é opcional, e pode ser utilizado para efetuar a carga upload de um arquivo JSON personalizado com as informações das credenciais de acesso programático referente a AWS de forma automática.
   * Botão Conectar e Importar VMs: Este botão é opcional, e pode ser utilizado para iniciar o processo de conexão deste Container e importar todas as máquinas virtuais (Virtual Machines - VMs) que existem no ambiente da credencial da AWS. Ao clicar com o mouse sobre este botão significa que o usuário optou por controlar os valores financeiros (Billing) e operar os recursos computacionais desta credencial da AWS através da Plataforma do uCloud.
   * Botão Conectar:  Após o usuário informar todos os parâmetros fundamentais para a criação do Container da credencial Amazon AWS, o usuário irá notar que este botão alterna para o modo ativo (verde). Basta clicar com o cursor do mouse sobre o botão Criar, para que a Plataforma do uCloud inicie o provisionamento e conexão deste Container AWS.
Caso este botão não esteja habilitado (cinza), significa que algum parâmetro anterior deixou de ser atendido ou algum campo está em branco, a Plataforma do uCloud não permitirá o provisionamento deste Container AWS.
   * Botão Cancelar:  O usuário pode usar este botão para cancelar o processo de criação de um Container AWS. A Plataforma do uCloud encerra a tela e retorna à tela anterior.


      1. Configurar Billing


Neste ponto é fundamental que o profissional do integrador deva ter em mãos a informação referente ao acesso às informações referentes do billing (ou bucket) desta credencial AWS - Veja o documento da Ustore sobre o passo a passo para criação de usuário programático para cada provedor de serviço de nuvem pública. Sem o correto acesso e a informação do nome do arquivo de Billing, não será possível efetuar a configuração referente ao acesso ao Billing da AWS.


Acessar o menu  Container, e selecionar o Container recém provisionado no processo acima, a Plataforma do uCloud irá apresentar uma tela com várias seções, veja na Seção Geral o campo:
  

Imagem 3 - Tela NOVA de Billing AWS


      * Configurações do Financeiro: Deve-se clicar com o cursor do mouse sobre o Ícone Edição   para a Plataforma do uCloud apresentar uma tela que permite editar as configurações do Billing AWS, conforme tela abaixo:
  

Imagem 4 - Tela NOVA de Billing AWS
         * Source: Este campo é obrigatório, trata-se de um campo do tipo “drop down list”, quando o usuário clicar sobre este será apresentada a lista das opções dos tipos que são suportados pela Plataforma do uCloud.
         * Selecionar a opção Cost and Usage Reports (CUR).
         * Bucket: Este campo é obrigatório e o usuário deve informar o nome do arquivo de billing (bucket) que foi provisionado na console da AWS. Veja o documento da Ustore sobre o passo a passo para criação de usuário programático para cada provedor de serviço de nuvem pública.
         * CUR: Este campo é obrigatório e o usuário deve informar o nome do arquivo de billing (bucket) que foi provisionado na console da AWS.
         * Região: Este campo é obrigatório, trata-se de um campo do tipo “drop down list”, quando o usuário clicar sobre este será apresentada a lista de todas as regiões globais da AWS. Deve ser selecionada a região global ao qual o arquivo de billing do cliente foi vinculado.
         * Botão Habilitar Impostos: Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que seja apresentados de forma EXPLÍCITA os valores de Billing AWS, esta opção permite identificar (segregar) os valores referentes às taxas dos impostos de cada um dos recursos computacionais de nuvem AWS dos relatórios financeiros da Plataforma do uCloud.[b]
         * Botão Habilitar Créditos:  Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que seja apresentados de forma EXPLÍCITA os valores dos créditos de valores de Billing AWS, esta opção permite identificar (segregar) os valores referentes créditos que foram adicionados a cada um dos recursos computacionais de nuvem AWS dos relatórios financeiros da Plataforma do uCloud.[c]
         * Botão Habilitar Descontos SavingsPlan: Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que seja apresentados de forma EXPLÍCITA os valores dos créditos de valores de Billing AWS, esta opção permite identificar (segregar) os valores referentes créditos que foram adicionados [d]a cada um dos recursos computacionais de nuvem AWS dos relatórios financeiros da Plataforma do uCloud.
         * Botão Habilitar Descontos Instância Reservada: Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que seja apresentados de forma EXPLÍCITA os valores dos créditos de valores de Billing AWS, esta opção permite identificar (segregar) os valores referentes créditos que foram adicionados a[e] cada um dos recursos computacionais de nuvem AWS dos relatórios financeiros da Plataforma do uCloud.
         * Botão Buscar em Outra Conta: Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que os valores de Billing deste Container sejam obtidos de outra credencial de Container AWS que tenha sido previamente provisionado na Plataforma do uCloud e que esta credencial de usuário possua acesso.[f]
         * Botão Salvar:  Após o usuário informar todos os parâmetros fundamentais para a criação do Billing AWS o usuário irá notar que este botão alterna para o modo ativo (verde). Basta clicar com o cursor do mouse sobre o botão Salvar, para que a Plataforma do uCloud inicie o provisionamento e do Billing AWS.
Caso este botão não esteja habilitado (cinza), significa que algum parâmetro anterior deixou de ser atendido ou algum campo está em branco, a Plataforma do uCloud não permitirá o provisionamento deste Billing AWS.
         * Botão Cancelar:  O usuário pode usar este botão para cancelar o processo de criação de um Billing AWS. A Plataforma do uCloud encerra a tela e retorna à tela anterior.
  

Imagem 3b - Tela antiga de Billing AWS





Terceira Etapa: Criar Contrato
------------------------------


O que é Contrato para a Plataforma do uCloud
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Conferência e Validação das informações Comerciais do Contrato
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Quarta Etapa: Criar Grupo
-------------------------


Quinta Etapa: Criar um VDC
--------------------------


Sexta Etapa: Conectar VDC ao Contrato
-------------------------------------


Sétima Etapa: Validação do ambiente e suas vinculações
------------------------------------------------------


Para conectar a nuvem Azure
~~~~~~~~~~~~~~~~~~~~~~~~~~~


Para conectar a nuvem GCP (Google)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Para conectar a nuvem Huawei
~~~~~~~~~~~~~~~~~~~~~~~~~~~~


Casos de Uso
============
Caso de Uso: Contrato Isolado para cada Provedor de Nuvem diferente
-------------------------------------------------------------------
