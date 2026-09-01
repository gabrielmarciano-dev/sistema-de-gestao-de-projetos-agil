# Stakeholders e Levantamento de Necessidades

[Voltar ao README](../readme.md)

---

## Contexto do problema

**Problema a resolver:** incompatibilidade de horários, demora e filas de espera no agendamento manual de consultas médicas, gerando falhas de comunicação e alto índice de faltas dos pacientes.

**Afetados:** pacientes, recepcionistas, médicos e gestores administrativos da clínica.

**Solução atual (baseline):** atendimento por telefone, presencial na recepção, mensagens manuais via WhatsApp e anotações descentralizadas em planilhas e agendas de papel.

### Principais dores do processo atual
- **Absenteísmo alto** — ausência de lembretes estruturados pré-consulta.
- **Overbooking** — duplicidade de marcações por falha no controle manual.
- **Gargalo de atendimento** — linhas telefônicas ocupadas e filas em horários de pico.

### Resultado esperado
Reduzir o tempo de espera no agendamento, automatizar lembretes para diminuir faltas e eliminar erros de duplicidade na gestão de agendas.

---

## Mapa de stakeholders

| ID | Stakeholder | Papel | Necessidade/Interesse | Influência |
|---|---|---|---|---|
| ST01 | **Paciente** | Usuário Final | Agendar, remarcar e cancelar consultas rapidamente online. | Alta |
| ST02 | Recepcionista | Operador | Visualizar e ajustar a grade de horários de forma centralizada. | Média |
| ST03 | Médico | Prestador de Serviço | Consultar a agenda diária atualizada em tempo real. | Alta |
| ST04 | Administrador | Gestor | Acompanhar métricas de atendimento e taxas de absenteísmo. | Média |
| ST05 | Equipe de TI | Suporte | Garantir a segurança dos dados e alta disponibilidade do sistema. | Baixa |

> **Stakeholder principal: Paciente (ST01)** — o paciente é o usuário final da ponta do processo. Se o fluxo de agendamento não for acessível, intuitivo e ágil, a solução não cumpre sua função primária e o gargalo de atendimento persiste.

---

## Entrevista-guia (síntese)

| Pergunta | Resposta |
|---|---|
| O que esse usuário precisa fazer? | Agendar, consultar, remarcar e cancelar consultas médicas. |
| Qual problema ele enfrenta atualmente? | Demora no atendimento telefônico e imprecisões no agendamento manual. |
| Quais informações ele precisa consultar? | Especialidades, médicos disponíveis, datas, horários e histórico de consultas. |
| Quais informações ele precisa cadastrar/alterar? | Dados pessoais, convênio médico, telefone e e-mail. |
| Quais tarefas são repetitivas? | Envio manual de mensagens de confirmação de consulta. |
| Quais tarefas consomem mais tempo? | Localizar horários vagos e conciliar agendas via telefone. |
| Quais erros acontecem atualmente? | Agendamento de múltiplos pacientes para o mesmo médico no mesmo horário. |
| Precisa de notificações? | Sim — confirmações instantâneas e lembretes automáticos pré-consulta. |
| Precisa gerar documentos/relatórios? | Sim — dados pessoais e históricos de consultas, conforme LGPD. |
| Há informações que precisam ser protegidas? | Sim — relatórios de atendimentos, cancelamentos e faltas. |
| Precisa se comunicar com outro sistema? | Não na primeira versão — sistema autônomo, sem integrações legadas. |
| Regras obrigatórias? | Cancelamento com 24h de antecedência; sem horários sobrepostos. |
| O que tornaria a solução satisfatória? | Concluir o agendamento em menos de 2 minutos, de forma segura e simples. |

---

## Necessidades identificadas

| ID | Stakeholder | Necessidade | Problema relacionado |
|---|---|---|---|
| N01 | Paciente | Autonomia para escolher horários vagos online. | Filas de espera no atendimento por telefone. |
| N02 | Paciente | Lembretes automáticos sobre o dia e hora da consulta. | Altas taxas de esquecimento e absenteísmo. |
| N03 | Recepcionista | Bloqueio e liberação ágil de horários na agenda. | Agendamento manual propenso a conflitos. |
| N04 | Recepcionista | Cadastro simplificado de novos pacientes. | Demora no atendimento presencial na recepção. |
| N05 | Médico | Acesso à agenda diária atualizada em tempo real. | Falta de visibilidade de cancelamentos de última hora. |
| N06 | Administrador | Relatórios estatísticos de atendimento e absenteísmo. | Dificuldade em metrificar ociosidade médica. |
| N07 | Equipe de TI | Proteção de dados em conformidade com a LGPD. | Riscos de vazamento de informações sensíveis. |
| N08 | Paciente | Cancelamento simplificado via plataforma. | Necessidade de ligar apenas para cancelar. |

Cada necessidade acima está mapeada para um ou mais [Requisitos Funcionais](requisitos-funcionais.md).

[Regras de Negócio](regras-negocio.md) · [Voltar ao README](../README.md) · [Próximo: Revisão e Checklist](revisao-e-checklist.md)
