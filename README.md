# Dash-varreduras

Dashboard em HTML para análise de **Relatório Detalhado de Viagem** de varredeira, com upload de planilha Excel e visualização de KPIs, gráficos e tabela.

## Visão geral

O arquivo principal do projeto é:

- `varredeira_dashboard.html`

Ele permite importar arquivos `.xlsx`/`.xls` e gera automaticamente uma visão analítica da operação.

## Funcionalidades principais

- Upload por clique ou arrastar/soltar
- Leitura de planilha com `SheetJS (xlsx)`
- Visualização de gráficos com `Chart.js`
- KPIs de operação:
  - Distância total
  - Tempo de condução
  - Tempo parado
  - Número de viagens
- Tabela detalhada por viagem

## Gráficos disponíveis

1. **Atividade diária** (distância e condução)
   - Tipos: barras, linha e radar
2. **Horas trabalhadas por período**
   - Tipos: pizza, rosca e polar area
3. **Condução vs parado**
   - Tipos: barras, linha e pizza

## Estrutura de dados esperada na planilha

O parser procura uma linha de cabeçalho contendo **`Data`** e utiliza as colunas observadas no relatório:

- Data
- Ativo
- Viagem Início
- Viagem Fim
- Tempo Condução
- Tempo Parado
- Duração
- Distância
- Velocidade média
- Velocidade máxima

## Como usar

1. Abra `varredeira_dashboard.html` no navegador.
2. Faça upload da planilha de relatório (`.xlsx` ou `.xls`).
3. Explore KPIs, gráficos e tabela para análise do período.