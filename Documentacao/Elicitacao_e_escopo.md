<div align="center">
  <h1>Elicitação e Escopo</h1>
</div>


## 1.0 Stakeholder / Solicitante

O stakeholder precisa:

* Criar novas demandas;
* Informar a descrição da atividade;
* Informar o prazo da atividade;
* Definir a prioridade;
* Acompanhar o andamento;
* Saber quem é o responsável pela atividade;
* Adicionar comentários;
* Validar a atividade após sua conclusão.

## 2.0 Gestor

O gestor precisa:

* Visualizar as demandas da equipe;
* Distribuir atividades;
* Definir o responsável pela atividade através da matrícula;
* Acompanhar os prazos;
* Identificar atividades atrasadas;
* Visualizar a quantidade de tarefas de cada colaborador;
* Acompanhar o andamento geral das demandas;
* Reorganizar prioridades quando necessário.

## 3.0 Desenvolvedor / Colaborador

O colaborador precisa:

* Visualizar suas atividades;
* Saber o prazo de cada tarefa;
* Consultar a descrição da atividade;
* Identificar a prioridade;
* Atualizar o status;
* Adicionar comentários;
* Anexar arquivos quando necessário;
* Enviar a atividade para validação.

# Processo de Elicitação de Requisitos

A elicitação abrange **quatro níveis/tipos de requisitos** fundamentais para a definição e entrega de uma solução de software.

---

## 1. Requisitos de Negócios
> Relacionados aos objetivos, metas ou necessidades estratégicas da organização em seu contexto de negócios.

* **Objetivo Principal:** Diminuir a superlotação no transporte público por meio de monitoramento e organização pelo fluxo de passageiros.

---

## 2. Requisitos das Partes Interessadas (*Stakeholders*)
> Necessidades das partes interessadas em relação à solução (como ela deve operar para agregar valor ao usuário/gestor).

* Contabilização de pessoas em fluxo.
* Notificação de previsão de chegada.
* Alertas e monitoramento de superlotação.

---

## 3. Requisitos da Solução
> Características e capacidades que a solução deve possuir. A análise de requisitos transforma as necessidades dos *stakeholders* em requisitos de solução e especificações técnicas.

### 3.1. Requisitos Funcionais (RF)
O **FlowOps** possui os seguintes requisitos funcionais principais:

| Código | Requisito |
| :---: | :--- |
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

### 3.2. Requisitos Não Funcionais (RNF)
Critérios de qualidade, restrições e atributos do sistema:

| Código | Requisito |
| :---: | :--- |
| **RNF01** | Usabilidade |
| **RNF02** | Responsividade |
| **RNF03** | Segurança |
| **RNF04** | Desempenho |
| **RNF05** | Disponibilidade |
| **RNF06** | Manutenibilidade |

---

## 4. Requisitos de Transição (RT)
> Requisitos temporários que a solução deve satisfazer para migrar da situação atual (*AS-IS*) para a situação desejada (*TO-BE*).

| Código | Requisito |
| :---: | :--- |
| **RT01** | Cadastro inicial dos usuários e matrículas |
| **RT02** | Cadastro das equipes e gestores |
| **RT03** | Migração de demandas de planilhas ou sistemas antigos |
| **RT04** | Orientação básica dos usuários antes da implantação |
