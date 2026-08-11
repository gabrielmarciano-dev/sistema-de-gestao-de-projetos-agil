<div align="center">

<img src="./assets/flowops-logo.png" alt="FlowOps" width="500">

<h1>FlowOps</h1>

<p>Sistema para organização e acompanhamento de demandas.</p>

</div>

---

## Sobre o projeto

O **FlowOps** é uma ideia de sistema para ajudar equipes a organizar melhor suas atividades e demandas.

A ideia surgiu a partir de um problema comum: muitas vezes as tarefas são passadas por mensagens, e-mails ou conversas, o que pode causar confusão sobre quem deve fazer cada atividade e qual é o prazo para entrega.

O sistema funcionaria de forma parecida com um quadro de tarefas, como o Trello, mas com foco na organização das demandas entre o **Stakeholder, o gestor e a equipe responsável pela execução**.

---

## Como funciona

O fluxo principal do FlowOps funciona da seguinte maneira:

**Stakeholder solicita → Gestor distribui → Colaborador executa → Teste → Stakeholder valida → Concluído**

O Stakeholder cadastra uma atividade no sistema, informando o que precisa ser feito, a prioridade e o prazo.

Depois, o gestor pode distribuir essa atividade para um funcionário através da sua **matrícula**.

O colaborador recebe a tarefa, consulta as informações e atualiza o andamento conforme o trabalho é realizado.

As atividades passam pelas seguintes etapas:

**A Fazer → Em Desenvolvimento → Em Teste → Em Validação → Concluído**

Caso a atividade seja reprovada durante a validação, ela pode retornar para desenvolvimento:

**Em Validação → Ajustes necessários → Em Desenvolvimento**

---

## Objetivo

O principal objetivo do FlowOps é diminuir a desorganização no ambiente de trabalho, centralizando as demandas em um único sistema.

Com isso, seria possível ter mais controle sobre:

- Quem é responsável por cada tarefa;
- Prazo de entrega;
- Prioridade das atividades;
- Andamento das tarefas;
- Atividades atrasadas;
- Demandas que já foram concluídas.

---

## Principais usuários

### Stakeholder / Solicitante

O Stakeholder é responsável por solicitar e acompanhar as demandas.

Pode:

- Criar demandas;
- Informar título e descrição;
- Definir prazo;
- Definir prioridade;
- Acompanhar o andamento;
- Saber quem é o responsável;
- Adicionar comentários;
- Validar a entrega.

### Gestor

O gestor é responsável por organizar e distribuir as demandas da equipe.

Pode:

- Visualizar as demandas da equipe;
- Distribuir atividades;
- Definir o responsável através da matrícula;
- Acompanhar prazos;
- Identificar atividades atrasadas;
- Acompanhar o andamento;
- Reorganizar prioridades;
- Visualizar a quantidade de tarefas por colaborador.

### Desenvolvedor / Colaborador

O colaborador é responsável pela execução das atividades.

Pode:

- Visualizar suas atividades;
- Consultar o prazo;
- Consultar a descrição;
- Ver a prioridade;
- Atualizar o status;
- Adicionar comentários;
- Anexar arquivos;
- Enviar a atividade para validação.

---

## Status das atividades

O FlowOps utiliza um fluxo de etapas para acompanhar cada demanda:

| Status | Descrição |
|---|---|
| **A Fazer** | A atividade foi cadastrada e ainda não começou. |
| **Em Desenvolvimento** | O colaborador está trabalhando na atividade. |
| **Em Teste** | A atividade foi desenvolvida e está sendo testada. |
| **Em Validação** | A atividade está aguardando a aprovação do Stakeholder. |
| **Concluído** | A atividade foi aprovada e finalizada. |

Quando forem necessários ajustes, a atividade pode retornar para desenvolvimento.

**Em Validação → Ajustes necessários → Em Desenvolvimento**

---

## Prioridades

Cada demanda pode receber uma prioridade:

- **Crítica**
- **Alta**
- **Média**
- **Baixa**

A prioridade ajuda o gestor e a equipe a identificar quais atividades precisam de maior atenção.

---

## Principais funcionalidades

Entre as principais funcionalidades planejadas para o FlowOps estão:

- Cadastro de usuários;
- Cadastro de demandas;
- Definição de prioridade;
- Definição de prazo;
- Distribuição de atividades;
- Controle de status;
- Acompanhamento das demandas;
- Comentários;
- Anexos;
- Histórico de alterações;
- Identificação de atividades atrasadas;
- Validação das entregas;
- Retorno de atividades para desenvolvimento;
- Visualização das demandas em quadro Kanban.

---

## Priorização

As funcionalidades do FlowOps foram divididas de acordo com sua importância para o projeto.

### Essenciais

- Cadastro de usuários;
- Cadastro de demandas;
- Definição de responsável;
- Definição de prazo;
- Definição de prioridade;
- Controle de status;
- Visualização das demandas;
- Identificação de atrasos;
- Acompanhamento;
- Validação.

### Importantes

- Comentários;
- Histórico;
- Anexos;
- Dashboard;
- Controle de equipes;
- Filtros;
- Indicadores.

### Desejáveis

- Notificações;
- Integrações;
- Relatórios avançados;
- Integração com e-mail;
- Integração com Teams/Slack;
- Sugestão automática de responsáveis;
- Inteligência Artificial;
- Previsão de atrasos.

---

## Mapa Mental

O mapa mental apresenta outras informações e ideias relacionadas ao projeto.

**[Acessar Mapa Mental no Miro](https://miro.com/welcomeonboard/L1RRcGI5cnpibitWb3NEdS9acVR3bmpNSHdkZXFxd3greWpsMkI2NjJYRmFsMjA2UHFqdHVuZUFudEVkYkpPUHRkQXBja1lJRTBOZC80ZXBEOFZiYkt4QjZhR3RWQVVOYno2aTNPUVZXWXcxQXhpTkVPOCtxcE56THNkb3MraWI3QTNVZXpxSXBObEppZ0UxYUMzQnV3PT0hdjE=?share_link_id=704984603715)**

---

## Documentação

A documentação completa de **Engenharia de Requisitos** está disponível no arquivo:

[**requisitos.md**](./requisitos.md)

O documento apresenta:

- Cenário / Problema;
- Stakeholders envolvidos;
- Requisitos de negócio;
- Requisitos das partes interessadas;
- Requisitos funcionais;
- Requisitos não funcionais;
- Requisitos de transição;
- Priorização;
- Solução proposta;
- Justificativa.

---

## Requisitos

### Requisitos Funcionais

O FlowOps possui os seguintes requisitos funcionais principais:

| Código | Requisito |
|---|---|
| **RF01** | Cadastro de usuários |
| **RF02** | Cadastro de demandas |
| **RF03** | Definição de prioridade |
| **RF04** | Definição de prazo |
| **RF05** | Distribuição de atividades |
| **RF06** | Controle de status |
| **RF07** | Acompanhamento |
| **RF08** | Comentários |
| **RF09** | Anexos |
| **RF10** | Histórico |
| **RF11** | Identificação de atrasos |
| **RF12** | Validação |
| **RF13** | Retorno para desenvolvimento |
| **RF14** | Visualização em quadro Kanban |

### Requisitos Não Funcionais

| Código | Requisito |
|---|---|
| **RNF01** | Usabilidade |
| **RNF02** | Responsividade |
| **RNF03** | Segurança |
| **RNF04** | Desempenho |
| **RNF05** | Disponibilidade |
| **RNF06** | Manutenibilidade |

### Requisitos de Transição

| Código | Requisito |
|---|---|
| **RT01** | Cadastro inicial dos usuários e matrículas |
| **RT02** | Cadastro das equipes e gestores |
| **RT03** | Migração de demandas de planilhas ou sistemas antigos |
| **RT04** | Orientação básica dos usuários antes da implantação |

Para consultar a descrição completa dos requisitos:

[**Ver documentação completa de requisitos**](./requisitos.md)

---

## Estrutura do projeto

```text
FlowOps/
│
├── README.md
│
├── requisitos.md
│
└── assets/
    └── flowops-logo.png
```

---

## Tecnologias

O FlowOps é um projeto acadêmico desenvolvido inicialmente como uma proposta de sistema.

As tecnologias de desenvolvimento poderão ser definidas durante a implementação do projeto.

---

## Conclusão

O **FlowOps** é uma proposta de sistema que busca tornar a organização das atividades mais simples e clara.

A ideia é evitar que informações importantes fiquem espalhadas em diferentes lugares e facilitar a comunicação entre quem solicita, quem gerencia e quem executa as atividades.

Dessa forma, o sistema pode ajudar a equipe a ter uma visão melhor das demandas, dos responsáveis, dos prazos e do andamento de cada atividade.

---

<div align="center">

**FlowOps**

Organizando demandas. Facilitando o fluxo.

</div>
