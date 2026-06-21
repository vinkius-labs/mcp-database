# BCB Juros — Selic, CDI e Expectativas Focus MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bcb-juros-selic-cdi-e-expectativas-focus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bcb-juros-selic-cdi-e-expectativas-focus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bcb-juros-selic-cdi-e-expectativas-focus-mcp)
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


## Installation & Usage

To install and use the **BCB Juros — Selic, CDI e Expectativas Focus** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcb-juros-selic-cdi-e-expectativas-focus](https://vinkius.com/mcp/bcb-juros-selic-cdi-e-expectativas-focus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
