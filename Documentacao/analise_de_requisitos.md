<div align="center">
  <h1>Análise de Requisitos</h1>
</div>

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
