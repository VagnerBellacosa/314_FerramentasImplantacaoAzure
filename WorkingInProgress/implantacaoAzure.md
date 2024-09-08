# O que são Ambientes de Implantação Azure?

[Cenários de uso](https://learn.microsoft.com/pt-br/azure/deployment-environments/overview-what-is-azure-deployment-environments#usage-scenarios)

[Benefícios](https://learn.microsoft.com/pt-br/azure/deployment-environments/overview-what-is-azure-deployment-environments#benefits)

[Componentes compartilhados com o Microsoft Dev Box](https://learn.microsoft.com/pt-br/azure/deployment-environments/overview-what-is-azure-deployment-environments#components-shared-with-microsoft-dev-box)

[Conteúdo relacionado](https://learn.microsoft.com/pt-br/azure/deployment-environments/overview-what-is-azure-deployment-environments#related-content)

Os Ambientes de Implantação Azure capacitam as equipes de desenvolvimento a desenvolver de forma rápida e fácil a infraestrutura de aplicativos com modelos baseados em projeto, que estabelecem consistência e melhores práticas, maximizando a segurança, a conformidade e a eficiência de custos. Esse acesso sob demanda a ambientes seguros acelera os diferentes estágios do ciclo de vida do desenvolvimento de software com conformidade e economia.

Um [*ambiente de implantação*](https://learn.microsoft.com/pt-br/azure/deployment-environments/concept-environments-key-concepts#environments) é uma coleção de recursos de infraestrutura do Azure definidos em um modelo chamado de [*definição de ambiente*](https://learn.microsoft.com/pt-br/azure/deployment-environments/concept-environments-key-concepts#environment-definitions). Os desenvolvedores podem implementar a infraestrutura definida nos modelos nas assinaturas às quais têm acesso e criar seus aplicativos na infraestrutura. Por exemplo, você pode definir um ambiente de implantação que inclui um aplicativo Web, um banco de dados e uma conta de armazenamento. Seu desenvolvedor Web pode começar a codificar o aplicativo Web sem se preocupar com a infraestrutura subjacente.

Os engenheiros de plataforma podem criar e gerenciar definições de ambiente. Para especificar quais definições de ambiente estão disponíveis aos desenvolvedores, os engenheiros de plataforma podem associar definições de ambiente aos projetos e atribuírem permissões aos desenvolvedores.

Os Ambientes de Implantação do Azure ajudam os engenheiros de plataforma a aplicarem o conjunto certo de políticas e configurações em vários tipos de ambientes, controlarem a configuração de recursos que os desenvolvedores podem criar e acompanharem ambientes entre os projetos. Eles podem aplicar a governança do Azure com base no tipo de ambiente, como área restrita, teste, preparo ou produção.

O diagrama a seguir mostra uma visão geral dos recursos de Ambientes de Implantação do Azure. Os engenheiros de plataforma definem modelos de infraestrutura e configuram assinaturas, identidade e permissões. Os desenvolvedores criam ambientes com base nos modelos e criam e implantam aplicativos na infraestrutura. Os ambientes podem dar suporte a diferentes cenários, como ambientes sob demanda, ambientes de área restrita para teste e pipelines de CI/CD para integração contínua e implantação contínua.

[![Diagrama que mostra o fluxo de cenário dos Ambientes de Implantação Azure.](https://learn.microsoft.com/pt-br/azure/deployment-environments/media/overview-what-is-azure-deployment-environments/azure-deployment-environments-scenarios-sml.png)](https://learn.microsoft.com/pt-br/azure/deployment-environments/media/overview-what-is-azure-deployment-environments/azure-deployment-environments-scenarios.png#lightbox)

[Saiba mais sobre os principais conceitos para Ambientes de Implantação Azure](https://learn.microsoft.com/pt-br/azure/deployment-environments/concept-environments-key-concepts).



## Cenários de uso

Os cenários comuns nos Ambientes de Implantação do Azure incluem:



### Ambientes como parte de um pipeline de CI/CD

Criar e gerenciar ambientes de teste em toda a empresa pode exigir um esforço significativo. Com os Ambientes de Implantação do Azure, os desenvolvedores podem incorporar diferentes tipos de ambientes de ciclo de vida do produto (como desenvolvimento, teste, preparo, pré-produção e produção) em um pipeline de integração contínua e entrega contínua (CI/CD).

Neste cenário:

- As equipes de desenvolvimento podem conectar seus ambientes a pipelines de CI/CD para habilitar cenários de DevOps.
- As equipes de TI de desenvolvimento central podem controlar centralmente os custos, controlar alertas de segurança e gerenciar ambientes entre projetos e centros de desenvolvimento.



### Ambientes de área restrita para investigações

Os desenvolvedores costumam investigar diferentes tecnologias ou designs de infraestrutura. Por padrão, todos os ambientes criados com os Ambientes de Implantação Azure estão no próprio grupo de recursos. Os membros do projeto obtêm acesso de colaborador a esses recursos por padrão.

Neste cenário:

- Os desenvolvedores podem adicionar e alterar recursos do Azure conforme for necessário para seus ambientes de desenvolvimento ou de teste.
- As equipes de TI de desenvolvimento central podem acompanhar com facilidade os custos de todos os ambientes usados para fins de investigação.



### Ambientes de teste sob demanda

Os desenvolvedores podem criar ambientes ad hoc que imitam seus ambientes formais de desenvolvimento ou teste, para testar uma nova funcionalidade antes de verificar o código e executar um pipeline.

Neste cenário:

- Os desenvolvedores podem testar a versão mais recente de um aplicativo usando modelos reutilizáveis para criar rapidamente ambientes ad hoc.



### Treinamento, laboratórios práticos e hackathons

Um projeto nos Ambientes de Implantação do Azure atua como um contêiner para atividades transitórias, como workshops, laboratórios práticos, treinamento ou hackathons. Você pode criar um projeto para fornecer modelos personalizados para cada usuário.

Nesse cenário, os Ambientes de Implantação Azure oferecem os seguintes benefícios:

- Cada usuário pode criar ambientes idênticos e isolados para treinamento.
- Você pode excluir facilmente um projeto e todos os recursos relacionados quando o treinamento for concluído.



## Benefícios

Os Ambientes de Implantação Azure fornecem os seguintes benefícios para criar, configurar e gerenciar ambientes na nuvem:

- **Padronização e colaboração**: capture e compartilhe modelos de IaC no controle do código-fonte em sua equipe ou organização para criar ambientes sob demanda facilmente. Promova a colaboração por meio do fornecimento interno de modelos através de repositórios de controle do código-fonte.
- **Conformidade e governança**: as equipes de engenharia de plataforma podem coletar definições de ambiente para impor políticas de segurança corporativa e mapear projetos para assinaturas, identidades e permissões do Azure por tipos de ambiente.
- **Configurações baseadas em projeto**: organize as definições de ambiente pelo tipo de aplicativo em que as equipes de desenvolvimento estão trabalhando, em vez de usar uma lista de modelos não reorganizada ou uma configuração de IaC tradicional.
- **Autoatendimento sem preocupações**: capacite as equipes de desenvolvimento para criar rápida e facilmente recursos de infraestrutura de aplicativo (PaaS, sem servidor e muito mais), usando um conjunto de modelos pré-configurados. Você também pode controlar os custos desses recursos para não exceder seu orçamento.
- **Integração com a cadeia de ferramentas existente**: use as APIs para provisionar ambientes diretamente na ferramenta preferida de CI (integração contínua), IDE (ambiente de desenvolvimento integrado) ou pipeline de lançamento automatizado. Você também pode usar a ferramenta de linha de comando abrangente.



## Componentes compartilhados com o Microsoft Dev Box

O [Microsoft Dev Box](https://learn.microsoft.com/pt-br/azure/dev-box/overview-what-is-microsoft-dev-box) e os Ambientes de Implantação do Azure são serviços complementares que compartilham determinados componentes arquitetônicos. O Computador de Desenvolvimento fornece aos desenvolvedores uma estação de trabalho de desenvolvimento baseada em nuvem, chamada de computador de desenvolvimento, que é configurada com as ferramentas necessárias para o seu trabalho. Centros de desenvolvimento e projetos são comuns a ambos os serviços e ajudam a organizar recursos em uma empresa.

Ao configurar Ambientes de Implantação, você poderá ver os recursos e componentes do Computador de Desenvolvimento. Você pode até mesmo ver mensagens informativas sobre os recursos do Computador de Desenvolvimento. Se você não estiver configurando nenhum recurso do Computador de Desenvolvimento, poderá ignorar essas mensagens com segurança.



## Conteúdo relacionado

- [Início rápido: criar e configurar um centro de desenvolvimento](https://learn.microsoft.com/pt-br/azure/deployment-environments/quickstart-create-and-configure-devcenter)
- [Início Rápido: criar o Centro de desenvolvimento e projetos (Azure Resource Manager)](https://learn.microsoft.com/pt-br/azure/deployment-environments/quickstart-create-dev-center-project-azure-resource-manager)