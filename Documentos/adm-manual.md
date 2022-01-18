## Passo a passo provisionamento de Novos Clientes na Plataforma uCloud.


### Padronização e Melhores Práticas para a correta criação de Usuários, Grupos, Contratos, VDCs, Container, Billing Settings e Casos de Uso.



#### **Apresentação**

Este documento tem como objetivo explicar as tarefas associadas ao perfil de Administrador da Plataforma “uCloud”, uma plataforma de _Cloud Service Broker_ (broker de serviços em nuvem) que permite gerenciar múltiplos provedores de serviços de nuvem, tanto privados quanto provedores de nuvem pública.

Neste documento são apresentados as ações e configurações que são específicas do usuário com perfil  ”Administrador da Plataforma - Administrador do Sistema”. Este perfil possui capacidades de provisionamento diferentes de todos os outros perfis de usuários.

Importante ressaltar que algumas das ações descritas neste manual serão efetuadas somente uma única vez, e a correção de algum parâmetro pode .

Apreciamos o _feedback_ com o seu relato de experiência de uso da nossa aplicação, se tiver algo a nos sugerir, favor enviar correio eletrônico, o endereço encontra-se na página anterior.


## Introdução

Neste documento seguem as atividades iniciais que devem ser executadas por profissionais (funcionários) do integrador (Serpro, Embratel, Telmex, etc) quando houver a necessidade de provisionar um novo cliente/empresa que irá necessitar conectar 3 nuvens. AWS, Azure, Google (GCP).

As atividades para todas as etapas, devem ser efetuadas por um usuário da organização do integrador, e que tenha o perfil de Administrador (apenas como exemplo perfil: “Admin/Admin). Este deve iniciar uma sessão na Plataforma do uCloud e provisionar um novo usuário. Na tela de inclusão de usuários deve selecionar no campo <strong>Perfil de Usuários </strong>a opção “<strong>Administrador</strong>”, para representar este novo cliente, ou empresa, ao qual o novo usuário ficará vinculado e será utilizado para todas as configurações referentes ao(s) provedor(es) de serviço de nuvem pública.

### **Primeira Etapa**: Criação do Usuário (perfil Administrador)

Criar usuário com perfil _Administrador_ que será responsável por conectar os containers e configurar _Billing Settings (Bucket)_, criar Grupo, VDC e Contrato. Veja a figura com o exemplo da tela abaixo (Imagem 1).

Esse usuário não será um usuário normal que deve ser utilizado para provisionar recursos computacionais na(s) nuvem(ns) do(s) provedores de serviço, pois ele é uma abstração das nuvens conectadas.

Importante colocar nome de identificação da nuvem e deixar claro que esse é o usuário de conexão (abstrato).

Seguido o seguinte formato: _&lt;Nome_do_Cliente>**Admin<span style="text-decoration:underline;">Sistema[Provedor]</span>**_.

Abaixo listamos exemplos de padronização para a criação de usuários na Plataforma do uCloud, e ressaltamos que são meros exemplos  ilustrativos, mas usaremos estes exemplos para ilustrar os todas os processos de cada etapa deste docuento.



* No caso AWS Exemplo de usuário: _Cliente1**Admin**Sistema**AWS**_
* No caso Azure Exemplo de usuário: _Cliente1**Admin<span style="text-decoration:underline;">SistemaAzure</span>**_.
* No caso Google Exemplo de usuário: _Cliente1**Admin<span style="text-decoration:underline;">SistemaGCP</span>**_.
* No caso Huawei Exemplo de usuário: _Cliente1**Admin<span style="text-decoration:underline;">SistemaHuawei</span>**_.






![alt_text](images/image1.png "image_tooltip")


_Imagem 1 - Criação de Usuário Administrador_



* **Perfil do Usuário**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, trata-se de um campo do tipo “_drop down list_”, quando o usuário clicar sobre este será apresentada a lista com três opções:
    * Selecionar opção: **<span style="text-decoration:underline;">Administrador</span>**.
* **Grupo**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar um grupo previamente provisionado na Plataforma do uCloud, pois não será possível continuar o cadastramento de um usuário sem vincular este novo usuário a um grupo existente.
    * Pode-se informar parte do nome de um grupo e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo:



<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image2.png "image_tooltip")




    * _<span style="text-decoration:underline;">Importante ressaltar que esta etapa é temporária, posteriormente este novo usuário será vinculado a outro Grupo, portanto informar e selecionar o Grupo “**Admins**”.</span>_
* **Nome**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com o nome do usuário que se está provisionando.
* **Login**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com a sequência de caracteres que será utilizada para identificar o usuário durante o processo de login no uCloud.  O usuário do integrador deverá seguir a padronização e uniformização citada acima:
    * **Login para AWS Informar**: _<span style="text-decoration:underline;">Cliente1**Admin**Sistema**AWS**</span>_
    * **Login para Azure Informar**: _<span style="text-decoration:underline;">Cliente1**Admin**Sistema**Azure**</span>_
    * **Login para GCP Informar**: _<span style="text-decoration:underline;">Cliente1**Admin**Sistema**GCP**</span>_
    * **Login para Huaewi Informar**: _<span style="text-decoration:underline;">Cliente1**Admin**Sistema**Huawei**</span>_
* **Senha**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com a sequência de caracteres da senha do usuário. Importante ressaltar que esta sequência deve ser maior do que quatro (04) caracteres alfanuméricos. Deve seguir a recomendação de uso de senhas “fortes e de alta complexidade”. _<span style="text-decoration:underline;">A recomendação é de no mínimo oito (08) e no máximo setenta e dois (72) caracteres e deve conter caracteres de três das seguintes categorias:</span>_
    * Letras maiúsculas e minúsculas (A a Z)
    * Números de base 10 (de 0 a 9)
    * Caracteres não alfanuméricos (caracteres especiais): (~! @ # $% ^& * -+ = ' | \ \ () {} \ []:; "' &lt;>,.? /) – _Importante ressaltar que símbolos de moeda como o euro ou a libra britânica não são contados como caracteres especiais para essa configuração de política._
* **Confirmar** **Senha**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com a mesma sequência de caracteres informados no campo anterior. Caso a sequência informada neste campo seja diferente da anterior, será apresentado um _pop-up_ com uma mensagem de erro na tela.



<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image3.png "image_tooltip")




* **Email**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, nele deve ser informado um endereço de correio eletrônico (e-mail) válido. Este endereço de correio eletrônico será fundamental durante o processo de redefinição de senha pelo usuário, pois a Plataforma do uCloud utiliza este e-mail para o envio de uma mensagem que permite ao usuário criar uma senha, para ele, de forma automática.

<table>
  <tr>
   <td>
<strong>✋</strong>
<p>
<strong>Atenção</strong>
   </td>
   <td><em>Importante ressaltar que a Plataforma do uCloud não efetua qualquer validação prévia referente a existência do e-mail informado ou seu efetivo funcionamento. No caso de inexistência do e-mail destino, ou erro em sua digitação, o usuário ficará impossibilitado de executar a redefinição da sua senha de acesso. Neste caso deverá contactar o administrador do seu grupo/contrato.</em>
   </td>
  </tr>
</table>




* **Telefone**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, e deve ser preenchido com um número de telefone de serviço móvel celular, utilizar o seguinte formato:
    * dois (02) números que identificam o código de área do número de telefone de serviço móvel celular (XX). _Não é necessário informar o número ‘zero (0)’ que antecede ao código de área no padrão brasileiro_.
    * nove (09) números que identificam o número de telefone do serviço móvel celular do usuário. Não é necessário informar qualquer outro caractere para separação dos grupos de números de telefone serviço móvel celular.
    * Exemplo de preenchimento: **11999991234**
* **Cargo**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, mas é meramente informativo para identificar o cargo do usuário que se deseja provisionar.
* **Empresa**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, mas é meramente informativo para identificar a organização a qual este usuário está associado.
* **Tipo de Cota**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, trata-se de um campo do tipo “_drop down list_”, quando o usuário clicar sobre este será apresentada a lista das opções de tipos de cota disponíveis para provisionar um usuário, veja as opções abaixo:



<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image4.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image4.png "image_tooltip")

* **Cota de Grupo**: Quando selecionada esta opção o usuário compartilha dos limites (cotas) financeiros ou de recursos computacionais que estão definidos nas configurações do Grupo. Usuários com cota de grupo devem ficar atentos nas informações apresentadas na tela inicial (_dashboard_ – veja item **Dashboard**) uma vez que a Plataforma do uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites disponíveis no grupo ao qual o usuário está vinculado.
  * Selecionar: **Cota de Grupo**
* **Cota de Usuário**: Quando selecionada esta opção pelo usuário, a Plataforma do uCloud solicita que sejam informados os limites (cotas) financeiros ou de recursos computacionais específicos e individuais para este usuário, conforme a tela abaixo:



<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image5.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image5.png "image_tooltip")

* **Cota de CPU**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser informado um número inteiro que representa o limite máximo de consumo do recurso computacional de CPUs para todas as máquinas virtuais criadas nos provedores de serviço de nuvem (público e/ou privado), por este usuário.
  * **Cota de Faturamento**: Este campo é _opcional_ e deve ser informado um número inteiro que será estabelecido como limite máximo referente aos valores financeiros dos custos de consumo dos recursos computacionais para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado).
  * **Cota de Memória**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Memória para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado). Pode ser selecionado o limite em **Gigabytes** ou um limite em **Terabytes**.
  * **Cota de Disco**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de Disco para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado). Pode ser selecionado o limite em **Gigabytes** ou um limite em **Terabytes**.
    * **Cota de IPs Públicos**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser informado um número inteiro que será estabelecido como limite máximo de consumo do recurso computacional de IPs Públicos para todas as máquinas virtuais criadas, por este usuário, nos provedores de serviço de nuvem (público e/ou privado).
    
.. note:: _Importante ressaltar que os usuários com cotas individuais: esta cota individual será subtraída (retirada) da cota do Grupo ao qual este usuário está vinculado_.
>  Em outras palavras, os usuários sem cota individual podem consumir a cota definida no Grupo; quando definida uma cota para um usuário, uma parte da cota do Grupo é alocada para o usuário, esta parte da cota do Grupo não será acessível a outros usuários do Grupo.


        Quando um usuário se registra, ele deve observar as informações apresentadas na tela inicial (_dashboard_ – veja item **Dashboard** na página ) pois a Plataforma do uCloud nega a criação de quaisquer recursos computacionais ou consumo de valores financeiros que ultrapassem os limites definidos para este usuário.

* **Ativar Autenticação Multifator**: Este campo é um campo de seleção “_check box_” que indica se este usuário terá seu processo de autenticação na plataforma (login) sendo verificado duplamente antes de aprovar que este usuário tenha acesso a Plataforma do uCloud. Será enviada uma mensagem para o número de telefone do serviço móvel de celular.
    * **Não selecionar este “check box” - Manter em BRANCO**
* **Ativar cota de Faturamento**: Este campo é um campo de seleção “_check box_” que indica se este usuário terá seu faturamento computado constantemente na relação de consumo de Faturamento (ver item Financeiro).
    * **Não selecionar este “check box” - Manter em BRANCO**
* **Administrador precisa aprovar a realização de atividades**: Este campo é um campo de seleção "checkbox" que indica todas as ações e solicitações efetuadas na interface da Plataforma do uCloud, elas devem ser aprovadas por um usuário Administrador do Grupo. Esta é uma funcionalidade destinada a aumentar o controle de governança de custos e operações.
    * **Não selecionar este “check box” - Manter em BRANCO**
* **Criar Usuário na Nuvem**: Este campo é um campo de seleção "_checkbox_" que indica as credenciais de login e senha deste usuário (informadas acima), elas serão enviadas ao provedor de serviço de nuvem pública para que seja provisionado um usuário com as mesmas credenciais de acesso no provedor de serviço de nuvem pública selecionado abaixo.
    * **Não selecionar este “check box” - Manter em BRANCO**
* **Permissões**: O usuário recebe/herda todas as permissões definidas no Grupo ao qual ele pertence, bem como as permissões estabelecidas no Contrato e por último as permissões específicas deste usuário. Esta tabela é opcional, ela permite adicionar ou revogar as permissões que este usuário recebe, o que permite efetuar ações ou acessar menus na Plataforma do uCloud. São cento e trinta e duas (132) permissões disponíveis que podem ser associadas ao usuário (todas ou apenas uma parte). Qualquer alteração efetuada nas permissões disponíveis (inclusão ou revogação) será aplicada de forma imediata no login deste usuário após a confirmação. Veja o item Configurações / Perfis de Permissionamento para uma forma alternativa de criar grupos de permissões customizados para sua empresa.
* **Botão Cancelar: ** O usuário pode usar este botão para cancelar o processo de criação de um Usuário. A Plataforma do uCloud encerra a tela e retorna à tela anterior.
* **Botão Criar**: Após todos os campos obrigatórios e opcionais para provisionar o novo usuário estarem preenchidos o usuário pode clicar com o cursor do mouse no botão verde **Criar,** assim a Plataforma do uCloud provisiona o novo usuário em suas bases de dados internas. Caso o botão **Criar** não seja apresentado na cor verde, significa que algum campo obrigatório permanece sem preenchimento (o usuário deve checar e corrigir) ou a sequência de caracteres da senha do login deve ser inferior a quatro (04) caracteres.

Após o provisionamento do(s) usuário(s) para o novo cliente, o profissional do integrador deve encerrar a sessão com a sua credencial na Plataforma do uCloud, e efetuar o login de uma nova sessão com as credenciais recém criadas acima e seguir as etapas abaixo.

Após a criação do(s) usuário(s) acima, o operador deve encerrar a sessão com o seu login e senha do integrador.

Neste ponto o usuário do integrador deve iniciar uma nova sessão na Plataforma do uCloud, mas utilizando as informações de login/senha das novas credenciais criadas (usuário e senha) definidos para a credencial (exemplo **Cliente1AdminSistemaAWS)**. 

_<span style="text-decoration:underline;">Importante ressaltar que o usuário do integrador deverá efetuar todos os procedimentos descritos nas etapas abaixo, com uma sessão ativa com a credencial acima criada.</span>_

### Segunda Etapa: Conectar Container de Provedor de Nuvem Pública

Neste ponto é fundamental que o profissional do integrador deva ter em mãos a informação referente a credencial de acesso de usuário programático (_Programmatic User/Access)_ que contenha as informações específicas de cada provedor -- _Entre em contato com a equipe técnica da Ustore para obter o documento que descreve o passo a passo para criação de usuário programático para cada provedor de serviço de nuvem pública._

Apenas como exemplo ilustrativo, iremos iniciar a descrição dos procedimentos de um novo cliente com as informações referentes ao provedor de serviço AWS (Amazon Web Service).

Caso o cliente em questão deseja adicionar mais de um ambiente de provedor de serviço de nuvem pública, deve-se repetir os passos conforme descritos ao final deste documento

O profissional do integrador deve acessar o menu **Container**,  selecionar o botão “**Conectar Container**”, clicar com o cursor do mouse sobre o campo **Tipo de Container** e selecionar a opção **AWS**. Preencher os dados conforme os campos da tela abaixo:



<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image6.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image6.png "image_tooltip")


_Imagem 2 - Conectar Container AWS_



* **Tipo de Container**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, trata-se de um campo do tipo “_drop down list_”, quando o usuário clicar sobre este será apresentada a lista das opções de tipos provedores (públicos e privados) que são suportados pela Plataforma do uCloud.
    * Selecionar a opção: **_AWS_**
* **Nome do Container**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser informado o nome com o qual deseja identificar este _container_ :
    * Informar: **_Cliente1AWS_**
* **Access Key**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com a informação específica referente a credencial de acesso programático que foi criada diretamente na console da AWS para esta finalidade. _Importante ressaltar que o conjunto de Access Key, só pode ser utilizado uma única tentativa, em caso de erro de digitação o conjunto de informações ficará invalidado e outra credencial de acesso programático deverá ser provisionada na console da AWS._
* **Secret Key**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com a informação específica referente a credencial de acesso programático que foi criada diretamente na console da AWS para esta finalidade. _Importante ressaltar que o conjunto de Secret Key, só pode ser utilizado uma única tentativa, em caso de erro de digitação o conjunto de informações ficará invalidado e outra credencial de acesso programático deverá ser provisionada na console da AWS._
* **Importar sem recursos**: Este botão é opcional e alternar este botão para o modo ATIVO indica para a Plataforma do uCloud que o processo de conexão a esta credencial da AWS deve sincronizar e importar o inventário completo de todos os recursos computacionais existentes no ambiente da AWS. \
  Manter este botão no modo NÃO ATIVO significa que a Plataforma do uCloud irá somente se conectar aos dados de faturamento e _billing_ desta credencial. Significa que a empresa optou por não efetuar a operação dos recursos computacionais existentes na AWS através da interface da Plataforma do uCloud.
    * **Não selecionar este “check box” - Manter em BRANCO**

<table>
  <tr>
   <td>
<strong>👉</strong>
<p>
<strong>Importante</strong>
   </td>
   <td><em>Importante esclarecer que devem ser concedidas/vinculadas certas permissões de acesso aos recursos computacionais ao usuário programático utilizado neste processo. de acesso de forma que seja possível ‘importar’ todos os recursos computacionais existentes no provedor (ex.: AWS). Se este usuário programático, não possuir estas permissões, a Plataforma do uCloud não irá apresentar nenhum recurso computacional existente neste provedor de serviço de nuvem pública (ex.: AWS). Entre em contato com a equipe técnica da Ustore para obter o documento que descreve o passo a passo para criação de usuário programático para cada provedor de serviço de nuvem pública.</em>
   </td>
  </tr>
</table>




* **Atrelar Container ao VDC**: Este botão é opcional e alternar este botão para o modo ATIVO indica para a Plataforma do uCloud que o processo de conexão a esta credencial da AWS vincular este ambiente a um _Virtual Datacenter _(VDC) previamente provisionado no ambiente da Plataforma do uCloud.
    * **Não selecionar este “check box” - Manter em BRANCO**
* **Botão Baixar Demo JSON**: Este botão é opcional, e pode ser utilizado para efetuar o download de um arquivo JSON de demonstração, com suas informações em branco, e pode ser utilizado como um exemplo para automatizar o processo de criação de outras credenciais da AWS.
* **Botão Importar JSON**: Este botão é opcional, e pode ser utilizado para efetuar a carga upload de um arquivo JSON personalizado com as informações das credenciais de acesso programático referente a AWS de forma automática.
* **Botão Conectar e Importar VMs**: Este botão é opcional, e pode ser utilizado para iniciar o processo de conexão deste _Container_ e importar todas as máquinas virtuais (_Virtual Machines - VMs_) que existem no ambiente da credencial da AWS. Ao clicar com o mouse sobre este botão significa que o usuário optou por controlar os valores financeiros (_Billing_) e operar os recursos computacionais desta credencial da AWS através da Plataforma do uCloud.
* **Botão Conectar: ** Após o usuário informar todos os parâmetros fundamentais para a criação do _Container_ da credencial Amazon AWS, o usuário irá notar que este botão alterna para o modo ativo (verde). Basta clicar com o cursor do mouse sobre o botão Criar, para que a Plataforma do uCloud inicie o provisionamento e conexão deste _Container AWS_. \
Caso este botão não esteja habilitado (cinza), significa que algum parâmetro anterior deixou de ser atendido ou algum campo está em branco, a Plataforma do uCloud não permitirá o provisionamento deste _Container AWS_.
* **Botão Cancelar: ** O usuário pode usar este botão para cancelar o processo de criação de um _Container AWS_. A Plataforma do uCloud encerra a tela e retorna à tela anterior.
    1. **Configurar Billing**

Neste ponto é fundamental que o profissional do integrador deva ter em mãos a informação referente ao acesso às informações referentes do _billing_ (ou _bucket_) desta credencial AWS - _Veja o documento da Ustore sobre o passo a passo para criação de usuário programático para cada provedor de serviço de nuvem pública. Sem o correto acesso e a informação do nome do arquivo de Billing, não será possível efetuar a configuração referente ao acesso ao Billing da AWS._

Acessar o menu  **Container**, e selecionar o _Container_ recém provisionado no processo acima, a Plataforma do uCloud irá apresentar uma tela com várias seções, veja na Seção Geral o campo:



<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image7.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image7.png "image_tooltip")


Imagem 3 - Tela NOVA de Billing AWS



* **Configurações do Financeiro**: Deve-se clicar com o cursor do mouse sobre o **Ícone Edição**

<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image8.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image8.png "image_tooltip")
 para a Plataforma do uCloud apresentar uma tela que permite editar as configurações do _Billing AWS_, conforme tela abaixo:



<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image9.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image9.png "image_tooltip")


Imagem 4 - Tela NOVA de Billing AWS



* **_Source_**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, trata-se de um campo do tipo “_drop down list_”, quando o usuário clicar sobre este será apresentada a lista das opções dos tipos que são suportados pela Plataforma do uCloud.
    * Selecionar a opção **_Cost and Usage Report_s (CUR)**.
* **_Bucket_**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar o nome do arquivo de _billing (bucket)_ que foi provisionado na console da AWS. _Veja o documento da Ustore sobre o passo a passo para criação de usuário programático para cada provedor de serviço de nuvem pública._
* **CUR**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar o nome do arquivo de _billing (bucket)_ que foi provisionado na console da AWS.
* **Região**: <span style="text-decoration:underline;">Este campo é obrigatório</span>, trata-se de um campo do tipo “_drop down list_”, quando o usuário clicar sobre este será apresentada a lista de todas as regiões globais da AWS. Deve ser selecionada a região global ao qual o arquivo de _billing_ do cliente foi vinculado.
* **Botão Habilitar Impostos**: Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que seja apresentados de forma EXPLÍCITA os valores de _Billing AWS_, esta opção permite identificar (segregar) os valores referentes às taxas dos impostos de cada um dos recursos computacionais de nuvem AWS dos relatórios financeiros da Plataforma do uCloud.
* **Botão Habilitar Créditos**:  Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que seja apresentados de forma EXPLÍCITA os valores dos créditos de valores de _Billing AWS_, esta opção permite identificar (segregar) os valores referentes créditos que foram adicionados a cada um dos recursos computacionais de nuvem AWS dos relatórios financeiros da Plataforma do uCloud.
* **Botão Habilitar Descontos SavingsPlan**: Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que seja apresentados de forma EXPLÍCITA os valores dos créditos de valores de _Billing AWS_, esta opção permite identificar (segregar) os valores referentes créditos que foram adicionados a cada um dos recursos computacionais de nuvem AWS dos relatórios financeiros da Plataforma do uCloud.
* **Botão Habilitar Descontos Instância Reservada**: Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que seja apresentados de forma EXPLÍCITA os valores dos créditos de valores de _Billing AWS_, esta opção permite identificar (segregar) os valores referentes créditos que foram adicionados a cada um dos recursos computacionais de nuvem AWS dos relatórios financeiros da Plataforma do uCloud.
* **Botão Buscar em Outra Conta**: Este botão é opcional, seu estado padrão é INATIVO. Somente deve ser alterado para o modo ATIVO quando o cliente deseja que os valores de _Billing_ deste _Container_ sejam obtidos de outra credencial de _Container AWS_ que tenha sido previamente provisionado na Plataforma do uCloud e que esta credencial de usuário possua acesso.
* **Botão Salvar: ** Após o usuário informar todos os parâmetros fundamentais para a criação do _Billing AWS_ o usuário irá notar que este botão alterna para o modo ativo (verde). Basta clicar com o cursor do mouse sobre o botão Salvar, para que a Plataforma do uCloud inicie o provisionamento e do _Billing AWS_. \
Caso este botão não esteja habilitado (cinza), significa que algum parâmetro anterior deixou de ser atendido ou algum campo está em branco, a Plataforma do uCloud não permitirá o provisionamento deste _Billing AWS_.
* **Botão Cancelar: ** O usuário pode usar este botão para cancelar o processo de criação de um _Billing AWS_. A Plataforma do uCloud encerra a tela e retorna à tela anterior.



<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image10.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image10.png "image_tooltip")


Imagem 3b - Tela antiga de Billing AWS



### Terceira Etapa: Criar Contrato

Neste ponto é fundamental que o profissional do integrador deva ter em mãos as informações referentes ao contrato comercial do cliente com o integrador, pois esta etapa estabelece as regras da relação comercial do cliente com o integrador.

Neste exemplo iremos descrever o processo da criação de um Contrato para o ambiente da AWS identificado com: **_Cliente1 _**

Para ilustrar e exemplificar este processo iremos assumir que o profissional do integrador está com uma sessão ativa na Plataforma do uCloud utilizando o login do usuário: _Cliente1**Admin**Sistema**AWS**_ (perfil Administrador).



    2. O que é Contrato para a Plataforma do uCloud

O Contrato é onde a empresa usuária do uCloud estabelece a forma com esta empresa irá gerenciar os aspectos comerciais da relação com o provedor de serviço de nuvem (pública ou privada), os limites financeiros (ou limite da quantidade dos recursos computacionais), define os seus valores para recursos computacionais de forma individualizada (válido somente para uma nuvem privada), vincula os grupos e usuários, entre outros.

No Contrato é onde se configura parâmetros de conversão de moeda, alertas de consumo e a vinculação com os seus respectivos Virtual Datacenters.

Muito importante ressaltar que todos os provedores de recursos de nuvem pública, efetuam a tarifação dos valores dos recursos computacionais em nuvem em Dólares Americanos, e apresentam os valores na interface de suas respectivas consoles em Reais utilizando de suas respectivas consoles para apresentar os valores em moeda local (R$ - Real).

Na tela abaixo podemos ver um exemplo da seção (card) de um contrato que apresenta os limites financeiros, e de quantidade de recursos, que a empresa definiu para o contrato.

Acessar o Menu **Administração / Contrato_ e selecionar o botão _Criar Contrato** e a Plataforma do uCloud apresenta a tela abaixo:



<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image11.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image11.png "image_tooltip")


Imagem 5 - Criando um Contrato



* **Nome do Contrato**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar o nome com o qual deverá ser identificado este contrato, Em outras palavras deve-se informar o mesmo nome de empresa o qual foi utilizado para identificar as credenciais do usuário provisionado na Primeira Etapa:  _<span style="text-decoration:underline;">Cliente1**Admin**</span>Sistema**AWS**_. 

    Seguido o seguinte formato: _&lt;Nome_do_Cliente><span style="text-decoration:underline;">[Provedor]</span>_.


    Abaixo listamos exemplos de padronização para a criação de usuários na Plataforma do uCloud, e ressaltamos que são meros exemplos  ilustrativos, mas usaremos estes exemplos para ilustrar todos os processos de cada etapa deste documento.
    
    * No caso AWS Exemplo de nome do contrato: _Cliente1**AWS**_
    * No caso Azure Exemplo de nome do contrato: _Cliente1**<span style="text-decoration:underline;">Azure</span>**_.
    * No caso Google Exemplo de nome do contrato: _Cliente1**<span style="text-decoration:underline;">GCP</span>**_.
    * No caso Huawei Exemplo de nome do contrato: _Cliente1**<span style="text-decoration:underline;">Huawei</span>**_.
    
    Para ilustrar este exemplo e seguir a padronização sugerida pela Ustore:
    
    * Informar: **Cliente1AWS**
* **Nome da Empresa**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar o nome com da Empresa (Razão Social, ou nome Fantasia).
* **CPF/CNPJ**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar o número do Cadastro Nacional de Pessoa Jurídica (CNPJ) ou Cadastro de Pessoa Física (CPF) com o qual deverá ser identificado este contrato. 
* **Dia da Fatura**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar o dia do fechamento da fatura deste contrato.
* **Admin Login**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar o login de usuário que foi provisionado na Primeira Etapa: Criação de Usuário (Perfil Administrador).
    * Informar: _<span style="text-decoration:underline;">Cliente1**Admin**</span>Sistema**AWS**_
* **Configuração Automática de Contrato**: Este campo NÃO é obrigatório e deve ser deixado em branco.
    * **Não selecionar este “check box” - Manter em BRANCO**
* **Auto Criar administrador**: Este campo NÃO é obrigatório e deve ser deixado em branco.
    * **Não selecionar este “check box” - Manter em BRANCO**
* **PTAX Variável**: Este campo NÃO é obrigatório e deve ser deixado em branco - Não selecionar este “check box”.
    * **Não selecionar este “check box” - Manter em BRANCO**
* **Botão Criar**: Após preencher todos os campos obrigatórios e opcionais para provisionar o novo Contrato, o usuário pode clicar com o cursor do mouse no botão verde **Criar** para que a Plataforma do uCloud provisione o novo Contrato em suas bases de dados internas. Caso o botão **Criar** não seja apresentado na cor verde, isto indica que algum campo obrigatório foi deixado sem preenchimento.
* **Botão Cancelar: ** O usuário pode usar este botão para cancelar o processo de criação de um Contrato. A Plataforma do uCloud encerra a tela e retorna à tela anterior.
    3. Conferência e _Validação das informações _Comerciais _do Contrato_

Após a inclusão de um contrato, este será adicionado com alguns campos que necessitam ser personalizados de forma a refletir os valores financeiros de forma correta.

Para se editar um Contrato deve-se clicar com o cursor do mouse sobre o nome do Contrato recém provisionado. Neste ponto a Plataforma do uCloud irá apresentar uma longa tela dividida em várias seções, encontre a seção Regras de Faturamento.

Nesta seção o Administrador do Contrato pode personalizar as regras de como os valores dos custos do contrato podem ser convertidos para moeda local, também personaliza, se para o cálculo de conversão de moeda aplicará no fator de conversão: um valor fixo ou um valor variável. Para o valor variável, a Plataforma do uCloud está configurada para obter a taxa do valor de conversão diretamente do site do Banco Central do Brasil, local onde pode extrair a taxa PTAX do último dia útil do mês, conforme o exemplo abaixo: 



<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image12.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image12.png "image_tooltip")


Abaixo descrevemos os campos desta seção:



* **Taxa de Faturamento**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e somente um usuário com perfil de Administrador (Admim/Admim) poderá visualizar e alterar este campo. Taxa de O valor informado neste campo o usuário do integrador, deverá informar o percentual da Taxa de Administração do Contrato. Este valor é informado utilizando a notação de 1,xx; onde “XX” representa o valor percentual que será adicionado aos valores do Contrato após a sua conversão de Dólar Americano para Real (Ex.: 1,20 = 20%).
* **Moeda**: <span style="text-decoration:underline;">Este campo é obrigatório</span> do tipo "drop down", quando o usuário clicar com o cursor do mouse a Plataforma do uCloud apresenta uma lista com todos os nomes de moedas configuradas na versão corrente do software. Basta o usuário clicar com o cursor do mouse sobre a moeda desejada.
* **Formatação de Data**: <span style="text-decoration:underline;">Este campo é obrigatório</span> do tipo “_dropdown_”, quando o usuário clicar com o cursor do mouse a Plataforma do uCloud apresenta uma lista com os formatos de datas disponíveis na Plataforma do uCloud:
    * **Formato Brasileiro**: DD/MM/YYY (Dia/Mês/Ano) **_<&lt; DEFAULT>>_**
    * **Formato Americano**: MM/DD/YYYY (Mês/Dia/Ano)
    * **Formato ISO**: YYYY/MM/DD (Ano/Mês/Dia)

    _Importante ressaltar que esta formatação é fundamental para controlar a forma como a Plataforma do uCloud irá calcular e apresentar as datas para o usuário, calcular datas de fechamento e receber os dados de bilhetagem do provedor de serviço de nuvem pública._


    _Se for deixado em branco a Plataforma do uCloud irá assumir o formato padrão de data Brasileiro (DD/MM/AAAA)._

* **Tipo de Cotação do Dólar**: <span style="text-decoration:underline;">Este campo é obrigatório</span> Deve-se clicar com o cursor do mouse sobre o **Ícone Edição**

<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image13.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image13.png "image_tooltip")
 para a Plataforma do uCloud permitir alterar o conteúdo deste campo, e existe apenas duas opções para este campo conforme descrito abaixo:
    * **Opção _Variável_**:Quando selecionada esta opção, significa que a Plataforma do uCloud irá obter (via API) do **site do Banco Central do Brasil **o valor da taxa **PTAX** na data informada no campo seguinte, para conversão dos valores de Dólar para Real.
        * **Dia de Cotação do Dólar**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e somente será apresentado quando o usuário selecionar a opção _variável_ para a taxa de cotação de Dólar. Este campo deve ser preenchido com a data do mês desejada para obtenção da taxa **PTAX**.
    * **Opção _Fixo_**: Quando selecionada esta opção, significa que a Plataforma do uCloud irá efetuar a conversão dos valores do billing do provedor de serviço de nuvem de Dólar para Real, com o valor informado no campo seguinte..
        * **Cotação do Dólar**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e somente será apresentado quando o usuário selecionar a opção _fixo_ para a taxa de cotação de Dólar. Este campo deve ser preenchido com o valor estabelecido para este contrato.
* **Quantidade de casas decimais**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com um número integral que especifique a quantidade de casas decimais (após a vírgula) para a apresentação de todos os valores financeiros na interface da Plataforma do uCloud.
* **Perfil de Tagueamento**: Este campo NÃO é obrigatório e deve ser deixado em branco.
    * **Manter em BRANCO**
* **Dia da fatura**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com um número integral que especifique a data de fechamento dos valores da fatura do provedor.

    Importante ressaltar que esta data determina a forma com todos os relatórios financeiros da Plataforma do uCloud, irão apresentar as respectivas representações de valores são faturamento a quantidade de casas decimais (após a vírgula) para a apresentação de todos os valores financeiros na interface da Plataforma do uCloud.





### Quarta Etapa: Criar **Grupo**

Importante ressaltar que o profissional do integrador deve seguir a padronização de nomes sugeridos nestes exemplos, de forma a que o ambiente da Plataforma do uCloud possa ter todas as vinculações financeiras entre Contrato, Grupos, _Virtual Datacenter_ e usuários, de forma que este ambiente possa ser refletido nos relatórios financeiros.

O usuário do integrador deve estar com uma sessão ativa na Plataforma do uCloud utilizando as credenciais do **Cliente1 **conforme descritos na Primeira Etapa: Criação do Usuário (perfil Administrador). Para ilustrar e exemplificar este processo iremos assumir que o profissional do integrador está com uma sessão ativa na Plataforma do uCloud utilizando o login do usuário: _Cliente1**Admin**Sistema**AWS**_.

Acessar o Menu **Administração / Grupo** e _selecionar o botão **Criar Grupo**_ e a Plataforma do uCloud apresenta a tela abaixo:



<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image14.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image14.png "image_tooltip")


Imagem 6 - Tela de Criação de Grupo



* **Nome**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com o nome do grupo. Para ilustrar este exemplo e seguir a padronização sugerida pela Ustore. Em outras palavras deve-se informar o mesmo nome de empresa o qual foi utilizado para identificar as credenciais do usuário provisionado na Primeira Etapa:  _<span style="text-decoration:underline;">Cliente1**Admin**</span>Sistema**AWS**_.
    * Informar: **Cliente1GrupoAWS**
* **Contrato**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser informado o nome do contrato, ao qual o grupo está vinculado. Para ilustrar este exemplo e seguir a padronização sugerida pela Ustore. Em outras palavras deve-se informar o mesmo nome de empresa o qual foi utilizado para identificar as credenciais do usuário provisionado na Primeira Etapa:  _<span style="text-decoration:underline;">Cliente1**Admin**</span>Sistema**AWS**_.
    * Informar: **Cliente1AWS**

        Pode-se informar parte do nome de um contrato e clicar com o cursor do mouse (ou a tecla Enter) para que a Plataforma do uCloud possa apresentar uma lista com todos os grupos que possuem a mesma sequência de caracteres informados, veja exemplo abaixo:




<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image15.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image15.png "image_tooltip")



        Serão listados apenas os contratos aos quais o perfil do usuário tem a permissão de visualizar. Assim que selecionado o grupo ficará vinculado ao contrato.


        Assim que um contrato é selecionado, a Plataforma do uCloud apresenta, na coluna à direita desta tela, o grupo de Permissões que foram definidas no Contrato.



<p id="gdcalert16" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image16.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert17">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image16.png "image_tooltip")


Imagem 7 - Permissões do Grupo


        Importante ressaltar que todos os usuários que pertencem ao grupo recebem as mesmas permissões. Existem duas formas diferentes que podem ser utilizadas neste momento para repassar as permissões do contrato para o grupo.



* **Utilizar as permissões padrões**: Esta opção engloba um conjunto padrão de permissões para o grupo, assim todos os usuários herdam este grupo de permissões padrão.
* **Definir manualmente as permissões**: Ao lado de cada linha de permissão existe um campo do tipo “_check box_”, ao ser selecionado, adiciona a respectiva permissão ao grupo e aos usuários pertencentes a este grupo. Este processo é detalhado, pois existem mais de cento e sessenta permissões na Plataforma do uCloud. Se o "checkbox" existente no topo da tabela for selecionado, significa marcar todas as permissões de uma única vez.
* **Apenas permissões de leitura**: Este campo é do tipo "radiobutton" ao ser selecionado configura que este grupo (e os usuários que o compõem) estão restritos a visualizar as informações do ambiente de nuvem. Os usuários vinculados a este grupo não possuem permissão de criação e/ou modificação de qualquer recurso computacional nos provedores de nuvem (público e/ou privado).
* **Cota de IPs Públicos**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo de Endereços TCP-IP Públicos que poderão ser consumidos por todos os usuários do grupo.
* **Cota de CPU**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais das CPUs que poderão ser consumidos por todos os usuários do grupo.
* **Cota de Memória**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais de Memória que poderão ser consumidos por todos os usuários do grupo. Pode ser selecionado o limite em **Megabytes** ou em **Gigabytes**.
* **Cota do Disco**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e deve ser preenchido com um número inteiro que representa a cota ou o limite máximo dos recursos computacionais de Disco de Armazenamento que poderá ser consumido por todos os usuários do grupo. Pode ser selecionado o limite em **Gigabytes**, **Megabytes** ou em **Terabytes**.
* **Botão Criar**: Após preencher todos os campos obrigatórios e opcionais para provisionar o novo Grupo, o usuário pode clicar com o cursor do mouse no botão verde **Criar** para que a Plataforma do uCloud provisione o novo Grupo em suas bases de dados internas. Caso o botão **Criar** não seja apresentado na cor verde, isto indica que algum campo obrigatório foi deixado sem preenchimento.
* **Botão Cancelar: ** O usuário pode usar este botão para cancelar o processo de criação de um Grupo. A Plataforma do uCloud encerra a tela e retorna à tela anterior.

    Após o usuário confirmar a ação de criar um grupo, a Plataforma do uCloud encerra a tela anterior e retorna para a tela com a lista de grupos e o grupo recém criado se apresenta nesta lista.

    4. **Alterar o Grupo do usuário _<span style="text-decoration:underline;">Cliente1</span>AdminSistemaAWS_**

    As credenciais de usuário que foram provisionadas na Primeira Etapa: Criação do Usuário (**_<span style="text-decoration:underline;">Cliente1</span>AdminSistemaAWS_**), no momento de seu provisionamento ficou automaticamente vinculado a um Grupo ao qual este usuário não deveria pertencer (default: Grupo _Admins_).


    O profissional do integrador deve seguir a padronização de nomes sugeridos nestes exemplos, de forma a que o ambiente da Plataforma do uCloud possa ter todas as vinculações financeiras entre Contrato, Grupos, _Virtual Datacenter_ e usuários, de forma que este ambiente possa ser refletido nos relatórios financeiros.


    O usuário do integrador deve estar com uma sessão ativa na Plataforma do uCloud utilizando as credenciais do **Cliente1 **conforme descritos na Primeira Etapa: Criação do Usuário (perfil Administrador). Para ilustrar e exemplificar este processo iremos assumir que o profissional do integrador está com uma sessão ativa na Plataforma do uCloud utilizando o login do usuário: _Cliente1**Admin**Sistema**AWS**_.


    Acessar o menu **Adminstração / Usuários**, e selecionar o usuário _Cliente1**Admin**Sistema**AWS**_. Na seção Geral encontramos o campo **Grupo** (primeiro campo listado na coluna da direita). Deve-se clicar com o cursor do mouse sobre o **Ícone Edição**

<p id="gdcalert17" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image17.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert18">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image17.png "image_tooltip")
 para a Plataforma do uCloud permitir alterar o conteúdo deste campo, para informar o novo Grupo recém provisionado nas ações acima listadas, neste ponto a tela da Plataforma do uCloud irá apresentar a tela abaixo:


​    

<p id="gdcalert18" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image18.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert19">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image18.png "image_tooltip")



    Imagem 7 - Alterar Grupo do Usuário

* **Ícone de Confirmação **

<p id="gdcalert19" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image19.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert20">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image19.png "image_tooltip")
: Quando o usuário deseja confirmar a vinculação do usuário ao seu novo grupo, a Plataforma do uCloud apresenta um ícone de confirmação. Após ter finalizado a digitação do nome do grupo “**Cliente1**” o usuário deve clicar com o cursor do mouse no botão verde para confirmar a vinculação. A Plataforma do uCloud atualiza suas bases de dados internas de forma imediata e instantânea, e vincula o usuário ao seu novo grupo.
    * Informar: **Cliente1GrupoAWS**
* **Ícone de Cancelamento **

<p id="gdcalert20" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image20.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert21">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image20.png "image_tooltip")
: Caso o usuário tenha clicado sobre o Ícone de Edição por engano ou não deseja que a vinculação do usuário ao Grupo recém provisionado, basta o usuário clicar com o cursor do mouse sobre o ícone vermelho. O ícone vermelho cancela as alterações e o conteúdo do campo retorna para os valores iniciais, antes de proceder qualquer preenchimento ou alteração.

Neste ponto devemos passar para a próxima etapa que é o provisionamento de um _Virtual Datacenter_.


### Quinta Etapa: Criar um **VDC**


    O profissional do integrador deve seguir a padronização de nomes sugeridos nestes exemplos, de forma a que o ambiente da Plataforma do uCloud possa ter todas as vinculações financeiras entre Contrato, Grupos, _Virtual Datacenter_ e usuários, de forma que este ambiente possa ser refletido nos relatórios financeiros.


    Neste exemplo iremos descrever o processo da criação de um VDC para o ambiente da AWS identificado com: **_Cliente1AWSVDC _**


    O usuário do integrador deve estar com uma sessão ativa na Plataforma do uCloud utilizando as credenciais do **Cliente1 **conforme descritos na Primeira Etapa: Criação do Usuário (perfil Administrador). Para ilustrar e exemplificar este processo iremos assumir que o profissional do integrador está com uma sessão ativa na Plataforma do uCloud utilizando o login do usuário: _Cliente1**Admin**Sistema**AWS**_.


    Acessar o menu Virtual Datacenters, basta o usuário clicar sobre o botão “Criar Virtual Datacenter”, conforme a figura abaixo:



<p id="gdcalert21" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image21.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert22">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image21.png "image_tooltip")



    O processo inicia quando a Plataforma do uCloud apresenta a primeira tela “**Criar Virtual Datacenter**”:



<p id="gdcalert22" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image22.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert23">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image22.png "image_tooltip")




* **Nome**: <span style="text-decoration:underline;">Este campo é obrigatório,</span> o usuário deve informar o nome do VDC com o qual deseja identificar este _Virtual Datacenter_. Sugestão: utilizar somente os caracteres ASCII padrão, <span style="text-decoration:underline;">não usar espaços em branco ou caracteres acentuados_ (ASCII Extendido)_</span>.
    * Informar: **_Cliente1AWSVDC_**
* **Container**: <span style="text-decoration:underline;">Este campo é obrigatório</span> do tipo “_dropdown_”, quando o usuário clicar com o cursor do mouse a Plataforma do uCloud apresenta uma lista com todos os provedores de serviço de nuvem configurados no ambiente da Plataforma do uCloud, neste momento, o usuário deve selecionar o _Container_ criado na Segunda Etapa: Conectar Container. Esta seleção determina como a Plataforma do uCloud apresenta as próximas telas.
    * Selecionar: **_Cliente1AWS_** 

    Assim que o usuário selecionar o provedor AWS (_container_) a Plataforma do uCloud apresenta a tela abaixo:




<p id="gdcalert23" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image23.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert24">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image23.png "image_tooltip")




* **Ícone para Ampliar a Seleção (**

<p id="gdcalert24" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image24.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert25">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image24.png "image_tooltip")
**)**: Para que a Plataforma do uCloud possa apresentar a lista de recursos computacionais respectivos de cada seção, o usuário deve clicar com o cursor do mouse sobre o ícone de cada seção desejada. 

    Quando o usuário amplia a seção desejada, os procedimentos para incluir (ou excluir) são os mesmos para qualquer uma das seções abaixo, portanto os esclarecimentos a seguir usam como exemplo a seção de **_Regiões_**, os processos são idênticos.

* **Coluna Acionável** (

<p id="gdcalert25" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image25.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert26">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image25.png "image_tooltip")
): Cada linha está representada por um ícone selecionável (

<p id="gdcalert26" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image26.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert27">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image26.png "image_tooltip")
” – ou do tipo “_check box_”). Quando o usuário seleciona uma linha, ou várias, a Plataforma do uCloud apresenta o ícone com status marcado (“

<p id="gdcalert27" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image27.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert28">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image27.png "image_tooltip")
), e um número ao lado do nome da seção com a quantidade selecionada de linhas referente a seção (

<p id="gdcalert28" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image28.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert29">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image28.png "image_tooltip")
). Veja o exemplo abaixo:



<p id="gdcalert29" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image29.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert30">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image29.png "image_tooltip")




* Se o usuário deseja selecionar todas as linhas da seção de uma única vez, este deve clicar com o cursor do mouse no ícone acionável que fica localizado na linha do cabeçalho da seção. Desta forma, a Plataforma do uCloud preenche todos os ícones de forma imediata e atualiza o número de linhas selecionadas no título da seção, de acordo com a quantidade de opções da seção. Veja o exemplo abaixo:



<p id="gdcalert30" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image30.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert31">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image30.png "image_tooltip")



    O usuário deve repetir estes procedimentos para cada uma das seções abaixo, até que a relação de recursos computacionais de nuvem de cada seção abaixo, fique na quantidade e características ideais para o seu uso na Plataforma do uCloud.



* **Regiões**: Esta seção apresenta todas as Regiões globais disponíveis no provedor de serviço de nuvem, após a seleção somente as regiões previamente definidas permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **_Templates_**: Esta seção apresenta todos os _Templates _disponíveis no provedor de serviço de nuvem, após a seleção somente os _templates_ previamente definidos permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **Redes**: Esta seção apresenta todas as Redes existentes, bem como as que foram provisionadas, no provedor de serviço de nuvem. Após a seleção somente as Redes previamente definidas permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **_Storage_**: Esta seção apresenta todos os tipos de Storages_ _disponíveis no provedor de serviço de nuvem, após a seleção somente os _storages_ previamente definidos permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **_Flavors_**: Esta seção apresenta todos os _Flavors _disponíveis no provedor de serviço de nuvem, após a seleção somente os _flavors_ previamente definidos permanecem disponíveis aos usuários, quando estes selecionarem o VDC.
* **Máquinas Virtuais**: Esta seção, quando expandida, apresenta a lista de todas as máquinas virtuais previamente criadas ao selecionar o provedor de serviço de nuvem ao qual o VDC está vinculado. O usuário pode incluir ou remover as máquinas virtuais vinculadas ao VDC. Este número será considerado no parâmetro **Max. Máquinas Virtuais**, que permite definir que este VDC tenha um número específico de máquinas virtuais.
* **Botão Criar**: Após efetuar a seleção de todos as opções desejadas para este VDC o usuário pode clicar com o cursor do mouse no botão verde **Criar** para que a Plataforma do uCloud provisione o novo _Virtual Datacenter _em suas bases de dados internas.
* **Botão Cancelar: ** O usuário pode usar este botão para cancelar o processo de criação de um _Virtual Datacenter_. A Plataforma do uCloud encerra a tela e retorna à tela anterior.

    Importante ressaltar que toda alteração, seja de inclusão ou de remoção, de recursos computacionais reflete de forma imediata na Plataforma do uCloud. Caso um usuário não seja capaz de visualizar um recurso computacional de nuvem (por exemplo: um _template_ ou um _flavor_), ao proceder a adição do recurso computacional, este recurso será imediatamente visualizado por todos os outros usuários.

### 

### Sexta Etapa: Conectar VDC **ao Contrato.**


    O usuário do integrador deve estar com uma sessão ativa na Plataforma do uCloud utilizando as credenciais do **Cliente1 **conforme descritos na Primeira Etapa: Criação do Usuário (perfil Administrador).


    Para ilustrar e exemplificar este processo iremos assumir que o profissional do integrador está com uma sessão ativa na Plataforma do uCloud utilizando o login do usuário: _Cliente1**Admin**Sistema**AWS**_.


    Acessar o Menu **Administração / Contrato** e na lista apresentada, selecionar o contrato que foi criado na Terceira Etapa: **Cliente1** e a Plataforma do uCloud apresenta a tela de visualização de contrato.
    
    5. Seção Virtual Datacenters Concedidos
    
    Esta é a uma das mais longas telas da Plataforma uCloud e com a quantidade de dezesseis (16) seções (cards), identifique e localize a _Seção Virtual Datacenter Concedidos_, e edite a vinculação deste contrato com, o VDC provisionado nos procedimentos da Quinta Etapa.


    Nesta seção o usuário deve clicar sobre o botão 

<p id="gdcalert31" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image31.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert32">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image31.png "image_tooltip")
, para a Plataforma do uCloud apresentar a tela para editar a vinculação do Contrado ao VDC.


    Esta tela possui apresenta colunas, na coluna da esquerda são listados todos os _Virtual Datacenters_ que já estão vinculados ao contrato. Por se tratar de um contrato recém provisionado, esta coluna da esquerda deve estar em branco (nenhum VDC vinculado).


    Na coluna da direita, será apresentada uma lista de todos os _Virtual Datacenters_ provisionados no ambiente da Plataforma do uCloud.


    O usuário do integrador deve preencher, no campo de “Busca Rápida” logo abaixo ao nome da coluna **Datacenter**, e preencher com o nome do VDC da Amazon AWS, criado na Quinta Etapa**.**




<p id="gdcalert32" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image32.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert33">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image32.png "image_tooltip")




* **Datacenter**: <span style="text-decoration:underline;">Este campo é obrigatório</span> e o usuário deve informar o nome com o qual foi provisionado o VDD para o ambiente da Amazon AWS.
    * Selecionar: **_Cliente1AWSVDC._**
* **Coluna Acionável** (“

<p id="gdcalert33" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image33.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert34">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image33.png "image_tooltip")
”): Na coluna ao lado do nome está representada por um ícone selecionável (“

<p id="gdcalert34" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image34.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert35">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image34.png "image_tooltip")
” – ou do tipo “_check box_”). Quando o usuário selecionar este ícone a Plataforma do uCloud apresenta o ícone com status marcado (“

<p id="gdcalert35" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image35.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert36">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image35.png "image_tooltip")
”), para confirmar que este VDC deve ser vinculado ao Contrato.
* **Botão Aplicar**: Após efetuar a seleção do _Virtual Datacenter_ o usuário deve clicar com o cursor do mouse no botão verde **Aplicar** para que a Plataforma do uCloud vincule o VDC_ _ao Contrato.
* **Botão Cancelar: ** O usuário pode usar este botão para cancelar o processo de vinculação de um _Virtual Datacenter_. A Plataforma do uCloud encerra a tela e retorna à tela anterior.


### Sétima Etapa: Validação do ambiente e suas vinculações


    Recomendamos como melhor prática, que o usuário do integrador, com uma sessão ativa na Plataforma do uCloud utilizando as credenciais do **Cliente1**, o login do usuário: _Cliente1**Admin**Sistema**AWS**_.


    Entrar nas respectivas opções de menu e validar se todas as configurações e personalizações do ambiente referente ao **Cliente1** estão corretas, seguindo a padronização e as identificações referente aos exemplos para o ambiente do provedor de nuvem Amazon AWS para o **Cliente1**:



* **Container: Cliente1_AWS_**
* **Virtual Datacenter: _Cliente1AWSVDC_**
* **Contrato Nome: Cliente1AWS**
    * **_Administrador do Contrato: Cliente1AdminSistemaAWS_**
    * **_Virtual Datacenter do Contrato: Cliente1AWSVDC_**
* **Grupo: _Cliente1GrupoAWS_**
    * **_Administrador do Grupo: Cliente1AdminSistemaAWS_**
* **Usuário: _Cliente1AdminSistemaAWS_**
* **Virtual Datacenter: _Cliente1AWSVDC_**

    Se todas as vinculações estejam corretas o ambiente AWS para este cliente está dentro das melhores práticas e seguindo a padronização indicada.


    Neste ponto o usuário do integrador deve reiniciar os procedimentos (Primeira Etapa) para conectar os ambiente dos outros provedores de serviço de nuvem pública adaptando os nomes de usuários, Containers, VDC, Grupos conforme os exemplos padronizados apresentados abaixo.



### Para conectar a nuvem Azure



* **Container: Cliente1_Azure_**
* **Virtual Datacenter: _Cliente1AzureVDC_**
* **Contrato Nome: Cliente1Azure**
    * **_Administrador do Contrato: Cliente1AdminSistemaAzure_**
    * **_Virtual Datacenter do Contrato: Cliente1AzureVDC_**
* **Grupo: _Cliente1GrupoAWS_**
    * **_Administrador do Grupo: Cliente1AdminSistemaAzure_**
* **Usuário: _Cliente1AdminSistemaAzure_**
* **Virtual Datacenter: _Cliente1AzureVDC_**



<p id="gdcalert36" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image36.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert37">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image36.png "image_tooltip")




<p id="gdcalert37" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image37.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert38">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image37.png "image_tooltip")




<p id="gdcalert38" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image38.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert39">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image38.png "image_tooltip")



### Para conectar a nuvem GCP (Google)



* **Container: Cliente1GCP**
* **Virtual Datacenter: _Cliente1GCPVDC_**
* **Contrato Nome: Cliente1GCP**
    * **_Administrador do Contrato: Cliente1AdminSistemaGCP_**
    * **_Virtual Datacenter do Contrato: Cliente1GCPVDC_**
* **Grupo: _Cliente1GrupoGCP_**
    * **_Administrador do Grupo: Cliente1AdminSistemaGCP_**
* **Usuário: _Cliente1AdminSistemaGCP_**
* **Virtual Datacenter: _Cliente1GCPVDC_**



<p id="gdcalert39" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image39.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert40">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image39.png "image_tooltip")




<p id="gdcalert40" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image40.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert41">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image40.png "image_tooltip")



### Para conectar a nuvem Huawei

* **Container: Cliente1Huawei**
* **Virtual Datacenter: _Cliente1HuaweiVDC_**
* **Contrato Nome: Cliente1Huawei**
    * **_Administrador do Contrato: Cliente1AdminSistemaHuawei_**
    * **_Virtual Datacenter do Contrato: Cliente1HuaweiVDC_**
* **Grupo: _Cliente1GrupoHuawei_**
    * **_Administrador do Grupo: Cliente1AdminSistemaHuawei_**
* **Usuário: _Cliente1AdminSistemaHuawei_**
* **Virtual Datacenter: _Cliente1HuaweiVDC_**

## Casos de Uso

Abaixo iremos descrever uma sugestão de como o Contrato, VDC e Container se relacionam para que a Plataforma do uCloud possa apresentar os valores mensais referente aos custos dos recursos computacionais de nuvem pública.

O caso de  uso que apresentaremos abaixo, são uma referência e podem ser utilizados como um modelo para os clientes do integrador.

Em caso de dúvida, entre em contato com a equipe da Ustore para receber instruções de como aplicar as melhores práticas de personalização do ambiente do cliente final, para que os relatórios financeiros sejam coerentes com os valores de consumo dos recursos computacionais de nuvem pública.


### 
    Caso de Uso: Contrato Isolado para cada Provedor de Nuvem diferente

Veja a figura abaixo, para descrever o cenário em que cada provedor de serviço de nuvem possui o seu próprio Contrato em separado.

Este cenário é altamente recomendável quando a relação comercial de cada provedor de serviço de nuvem pública utiliza diferentes taxas de conversão de valores de moeda corrente (em Dólar ⇒ Real) e diferentes valores de taxas administrativas. Importante mencionar que este cenário é altamente recomendável quando o pagamento dos valores mensais são efetuados através de notas fiscais isoladas e diferentes.

Este ambiente se justifica quando o cliente deseja utilizar a Plataforma do uCloud oferecida pelo integrador para que o cliente possa controlar os valores mensais dos recursos computacionais de nuvem de cada provedor de serviço de nuvem pública com os quais este cliente possui relacionamento. Neste caso de uso os valores de conversão de moeda (em Dólar ⇒ Real) e as taxas são individualizados para cada provedor de serviço de nuvem pública de forma independente e segregada.

Neste ambiente não existirá um contrato que será o grande agregador de valores mensais, os valores financeiros de cada contrato deverá ser avaliado de forma isolada e separadamente.



<p id="gdcalert41" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image41.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert42">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image41.png "image_tooltip")


Os procedimentos acima descritos neste documento de provisionamento de Contrato, Grupo, Usuário, VDC e Container devem ser repetidos de forma isolada para representar o ambiente da figura acima.



* **Container:**
    * **_AWSPerfil1_**
* **Virtual Datacenter AWS:**
    * **_VDC_Receita1_**
* **Grupo AWS:**
    * **_Grupo_DEVOPSReceita1_**
* **Contrato AWS: **
    * **_Contrato_RECEITA1_**
    * **_Administradores do Contrato:_**
        * **_admin_contrato_receita_**
        * **_admin_contrato_receita1_**
    * **_Virtual Datacenter do Contrato:_**
        * **_VDC_Receita1_**
    * **_Grupo do Contrato_**
        * **_Grupo_DEVOPSReceita1_**
* **Usuários:**
    * **_admin_contrato_receita_**
    * **_admin_contrato_receita1_**
    * **_user_receita1_**

Importante ressaltar que os usuários **_admin_contrato_receita_** e **_admin_contrato_receita1 _**estão vinculados no campo “Administrador do Contrato” do Contrato de cada provedor, isto significa que estes usuários têm autorização para acessar os relatórios financeiros da Plataforma do uCloud e acompanhar os valores de consumo mensal de todos os recursos computacionais de nuvem de cada provedor. Neste cenário, este usuário deve selecionar o contrato do provedor específico para acompanhar os valores mensais de consumo individualizado.

Em outras palavras, quando o usuário iniciar uma sessão na Plataforma do uCloud com a credencial de login **_admin_contrato_receita_** e estiver com uma sessão ativa na Plataforma do uCloud este poderá acessar o menu Financeiro, e selecionar um contrato específico e para acessar os relatórios de valores de consumo mensal deste contrato isoladamente.
