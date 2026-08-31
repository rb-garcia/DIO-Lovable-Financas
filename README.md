# DIO-Lovable-Financas
DIO-Lovable-Financas

# Prompt Otimizado
# App: Finanças Pessoais Conversacional

## Conceito
Controle financeiro 100% via chat com IA. Sem formulários manuais.
Público: iniciantes em organização financeira.

## Funcionalidades
1. Registro de gastos via chat (linguagem natural)
2. Classificação automática de transações
3. Metas financeiras com acompanhamento
4. "Agente Financeiro": dicas e planos de economia personalizados
5. Relatórios simples e personalizados

## Entregável
Plano de MVP em português contendo:
- Telas principais
- Recursos técnicos necessários
- Esboço de validação inicial

## Recomendação de uso no Lovable
- Primeiro prompt (mais caro): usar a versão otimizada como prompt inicial completo
- Itegrações seguintes: nunca reenviar o contexto completo. Utilizar comandos incrementais curtos
- Versão parametrizada: para reutilizar em outros apps conversacionais
- O prompt criado foi otimizado para entregar 100% dos requisitos funcionais

# Resumo Finanças Pessoais Conversacional

## Visão
App de controle financeiro onde toda a interação acontece por chat com IA: o usuário escreve "gastei 45 no mercado" e o app registra, classifica e responde com insights. Público: iniciantes em organização financeira.

## Telas Principais
- Chat (tela principal) — conversa com o Agente Financeiro; registra gastos/receitas, responde perguntas ("quanto gastei com comida esse mês?"), envia dicas proativas. Inclui chips de ações rápidas ("Registrar gasto", "Ver resumo", "Minhas metas")
- Dashboard / Resumo — visão do mês: total gasto, receitas, saldo, gráfico por categoria, comparativo com mês anterior
- Transações — lista do histórico classificado por categoria, com edição simples (corrigir categoria/valor quando a IA errar)
- Metas — criar e acompanhar metas ("guardar R$ 500/mês", "reduzir delivery em 30%") com barra de progresso e alertas no chat
- Relatórios — relatório mensal simples gerado pela IA em linguagem natural, com opção de pedir recortes ("relatório só de transporte")
- Onboarding + Login — cadastro e um breve questionário via chat (renda, principais gastos, objetivo) para personalizar o agente

## Recursos Técnicos Necessários
- Frontend: React + TanStack Start (este projeto), UI de chat com streaming e renderização de markdown
- Backend: Lovable Cloud — banco de dados, autenticação (e-mail/Google) e funções server-side
- IA: Lovable AI Gateway — interpretação de linguagem natural, classificação automática de transações (categorias fixas: moradia, alimentação, transporte, lazer, saúde, etc.), geração de dicas e relatórios
- Banco de dados (tabelas): transactions (valor, descrição, categoria, data, usuário), goals (nome, valor-alvo, prazo, progresso), chat_messages (histórico por conversa, enviado completo a cada chamada da IA), profiles (renda e preferências do onboarding)
- Regras de segurança: cada usuário só acessa os próprios dados (RLS)

## Escopo do MVP (O que fica fora)
- Não entram: integração bancária/Open Finance, anexos de comprovantes, moedas múltiplas, compartilhamento familiar. Tudo manual-via-chat


