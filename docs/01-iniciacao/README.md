# Iniciação

> A fase de iniciação, em gerência de projetos, é o estágio que estabelece as bases para o sucesso do empreendimento. 
> Durante essa etapa, os objetivos definidos, identificando-se suas metas, escopo, partes interessadas (*stakeholders*) e restrições. 
> É o momento em que a viabilidade do projeto é avaliada, analisando-se recursos necessários, riscos potenciais e benefícios esperados.
> Nesta etapa é elaborado o Termo de Abertura do Projeto (TAP).
> Essa fase serve como um alicerce estratégico, proporcionando uma compreensão abrangente do que o projeto busca alcançar e delineando as diretrizes que orientarão as etapas subsequentes. 
> O sucesso na fase de iniciação contribui significativamente para a eficácia do gerenciamento de projetos como um todo.

# Estrutura do Documento

- [Fase de Iniciação](#iniciação)
- [Introdução](#introdução)
  - [Problema](#problema)
  - [Objetivos](#objetivos)
- [Especificações do Projeto](#especificações-do-projeto)
  - [Critérios de Sucessos](#critérios-de-sucesso)
  - [Histórias de Usuários](#histórias-de-usuários)
  - [Requisitos Preliminares](#requisitos-preliminares)
- [Partes Interessadas](#partes-interessadas)
- [Estimativa de Custo e Prazo](#estimativa-de-custo-e-prazo)
  - [Estimativa de Custo](#estimativa-de-custo)
  - [Estimativa de Prazo](#estimativa-de-prazo)
- [Metodologia](#metodologia)
  - [Divisão de Papéis](#divisão-de-papéis)
  - [Ferramentas](#ferramentas)
- [Documentos](#documentos)
  - [Declaração de Escopo](#declaração-de-escopo)
  - [Registro de Partes Interessadas](#registro-de-partes-interessadas)
  - [Termo de Abertura do Projeto (TAP)](#termo-de-abertura-do-projeto-tap)

# Introdução

## Problema

A segurança no transporte de mercadorias e de pessoas é uma preocupação constante para empresas e indivíduos. Motoristas enfrentam diversos riscos, incluindo acidentes, roubos, desvios de rota e situações de emergência. Atualmente, não há uma solução eficaz e integrada que permita monitorar em tempo real o comportamento do veículo e do motorista, fornecendo alertas imediatos para prevenir ou responder rapidamente a incidentes. Essa lacuna deixa motoristas, passageiros e cargas vulneráveis, impactando negativamente na eficiência das entregas e na segurança dos envolvidos.

## Objetivos

**Objetivo Geral**

Desenvolver um aplicativo móvel para monitoramento veicular, visando aumentar a segurança de motoristas, passageiros e mercadorias.

**Objetivos Específicos**

1. Implementar um sistema de rastreamento preciso utilizando funcionalidades nativas dos dispositivos móveis.
2. Criar um mecanismo de alerta para situações anormais, como paradas prolongadas ou desvios de rota.
3. Permitir o cadastro de contatos responsáveis que receberão notificações de segurança.
4. Garantir uma interface intuitiva e de fácil utilização para motoristas e administradores.

# Especificações do Projeto

Nesta seção, serão detalhadas as especificações técnicas e funcionais do aplicativo Safe Route. O desenvolvimento do projeto utilizará as seguintes técnicas e ferramentas:

1. Tecnologia de Rastreamento GPS: Utilização das APIs nativas dos sistemas operacionais Android e iOS para obter dados de localização em tempo real.
2. Sistema de Notificações Push: Implementação de um sistema de notificações para alertas de segurança utilizando Firebase Cloud Messaging (FCM) para Android e Apple Push Notification Service (APNs) para iOS.
3. Backend em Nuvem: Desenvolvimento de um backend escalável utilizando serviços em nuvem como AWS ou Google Cloud para processamento de dados e armazenamento seguro das informações.
4. Interface do Usuário (UI/UX): Criação de uma interface amigável e responsiva utilizando frameworks como React Native ou Flutter, garantindo compatibilidade com diferentes dispositivos móveis.
5. Segurança e Privacidade: Implementação de medidas de segurança, como criptografia de dados e autenticação de usuários, para proteger as informações sensíveis.


## Critérios de Sucesso

Os critérios de sucesso para o projeto Safe Route serão baseados nas seguintes dimensões:

1. Entrega no Prazo e Orçamento: O projeto deve ser concluído dentro dos prazos estabelecidos e do orçamento previsto.
2. Satisfação do Cliente: A Car Excellence Inc. e a Driving Better Corporation devem estar plenamente satisfeitas com a funcionalidade e a usabilidade do aplicativo.
3. Qualidade do Produto: O aplicativo deve ser estável, seguro e de alta precisão na localização e monitoramento, conforme os requisitos de qualidade estabelecidos.
4. Adoção e Utilização: O aplicativo deve ser adotado e utilizado efetivamente pelos motoristas e administradores, demonstrando a eficácia e a utilidade das funcionalidades implementadas.
5. Gerenciamento de Riscos: O projeto deve identificar, monitorar e mitigar riscos eficazmente ao longo do seu ciclo de vida.
6. Feedback das Partes Interessadas: O projeto deve receber feedback positivo das partes interessadas, evidenciando que os requisitos e expectativas foram atendidos.


 
## Histórias de Usuários

Com base na análise das personas forma identificadas as seguintes histórias de usuários:

|EU COMO... `PERSONA`| QUERO/PRECISO ... `FUNCIONALIDADE` |PARA ... `MOTIVO/VALOR`                 |
|--------------------|------------------------------------|----------------------------------------|
|Usuário do sistema  | Registrar minhas tarefas           | Não esquecer de fazê-las               |
|Administrador       | Alterar permissões                 | Permitir que possam administrar contas |
|Motorista | Cadastrar meu veículo no aplicativo	           | Que ele possa ser monitorado em tempo real             |
|Motorista       | Receber alertas sobre desvios de rota             | Saber quando estou fora da rota planejada |
|Motorista | 	Receber alertas sobre paradas prolongadas          | Agir rapidamente caso esteja em uma situação de risco              |
|Motorista      | 	Enviar meu status de segurança manualmente           | Informar que estou em segurança ou em situação de emergência |
|Administrador de Frota  | Visualizar a localização de todos os veículos        | Monitorar a frota e garantir a segurança         |
|Administrador de Frota    | Receber relatórios de trajetos percorridos               | Analisar a eficiência e segurança das rotas |
|Administrador de Frota  | Configurar contatos responsáveis para alertas        | Designar responsáveis para responder a alertas de segurança              |
|Familiar de Motorista       | Receber alertas de segurança               | Saber imediatamente se algo está errado |
|Familiar de Motorista | Visualizar a localização do veículo do motorista           | Ter certeza de onde o motorista está              |
|Motorista       | 	Ver o histórico de minhas rotas                 | Revisar os trajetos percorridos |
|Administrador de Frota  | Configurar parâmetros de alerta          | Ajustar as condições que disparam alertas de segurança               |
|Motorista       | Editar meu perfil e informações do veículo | Manter meus dados e os do veículo atualizados |
|Administrador de Frota  | Excluir veículos da frota          | Manter a lista de veículos atualizada          |
|Motorista       | Receber orientações em caso de emergência               | Saber o que fazer em situações de risco |
|Administrador de Frota | Integrar o sistema com outros softwares de gestão           | Melhorar a eficiência da gestão de frota         |
|Motorista       | Receber assistência imediata em emergências           | Garantir minha segurança e a do veículo |
|Administrador de Frota | 	Exportar dados para análises externas        | Realizar análises detalhadas fora do aplicativo          |
|Familiar de Motorista      | 	Configurar notificações personalizadas	   | 	Receber notificações conforme minha preferência |
|Motorista   | Acessar o aplicativo offline        | 	Consultar informações mesmo sem conexão com a internet       |
|Administrador de Frota   | Gerar gráficos de desempenho        | 	Visualizar o desempenho da frota de forma visual e clara |

## Requisitos Preliminares

### Requisitos Funcionais

A tabela a seguir apresenta os requisitos funcionais do projeto. 

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|-------|
|RF-001|	Permitir que o usuário cadastre seu veículo no aplicativo|	ALTA|
|RF-002|	Permitir que o usuário receba alertas de desvios de rota	|ALTA|
|RF-003|	Permitir que o usuário receba alertas de paradas prolongadas|	ALTA|
|RF-004|	Permitir que o usuário envie manualmente seu status de segurança	|ALTA|
|RF-005	|Permitir que o administrador visualize a localização dos veículos	|ALTA|
|RF-006|	Permitir que o administrador receba relatórios de trajetos|	MÉDIA|
|RF-007	|Permitir que o administrador configure contatos responsáveis	|ALTA|
|RF-008|	Permitir que familiares recebam alertas de segurança	|ALTA|
|RF-009|	Permitir que familiares visualizem a localização do veículo	|ALTA|
|RF-010	|Permitir que o usuário veja o histórico de suas rotas	|MÉDIA|
|RF-011	|Permitir que o administrador configure parâmetros de alertas	|MÉDIA|
|RF-012|	Permitir que o usuário edite seu perfil e informações do veículo|	MÉDIA|
|RF-013|	Permitir que o administrador exclua veículos da frota|	MÉDIA|
|RF-014|	Permitir que o usuário receba orientações em caso de emergência	|ALTA|
|RF-015	|Integrar o sistema com outros softwares de gestão|	BAIXA|
|RF-016|	Permitir que o usuário receba assistência imediata em emergências|	ALTA|
|RF-017	|Permitir que o administrador exporte dados para análises externas|	MÉDIA|
|RF-018|	Permitir que familiares configurem notificações personalizadas	|MÉDIA|
|RF-019|	Permitir que o usuário acesse o aplicativo offline	|BAIXA|
|RF-020	|Permitir que o administrador gere gráficos de desempenho|	MÉDIA|

### Requisitos Não Funcionais

A tabela a seguir apresenta os requisitos não funcionais do projeto. 

|ID     | Descrição do Requisito                                            |Prioridade |
|-------|-------------------------------------------------------------------|-----------|
|RNF-001|	O sistema deve ser responsivo para rodar em dispositivos móveis|	ALTA|
|RNF-002|	O sistema deve processar requisições do usuário em no máximo 2s|	MÉDIA|
|RNF-003|	O sistema deve garantir a criptografia de dados sensíveis	|ALTA|
|RNF-004|	O sistema deve ser compatível com Android e iOS|	ALTA|
|RNF-005|	O sistema deve garantir alta disponibilidade (99.9% uptime)	|ALTA|
|RNF-006|	O sistema deve permitir escalabilidade para suportar até 10.000 usuários simultâneos	|MÉDIA|
|RNF-007|	O sistema deve ter interface amigável e intuitiva	|ALTA|
|RNF-008|	O sistema deve garantir a integridade dos dados armazenados|	ALTA|
|RNF-009|	O sistema deve permitir fácil integração com APIs externas|	MÉDIA|
|RNF-010|	O sistema deve seguir as normas de acessibilidade|	MÉDIA|

### Restrições

A tabela a seguir apresenta as restrições do projeto. 

|ID    | Descrição do Requisito  | Prioridade |
|------|-----------------------------------------|-------|
|RE-001|	O desenvolvimento deve ser concluído em 6 meses	|ALTA|
|RE-002|	O orçamento do projeto deve ser de até R$ 500.000,00|	ALTA|
|RE-003|	O aplicativo deve suportar múltiplos idiomas|	MÉDIA|
|RE-004|	A integração com outros sistemas deve ser limitada a REST APIs|	MÉDIA|
|RE-005|	O aplicativo não deve requerer hardware adicional	|ALTA|

# Partes Interessadas

Nome  |  Relação ao Projeto  |  Nível de influência
------|----------------------|-----------------------
Josué Nogueira | Gerente | Alta
Leonardo Avelar | Desenvolvedor | Alta
Lucas Diniz | Desenvolvedor | Alta
João Alves | Desenvolvedor | Moderada
André Silva | Desenvolvedor | Moderada
Ana Carvalho | Desenvolvedor | Moderada
Carlos Andrade | Equipe Marketing | Baixa
Vinicius Souza | Equipe Marketing | Baixa
Car Excellence Inc. | Cliente | Moderada
Driving Better Corporation | Cliente | Moderada

# Estimativa de Custo e Prazo

## Estimativa de Custo

| Item de Custo           | Descrição | Qtd. horas | Valor / hora | Valor total |
|-------------------------|-----------|------------|--------------|-------------|
| Recursos Humanos        |     -      |    3400        |       15       |       51.000      |
| Hardware                |      -     |      -      |       -       |       -      |
| Serviços de Rede        |      -     |      150      |       5       |       1500      |
| Hospedagem e Nuvem      |     -      |      150      |       5       |       1500      |
| Software de terceiros   |      -     |      -      |       -       |       -      |
| Serviços e treinamento  |      -     |      240      |       10       |       2400      |
| **Total Geral**         |      -     |      3940      |       14,31       |      56400       |


## Estimativa de Prazo

* Prazo previsto (em horas): 3940
* Data de início: 01/03/2024
* Data de término: 08/06/2024


# Metodologia

A metodologia adotada para o desenvolvimento do projeto Safe Route é baseada no framework ágil Scrum. O Scrum é uma abordagem iterativa e incremental para o desenvolvimento de software, que foca em entregas rápidas e frequentes de partes funcionais do produto, com ênfase na colaboração entre a equipe e as partes interessadas.

**Processo de Trabalho**
- Sprint Planning: Planejamento das tarefas a serem realizadas em cada sprint, definindo prioridades e alocando recursos.
- Daily Stand-up: Reuniões diárias rápidas para acompanhar o progresso, identificar impedimentos e ajustar o trabalho conforme necessário.
- Sprint Review: Apresentação das funcionalidades desenvolvidas ao final de cada sprint para os stakeholders, coletando feedback e ajustando o backlog do produto.
- Sprint Retrospective: Reflexão sobre o processo de trabalho, identificando pontos de melhoria para o próximo sprint.

## Divisão de Papéis

- Gerente do projeto: Responsável por definir a visão do produto, priorizar o backlog e assegurar que o trabalho da equipe de desenvolvimento está alinhado com as necessidades do cliente.
- Scrum Master: Facilita o processo Scrum, removendo impedimentos e garantindo que a equipe siga os princípios e práticas ágeis.
- Equipe de Desenvolvimento: Conjunto de desenvolvedores responsáveis pela implementação das funcionalidades do produto.
- Stakeholders: Representantes do cliente e outras partes interessadas que fornecem feedback contínuo sobre o produto.

## Ferramentas

| Ambiente              | Plataforma         | Link de Acesso             | Justificativa |
|-----------------------|--------------------|----------------------------|---------------|
| Quadro Kanban         | Github             | [https://github.com/orgs/ICEI-PUC-Minas-PMG-EC-GPS/projects/12](https://github.com/orgs/ICEI-PUC-Minas-PMG-EC-GPS/projects/12) | Centralização e organização do projeto no próprio repositório. |
| Repositório de código | GitHub             | [https://github.com/ICEI-PUC-Minas-PMG-EC-GPS/pmg-ec-2024-01-gps-92470101-safe-route](https://github.com/ICEI-PUC-Minas-PMG-EC-GPS/pmg-ec-2024-01-gps-92470101-safe-route) |Organizar os arquivos do projeto               |
| Protótipo Interativo  | MavelApp ou Figma  | [https://figma.com/design/dWVCaWA6MDgvu7O2hVx9Z1/Safe-Route?node-id=0-1&t=hpmHKIsmoLwjHmGb-0](https://www.figma.com/design/dWVCaWA6MDgvu7O2hVx9Z1/Safe-Route?node-id=0-1&t=hpmHKIsmoLwjHmGb-0)  | Visualizar a interface do app              |
| Documentos Textuais   | Google Docs | N/A                        | Documentar o projeto              |
| Planilhas e Gráficos  | Google Planilhas   | https://docs.google.com/   |Documentar o projeto               |
| EAP / WBS             |Miro |[https://miro.com/app/board/uXjVNgV2MPk=/](https://miro.com/app/board/uXjVNgV2MPk=/) |Organização das tarefas |
| Cronograma do Projeto |Project Libre |[artefatos/SafeRoute.pdf](artefatos/SafeRoute.pdf) |Organizar as datas do projeto |
| Matriz RACI           | Google Docs |[artefatos/MatrizRACIGrupo4.pdf](artefatos/MatrizRACIGrupo4.pdf) |Delegar as responsabilidades do projeto |

# Documentos

> Nesta seção estão armazenados e listados os documentos e artefatos produzidos durante as aulas.

## Declaração de Escopo

- [Declaração de Escopo](artefatos/DeclaracaoEscopoGrupo4.pdf)

## Registro de Partes Interessadas

- [Registro de Partes Interessadas](artefatos/PlanilhaGerenciaPartesInteressadasUpdate.xlsx)

## Termo de Abertura do Projeto (TAP)

- [Termo de Abertura do Projeto](artefatos/TermoDeAberturaDeProjeto.pdf)
