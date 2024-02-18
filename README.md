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
    1. Começo
    2. Elaboração
    3. Construção
    4. Transição

  DISCIPLINES:
    1. Business Modelling (inicial)
    2. Requisitos (início e elaboração)
    3. Análise e Design (elaboração e construção)
    4. Implementação de testes (elaboração e construção)
    5. Deployment (construção e transição)
    6. Ambiente, Manage do projeto e configuração (todas as fases)

  ITERATIONS:
    1. Initial
    2. Elaboração (1 e 2)
    3. Construção (1 e 2 e #N)
    4. Transição (1 e 2)
    
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
    
