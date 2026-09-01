# Requisitos Funcionais (RF)

[Voltar ao README](../README.md)

Requisitos que descrevem **o que o sistema deve permitir que os usuários façam**. Cada requisito é atômico, rastreável a uma necessidade de stakeholder e priorizado segundo seu impacto no problema central.

---

## RF01 — Cadastro e atualização de dados do paciente

| Campo | Detalhe |
|---|---|
| **Descrição** | O sistema deve permitir que o paciente cadastre e atualize seus dados pessoais. |
| **Stakeholder / Fonte** | Paciente (ST01) |
| **Necessidade relacionada** | N04 — Cadastro simplificado de novos pacientes |
| **Prioridade** | Alta |

---

## RF02 — Consulta de horários disponíveis

| Campo | Detalhe |
|---|---|
| **Descrição** | O sistema deve permitir a consulta de horários disponíveis por médico e especialidade. |
| **Stakeholder / Fonte** | Paciente (ST01) |
| **Necessidade relacionada** | N01 — Autonomia para escolher horários vagos online |
| **Prioridade** | Alta |

---

## RF03 — Agendamento de consultas

| Campo | Detalhe |
|---|---|
| **Descrição** | O sistema deve permitir que o paciente realize o agendamento de consultas. |
| **Stakeholder / Fonte** | Paciente (ST01) |
| **Necessidade relacionada** | N01 — Autonomia para escolher horários vagos online |
| **Prioridade** | Alta |

---

## RF04 — Cancelamento de agendamento

| Campo | Detalhe |
|---|---|
| **Descrição** | O sistema deve permitir o cancelamento do agendamento pelo paciente. |
| **Stakeholder / Fonte** | Paciente (ST01) |
| **Necessidade relacionada** | N08 — Cancelamento simplificado via plataforma |
| **Prioridade** | Alta |
| **Regra associada** | [RN02](regras-negocio.md#rn02) — cancelamento sem taxa até 24h antes |

---

## RF05 — Notificações de lembrete

| Campo | Detalhe |
|---|---|
| **Descrição** | O sistema deve enviar uma notificação por e-mail ou WhatsApp com o lembrete da consulta. |
| **Stakeholder / Fonte** | Paciente (ST01) |
| **Necessidade relacionada** | N02 — Lembretes automáticos sobre o dia e hora da consulta |
| **Prioridade** | Média |
| **Observação** | Requisito mais discutido pelo grupo — ver [Revisão e Checklist](revisao-e-checklist.md#reflexão-final-do-grupo). |

---

## RF06 — Visualização da agenda pelo médico

| Campo | Detalhe |
|---|---|
| **Descrição** | O sistema deve permitir que o médico visualize sua agenda diária de atendimentos. |
| **Stakeholder / Fonte** | Médico (ST03) |
| **Necessidade relacionada** | N05 — Acesso à agenda diária atualizada em tempo real |
| **Prioridade** | Alta |

---

## RF07 — Bloqueio de horários pela recepção

| Campo | Detalhe |
|---|---|
| **Descrição** | O sistema deve permitir que a recepcionista bloqueie horários na agenda dos médicos. |
| **Stakeholder / Fonte** | Recepcionista (ST02) |
| **Necessidade relacionada** | N03 — Bloqueio e liberação ágil de horários na agenda |
| **Prioridade** | Média |
| **Observação** | Requisito implícito, identificado apenas durante a discussão do grupo — não constava na entrevista inicial. |

---

## RF08 — Relatórios de consultas e faltas

| Campo | Detalhe |
|---|---|
| **Descrição** | O sistema deve gerar relatórios com o quantitativo de consultas e faltas por período. |
| **Stakeholder / Fonte** | Administrador (ST04) |
| **Necessidade relacionada** | N06 — Relatórios estatísticos de atendimento e absenteísmo |
| **Prioridade** | Baixa |

---

### Resumo

| ID | Requisito | Prioridade |
|---|---|---|
| RF01 | Cadastro e atualização de dados do paciente | Alta |
| RF02 | Consulta de horários disponíveis | Alta |
| RF03 | Agendamento de consultas | Alta |
| RF04 | Cancelamento de agendamento | Alta |
| RF05 | Notificações de lembrete | Média |
| RF06 | Visualização da agenda pelo médico | Alta |
| RF07 | Bloqueio de horários pela recepção | Média |
| RF08 | Relatórios de consultas e faltas | Baixa |

[Voltar ao README](../README.md) · [Próximo: Requisitos de Qualidade](requisitos-qualidade.md)

# Requisitos de Qualidade (RQ)

[Voltar ao README](../README.md)

Requisitos que definem **características mensuráveis e verificáveis** que o sistema deve apresentar, além de funcionar corretamente. Termos vagos (ex: "rápido", "seguro", "fácil de usar") foram eliminados na revisão por pares — ver [Revisão por pares](revisao-e-checklist.md).

---

## RQ01 — Desempenho

| Campo | Detalhe |
|---|---|
| **Requisito mensurável** | O sistema deve exibir os horários disponíveis em no máximo **2 segundos** para **95%** das requisições. |
| **Como verificar** | Testes de carga com **Apache JMeter**, simulando 100 acessos simultâneos. |
| **Requisito funcional relacionado** | [RF02](requisitos-funcionais.md#rf02--consulta-de-horários-disponíveis) |

---

## RQ02 — Segurança

| Campo | Detalhe |
|---|---|
| **Requisito mensurável** | O sistema deve armazenar senhas com algoritmo hash forte (**BCrypt**) e trafegar dados sob protocolo **HTTPS/TLS**. |
| **Como verificar** | Análise estática de código e inspeção de pacotes de rede via **Wireshark**. |
| **Restrição relacionada** | [RES03](restricoes.md#res03) — conformidade com a LGPD |

---

## RQ03 — Usabilidade / Interação

| Campo | Detalhe |
|---|---|
| **Requisito mensurável** | O sistema deve permitir que o agendamento da consulta seja concluído em no máximo **4 cliques** a partir da tela inicial. |
| **Como verificar** | Testes de usabilidade aplicados com amostragem de **10 usuários finais**. |
| **Requisito funcional relacionado** | [RF03](requisitos-funcionais.md#rf03--agendamento-de-consultas) |

---

## RQ04 — Confiabilidade

| Campo | Detalhe |
|---|---|
| **Requisito mensurável** | O sistema deve apresentar disponibilidade (*uptime*) mínima de **99%** no horário comercial. |
| **Como verificar** | Monitoramento automatizado com ferramentas de checagem contínua. |

---

## RQ05 — Compatibilidade / Portabilidade

| Campo | Detalhe |
|---|---|
| **Requisito mensurável** | O sistema deve ser responsivo e compatível com os navegadores **Chrome, Edge e Safari** (desktop e mobile). |
| **Como verificar** | Testes automatizados *cross-browser* em ambiente de homologação. |

---

### Resumo

| ID | Característica | Métrica-chave |
|---|---|---|
| RQ01 | Desempenho | ≤ 2s em 95% das requisições |
| RQ02 | Segurança | BCrypt + HTTPS/TLS |
| RQ03 | Usabilidade | ≤ 4 cliques |
| RQ04 | Confiabilidade | Uptime ≥ 99% |
| RQ05 | Compatibilidade | Chrome / Edge / Safari |

[Requisitos Funcionais](requisitos-funcionais.md) · [Voltar ao README](../README.md) · [Próximo: Restrições](restricoes.md)
