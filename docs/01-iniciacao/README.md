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
> **Link Útil**:
> - [Objetivo geral e objetivo específico: como fazer e quais verbos utilizar](https://blog.mettzer.com/diferenca-entre-objetivo-geral-e-objetivo-especifico/)

 
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


> Seguindo o modelo acima, apresente aqui as histórias de usuário que são relevantes para o projeto de sua solução. 
> As Histórias de Usuário consistem em uma ferramenta importante para a compreensão e elicitação dos requisitos.
> Defina atores (ou personas), se for o caso, um administrador para criação das histõrias de usuário.
> As histórias de usuário posteriormente devem ser utilizadas para preenchimento dos Requisitos Funcionais.
>
> **Links Úteis**:
> - [Histórias de usuários com exemplos e template](https://www.atlassian.com/br/agile/project-management/user-stories)
> - [Como escrever boas histórias de usuário (User Stories)](https://medium.com/vertice/como-escrever-boas-users-stories-hist%C3%B3rias-de-usu%C3%A1rios-b29c75043fac)

## Requisitos Preliminares

> Os requisitos preliminares fornecem uma visão inicial do escopo, funcionalidades-chave e as expectativas a serem atendidas. 
> 
> ***A quantidade mínima de requisitos a serem preenchidos nas seções abaixo não incluem os exemplos previamente fornecidos.***

> Com base nas Histórias de Usuário, enumere os requisitos da sua
> solução. Classifique esses requisitos em dois grupos:
>
> - [Requisitos Funcionais (RF)](https://pt.wikipedia.org/wiki/Requisito_funcional):
>   correspondem a uma funcionalidade que deve estar presente na
>   plataforma (ex: cadastro de usuário).
>
> - [Requisitos Não Funcionais (RNF)](https://pt.wikipedia.org/wiki/Requisito_n%C3%A3o_funcional):
>   correspondem a uma característica técnica, seja de usabilidade,
>   desempenho, confiabilidade, segurança ou outro (ex: suporte a
>   dispositivos iOS e Android).
>
> Lembre-se que cada requisito deve corresponder à uma e somente uma
> característica alvo da sua solução. Além disso, certifique-se de que
> todos os aspectos capturados nas Histórias de Usuário foram cobertos.
> 
> **Links Úteis**:
> 
> - [O que são Requisitos Funcionais e Requisitos Não Funcionais?](https://codificar.com.br/requisitos-funcionais-nao-funcionais/)
> - [O que são requisitos funcionais e requisitos não funcionais?](https://analisederequisitos.com.br/requisitos-funcionais-e-requisitos-nao-funcionais-o-que-sao/)


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

> Relacione as partes interessadas no seu projeto. 
> Você deve descrever as partes interessadas e indicar qual o nível de influência em relação ao projeto.
> Indique as principais pessoas (clientes, fornecedores, etc), indicando possíveis expectativas, nível de influência e possível importância para o sucesso do projeto.


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


> A avaliação da viabilidade econômica busca determinar a sustentabilidade financeira e o retorno sobre o investimento do empreendimento. 
> Este processo envolve a análise dos custos associados ao projeto, incluindo investimentos iniciais, despesas operacionais e potenciais custos de manutenção. 
> Simultaneamente, são examinados os benefícios esperados, como receitas, economias de custos e ganhos tangíveis e intangíveis. 
> A elaboração de projeções financeiras realistas e a aplicação de métricas como o Valor Presente Líquido (VPL) e a Taxa Interna de Retorno (TIR) contribuem para uma avaliação abrangente da viabilidade econômica do projeto. 
> Este processo permite que os gestores de projeto e as partes interessadas tomem decisões informadas sobre a continuidade, ajustes ou mesmo a interrupção do projeto, garantindo uma alocação eficiente de recursos e maximizando os benefícios econômicos esperados.

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

> A estimativa de prazo orienta tanto o cliente quanto a equipe de desenvolvimento do projeto em termos do tempo necessário para a conclusão do projeto como um todo. 
> Esta estimativa possibilita a criação de um cronograma realista e viável, permitindo o planejamento adequado das fases do projeto, alocação de recursos de maneira eficiente e antecipação de eventuais desafios.
> Uma estimativa precisa orienta a execução do projeto, contribui para a gestão de expectativas e para o estabelecimento de metas alcançáveis.

> Indique:
> * Prazo previsto (em horas) 
> * Data de início
> * Data de término
* Prazo previsto (em horas): 3940
* Data de início: 01/03/2024
* Data de término: 08/06/2024


# Metodologia

......  COLOQUE AQUI O SEU TEXTO ......

> Nesta parte do documento, você deve apresentar a metodologia adotada pelo grupo, descrevendo o processo de trabalho baseado nas metodologias ágeis, a divisão de papéis e tarefas e as ferramentas empregadas.
>
> Coloque detalhes sobre o processo utilizado e a implementação do Framework Scrum seguido pelo grupo. 
> O grupo deverá gerenciar as tarefas utilizando o GitHub Project para acompanhar o andamento do projeto, a execução das tarefas e o status de desenvolvimento da solução.
> 
> **Links Úteis**:
> - [Github Project](https://docs.github.com/en/issues/planning-and-tracking-with-projects/creating-projects/creating-a-project)
> - [O que é o GitHub Projects? | Guia de Iniciantes](https://www.youtube.com/watch?v=vxYTpsFKdiQ&ab_channel=JulioArruda)
> - [Introduction to GitHub Project Boards](https://www.youtube.com/watch?v=idZyqNIrt84&list=PLiO7XHcmTslc5hGrbnnmHIb0SeJLTpOEu&ab_channel=MickeyGousset)
> - [11 Passos Essenciais para Implantar Scrum no seu Projeto](https://mindmaster.com.br/scrum-11-passos/)
> - [Scrum em 9 minutos](https://www.youtube.com/watch?v=XfvQWnRgxG0)

## Divisão de Papéis

......  COLOQUE AQUI O SEU TEXTO ......

> Apresente a divisão de papéis e tarefas entre os membros do grupo.
> Indique as responsabilidades de cada membro do grupo no projeto.

## Ferramentas

......  COLOQUE AQUI O SEU TEXTO - SIGA O EXEMPLO DA TABELA ABAIXO  ......

> Liste as ferramentas empregadas no desenvolvimento do projeto, justificando a escolha delas, sempre que possível.
> Todas as ferramentas utilizadas devem ser listadas.
> Qualquer tipo de ferramenta que for utilizada para construção de um artefato deve ser identificada, uma vez que podem ser necessárias alterações.
> A necessidade de uso de licenças e possíveis custos relacionados devem ser indicados.

| Ambiente              | Plataforma         | Link de Acesso             | Justificativa |
|-----------------------|--------------------|----------------------------|---------------|
| Quadro Kanban         | Github             | [https://github.com/orgs/ICEI-PUC-Minas-PMG-EC-GPS/projects/12](https://github.com/orgs/ICEI-PUC-Minas-PMG-EC-GPS/projects/12) | Centralização e organização do projeto no próprio repositório. |
| Repositório de código | GitHub             | https://github.com/XXXXXXX |               |
| Protótipo Interativo  | MavelApp ou Figma  | https://figma.com/XXXXXXX  |               |
| Documentos Textuais   | Google Docs | N/A                        |               |
| Planilhas e Gráficos  | Google Planilhas   | https://docs.google.com/   |               |
| EAP / WBS             | | | |
| Cronograma do Projeto | | | |
| Matriz RACI           | Google Docs |[artefatos/MatrizRACIGrupo4.pdf](artefatos/MatrizRACIGrupo4.pdf) | |

# Documentos

> Esta seção deve ser utilizada para armazenamento e listagem dos documentos e artefatos produzidos durante as aulas.
> Atualize os documentos nos respectivos links.

## Declaração de Escopo

> Você deve preencher o seguinte documento:
- [Declaração de Escopo](artefatos/declaracao-escopo.docx)

## Registro de Partes Interessadas

> Você deve preencher o seguinte documento:
- [Registro de Partes Interessadas](artefatos/registro-partes-interessadas.xlsx)

## Termo de Abertura do Projeto (TAP)

> O Termo de Abertura do Projeto (TAP) representa o ponto de partida oficial para o empreendimento. 
> Ele sintetiza de maneira clara e concisa os objetivos, escopo, partes interessadas envolvidas, entregas esperadas, cronograma preliminar e recursos necessários para a execução bem-sucedida do projeto. 
> O TAP funciona como um contrato inicial entre a equipe do projeto e as partes interessadas, estabelecendo as bases para uma compreensão compartilhada dos propósitos e limites do projeto. 
> Ao delinear esses elementos de forma detalhada, o Termo de Abertura do Projeto (TAP) fornece uma direção sólida para orientar as atividades subsequentes, facilitando a gestão eficaz do projeto desde o início até o encerramento. 
> Essa documentação garante a clareza, alinhamento e comprometimento de todos os envolvidos, contribuindo assim para o sucesso do projeto.

> Você deve preencher o seguinte documento:
> - [Termo de Abertura do Projeto](artefatos/TermoDeAberturaDeProjeto.pdf)
