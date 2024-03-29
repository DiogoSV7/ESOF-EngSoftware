# Resumos-Engenharia-Software
Resumos para a cadeira de Engenharia de Software - FEUP 2º ano

## Software verification and validation

  (V&V) - Verificação e validação tem como objetivo mostrar:
          1. O sistema cumpre os seus requisitos
          2. O sistema cumpre os requisitos do seu cliente

        - Feito através de testes, reviews e inpeções 
        (unit testing, integration testing, system testing e acceptance testing)
        
### Software evolution (or maintenance)

  1. Software é flexível e pode mudar
  2. Mudanças de requirements, software tem de acompanhar essas mudanças
  3. Tipos de atividades
       - Corrective (corrigir bugs)
       - Adaptive (adotar novas tecnologias)
       - Perfective (novas funcionalidades)

### Software process models

  - Waterfall model (plan-driven model, ou seja, diferentes fases de especificação e desenvolvimento)

  - Incremental development (especificação, desenvolvimento e validação são interligados. Pode ser plan-driven ou agile)

  - Integration and Configuration (O sistema é assembled de componentes existentes configuráveis)

  - Software prototyping (Não é bem um modelo mas é um approach to cope)

### Waterfall model (plan-driven model) 

  1. System requirements 
  2. Software requirements
  3. Analysis
  4. Program design
  5. Coding
  6. Testing
  7. Operations

  - Unidirecional (1 -> 2 -> 3 -> 4 -> 5 -> 6 ->7 )
  - Uma fase tem de estar completa antes de se avançar para a próxima.
  - Ao partir o projeto em tantas fases, torna difícil alterar os customer requirements.

### Incremental development 

  1. System requirements 
  2. Software requirements
  3. Analysis
  4. Program design
  5. Coding
  6. Testing
  7. Operations

  - Bidirecional (1 -> 2 -> 3 -> 4 -> 5 -> 6 ->7 ) (7 -> 6 -> 5 -> 4 -> 3 -> 2 -> 1)
  - Especificação (versão inicial) , desenvolvimento (versões intermédias), validation (versão final) podem ser concorrentes.

#### Incremental development problems

  1. A estrutura tende a degradar com novas adições ao sistema.
  2. Pode ser difícil de identificar futuros features, então o seu nível de reuso pode não ser ótimo.
  3. Incremental delivery pode não ser possível para replacement systems, uma vez que incrementos têm menos funcionalidade do que substituir o sistema.
  4. A natureza de incremental development pode não ser adequada para establecer um contrato de desenvolvimento no início.

### Software prototyping

  1. Establecer objetivos do protótipo (prototyping plan)
  2. Definir a sua funcionalidade (outline definition)
  3. Desenvolver o protótipo (Executable prototype)
  4. Avaliar o protótipo (Evaluation report)

## Rational Unified Process 

  - Processos incrementais e iterativos
  - Rational Unified Process (RUP) desenvolvido com UML
  - Architecture-centric
  - Baseado em casos de uso

### Iterations, phases and disciplines

  PHASES:
    1. Começo.
    2. Elaboração.
    3. Construção.
    4. Transição.

  DISCIPLINES:
    1. Business Modelling (inicial).
    2. Requisitos (início e elaboração).
    3. Análise e Design (elaboração e construção).
    4. Implementação de testes (elaboração e construção).
    5. Deployment (construção e transição).
    6. Ambiente, Manage do projeto e configuração (todas as fases).

  ITERATIONS:
    1. Initial.
    2. Elaboração (1 e 2).
    3. Construção (1 e 2 e #N).
    4. Transição (1 e 2).
    
### Inception phase

   - Establecer o objetivo do projeto, incluindo visões operacionais, critérios de aceitação e o que o produto será e não será.
   - Preparar ambiente do projeto.
   - Discriminar e discutir usos críticos do sistema para escolher o melhor.
   - Estimar o custo e marcar datas para o projeto.

### Elaboration phase

    - Definir, validar e baseline a arquitetura.
    - Refinar a visão, baseando-se em novas informações obtidas durante a fase.
    - Definir iterações base e detalhadas para a construção do projeto.
    - Basicamente, uma refinação da primeira fase com mais informações.

### Construction phase

    - Management de recursos, controlos e otimização de processos.
    - Desenvolvimento completo do componente e testar contra os critérios establecidos.
    - Verificar assessment do produto contra o critério de aceitação establecido na visão.

### Transition phase

    - Executar os planos de lançamento.
    - Finalizar end-user material de suporte.
    - Testar o produto entregável no tamanho de desenvolvimento.
    - Receber feedback dos utilizadores.
    - Melhorar o produto baseado no feedback.
    - Tornar o produto disponível para os utilizadores.

## eXtreme Programming (XP)

### Agile methods

  O objetico dos agile methods é reduzir o overhead no processo do software e ter capacidade de responder rapidamente à mudança dos requerimentos.

### eXtreme Programming (one of the first agile methods)

  eXtreme Programming é uma alternativa a "heavy-weight" software development models.

  XP motto : "EMBRACE CHANGE"

  - Um dos valores fundamentais do XP é que o custo de alterar um programa seja sempre constante.
  - Hence XP é um processo leve (agile) -> Enfatiza feedback, ao invés de muita documentação do que o utilizador pretende. Elimina defeitos cedo, reduzindo os custos.

### Valores fundamentais de XP

  - Comunicação, Simplicidade, Feedback e Coragem

### Práticas XP 

  1. Planning game (Comum ao Scrum)
  2. Small releases (Comum ao Scrum)
  3. System metaphor
  4. Simple design
  5. Test-driven development
  6. Refactoring
  7. Pair programming
  8. Collective code ownership
  9. Continuous integration
  10. Sustainable pace
  11. On-site Customer
  12. Coding Standarts

### Planning Game 

  - Cliente tem lista com features desejados
  - Cada feature é escrito como "user story"
  - Desenvolvedores estimam tamanho de cada "user story"
  - Velocidade do projeto = tamanho total / iteração
  - Dadas estas estimativas de velocidades, cliente escolhe que stories implementar

Clientes decidem :
    User stories, prioridades, conteúdo de lançamento, datas de lançamento.

Desenvolvedores decidem : 
    Esforço, consequências, processo e schedules detalhados.

### Small Releases 

  - Começar com o feature set mais pequeno.
  - Lançar cedo e frequentemente, adicionando mais features.
  - Datas de lançamento podem ser date driven ou user story driven.

### System methapor 

  É uma story que todos - programadores, clientes e managers - podem perceber como o sistema funciona.
  É similar a architectural patterns.
  Desenhinho simples e metafórico que permite a toda a gente perceber como funciona.

### Simple Design

  - Utilizar a solução mais simples gets the job done.
  - Os requerimentos mudarão amanhã, então faz só o que encontra os requisitos de hoje.
  - Evitar big up-front design.

### Collective Code Ownership

  - Nenhuma pessoa é dona de um módulo, qualquer desenvolvedor pode trabalhar em qualquer parte do código a qualquer momento.
  - Ninguém tem responsabilidade pelo código completo.
  - Pressão cria código de melhor qualidade

### Continuous integration

  - Todas as mudanças são integradas no código base, no mínimo, diariamente.
  - Testes têm de correr 100% antes de serem integrados.
  - Permite lançamentos frequentes.

### Sustainable pace

  - Programmers go home on time, permite manter um bom ritmo de trabalho sem burnout.

### On-site Customer

  - Equipa de desenvolvimento tem contínuo acesso ao real libe customer, alguém que vai utilizar o sistema.

### Coding standards

  - Toda a gente tem de utilizar a mesma convenção (nome de variávies, funções, ...)
  - Idealmente, não poderemos olhar para uma parte do código e saber quem a fez apenas olhando.

### Conclusions

  - eXtreme programming é um agile method que integra um range de boas práticas de engenharia e de management de projetos, integrando lançamentos frequentes, evolução contínua do design,...
  - Parte forte do eXtreme programming é o desenvolvimento de automated tests antes de um feature ser criado.

## Requirements Engineering

- Requirements engineering (RE) : processo de estudar customer and user needs para chegar a uma definição do sistema, hardware e necessidades de software.

- Software requirement: propriedade que deve ser exibida pelo software desenvolvido ou adotado para resolver um determinado problema

### Principais dificuldades de RE

- Garantir requisitos, comunicação e entendimento
- Gerir requisitos de evolução

### Tipos de requisitos

$ Functional requirements : descrever as funções que o software deve ser capaz de executar
$ Nonfunctional requirements : são os requisitos que devem agir para chegar a uma solução

### Características de qualidade

1. Functionality suitability
2. Eficiência de performance
3. Reliabilidade
4. Usabilidade
5. Compatibilidade
6. Maintability
7. Portabilidade
8. Segurança

### Fonte de requisitos: stakeholders

*Stakeholders são a fonte principal de requisitos. Pessoas que serão afetadas pelo sistema que têm uma direta ou indireta influência na elaboração de requisitos.*

### Atividades de RE

 - Elicitation : interagir com stakeholders e com outras sources para entender as suas necessidades e requisitos.
 - Analysis : organizar e aceder à informação coletada, para chegar a uma lista de prioridade dos requisitos
 - Specification : produzir documentação dos requisitos com um nível apropriado de detalhe, dependendo do contexto
 - Validation : make sure que a documentação dos requisitos permite chegar aos objetivos do projeto

!!!! SLIDES CONTÊM INFORMAÇÃO MAIS ESPECÍFICA SOBRE ESTES 4 TIPOS DE ATIVIDADE E EXEMPLOS REAIS, CONSULTAR

### Artefactos de RE

 - Lista de requisitos (OBRIGATÓRIO)
 - Modelo de sistemas (USE CASE AND DOMAIN MODELS)
 - Protótipos e Mock-ups de interfaces de utilizadores
 - Testes de aceitação

   *EXEMPLOS*:Scrum, XP, Watterfall model

### User Stories

   *A user story is a promise for a conversation*. Ou seja, é uma forma leve de se demonstrar uma necessidade de um software.
   Deve incluir, "WHO", "WHAT", "WHY"

### User Stories - INVEST

   - Independent
   - Negotiable
   - Valuable
   - Estimable
   - Small
   - Testable

   EXEMPLO:

   As an automobile driver, i want to be able to remotely start my car so that it will be warmed up by the time i get to it.

### Acceptance tests

São test cases definidos pelos clientes para decidir se um sistema ou uma implementação de feature pode ser aceitada . Nos agile processes, um ou mais acceptance tests podem ser definidos para cada uma das user stories.

 - Formato comum é Behaviour-Driven-Development(BDD):
 - GIVEN [initial context]
 - WHEN [event occur(s)]
 - THEN [ensure some outcomes or postconditions]

## Software Processes: Agile

### Vuca World

* Volatilidade - mudança rápida e imprevisível é a sua natureza
* Incerteza - o presente não é claro e o futuro é incerto
* Complexidade - muitos fatores interconectados são trazidos para o jogo, com a sua confusão tudo se pode tornar muito complexo
* Ambiguidade - falta de claridade ou consciência do que a realidade é

*O QUE AS PESSOAS QUEREM É*
1. Serviço/Produto com alta qualidade
2. Grande produtividade de construção
3. Uma boa previsão dos resultados finais

### The Iron Triangle

PARA SE ALCANÇAR *QUALIDADE* (centro do triângulo) TEMOS DE INTERCALOR 3 FATORES (3 vértices do triângulo):

1. Recursos - budget, custo, ...
2. Schedule - tempo que demora, ...
3. Scope - features, funcionalidades, ...

### Software Processes: Scrum

* Scrum é um framework
* Baseado em : Artifacts, Meetings and Roles
* Artifacts : backlog do produto, ...
* Meetings : daily meeting, ...
* Roles : Team, product-owner, ...

### Fundações do Scrum

* Trust
* Foco
* Transparência
* Coragem
* Respeito
* Empenho

### Equipa

* 5-9 elementos
* Programadores, testers, user experience designers
* Members devem ser full-time
* São self-organizing
* Membership deve alterar apenas entre sprints (1-4 semanas)

### Scrum Master

* Representa o management para o projeto
* Remove impedimentos
* Garante que a equipa está totalmente operacional
* Proteje a equipa de interferências externas

### Product Owner

* Define features do produto
* Decide release date e conteúdo
* Aceita ou Rejeita o resulta do trabalho

### Github Projects: Board & Columns

*PRODUCT BACKLOG* 

* Ordered list de itens que contêm todos os epics, user stories, e todos os work items que necessários para a terminação do projeto
* A ordem é sempre feita da prespetiva do customer, baseado num ratio de valor e esforço
* Cada item deve ser percebido tanto por não technical personal como todos os outros


*SPRINT BACKLOG*

* Subset de itens (epic, user stories, work items) retirados do topo do Product Backlog, baseado no esforço, estimado em ser capaz de implementar durante a iteração. Itens devem ser facilmente entendidos pela equipa.


*IN PROGRESS*

* Itens a ser desenvolvidos no momento e apenas no momento
* Itens devem ter membros da equipa assigned
* Work in Progress (WIP) não deve ser maior do que o número de elementos, ou pares, da equipa


*DONE*

* Itens implementados e testados pela equipa mas ainda não aceites pelos clientes


*DONE, DONE, DONE*

* Itens aceites pelos clientes, já válidos e corretos

### Estimativa

* Não conseguimos estimar o desconhecido, ou seja, existem coisas que não sabemos que não sabemos
* Então, devemos estimar quais são os requisitos numa feature-by-feature, ao contrário de uma estimativa overall do projeto

### Valor e Esforço

 - Valor : Vamos utilizar o MoSCoW method para dar assign valor a cada Product backlog item
 - Must have, Should have, Could have, Will not Have (yet)


 - Esforço : Vamos usar o método de Fibonacci para determinar um esforço estimado para cada Product Backlog
 - 1,2,3,4,5,6,7,8,..

### Evolução do Scope

* Realidade é mais complexa que o scope creep consegue lidar
* Scope changes para tentar encontrar o que o cliente realmente quer

### Sprint Review

- Equipa apresenta oq conseguiu alcançar ao longo do sprint
- Tipicamente tem uma forma demo para demonstrar os novos features
- Informal
- A equipa inteira participa

### Práticas essenciais do Scrum

* Organizar o trabalho em cíclos curtos
* O management não interrompe a equipa num working cycle
* Equipa reporta ao cliente e não ao manager
* Equipa decide quanto trabalho eles conseguem fazer numa iteração
* Equipa mede a sua própria performance
* Definir goals antes dos ciclos começarem e através de user stories

  
