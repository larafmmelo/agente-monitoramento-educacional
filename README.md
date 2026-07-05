# agente-monitoramento-educacional
# Agente Inteligente de Monitoramento Educacional Global 🌍📚

Este projeto consiste em um pipeline automatizado para coleta, tratamento, análise e geração de relatórios executivos sobre os indicadores educacionais mundiais, utilizando a base de dados **EdStats (World Bank)**[cite: 1].

Projeto desenvolvido como parte do desafio do **Aceler.AI**[cite: 1].

## 🛠️ Tecnologias Utilizadas
* **Python**: Estruturação do script de limpeza, seleção de indicadores e lógica de agrupamento.
* **n8n**: Orquestração e automação de todo o fluxo de ponta a ponta.
* **OpenAI (GPT-4o)**: Geração de insights executivos e análise analítica contextualizada.
* **Claude Code / Codex**: Assistência no desenvolvimento do código e otimizações.

## 📂 Estrutura do Projeto
* `processar_dados.py`: Script Python responsável pelas 4 atividades obrigatórias de manipulação de dados.
* `dados_educacao_tratados.csv`: Base de dados limpa, tratada e otimizada com a seleção de indicadores e rankings para o consumo da IA.
* `skill_agente.txt`: Arquivo contendo a Skill especializada desenvolvida e versionada para o agente de IA.
* `workflow.json`: Exportação do fluxo de automação estruturado no n8n.

## 🤖 Como o Codex / Claude Code foi Utilizado
Conforme os requisitos do projeto, ferramentas de IA focadas em código foram utilizadas para acelerar o desenvolvimento:
1. **Criação de Funções Python**: Utilizado para estruturar a lógica de pivotagem (`melt` e `pivot`) do pandas para agregar anos históricos em colunas executivas.
2. **Tratamento de Dados**: A estratégia de preenchimento inteligente de valores nulos utilizando métodos de preenchimento progressivo/regressivo (`ffill` e `bfill`) por grupo de países foi sugerida pela IA.
3. **Documentação**: Geração de docstrings eficientes seguindo o padrão PEP 257 para as funções do script.

## 🎯 Definição da Skill Versionada
A Skill do agente foi projetada para focar em análise educacional macroeconômica. Ela instrui o modelo a atuar como um Consultor Sênior em Políticas Públicas de Educação, proibindo resumos numéricos simples e exigindo análises de correlação profunda entre investimento público (% do PIB) e taxas de alfabetização reais.

## 🔧 Funcionalidades Mínimas Atendidas
- [x] Selecionar países
- [x] Selecionar indicadores
- [x] Comparar países
- [x] Gerar ranking
- [x] Gerar insights
- [x] Produzir relatório
