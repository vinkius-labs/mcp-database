# BCB Economia — PIB, Dívida, Reservas, PIX e SGS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bcb-economia-pib-divida-reservas-pix-e-sgs)
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


## Available Tools (7)
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
- **get_pib**: Este é o indicador IBC-Br (Índice de Atividade Econômica do Banco Central), uma proxy mensal do PIB. Série SGS: 4380.

Obter o PIB mensal do Brasil — variação percentual


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


## ❓ FAQ

**Q: What is IBC-Br?**
IBC-Br (Índice de Atividade Econômica do Banco Central) is a monthly GDP proxy produced by Brazil's Central Bank. It's released ~45 days after the reference month and provides earlier economic activity signals than the quarterly GDP published by IBGE.

**Q: Can I query customized long-term structural APIs directly?**
Yes. This configuration enables your AI native access to over 20,000 deep SGS temporal archives covering from inflation matrices to trade balance flows continuously maintained by true financial experts.

**Q: Do I need a proprietary token issued by the Brazilian Government?**
No access token required. The BCB Economia tools strictly map transparent endpoint infrastructures built via OData, keeping your usage straightforward and natively compliant without friction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcb-economia-pib-divida-reservas-pix-e-sgs](https://vinkius.com/mcp/bcb-economia-pib-divida-reservas-pix-e-sgs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BCB Economia — PIB, Dívida, Reservas, PIX e SGS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bcb-economia-pib-divida-reservas-pix-e-sgs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BCB Economia — PIB, Dívida, Reservas, PIX e SGS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bcb-economia-pib-divida-reservas-pix-e-sgs": {
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
