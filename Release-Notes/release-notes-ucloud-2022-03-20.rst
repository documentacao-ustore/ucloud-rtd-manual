Apresentação
============

Atualmente todo profissional de infraestrutura de TI utiliza diversos *consoles* diferentes para provisionar recursos computacionais, seja dentro da empresa (data center privado) ou em em algum provedor(es) de nuvem(ns). Desta forma, se manter atualizado e preparado, em todas as "consoles" é um dos desafios atuais para qualquer profissional de TI.

Na tentativa de aumentar a produtividade e reduzir o grau de dependência destes *consoles* o mercado desenvolveu o conceito de Infraestrutura como Código (IaaC - Infrastructure as a Code). Mas este conceito endereça somente o momento do provisionamento inicial (mesmo com o uso de scripts para instalação de padrões e softwares), mas podem existir demandas em que o profissional de TI terá de se conectar ao *console* do ambiente para executar alguma intervenção na infraestrutura que não é possível através do conceito de IaaC. Estar conectado e ficar alternando entre os diversos consoles de nuvem, demanda uma grande especialização e conhecimento do profissional de TI.

As plataformas de CSB (Cloud Service Broker) foram desenvolvidas para ocupar esse nicho e concentrar o inventário dos recursos computacionais de nuvens públicas e privadas em uma única interface e que transfere para o usuário o controle e operação destes recursos multi-nuvem.

Como mencionamos, o próprio mercado desenvolveu as metodologias de provisionamento de recursos computacionais através de scripts automatizados (também chamados de playbooks). Dentre estes formatos existem alguns que o mercado mundial adotou mais largamente, e podemos citar o Ansible, Terraform e Puppet.

O mercado também criou a demanda de programar a execução de uma sequência de diversos scripts dentro de um fluxo controlado e encadeado de forma que um erro em um destes scripts pode interromper todo o fluxo para evitar o provisionamento de uma infraestrutura computacional sem a devida qualidade.

Mas, muito importante é o nível de permissão das respectivas ações deste profissional seja na nuvem pública ou na nuvem privada. Independente se o profissional executa as ações via console ou via script automatizado, as plataformas de CSB devem possuir mecanismos que de provisionar um Perfil de Permissionamento e que estes possam ser vinculados às credenciais de acesso do usuário para controlar, adequar ou restringir as ações deste usuário.

Atenta à evolução constante do mercado brasileiro e às demandas de nossos usuários, a Ustore apresenta as novas funcionalidades que podem transformar a forma de gerenciar nuvens públicas e privadas com o uCloud.
Entre as novidades da nova versão destaca o Switch Roles, o Perfil de Permissionamento, o Catálogo de Serviços e o Workflow; que descreveremos a seguir.

Novas implementações
--------------------

Abaixo apresentamos a lista de novas implementações:
* Switch Roles
* Workflows
* Catálogo de Serviços
* Perfis de Permissionamento
Abaixo iremos esclarecer e descrever as novas implementações acima listadas.
Correções de Erros
Abaixo descrevemos as ações corretivas devido a situações que foram reportados erros e quais foram as ações corretivas de nossa equipe de desenvolvimento.
Amazon Web Services (AWS)
Não existe nenhuma menção referente a qualquer alteração para o presente documento.
Microsoft Azure (Azure)
Em janeiro de 2022 a Azure parou de adicionar informações de billing em moeda americana (dólar) e iniciou cobranças dos valores das faturas em moeda brasileira (Real), somente para os contratos CSP.
Isto acarretou que o desde 27 de janeiro de 2022, nenhum novo registro com valor do custo de recurso computacional é adicionado no arquivo de billing em dólar, e o bucket existente não está sendo atualizado e os valores não se encontram mais nesta área de armazenamento (bucket). Desta forma, os valores dos relatórios financeiros das faturas Azure se apresentam zerados. Isto não é um erro, pois a Plataforma uCloud está corretamente configurada para coletar os valores do billing na área dólar americano, mas a Azure não está atualizando mais as informações contidas no arquivo de billing.
A Azure criou uma nova área de bucket para armazenar o billing em Real, e esta nova área de bucket deve ser corretamente configurada na Plataforma uCloud.
A Plataforma uCloud por padrão pode ser configurada para cobranças em diversas moedas (Real, Dólar Americano, Pesos Colombianos, Pesos Mexicanos e Euro).
Para correção deste cenário, inicialmente deve-se validar se a credencial de billing provisionada na Plataforma uCloud possui acesso a esta nova área de bucket (Real Brasileiro).
Nos casos que a credencial atual permita o acesso à nova área de bucket, deveremos re-configurar a Plataforma uCloud para acessar esta nova área e processar o billing dos meses de fevereiro em diante.
Nos casos em que a credencial atual não permite o acesso à nova área de bucket o usuário com nível de administrador do ambiente Azure, deverá providenciar a criação de uma nova credencial de acesso com permissão Read-Only para esta área do bucket, e configurar esta nova área de bucket e sua respectiva credencial de acesso, na Plataforma uCloud.
Para ambos os casos, indicamos que o usuário entre em contato com a Equipe de Suporte da Ustore (chamados@usto.re) para ajudá-lo nesta configuração do bucket e a respectiva adequação das regras de faturamento do(s) contrato(s) que estão vinculados à Azure CSP.
Google Cloud Platform (GCP)
Não existe nenhuma menção referente a qualquer alteração para o presente documento.
Huawei Web Services (Huawei)
Não existe nenhuma menção referente a qualquer alteração para o presente documento.
VMware 6.5 ou superior (vCenter/vSphere)
Não existe nenhuma menção referente a qualquer alteração para o presente documento.


Atualização e Novas APIs
Não existe nenhuma menção referente a qualquer alteração para o presente documento.
