# Matriz de Rastreabilidade

[Voltar ao README](../readme.md)

Relaciona cada requisito à sua necessidade de origem e ao stakeholder correspondente, garantindo rastreabilidade do início ao fim do processo de levantamento.

| ID | Descrição | Tipo | Stakeholder/Fonte | Prioridade |
|---|---|---|---|---|
| [RF01](requisitos-funcionais.md#rf01--cadastro-e-atualização-de-dados-do-paciente) | Permitir cadastro e atualização de dados do paciente. | Funcional | ST01 – Paciente | Alta |
| [RF02](requisitos-funcionais.md#rf02--consulta-de-horários-disponíveis) | Permitir consulta de horários vagos por médico/especialidade. | Funcional | ST01 – Paciente | Alta |
| [RF03](requisitos-funcionais.md#rf03--agendamento-de-consultas) | Permitir agendamento de consultas médicas. | Funcional | ST01 – Paciente | Alta |
| [RF04](requisitos-funcionais.md#rf04--cancelamento-de-agendamento) | Permitir o cancelamento de agendamentos. | Funcional | ST01 – Paciente | Alta |
| [RF05](requisitos-funcionais.md#rf05--notificações-de-lembrete) | Enviar lembretes e confirmações por WhatsApp/E-mail. | Funcional / Qualidade / Restrição | ST01 – Paciente | Média |
| [RF06](requisitos-funcionais.md#rf06--visualização-da-agenda-pelo-médico) | Permitir visualização da agenda diária pelo médico. | Funcional / Qualidade / Restrição | ST03 – Médico | Alta |
| [RQ01](requisitos-qualidade.md#rq01--desempenho) | Retornar resultado da consulta em até 2 segundos. | Funcional / Qualidade / Restrição | ST01 – Paciente | Alta |
| [RQ02](requisitos-qualidade.md#rq02--segurança) | Criptografar senhas e dados confidenciais (BCrypt e HTTPS). | Funcional / Qualidade / Restrição | ST05 – Equipe de TI | Alta |
| [RQ03](requisitos-qualidade.md#rq03--usabilidade--interação) | Atendimento rigoroso aos termos legais da LGPD. | Funcional / Qualidade / Restrição | ST04 – Administrador | Alta |
| [RN01](regras-negocio.md#rn01--proibição-de-horários-coincidentes) | Proibição de marcações simultâneas para o mesmo paciente. | Regra de Negócio | ST04 – Administrador | Alta |

[Stakeholders](stakeholders.md) · [Voltar ao README](../README.md)
