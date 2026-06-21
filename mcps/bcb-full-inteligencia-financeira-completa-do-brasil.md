# BCB Full — Inteligência Financeira Completa do Brasil MCP Server

The definitive Brazil Central Bank Mega-Server: 22 tools spanning PTAX dollar quotes, 150+ currencies, Selic rates, CDI, IPCA/IGP-M inflation, Focus Survey expectations, GDP, debt, PIX, and universal access to 20,000+ SGS statistical time series.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bcb-full-inteligencia-financeira-completa-do-brasil)

## Overview
**Category:** industry-titans
**Tools Count:** 21

## Description
The **ultimate Brazil Central Bank Mega-Server** — 22 tools across 4 domains.

### 22 Tools
- 💱 Câmbio (5) — PTAX, period, any currency, catalog, SGS
- 🏦 Juros (4) — Selic target, Selic daily, CDI, Focus
- 📈 Inflação (5) — IPCA, IPCA-15, IGP-M, INPC, Focus
- 🇧🇷 Economia (8) — GDP, debt, reserves, trade, unemployment, PIX, SGS

### No API Key Required
### 2 Engines: SGS (20K+ series) + Olinda OData (PTAX/Focus/PIX)


## Available Tools
- **get_cotacao_dolar**: Inclui valores de compra e venda. O PTAX é a taxa de referência oficial do câmbio brasileiro, calculada a partir de consultas aos dealers de câmbio.

Obter a cotação do dólar americano (PTAX) em uma data específica
- **get_dolar_periodo**: Formato de data: MM-DD-YYYY. Máximo de 1 ano por consulta. Inclui valores de compra, venda e boletins (abertura, intermediário, fechamento).

Obter a série histórica do dólar PTAX em um período
- **get_cotacao_moeda**: Use listar_moedas para ver todos os 150+ códigos disponíveis. Inclui compra e venda.

Obter cotação de qualquer moeda estrangeira pelo código (EUR, GBP, JPY, etc.)
- **listar_moedas**: Inclui moedas exóticas como CLP, COP, MXN, THB, etc.

Listar todas as moedas disponíveis no sistema PTAX do Banco Central
- **get_dolar_sgs**: Séries: 1 (compra), 10813 (venda). Mais flexível que PTAX para séries longas. Formato de data: DD/MM/YYYY.

Obter a série histórica do dólar comercial (compra/venda) via SGS
- **get_pib**: Este é o indicador IBC-Br (Índice de Atividade Econômica do Banco Central), uma proxy mensal do PIB. Série SGS: 4380.

Obter o PIB mensal do Brasil — variação percentual
- **get_divida_pib**: Indicador fundamental de sustentabilidade fiscal. Série SGS: 4513.

Obter a dívida líquida do setor público como % do PIB
- **get_reservas**: Fundamental para avaliação da capacidade do país de honrar compromissos externos. Série SGS: 3546.

Obter as reservas internacionais do Brasil em USD
- **get_balanca_comercial**: O Brasil é um grande exportador de commodities agrícolas, minério e petróleo. Série SGS: 22707.

Obter o saldo da balança comercial brasileira
- **get_desemprego**: Indicador trimestral do mercado de trabalho brasileiro. Série SGS: 24369.

Obter a taxa de desemprego do Brasil (PNAD)
- **get_pix_estatisticas**: O PIX é o sistema de pagamentos instantâneos do Brasil, operado pelo BCB. Lançado em novembro de 2020, já é o meio de pagamento mais usado no país.

Obter estatísticas do PIX — volume e quantidade de transações
- **get_serie_bcb**: 000+ séries do Sistema Gerenciador de Séries Temporais (SGS). Pesquise códigos em bcb.gov.br/estabilidadefinanceira/seriestemporais. Exemplos: 11 (Selic), 433 (IPCA), 1 (Dólar).

Consultar qualquer série temporal do BCB pelo código SGS
- **get_ipca**: Usado como meta de inflação pelo BCB. Mede a variação de preços de uma cesta de consumo para famílias com renda de 1 a 40 salários mínimos. Série SGS: 433.

Obter o IPCA — Índice Nacional de Preços ao Consumidor Amplo
- **get_ipca15**: Muito acompanhado pelo mercado como antecipação do IPCA. Série SGS: 7478.

Obter o IPCA-15 — prévia da inflação oficial
- **get_igpm**: Usado como indexador de aluguéis e contratos. Composição: 60% IPA (atacado) + 30% IPC (consumo) + 10% INCC (construção). Série SGS: 189.

Obter o IGP-M — Índice Geral de Preços - Mercado
- **get_inpc**: Mede a inflação para famílias com renda de 1 a 5 salários mínimos. Usado como referência para reajustes salariais e do salário mínimo. Série SGS: 188.

Obter o INPC — Índice Nacional de Preços ao Consumidor
- **get_expectativas_inflacao**: Filtre por indicador: IPCA, IGP-DI, IGP-M. Inclui mediana, média, mínimo, máximo e desvio padrão.

Obter as expectativas do mercado para a inflação (Relatório Focus)
- **get_selic_meta**: A Selic é a taxa básica da economia brasileira e referência para todas as demais taxas de juros do país. Série SGS: 432.

Obter a meta da taxa Selic definida pelo COPOM
- **get_selic_diaria**: Reflete a execução real da política monetária. Série SGS: 11.

Obter a taxa Selic efetiva (diária)
- **get_cdi**: O CDI é a referência para a maioria dos investimentos em renda fixa no Brasil (CDBs, LCIs, LCAs, fundos DI). Geralmente fica muito próximo da Selic. Série SGS: 12.

Obter a taxa CDI (Certificado de Depósito Interbancário)
- **get_expectativas_selic**: Inclui mediana, média, mínimo e máximo das projeções das instituições financeiras. O Focus é publicado toda segunda-feira pelo BCB.

Obter as expectativas do mercado para a taxa Selic (Relatório Focus)


## Installation & Usage

To install and use the **BCB Full — Inteligência Financeira Completa do Brasil** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcb-full-inteligencia-financeira-completa-do-brasil](https://vinkius.com/mcp/bcb-full-inteligencia-financeira-completa-do-brasil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
