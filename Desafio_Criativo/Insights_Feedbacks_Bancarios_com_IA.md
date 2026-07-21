# 🎯 Desafio Criativo: Extraindo Insights de Feedbacks Bancários com IA

Repositório criado para a entrega do desafio de Prompt Engineering do curso da DIO.

## 📌 Objetivo do Prompt
Orientar um modelo de IA a analisar dados brutos de comentários e notas de clientes bancários, transformando-os em um relatório executivo com tabela estruturada e priorização de ações para o time de CX/Produto.

---

## 🧱 Construção do Prompt

### 1. Intenção
Analisar comentários e notas de satisfação dos canais digitais bancários para subsidiar reuniões de priorização do backlog de melhorias.

### 2. Contexto e Limitações
- **Contexto:** Ambientes de App, Pix e Chat.
- **Segurança:** Ocultação de dados sensíveis (PII) e proibição de alucinação/invenção de dados.
- **Estilo:** Executivo e focado em tomada de decisão.

---

## 🚀 Prompt Final

> **Papel:** Analista Senior de Experiência do Cliente (CX) e Analista de Dados.  
> **Tarefa:** Analisar feedbacks de clientes bancários (Pix, App, Cartões, Chat)...  
Atue como Analista Senior de Experiência do Cliente (CX) e Analista de Dados em um banco digital.

Sua tarefa é analisar uma base de feedbacks de clientes sobre canais digitais (aplicativo, Pix, cartão de crédito e atendimento por chat) para identificar padrões de insatisfação, elogios recorrentes e oportunidades prioritárias de melhoria.

Contexto:
A análise será utilizada pela equipe de Produto e CX para apoiar a decisão de priorização do backlog de desenvolvimento do aplicativo e treinar a equipe de atendimento, visando aumentar o NPS e reduzir a taxa de contatos no suporte.

Dados disponíveis:
Serão fornecidos registros em texto com os seguintes campos: Data do comentário, Canal de origem, Texto do feedback, Produto/Serviço citado e Nota de satisfação (1 a 5).

Instruções de análise:
1. Classifique os feedbacks por Tema principal, Sentimento (Positivo, Neutro, Negativo) e Nível de Urgência (Baixo, Médio, Alto).
2. Identifique os principais gargalos e pontos fortes expressos pelos clientes.
3. Aponte evidências diretamente extraídas dos textos dos comentários (sem expor dados pessoais).
4. Sugira ações práticas e acionáveis divididas por área responsável (Ex: Time de TI/App vs. Time de Atendimento).

Formato da resposta:
- Resumo Executivo: Um texto sucinto (até 5 linhas) destacando a visão geral do sentimento do cliente.
- Tabela de Insights: Contendo as colunas [Produto/Serviço] | [Tema] | [Sentimento] | [Evidência/Trecho] | [Ação Sugerida].
- Plano de Ação (Top 3 Prioridades): Lista priorizada das 3 ações mais urgentes com base no impacto e volume dos problemas apontados.

Restrições e Cuidados:
- Use estritamente os dados fornecidos no input; não invente métricas, estatísticas ou causais que não estejam explícitas.
- Mascare ou omita qualquer dado pessoal sensível (como nomes, CPF, e-mail ou números de conta) caso apareçam no texto do feedback.
- Se a base fornecida for insuficiente para tirar uma conclusão segura sobre determinado tema, declare expressamente essa limitação.
- Use linguagem executiva, objetiva, clara e focada em tomada de decisão.

---
