# BCB Câmbio — Dólar PTAX, Euro e 150+ Moedas MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bcb-cambio-dolar-ptax-euro-e-150-moedas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Official exchange rates from Brazil's Central Bank: daily PTAX dollar quotes (the official BRL/USD reference rate), historical series, any of 150+ currencies against BRL, complete currency catalog, and SGS time series for long-term FX data.

## Description
Official FX rates from Brazil.

### What you can do
- **PTAX** — Daily dollar rate (official reference)
- **Period** — Historical dollar series
- **Any Currency** — 150+ currencies vs BRL
- **Catalog** — All available currencies
- **SGS** — Long-term FX time series

### No API Key Required


## Available Tools (5)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BCB Câmbio — Dólar PTAX, Euro e 150+ Moedas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current dollar rate in Brazil?"

**🤖 AI Agent:**
> 💱 **Dólar PTAX — 04/04/2026**

Buy: R$ 5.7321
Sell: R$ 5.7327

The PTAX is the official BRL/USD reference rate, calculated by the Central Bank of Brazil from daily dealer consultations.

Source: BCB, PTAX

---

**👤 You:**
> "Show me the dollar/real exchange rate for the last 30 days"

**🤖 AI Agent:**
> 📊 **BRL/USD — Last 30 Days**

High: R$ 5.8912 (March 12)
Low: R$ 5.6543 (March 28)
Current: R$ 5.7327

Trend: -1.2% (strengthening BRL)

22 trading days shown

---

**👤 You:**
> "Convert 500 Euros to Brazilian Reais based on the latest Central Bank rate."

**🤖 AI Agent:**
> Using the latest EUR/BRL exchange rate of 6.1820... 500 EUR equals to 3091.00 BRL natively.


## ❓ FAQ

**Q: What is PTAX?**
PTAX is the official BRL/USD reference rate calculated by the Central Bank of Brazil. It's computed from daily consultations with foreign exchange dealers and is used as the benchmark for settling FX contracts, derivatives, and international transactions in Brazil.

**Q: Can I query currencies other than USD?**
Yes! The Central Bank holds an active catalog covering more than 150 different foreign exchange currencies against the Real (BRL). The AI will fetch daily crosses simply by mentioning the currency ticker.

**Q: Does it require an API authentication key or setup?**
No. The integration interfaces entirely with the Central Bank's open access OData portals. Subscribe the module and engage directly without generating account tokens.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcb-cambio-dolar-ptax-euro-e-150-moedas](https://vinkius.com/mcp/bcb-cambio-dolar-ptax-euro-e-150-moedas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BCB Câmbio — Dólar PTAX, Euro e 150+ Moedas** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bcb-cambio-dolar-ptax-euro-e-150-moedas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BCB Câmbio — Dólar PTAX, Euro e 150+ Moedas** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bcb-cambio-dolar-ptax-euro-e-150-moedas": {
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
