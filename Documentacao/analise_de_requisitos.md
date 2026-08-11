# Ficha de Requisitos – FlowOps

## 2. Stakeholders Envolvidos

Os principais stakeholders do sistema são:

* **Stakeholder/Solicitante:** pessoa que solicita uma atividade ou demanda.
* **Gestor:** responsável por organizar e distribuir as atividades.
* **Desenvolvedor/Colaborador:** responsável pela execução das atividades.
* **Gestão da organização:** interessada nos resultados e indicadores das demandas.

---

## 3. Requisitos de Negócio

O sistema deve contribuir para:

* Centralizar as demandas em um único lugar;
* Melhorar a comunicação entre stakeholders, gestores e equipes;
* Reduzir o número de atividades esquecidas ou atrasadas;
* Melhorar a organização das tarefas;
* Facilitar o acompanhamento dos projetos;
* Aumentar a visibilidade sobre o trabalho da equipe;
* Melhorar o controle dos prazos e responsáveis.

---

## 4. Requisitos das Partes Interessadas

### 4.1 Stakeholder / Solicitante

O stakeholder precisa:

* Criar novas demandas;
* Informar a descrição da atividade;
* Informar o prazo da atividade;
* Definir a prioridade;
* Acompanhar o andamento;
* Saber quem é o responsável pela atividade;
* Adicionar comentários;
* Validar a atividade após sua conclusão.

### 4.2 Gestor

O gestor precisa:

* Visualizar as demandas da equipe;
* Distribuir atividades;
* Definir o responsável pela atividade através da matrícula;
* Acompanhar os prazos;
* Identificar atividades atrasadas;
* Visualizar a quantidade de tarefas de cada colaborador;
* Acompanhar o andamento geral das demandas;
* Reorganizar prioridades quando necessário.

### 4.3 Desenvolvedor / Colaborador

O colaborador precisa:

* Visualizar suas atividades;
* Saber o prazo de cada tarefa;
* Consultar a descrição da atividade;
* Identificar a prioridade;
* Atualizar o status;
* Adicionar comentários;
* Anexar arquivos quando necessário;
* Enviar a atividade para validação.

---

# 5. Requisitos da Solução

## 5.1 Requisitos Funcionais

### RF01 – Cadastro de usuários

O sistema deve permitir o cadastro dos usuários, incluindo informações como nome, matrícula, equipe e perfil de acesso.

### RF02 – Cadastro de demandas

O sistema deve permitir que o stakeholder cadastre uma nova demanda.

A demanda deverá conter informações como:

* Título;
* Descrição;
* Prioridade;
* Prazo;
* Solicitante;
* Responsável.

### RF03 – Definição de prioridade

O sistema deve permitir definir a prioridade da demanda.

As prioridades inicialmente serão:

* Crítica;
* Alta;
* Média;
* Baixa.

### RF04 – Definição de prazo

O sistema deve permitir definir uma data de entrega para cada demanda.

### RF05 – Distribuição de atividades

O gestor deve poder atribuir uma demanda a um colaborador utilizando sua matrícula.

### RF06 – Controle de status

O sistema deve permitir atualizar o status da demanda.

Os status inicialmente serão:

* A Fazer;
* Em Desenvolvimento;
* Em Teste;
* Em Validação;
* Concluído.

### RF07 – Acompanhamento

O stakeholder e o gestor devem conseguir acompanhar o andamento das demandas.

### RF08 – Comentários

Os usuários devem poder adicionar comentários nas demandas para facilitar a comunicação entre os envolvidos.

### RF09 – Anexos

O sistema deve permitir que os usuários anexem arquivos relacionados às demandas.

### RF10 – Histórico

O sistema deve registrar as principais alterações realizadas nas demandas, permitindo acompanhar o histórico da atividade.

### RF11 – Identificação de atrasos

O sistema deve identificar demandas que ultrapassaram o prazo de entrega.

### RF12 – Validação da atividade

O stakeholder deve poder aprovar ou solicitar ajustes em uma atividade enviada para validação.

### RF13 – Retorno para desenvolvimento

Caso uma atividade não seja aprovada pelo stakeholder, o sistema deve permitir que ela retorne para a etapa de desenvolvimento.

### RF14 – Visualização das demandas

O sistema deve apresentar as demandas em um quadro visual, permitindo identificar facilmente o status de cada atividade.

---

## 5.2 Requisitos Não Funcionais

### RNF01 – Usabilidade

O sistema deve possuir uma interface simples e fácil de entender, permitindo que os usuários encontrem as informações necessárias sem dificuldade.

### RNF02 – Responsividade

O sistema deve funcionar adequadamente em computadores, tablets e celulares.

### RNF03 – Segurança

Cada usuário deve ter acesso somente às funcionalidades permitidas para seu perfil.

### RNF04 – Desempenho

As principais páginas do sistema devem carregar rapidamente e apresentar uma boa experiência para o usuário.

### RNF05 – Disponibilidade

O sistema deve estar disponível para utilização durante o horário de funcionamento da organização.

### RNF06 – Manutenibilidade

O sistema deve ser desenvolvido de forma organizada, facilitando futuras correções e melhorias.

---

## 5.3 Requisitos de Transição

### RT01 – Cadastro inicial

Na implantação do sistema, os usuários e suas respectivas matrículas deverão ser cadastrados.

### RT02 – Cadastro das equipes

As equipes e seus respectivos gestores deverão ser cadastrados antes da utilização do sistema.

### RT03 – Migração de demandas

Caso a equipe utilize planilhas ou outro sistema anteriormente, as demandas existentes poderão ser cadastradas ou migradas para o FlowOps.

### RT04 – Treinamento dos usuários

Os usuários deverão receber orientações básicas sobre a utilização do sistema antes da implantação.

---

# 6. Priorização

Os requisitos serão classificados em três níveis: **Essenciais, Importantes e Desejáveis**.

## 6.1 Essenciais

São os requisitos necessários para que a primeira versão do sistema funcione.

* Cadastro de usuários;
* Cadastro de demandas;
* Definição de responsável;
* Definição de prazo;
* Definição de prioridade;
* Controle de status;
* Visualização das demandas;
* Identificação de atividades atrasadas;
* Acompanhamento das demandas;
* Validação das atividades.

## 6.2 Importantes

São funcionalidades que melhoram a utilização do sistema, mas não são obrigatórias para a primeira versão.

* Comentários;
* Histórico;
* Anexos;
* Dashboard;
* Controle de equipes;
* Filtros de demandas;
* Indicadores de desempenho.

## 6.3 Desejáveis

São funcionalidades que podem ser desenvolvidas futuramente.

* Notificações automáticas;
* Integração com outras ferramentas;
* Relatórios avançados;
* Integração com e-mail;
* Integração com Microsoft Teams;
* Integração com Slack;
* Sugestão automática de responsáveis;
* Recursos de inteligência artificial;
* Previsão de possíveis atrasos.

---

# 7. Solução Proposta

A solução proposta é o **FlowOps**, um sistema web para gerenciamento de demandas e atividades.

O sistema permitirá que os stakeholders cadastrem solicitações, que os gestores distribuam as atividades para os responsáveis e que os colaboradores acompanhem e atualizem o andamento das tarefas.

A utilização de um quadro Kanban permitirá visualizar facilmente em qual etapa cada atividade se encontra.

O fluxo principal do sistema será:

```text
Stakeholder
     ↓
Cria uma demanda
     ↓
Gestor recebe e organiza
     ↓
Define o responsável
     ↓
Colaborador executa
     ↓
Em Desenvolvimento
     ↓
Em Teste
     ↓
Em Validação
     ↓
Stakeholder aprova
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
      ↓
Em Teste
      ↓
Em Validação
```

---

# 8. Justificativa

O FlowOps busca solucionar um problema comum nas equipes: a falta de organização e visibilidade das demandas.

Ao centralizar as atividades em um único sistema, cada demanda terá um responsável, uma prioridade e um prazo definido.

Isso facilita o trabalho dos colaboradores, permite que os gestores acompanhem melhor suas equipes e dá aos stakeholders uma visão mais clara sobre o andamento de suas solicitações.

A solução também permite manter um histórico das atividades, tornando o processo mais organizado e transparente.

Dessa forma, o sistema busca reduzir problemas de comunicação, diminuir o número de atividades esquecidas e facilitar o acompanhamento dos projetos.

---

# 9. Resumo da Solução

O FlowOps tem como principal proposta organizar o caminho de uma demanda desde sua solicitação até sua conclusão.

A ideia é que todos os envolvidos tenham acesso às informações necessárias e saibam exatamente qual é a situação de cada atividade.

Em resumo:

**Stakeholder solicita → Gestor distribui → Colaborador executa → Stakeholder valida → Demanda é concluída.**

O sistema pretende tornar esse processo mais simples, organizado e transparente.
