# 🎯 Desafio Criativo: Extraindo Insights do Feedback de Clientes Bancários

## 📌 Sobre o desafio

Este repositório contém a resolução do Desafio Criativo da DIO, cujo objetivo é construir um prompt estruturado para que uma IA possa extrair insights acionáveis a partir de feedbacks de clientes bancários, respeitando critérios de análise e cuidados com dados sensíveis (LGPD).

---

## 🧱 Passo 1 — Intenção

Quero que a IA analise **comentários de clientes bancários sobre aplicativo, Pix, cartão de crédito e atendimento por chat** para identificar **temas recorrentes, sentimento dos clientes, reclamações, elogios e oportunidades de melhoria**.

O resultado será usado por **uma equipe de experiência do cliente (CX)** para apoiar **a priorização de melhorias nos canais digitais e a redução de atritos no atendimento**.

A entrega deve conter **um resumo executivo, uma tabela com os principais temas (tema, sentimento, evidência e ação sugerida) e uma lista com as 3 prioridades mais importantes**.

O resultado será considerado bom se for **claro, organizado, baseado apenas nos comentários fornecidos, com evidências reais e útil para priorizar ações**.

---

## 🧱 Passo 2 — Contexto e Restrições

**Contexto:** Estou trabalhando com feedbacks de clientes bancários relacionados ao aplicativo, Pix, cartão de crédito e atendimento por chat.

**Dados disponíveis:** A base contém data do comentário, canal de atendimento, texto do feedback, produto citado e nota de satisfação de 1 a 5.

**Critérios de análise:** A IA deve classificar os feedbacks por tema, sentimento, urgência e produto citado, além de estimar o possível impacto na experiência do cliente.

**Cuidados e restrições:**

- Use apenas os dados fornecidos.
- Não invente números, causas ou conclusões.
- Não exponha dados pessoais ou sensíveis (nomes, CPF, conta, agência).
- Se houver informação insuficiente, indique a limitação.
- Use linguagem simples, direta e voltada para tomada de decisão.

---

## 🧱 Passo 3 — Prompt Final Refinado

```text
Atue como analista de dados e experiência do cliente em um banco.

Sua tarefa é analisar feedbacks de clientes sobre aplicativo bancário, Pix, cartão de crédito e atendimento por chat para identificar temas recorrentes, sentimento dos clientes e oportunidades de melhoria.

Contexto: A análise será usada por uma equipe de experiência do cliente para priorizar melhorias nos canais digitais e reduzir atritos no atendimento. O foco é transformar comentários soltos em insights claros e acionáveis.

Dados disponíveis: Serão fornecidos comentários com data, canal de atendimento, texto do feedback, produto citado e nota de satisfação de 1 a 5.

Instruções de análise:
1. Classifique os feedbacks por tema, sentimento, urgência e produto citado.
2. Identifique os principais padrões, problemas, elogios e oportunidades.
3. Aponte evidências nos dados fornecidos, usando exemplos curtos de comentários.
4. Sugira ações práticas para a equipe de experiência do cliente e para o time responsável pelos canais digitais.

Formato da resposta:
- Resumo executivo com até 5 linhas.
- Tabela com as colunas: Tema | Sentimento | Evidência | Ação sugerida.
- Lista final com as 3 prioridades mais importantes.

Restrições:
- Use apenas os dados fornecidos.
- Não invente números, causas ou conclusões.
- Não exponha dados pessoais ou sensíveis.
- Informe limitações quando os dados não forem suficientes.
- Use linguagem simples, direta e voltada para tomada de decisão.

Feedbacks a analisar:
[INSIRA AQUI OS COMENTÁRIOS]
