# Requisitos de Qualidade (RQ)

[Voltar ao README](../readme.md)

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

### **Resumo**

| ID | Característica | Métrica-chave |
|---|---|---|
| RQ01 | Desempenho | ≤ 2s em 95% das requisições |
| RQ02 | Segurança | BCrypt + HTTPS/TLS |
| RQ03 | Usabilidade | ≤ 4 cliques |
| RQ04 | Confiabilidade | Uptime ≥ 99% |
| RQ05 | Compatibilidade | Chrome / Edge / Safari |

[Requisitos Funcionais](requisitos-funcionais.md) · [Voltar ao README](../README.md) · [Próximo: Restrições](restricoes.md)
