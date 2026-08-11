<div align="center">

<img src="./assets/flowops-logo.png" alt="FlowOps" width="420">

# FlowOps

Sistema para organização e acompanhamento de demandas.

[Documentação](#documentação) · [Como funciona](#como-funciona) · [Funcionalidades](#funcionalidades-principais)

</div>

---

## Sobre o projeto

O **FlowOps** é uma proposta de sistema para ajudar equipes a organizar melhor suas atividades e demandas.

A ideia surgiu a partir de um problema comum: muitas vezes as tarefas são passadas por mensagens, e-mails ou conversas, o que pode causar confusão sobre quem deve fazer cada atividade, qual é o prazo e em que situação a tarefa se encontra.

O FlowOps busca centralizar essas informações em um único lugar, facilitando a comunicação entre quem solicita, quem gerencia e quem executa as atividades.

---

## Como funciona

O fluxo principal do FlowOps é:

```text
Stakeholder solicita
        ↓
Gestor distribui
        ↓
Colaborador executa
        ↓
Teste
        ↓
Stakeholder valida
        ↓
Concluído
```

O Stakeholder cadastra uma demanda informando o que precisa ser feito, a prioridade e o prazo.

Depois, o gestor pode distribuir a atividade para um colaborador utilizando sua **matrícula**.

O colaborador recebe a atividade e atualiza seu andamento conforme o trabalho é realizado.

### Fluxo das atividades

```text
A Fazer
   ↓
Em Desenvolvimento
   ↓
Em Teste
   ↓
Em Validação
   ↓
Concluído
```

Caso a atividade precise de ajustes:

```text
Em Validação
      ↓
Ajustes necessários
      ↓
Em Desenvolvimento
```

---

## Objetivo

O principal objetivo do FlowOps é diminuir a desorganização no ambiente de trabalho, centralizando as demandas em um único sistema.

Com isso, a equipe pode ter uma visão melhor sobre:

* Responsável por cada atividade;
* Prazo de entrega;
* Prioridade;
* Andamento;
* Atividades atrasadas;
* Demandas concluídas.

---

## Principais usuários

### Stakeholder / Solicitante

Responsável por solicitar e acompanhar as demandas.

Pode:

* Criar demandas;
* Informar descrição;
* Definir prazo;
* Definir prioridade;
* Acompanhar o andamento;
* Adicionar comentários;
* Validar a entrega.

### Gestor

Responsável por organizar e distribuir as demandas.

Pode:

* Visualizar demandas da equipe;
* Distribuir atividades;
* Definir responsáveis através da matrícula;
* Acompanhar prazos;
* Identificar atividades atrasadas;
* Acompanhar o andamento;
* Reorganizar prioridades.

### Desenvolvedor / Colaborador

Responsável pela execução das atividades.

Pode:

* Visualizar suas atividades;
* Consultar prazo e descrição;
* Ver a prioridade;
* Atualizar o status;
* Adicionar comentários;
* Anexar arquivos;
* Enviar a atividade para validação.

---

## Status das atividades

| Status                 | Descrição                                      |
| ---------------------- | ---------------------------------------------- |
| **A Fazer**            | Atividade cadastrada e ainda não iniciada.     |
| **Em Desenvolvimento** | Atividade em execução pelo colaborador.        |
| **Em Teste**           | Atividade desenvolvida aguardando testes.      |
| **Em Validação**       | Atividade aguardando aprovação do Stakeholder. |
| **Concluído**          | Atividade aprovada e finalizada.               |

---

## Prioridades

As demandas podem possuir quatro níveis de prioridade:

* **Crítica**
* **Alta**
* **Média**
* **Baixa**

---

## Funcionalidades principais

* Cadastro de usuários;
* Cadastro de demandas;
* Definição de prioridade;
* Definição de prazo;
* Distribuição de atividades;
* Controle de status;
* Acompanhamento das demandas;
* Comentários;
* Anexos;
* Histórico de alterações;
* Identificação de atrasos;
* Validação das entregas;
* Retorno para desenvolvimento;
* Visualização em quadro Kanban.

---

## Documentação

A documentação do projeto está organizada na pasta `Documentacao`.

| Documento                                                        | Descrição                                            |
| ---------------------------------------------------------------- | ---------------------------------------------------- |
| [Análise de Negócio](./Documentacao/Analise_de_negocio.md)       | Problema, contexto e necessidades do projeto.        |
| [Elicitação e Escopo](./Documentacao/Elicitacao_e_escopo.md)     | Levantamento das necessidades e definição do escopo. |
| [Análise de Requisitos](./Documentacao/analise_de_requisitos.md) | Requisitos levantados para o FlowOps.                |
| [Validação da Solução](./Documentacao/Validacao_da_solucao.md)   | Validação da proposta de solução.                    |

---

## Mapa Mental

O projeto também possui um mapa mental com informações complementares.

[**Acessar mapa mental no Miro →**](https://miro.com/welcomeonboard/L1RRcGI5cnpibitWb3NEdS9acVR3bmpNSHdkZXFxd3greWpsMkI2NjJYRmFsMjA2UHFqdHVuZUFudEVkYkpPUHRkQXBja1lJRTBOZC80ZXBEOFZiYkt4QjZhR3RWQVVOYno2aTNPUVZXWXcxQXhpTkVPOCtxcE56THNkb3MraWI3QTNVZXpxSXBObEppZ0UxYUMzQnV3PT0hdjE=?share_link_id=704984603715)

---

## Estrutura do projeto

```text
FlowOps/
│
├── assets/
│   └── flowops-logo.png
│
├── Documentacao/
│   ├── Analise_de_negocio.md
│   ├── analise_de_requisitos.md
│   ├── Elicitacao_e_escopo.md
│   └── Validacao_da_solucao.md
│
└── readme.md
```

---

## Fluxo resumido

```text
                    ┌─────────────────────┐
                    │     Stakeholder     │
                    │     Solicita        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       Gestor        │
                    │     Distribui       │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Colaborador      │
                    │      Executa        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │        Teste        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     Stakeholder     │
                    │      Valida         │
                    └──────────┬──────────┘
                               │
                         ┌─────┴─────┐
                         │           │
                         ▼           ▼
                    Aprovado     Reprovado
                         │           │
                         ▼           │
                    Concluído        │
                                     │
                                     ▼
                              Ajustes necessários
                                     │
                                     ▼
                              Desenvolvimento
```

---

<div align="center">

FlowOps — Sistema para organização e acompanhamento de demandas.

</div>
