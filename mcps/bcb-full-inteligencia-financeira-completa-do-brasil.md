# BCB Full — Inteligência Financeira Completa do Brasil MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bcb-full-inteligencia-financeira-completa-do-brasil)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The definitive Brazil Central Bank Mega-Server: 22 tools spanning PTAX dollar quotes, 150+ currencies, Selic rates, CDI, IPCA/IGP-M inflation, Focus Survey expectations, GDP, debt, PIX, and universal access to 20,000+ SGS statistical time series.

## Description
The **ultimate Brazil Central Bank Mega-Server** — 22 tools across 4 domains.

### 22 Tools
- 💱 Câmbio (5) — PTAX, period, any currency, catalog, SGS
- 🏦 Juros (4) — Selic target, Selic daily, CDI, Focus
- 📈 Inflação (5) — IPCA, IPCA-15, IGP-M, INPC, Focus
- 🇧🇷 Economia (8) — GDP, debt, reserves, trade, unemployment, PIX, SGS

### No API Key Required
### 2 Engines: SGS (20K+ series) + Olinda OData (PTAX/Focus/PIX)


## Available Tools (21)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BCB Full — Inteligência Financeira Completa do Brasil** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Complete Brazil financial briefing: dollar, Selic, inflation, and GDP"

**🤖 AI Agent:**
> 🇧🇷 **BCB Full Briefing**

💱 USD/BRL: R$ 5.7327 (PTAX)
🏦 Selic: 14.25% | CDI: 14.15%
📈 IPCA: 5.12% (12m) | IGP-M: 4.83%
📊 GDP (IBC-Br): +0.3% monthly
💳 Debt/GDP: 62.4%
🏦 Reserves: $356.2B
💳 PIX: 4.2B txns/month

7 BCB series queried simultaneously.

---

**👤 You:**
> "Compare the expected IPCA inflation against the Selic target for next year."

**🤖 AI Agent:**
> According to the latest Focus Survey, top institutions predict Selic to fall gracefully to 9.5% by end of next year, while IPCA points to a 3.8% inflationary threshold.

---

**👤 You:**
> "Extract the complete trade balance deficit metrics."

**🤖 AI Agent:**
> Querying structural OData files... Brazil reports a current surplus Trade Balance closing around +$6.8 billion strongly pushed by agribusiness exports.


## ❓ FAQ

**Q: What is the Focus Survey?**
The Focus Survey (Relatório Focus) is a weekly survey published every Monday by Brazil's Central Bank. It collects expectations from ~140 financial institutions about key economic variables: Selic, IPCA, GDP, exchange rate, and more. The median projections are closely watched by markets.

**Q: Does this MCP cover both daily currency exchanges and long-term macroeconomics?**
Yes! BCB Full is an 'all-in-one' Mega-Server that unifies the PTAX currency gateway alongside deep economic surveys (like the 20k+ SGS series and Focus survey). Use it simultaneously without flipping contexts.

**Q: What happens if local BCB APIs are temporarily unstable?**
The tool uses streamlined async fetches equipped with silent polling gracefully designed to mitigate brief BCB outages, delivering the latest known cache boundary when direct parsing fails.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcb-full-inteligencia-financeira-completa-do-brasil](https://vinkius.com/mcp/bcb-full-inteligencia-financeira-completa-do-brasil)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BCB Full — Inteligência Financeira Completa do Brasil** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bcb-full-inteligencia-financeira-completa-do-brasil` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BCB Full — Inteligência Financeira Completa do Brasil** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bcb-full-inteligencia-financeira-completa-do-brasil": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
