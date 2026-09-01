# Revisão por Pares e Checklist de Qualidade

[Voltar ao README](../README.md)

---

## Revisão por pares — Caça à ambiguidade

Os requisitos foram trocados com outro grupo em busca de termos vagos (*rápido, amigável, adequado, melhor, robusto, muitos, poucos, quando possível, se necessário*).

| ID | Problema encontrado | Sugestão do grupo revisor |
|---|---|---|
| 01 | Uso da expressão vaga **"resposta rápida do sistema"**. | Especificar o tempo mensurável: *"retorno da consulta em até 2 segundos para 95% das requisições"* → [RQ01](requisitos-qualidade.md#rq01--desempenho). |
| 02 | Uso do termo ambíguo **"sistema fácil de usar para todos"**. | Definir meta objetiva: *"permitir a realização da tarefa em no máximo 4 cliques a partir da tela inicial"* → [RQ03](requisitos-qualidade.md#rq03--usabilidade--interação). |

---

## Checklist de qualidade dos requisitos

| Pergunta | Status | Observação |
|---|:---:|---|
| O requisito está completo? | Sim | Todos os elementos essenciais foram detalhados. |
| Está correto em relação à necessidade do stakeholder? | Sim | Mapeado diretamente das necessidades do levantamento. |
| Descreve apenas uma capacidade ou característica? | Sim | Requisitos atômicos e isolados. |
| É necessário? | Sim | Alinhado à solução do problema principal. |
| É viável? | Sim | Compatível com as tecnologias e prazos propostos. |
| Possui prioridade? | Sim | Priorização categorizada (Alta/Média/Baixa). |
| Está livre de ambiguidades? | Sim | Ajustado e verificado na revisão por pares. |
| Pode ser verificado ou testado? | Sim | Critérios de aceitação mensuráveis e objetivos. |
| A fonte/stakeholder está identificada? | Sim | Rastreabilidade mantida do início ao fim. |

---

## Reflexão final do grupo

**Qual requisito gerou mais discussão durante o levantamento e por quê?**
O requisito [RF05](requisitos-funcionais.md#rf05--notificações-de-lembrete) (envio de notificações automáticas via WhatsApp/E-mail). A equipe debateu longamente se o envio por WhatsApp deveria ser tratado como indispensável (*Must Have*) na primeira entrega ou secundário (*Should Have*), considerando o custo de integração e a infraestrutura necessária.

**Qual necessidade do usuário inicialmente parecia simples, mas gerou vários requisitos?**
A necessidade do paciente de "agendar uma consulta". Essa solicitação atômica desdobrou-se em múltiplos requisitos: cadastro prévio de dados do usuário, busca com filtros por médico e especialidade, validação de disponibilidade e regras de não sobreposição.

**O grupo identificou algum requisito implícito que somente apareceu durante a discussão? Qual?**
Sim, o requisito de permissão para bloqueio manual de horários na agenda pelos recepcionistas ([RF07](requisitos-funcionais.md#rf07--bloqueio-de-horários-pela-recepção)). Essa necessidade não havia sido formalmente solicitada na entrevista inicial do paciente, mas se mostrou essencial para tratar emergências e ausências médicas não planejadas.

> **Orientação da etapa:** o foco não é projetar telas nem escolher tecnologias. O objetivo é compreender e registrar o que é necessário para resolver o problema, mantendo os requisitos claros, verificáveis e rastreáveis às necessidades dos stakeholders.

[Stakeholders](stakeholders.md) · [Voltar ao README](../README.md)
