# Regras de Negócio (RN)

[Voltar ao README](../readme.md)

Políticas e normas do domínio que definem ou restringem o comportamento do negócio, independentemente da implementação técnica.

---

## RN01 — Proibição de horários coincidentes

| Campo | Detalhe |
|---|---|
| **Regra** | Um paciente não pode agendar duas consultas com horários coincidentes na mesma clínica. |
| **Fonte** | Política da clínica / Administrador (ST04) |
| **Requisito relacionado** | [RF03 — Agendamento de consultas](requisitos-funcionais.md#rf03--agendamento-de-consultas) |

---

## RN02 — Prazo de cancelamento sem taxa

| Campo | Detalhe |
|---|---|
| **Regra** | O cancelamento sem cobrança de taxa de retenção deve ser efetuado em até **24 horas** antes do horário agendado. |
| **Fonte** | Regulamento interno da clínica / Administrador (ST04) |
| **Requisito relacionado** | [RF04 — Cancelamento de agendamento](requisitos-funcionais.md#rf04--cancelamento-de-agendamento) |

---

## RN03 — Cadastro ativo obrigatório

| Campo | Detalhe |
|---|---|
| **Regra** | Apenas pacientes com cadastro ativo e dados de contato válidos (e-mail/telefone) podem realizar marcações online. |
| **Fonte** | Diretriz operacional da recepção / Recepcionista (ST02) |
| **Requisito relacionado** | [RF01 — Cadastro e atualização de dados do paciente](requisitos-funcionais.md#rf01--cadastro-e-atualização-de-dados-do-paciente) |

---

### Resumo

| ID | Regra de negócio | Fonte |
|---|---|---|
| RN01 | Sem horários coincidentes por paciente | Administrador |
| RN02 | Cancelamento gratuito até 24h antes | Administrador |
| RN03 | Cadastro ativo obrigatório para marcação online | Recepcionista |

[Restrições](restricoes.md) · [Voltar ao README](../README.md) · [Próximo: Stakeholders](stakeholders.md)
