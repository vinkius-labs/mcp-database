# BCB Juros — Selic, CDI e Expectativas Focus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bcb-juros-selic-cdi-e-expectativas-focus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Brazilian interest rates: Selic target rate (COPOM decisions), daily effective Selic rate, CDI (interbank deposit certificate rate), and Focus Survey market expectations for future Selic rates from Brazil's Central Bank.

## Description
Brazilian interest rates.

### 4 Tools
- **Selic Target** — COPOM decisions
- **Selic Daily** — Effective overnight rate
- **CDI** — Interbank deposit certificate rate
- **Focus Expectations** — Market forecasts


## Available Tools
- **get_selic_meta**: A Selic é a taxa básica da economia brasileira e referência para todas as demais taxas de juros do país. Série SGS: 432.

Obter a meta da taxa Selic definida pelo COPOM
- **get_selic_diaria**: Reflete a execução real da política monetária. Série SGS: 11.

Obter a taxa Selic efetiva (diária)
- **get_cdi**: O CDI é a referência para a maioria dos investimentos em renda fixa no Brasil (CDBs, LCIs, LCAs, fundos DI). Geralmente fica muito próximo da Selic. Série SGS: 12.

Obter a taxa CDI (Certificado de Depósito Interbancário)
- **get_expectativas_selic**: Inclui mediana, média, mínimo e máximo das projeções das instituições financeiras. O Focus é publicado toda segunda-feira pelo BCB.

Obter as expectativas do mercado para a taxa Selic (Relatório Focus)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BCB Juros — Selic, CDI e Expectativas Focus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current Selic interest rate in Brazil?"

**🤖 AI Agent:**
> 🏦 **Selic Target Rate**

Current: 14.25% per year
Last decision: March 19, 2026 (COPOM)
Action: Maintained (+0bp)

The Selic is Brazil's benchmark interest rate, set by the COPOM committee every 45 days.

Source: BCB, SGS series 432

---

**👤 You:**
> "Fetch the CDI accumulated rate for the previous month."

**🤖 AI Agent:**
> According to the financial indices, the interbank CDI return for the last completed month accrued exactly 1.12%.

---

**👤 You:**
> "List the Focus survey expectation for the Selic rate by next December."

**🤖 AI Agent:**
> The median Focus panel agreement projects the Selic ending next year's cycle at approximately 9.50% p.a.


## ❓ FAQ

**Q: What is the difference between Selic and CDI?**
Selic is the overnight rate for government bond-backed interbank loans, set/targeted by the COPOM. CDI is the interbank rate for unsecured overnight deposits between banks. CDI closely tracks Selic and is the most common benchmark for fixed-income investments in Brazil.

**Q: Can I trust the Selic Daily effective values?**
Yes. The module pipes data strictly authenticated by the Brazilian Central Bank. The effective Selic updates are legally suitable for debt recalculations and financial modeling.

**Q: Does it include expected adjustments set by COPOM?**
Absolutely. By integrating the Focus expectations array, your AI is acutely aware of forward market opinions preceding actual COPOM rate cut decisions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcb-juros-selic-cdi-e-expectativas-focus](https://vinkius.com/mcp/bcb-juros-selic-cdi-e-expectativas-focus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BCB Juros — Selic, CDI e Expectativas Focus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bcb-juros-selic-cdi-e-expectativas-focus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BCB Juros — Selic, CDI e Expectativas Focus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bcb-juros-selic-cdi-e-expectativas-focus": {
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
