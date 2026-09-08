# Avaliação e Especificação de Qualidade de Software — ISO/IEC 25010:2023

**Instituição:** CEUB — Centro Universitário de Brasília  
**Curso:** Engenharia de Software  
**Disciplina:** Engenharia de Requisitos  
**Docente:** Profª Kadidja Valéria  
**Tema:** Modelo de Qualidade de Produto da ISO/IEC 25010:2023  

---

## 📋 Sumário
1. [Visão Geral](#1-visão-geral)
2. [Requisitos de Qualidade Especificados (RQ01 a RQ05)](#2-requisitos-de-qualidade-especificados-rq01-a-rq05)
3. [Atividade Prática — Avaliação do Sistema Acadêmico](#3-atividade-prática--avaliação-do-sistema-acadêmico)
4. [Análise de Conflitos de Qualidade (*Trade-offs*)](#4-análise-de-conflitos-de-qualidade-trade-offs)
5. [Gabarito dos Exercícios de Revisão](#5-gabarito-dos-exercícios-de-revisão)

---

## 1. Visão Geral

Este repositório/documento consolida as especificações de requisitos de qualidade, resolução do estudo de caso acadêmico e análise crítica de qualidade de software fundamentados no padrão internacional **ISO/IEC 25010:2023** (*Systems and software engineering — Systems and software Quality Requirements and Evaluation - SQuaRE*).

A edição de 2023 da norma estabelece **9 características principais** para a qualidade do produto de software:
- **Adequação funcional** (*Functional suitability*)
- **Eficiência de desempenho** (*Performance efficiency*)
- **Compatibilidade** (*Compatibility*)
- **Capacidade de interação** (*Interaction capability*)
- **Confiabilidade** (*Reliability*)
- **Segurança** (*Security*)
- **Manutenibilidade** (*Maintainability*)
- **Flexibilidade** (*Flexibility*)
- **Proteção contra riscos** (*Safety*)

---

## 2. Requisitos de Qualidade Especificados (RQ01 a RQ05)

Abaixo constam os Requisitos de Qualidade (RQ) padronizados e revisados segundo a estrutura recomendada pela ISO/IEC 25010:2023:  
`O sistema deverá [comportamento/propriedade], sob [condições], atingindo [limite/valor], verificado por [método].`

### RQ01 — Eficiência de Desempenho
* **Característica (ISO 25010:2023):** Eficiência de desempenho
* **Requisito mensurável:** O sistema deverá exibir os horários disponíveis em até **2 segundos**, sob carga de **100 acessos simultâneos**, atingindo a meta em no mínimo **95%** das requisições.
* **Método de verificação:** Testes de carga automatizados via **Apache JMeter** ou K6.
* **Relação:** [RF02 — Consulta de horários disponíveis]

### RQ02 — Segurança
* **Característica (ISO 25010:2023):** Segurança
* **Requisito mensurável:** O sistema deverá proteger a confidencialidade e integridade dos dados armazenando senhas com hash forte (**BCrypt**) e trafegando todas as informações sob protocolo **HTTPS/TLS 1.3**.
* **Método de verificação:** Análise estática de código (SAST - SonarQube) e inspeção de tráfego de rede via **Wireshark**.
* **Relação:** [RES03 — Conformidade com a LGPD]

### RQ03 — Capacidade de Interação
* **Característica (ISO 25010:2023):** Capacidade de interação
* **Requisito mensurável:** O sistema deverá permitir que o agendamento de consulta seja concluído em no máximo **4 cliques** a partir da tela inicial, em fluxo contínuo.
* **Método de verificação:** Testes de usabilidade aplicados com amostragem representativa de **10 usuários finais**.
* **Relação:** [RF03 — Agendamento de consultas]

### RQ04 — Confiabilidade
* **Característica (ISO 25010:2023):** Confiabilidade
* **Requisito mensurável:** O sistema deverá apresentar disponibilidade (*uptime*) mínima de **99%** durante o horário comercial de funcionamento (08h às 18h).
* **Método de verificação:** Monitoramento automatizado contínuo com ferramentas de checagem de disponibilidade (ex: Zabbix, Datadog).

### RQ05 — Flexibilidade
* **Característica (ISO 25010:2023):** Flexibilidade (Adaptabilidade e Portabilidade)
* **Requisito mensurável:** O sistema deverá ser totalmente responsivo e compatível com os navegadores **Google Chrome, Microsoft Edge e Apple Safari** (ambientes desktop e mobile).
* **Método de verificação:** Testes automatizados *cross-browser* em ambiente de homologação (ex: BrowserStack, Selenium).

---

### Resumo Matricial dos RQs

| ID | Característica (ISO/IEC 25010:2023) | Métrica-Chave | Método de Avaliação |
|---|---|---|---|
| **RQ01** | Eficiência de Desempenho | Tempo de resposta ≤ 2s em 95% das requisições | Testes de Carga (JMeter) |
| **RQ02** | Segurança | Hash BCrypt + Protocolo HTTPS/TLS 1.3 | Análise SAST + Wireshark |
| **RQ03** | Capacidade de Interação | Conclusão do fluxo em ≤ 4 cliques | Teste de Usabilidade (10 usuários) |
| **RQ04** | Confiabilidade | Disponibilidade (*uptime*) ≥ 99% em horário comercial | Monitoramento Contínuo |
| **RQ05** | Flexibilidade | Compatibilidade total com Chrome, Edge e Safari | Testes Automatizados Cross-Browser |

---

## 3. Atividade Prática — Avaliação do Sistema Acadêmico

Tabela de análise de qualidade referente ao estudo de caso de lançamento do aplicativo acadêmico (Seção 8 do material de apoio):

| Nº | Ocorrência | Característica Predominante | Justificativa | Requisito de Qualidade Mensurável | Critério de Aceitação | Teste ou Avaliação |
|--:|---|---|---|---|---|---|
| **1** | O cálculo da média final apresenta valores incorretos. | **Adequação funcional** | O sistema executa a função principal, mas gera resultados matematicamente incorretos. | O sistema deverá calcular a média final das disciplinas aplicando 100% das regras acadêmicas oficiais. | 0% de divergência entre a média calculada e a regra oficial em 1.000 simulações. | Testes unitários e de integração automatizados. |
| **2** | A página de notas demora aproximadamente 12 segundos para abrir. | **Eficiência de desempenho** | O tempo de resposta de 12s degrada severeamente a experiência do usuário. | O sistema deverá exibir a página de notas em até 2 segundos sob condições normais de uso. | Tempo médio de resposta ≤ 2,0s para 95% das requisições. | Testes de desempenho e tempo de resposta via JMeter. |
| **3** | Estudantes têm dificuldade para localizar a renovação de matrícula. | **Capacidade de interação** | A interface carece de clareza na navegabilidade e aprendizabilidade para funções críticas. | O sistema deverá permitir localizar o menu de renovação de matrícula em até 2 cliques a partir da home. | Pelo menos 90% dos usuários concluem a navegação em até 1 minuto sem auxílio. | Testes de usabilidade com observação direta de usuários. |
| **4** | O aplicativo deixa de funcionar quando muitos usuários acessam simultaneamente. | **Confiabilidade** (e Eficiência de Desempenho) | O sistema perde a disponibilidade e colapsa sob carga de acessos concorrentes. | O sistema deverá manter a operação normal suportando até 5.000 usuários simultâneos no período de matrículas. | Taxa de erro HTTP 5xx < 0,1% durante o pico simulação de carga. | Teste de estresse e capacidade (*Stress Testing*). |
| **5** | Um estudante conseguiu visualizar o histórico de outro usuário. | **Segurança** | Ocorre violação crítica de confidencialidade e falha grave no controle de acesso (IDOR). | O sistema deverá restringir a exibição do histórico acadêmico exclusivamente ao estudante dono da conta. | Zero ocorrências de acesso cruzado a dados de terceiros em testes de bypass de autorização. | Análise SAST, DAST e Teste de Penetração (*Pentest*). |
| **6** | Uma pequena alteração no cadastro provocou falhas em outros módulos. | **Manutenibilidade** | Acoplamento excessivo do código faz com que mudanças locais gerem efeitos colaterais indesejados. | O sistema deverá possuir arquitetura modular com componentes desacoplados. | 100% de aprovação na suíte de testes de regressão após alterações no módulo de cadastro. | Testes de regressão automatizados e análise estática de código (SonarQube). |
| **7** | O aplicativo não consegue importar informações do sistema financeiro. | **Compatibilidade** | O software é incapaz de realizar troca de dados e interoperar com sistemas legados/externos. | O sistema deverá comunicar-se com o sistema financeiro via API RESTful para sincronização contínua de dados. | Taxa de sucesso na importação e sincronização de dados ≥ 99,9%. | Testes de integração de API e validação de payload JSON/XML. |
| **8** | A implantação em um novo servidor exige diversas alterações manuais. | **Flexibilidade** (Instalabilidade / Adaptabilidade) | Alta complexidade de implantação e dependência de procedimentos manuais sujeitos a erro humano. | O sistema deverá permitir sua implantação automatizada via contêineres Docker em qualquer servidor homologado. | Implantação 100% concluída via pipeline CI/CD sem necessidade de passos manuais. | Teste de implantação (*Deployment Test*) automatizado. |
| **9** | Em funcionalidade de laboratório, equipamento é acionado mesmo com sensor informando condição insegura. | **Proteção contra riscos (*Safety*)** | Falha grave de segurança operacional que pode acarretar danos físicos a pessoas, patrimônio ou ambiente. | O sistema deverá interromper e bloquear o acionamento de equipamentos quando o sensor registrar estado inseguro. | 100% de bloqueios efetivos do acionamento em simulações de sinal de alerta dos sensores. | Testes de segurança operacional (*Safety Testing*) e simulação de sinais de erro de hardware. |

---

## 4. Análise de Conflitos de Qualidade (*Trade-offs*)

### 1. Impacto da Segurança na Eficiência de Desempenho
A adição de verificações rigorosas de segurança (ex: criptografia forte, validações de *token* JWT, inspeção *deep packet*, WAF) adiciona tempo de processamento (*overhead* de CPU e memória) e pode elevar a latência do tempo de resposta.  
* **Solução:** Aplicar mecanismos de *caching* para autorizações, otimizar algoritmos criptográficos em hardware e utilizar arquitetura distribuída.

### 2. Impacto da Segurança na Capacidade de Interação (Usabilidade)
A exigência de múltiplos fatores de autenticação (MFA), *captchas* frequentes e expiração curta de sessão aumenta a proteção, mas introduz atrito na experiência do usuário (*UX*).  
* **Solução:** Adotar autenticação adaptativa (*Risk-Based Authentication*), biometria em dispositivos móveis e suporte a *Single Sign-On* (SSO).

### 3. Impacto da Flexibilidade na Manutenibilidade
Projetar uma arquitetura extremamente flexível (ex: microsserviços altamente configuráveis, múltiplos pontos de extensão e parametrização dinâmica) aumenta substancialmente a complexidade do sistema, tornando a manutenção e o rastreio de erros mais complexos.  
* **Solução:** Equilibrar abstrações com simplicidade (*Keep It Simple, Stupid - KISS*) e manter documentação e testes automatizados abrangentes.

### 4. Impactos da Confiabilidade por Redundância
Aumentar a confiabilidade via redundância (servidores espelhados, múltiplos bancos de dados replicados, balanceadores de carga) eleva os custos financeiros de infraestrutura e a complexidade de sincronização e consistência dos dados.  
* **Solução:** Definir acordos de nível de serviço (SLA) realistas alinhados às necessidades reais do negócio para evitar *over-engineering*.

### 5. Priorização de Características de Qualidade
A equipe de engenharia de software deve priorizar as características de qualidade com base em:
1. **Análise de riscos do domínio de negócio** (ex: sistemas hospitalares priorizam *Safety*; bancários priorizam *Segurança* e *Confiabilidade*);
2. **Requisitos das partes interessadas (*stakeholders*)**;
3. **Restrições orçamentárias e temporais do projeto**.

---

## 5. Gabarito dos Exercícios de Revisão

### Respostas Múltipla Escolha
* **Questão 1:** **B. Eficiência de desempenho** (Tempo de resposta excessivo de 20s indica gargalo de desempenho).
* **Questão 2:** **A. Compatibilidade** (Interoperabilidade e capacidade de troca de dados com outros sistemas).
* **Questão 3:** **D. A consulta deve ser concluída em até dois segundos para 95% das requisições.** (Apresenta limite, métrica e condição verificável).
* **Questão 4:** **B. Manutenibilidade** (Facilidade de analisar, modificar e testar componentes).
* **Questão 5:** **C. Proteção contra riscos (*Safety*)** (Prevenção de danos físicos e situações perigosas para pessoas/pacientes).

### Questão 6 — Produção Textual Exemplar

* **Característica escolhida:** Confiabilidade
1. **Requisito vago:** *"O sistema deve ser altamente disponível e não pode cair."*
2. **Requisito mensurável:** *"O sistema deverá manter um nível de disponibilidade (uptime) de 99,5% no período das 07:00 às 22:00 de segunda a sábado, com tempo máximo de recuperação após falhas (MTTR) de até 15 minutos."*
3. **Critério de aceitação:** *"Relatórios de monitoramento mensal comprovando uptime ≥ 99,5% e nenhum incidente de indisponibilidade não planejada superior a 15 minutos."*
4. **Estratégia de teste:** *"Execução de testes de resiliência e engenharia do caos (Chaos Engineering), simulando a queda de nós do servidor principal para validar a transição automática para o ambiente de failover."*

---
