# BCB Economia — PIB, Dívida, Reservas, PIX e SGS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bcb-economia-pib-divida-reservas-pix-e-sgs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bcb-economia-pib-divida-reservas-pix-e-sgs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bcb-economia-pib-divida-reservas-pix-e-sgs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Brazilian economic indicators: monthly GDP proxy (IBC-Br), public debt/GDP ratio, international reserves, trade balance, unemployment rate (PNAD), PIX payment statistics, and universal access to 20,000+ BCB time series via SGS codes.

## Description
Brazilian economic data.

### 7 Tools
- **GDP** — Monthly IBC-Br proxy
- **Debt/GDP** — Public sector debt ratio
- **Reserves** — International reserves (USD)
- **Trade Balance** — Exports minus imports
- **Unemployment** — PNAD rate
- **PIX** — Instant payment statistics
- **SGS** — Any of 20,000+ time series


## Available Tools
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BCB Economia — PIB, Dívida, Reservas, PIX e SGS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a Brazil economic overview: GDP, debt, reserves, and unemployment"

**🤖 AI Agent:**
> 🇧🇷 **Brazil Economic Snapshot**

📈 GDP (IBC-Br): +0.3% monthly
💳 Debt/GDP: 62.4%
🏦 Reserves: $356.2B
⚖️ Trade Balance: +$6.8B
👥 Unemployment: 6.8%
💳 PIX: 4.2B transactions/month

6 BCB data sources queried.

---

**👤 You:**
> "Retrieve the latest PIX payment statistics."

**🤖 AI Agent:**
> Analyzing Central Bank data... The PIX network registered 4.2 billion active transfers in the last 30 days securely.

---

**👤 You:**
> "Get the historical series code 432 representing interest rates."

**🤖 AI Agent:**
> SGS Code 432 successfully pulled. The Selic reference target curve maintained a 10.50% steady metric over the last board meeting.


## Installation & Usage

To install and use the **BCB Economia — PIB, Dívida, Reservas, PIX e SGS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcb-economia-pib-divida-reservas-pix-e-sgs](https://vinkius.com/mcp/bcb-economia-pib-divida-reservas-pix-e-sgs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
