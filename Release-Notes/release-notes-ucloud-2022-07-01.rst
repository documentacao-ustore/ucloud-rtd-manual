**Notas Maio - 2022**
+++++++++++++++++++++

`Update tag 5.2-b35`

**Apresentação**
----------------

Em geral, o profissional de infraestrutura de TI utiliza diversos consoles para provisionar recursos computacionais, seja dentro da organização (datacenter privado) ou em algum provedor de nuvem. A computação em nuvem é uma evolução dos serviços e produtos de tecnologia da informação sob demanda, chamada por Brantner et al., 2008 de **Utility Computing**, a qual objetiva fornecer componentes básicos como: armazenamento, processamento e largura de banda de uma rede através de provedores especializados com um custo baixo por unidade utilizada. Na contemporaneidade, manter-se atualizado e preparado, em todas as «consoles» é um desafio para este profissional.

Na tentativa de aumentar a produtividade e reduzir o grau de dependência destes consoles o mercado desenvolveu o conceito de Infraestrutura como Código (IaaC - Infrastructure as a Code). Este conceito endereça somente o momento do provisionamento inicial (mesmo com o uso de scripts para instalação de padrões e softwares), podem existir demandas em que o profissional de TI deverá conectar-se à console do ambiente, para executar alguma intervenção na infraestrutura que não seja possível mediante o conceito de IaaC. Estar conectado e ficar alternando entre os diversos consoles de nuvem, demanda uma grande especialização e conhecimento do profissional de TI.

As plataformas de CSB (Cloud Service Broker) foram desenvolvidas para ocupar esse nicho e concentrar o inventário dos recursos computacionais de nuvens públicas e privadas em uma única interface e que transfere ao usuário o controle e a operação destes recursos multi-nuvem.

Como mencionado, o próprio mercado desenvolveu as metodologias de provisionamento de recursos computacionais através de scripts automatizados (também chamados de playbooks). Dentre estes formatos existem alguns que o mercado mundial adotou mais largamente, pode-se citar o Ansible, Terraform e Puppet.

O mercado também criou a demanda de programar a execução de uma sequência de diversos scripts dentro de um fluxo controlado e encadeado, de forma que um erro em um destes scripts pode interromper todo o fluxo para evitar o provisionamento de uma infraestrutura computacional sem a devida qualidade.

Atenta à evolução constante do mercado brasileiro e às demandas dos nossos usuários, a Ustore apresenta as novas implementações, as correções, as integrações, as atualizações no menu de funcionalidades e sua descrição detalhada. 

Além da ampliação do conceito existente, este release notes detalha o update ocorrido na plataforma uCloud, constante na (tag.5.2-b35) atendendo às diversas demandas mercadológicas dos nossos clientes, capazes de transformar a forma de gerenciar nuvens públicas e privadas com a plataforma uCloud.

**Novas implementações**
------------------------

As novidades apresentadas a seguir foram categorizadas em:

* As ações corretivas para adequação às mudanças ocorridas nos provedores de nuvens;
* As integrações realizadas no portal;
* Atualizações globais em alguns menus de funcionalidades do  portal.

Além das inovações mais robustas, elencadas em três temas. Estas novas implementações serão descritas, em detalhe, no transcorrer deste documento.

#. Account 
#. TAGs Virtuais
#. Oracle OPS

Abaixo apresentamos uma ilustração que apresenta o conceito completo da abrangência da funcionalidade Account implementada na Plataforma uCloud. Os nomes e denominações utilizados são meramente ilustrativos.

.. image:: /figuras/ucloud_arquitetura_conceitual001.png

As Contas Producer podem ter um administrador ou mais (neste nível o perfil deste usuário é de um Administrador do Sistema - ex.: root), os contratos param de ser criados quando o recurso da conta corporativa acaba, os perfis de visualização e permissionamento obedecem a regra de negócio aplicada pela conta integrator.
