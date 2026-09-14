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

---

# 2️⃣ ARQUIVO: `base-feedbacks-ficticios.md`

**Mensagem de commit:** `Adiciona base de feedbacks fictícios`

```markdown
# 📊 Base de Feedbacks Fictícios — Teste do Prompt

> ⚠️ **Aviso:** Todos os feedbacks abaixo são **100% fictícios**. Nenhum dado real de cliente, nome, CPF, conta ou agência foi utilizado. Uso seguro para testes de IA e em conformidade com a LGPD.

## 🎯 Objetivo

Validar o prompt criado no desafio, testando:

- Diferentes **temas** (Pix, Cartão, App, Atendimento, Segurança, Crédito, Investimentos)
- Diferentes **sentimentos** (positivo, neutro, negativo)
- Diferentes **níveis de urgência**
- Diferentes **canais** (Chat, SAC, App Store, Reclame Aqui)
- **Notas de satisfação** de 1 a 5

## 📋 Feedbacks

Formato: `Data | Canal | Produto | Nota | Comentário`

```text
01/03/2025 | Chat | Pix | 2 | "O app trava toda vez que tento fazer um Pix acima de R$ 500. Já é a terceira vez essa semana."
02/03/2025 | App Store | Cartão | 5 | "Adorei a nova função de cartão virtual, muito prático!"
02/03/2025 | Chat | Atendimento | 2 | "O atendimento por chat demora muito para responder. Fiquei 20 minutos esperando."
03/03/2025 | SAC | Cartão | 3 | "Não consigo aumentar o limite do cartão pelo app, tenho que ligar. Muito ruim."
03/03/2025 | App Store | Pix | 5 | "O Pix está funcionando perfeitamente, muito rápido. Parabéns!"
04/03/2025 | Chat | Cartão | 1 | "Tentei cancelar um cartão e o app não deixa. Péssimo."
04/03/2025 | Reclame Aqui | App | 1 | "O app caiu quando fui pagar um boleto. Tive que refazer tudo."
05/03/2025 | SAC | Atendimento | 3 | "Atendimento educado, mas resolveu meu problema só na segunda tentativa."
05/03/2025 | App Store | Pix | 5 | "A funcionalidade de Pix agendado é ótima, uso toda semana."
06/03/2025 | Chat | Cartão | 2 | "Não recebo notificação de compras no cartão. Já perdi tempo conferindo."
06/03/2025 | Reclame Aqui | Segurança | 1 | "Recebi um SMS suspeito pedindo meus dados. Fiquei com medo de golpe."
07/03/2025 | Chat | App | 2 | "A tela de login demora muito para carregar. Já desisti de entrar algumas vezes."
07/03/2025 | SAC | Crédito | 3 | "Pedi um empréstimo e não tive retorno sobre a aprovação. Fiquei no escuro."
08/03/2025 | App Store | App | 5 | "Interface nova ficou linda e mais fácil de usar. Parabéns ao time!"
08/03/2025 | Chat | Pix | 4 | "Pix funcionou bem, mas queria poder agendar para vários dias de uma vez."
09/03/2025 | Reclame Aqui | Atendimento | 1 | "Liguei 4 vezes e cada atendente pediu a mesma informação. Ninguém resolveu."
09/03/2025 | SAC | Cartão | 2 | "A fatura veio com cobrança que não reconheço. Preciso de ajuda urgente."
10/03/2025 | App Store | Investimentos | 5 | "A área de investimentos ficou bem mais clara. Consegui aplicar sozinho."
10/03/2025 | Chat | App | 3 | "O app é bom, mas consome muita bateria do celular."
11/03/2025 | SAC | Segurança | 2 | "Não recebo alerta quando alguém tenta acessar minha conta de outro dispositivo."

12/03/2025 | Chat | Pix | 3 | "Pix é ok. Nada demais, nada de menos."
12/03/2025 | SAC | Cartão | 2 | "Melhoraram o app mas o cartão continua ruim. Vai entender."
13/03/2025 | Reclame Aqui | Atendimento | 1 | "Atendimento ruim. App ruim. Banco ruim. Tudo ruim."
13/03/2025 | App Store | App | 4 | "Bom, mas trava às vezes quando tem muita gente usando."
14/03/2025 | Chat | Segurança | 2 | "Acho que clonaram meu cartão. Não sei como. Preciso resolver."
14/03/2025 | SAC | Crédito | 3 | "Queria saber se meu limite aumentou, mas ninguém me responde." 
