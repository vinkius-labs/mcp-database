# ANVISA (Portal de APIs) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anvisa-portal-de-apis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access official Brazilian health regulatory data — query medicines, prices, food registrations, cosmetics, and sanitizers directly from ANVISA.

## Description
Connect to the official **ANVISA (Brazilian Health Regulatory Agency)** API portal and integrate critical health regulatory data into your AI workflows.

### What you can do

- **Medicine Search** — Query registered medicines by commercial name, active ingredient, or registration number using `consultar_medicamentos`.
- **Pricing Intelligence** — Fetch maximum consumer prices (PMC) and factory prices (PF) for regulated drugs via `precos_medicamentos`.
- **Food & Nutrition** — Access the database of registered food products (`registros_alimentos`) and those requiring only notification (`notificacoes_alimentos`).
- **Cosmetics & Hygiene** — Verify registration data for perfumes, hygiene products, and cosmetics using `consultar_cosmeticos`.
- **Sanitizing Products** — Search for cleaning and sanitizing products registered with the agency via `consultar_saneantes`.
- **Pharmacopeia Standards** — Retrieve official monographs for chemical substances and health standards using `monografias_farmacopeia`.

### How it works

1. Subscribe to this server
2. Enter your ANVISA API Key
3. Start querying Brazilian regulatory data from Claude, Cursor, or any MCP client

### Who is this for?

- **Healthcare Professionals** — quickly verify medicine registrations and official pricing without manual portal searches
- **Regulatory & Compliance Teams** — automate the monitoring of food and cosmetic registrations to ensure market compliance
- **Pharmaceutical Researchers** — access Farmacopeia monographs and active ingredient data directly within research environments


## Available Tools
- **consultar_cosmeticos**: Search for registered cosmetic products
- **consultar_medicamentos**: Search for medicines by name, active ingredient, or registration number
- **consultar_saneantes**: Search for registered sanitizing products
- **monografias_farmacopeia**: Retrieve monographs for chemical substances
- **notificacoes_alimentos**: Access food products that only require notification
- **precos_medicamentos**: Retrieve maximum consumer prices (PMC) and factory prices (PF) for medicines
- **registros_alimentos**: List food products registered with ANVISA


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ANVISA (Portal de APIs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for medicines containing 'Paracetamol' as the active ingredient."

**🤖 AI Agent:**
> I've found several registered medicines with Paracetamol. Notable ones include [Brand A] (Reg: 123...) and [Brand B] (Reg: 456...). Would you like to see the pricing for any of these?

---

**👤 You:**
> "What is the maximum consumer price for the medicine 'Aspirina'?"

**🤖 AI Agent:**
> Querying ANVISA price database... For 'Aspirina', the Maximum Consumer Price (PMC) is [Value] and the Factory Price (PF) is [Value]. These values may vary based on state taxes (ICMS).

---

**👤 You:**
> "Check the registration status of the cosmetic product 'Protetor Solar'."

**🤖 AI Agent:**
> I've retrieved the data for 'Protetor Solar' from the cosmetics database. It is currently registered under number [Reg Number] with an active status. The manufacturer is [Company Name].


## ❓ FAQ

**Q: Can I check the maximum consumer price of a specific medicine?**
Yes. Use the `precos_medicamentos` tool providing the commercial name or registration number to get the PMC (Maximum Consumer Price) and PF (Factory Price).

**Q: How do I verify if a food product is registered or just notified?**
You can use `registros_alimentos` for products that require full registration and `notificacoes_alimentos` for those that only require notification to ANVISA.

**Q: Can I search for a medicine using its active ingredient?**
Absolutely. The `consultar_medicamentos` tool accepts a `principio_ativo` parameter to find all medicines containing that specific substance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anvisa-portal-de-apis](https://vinkius.com/mcp/anvisa-portal-de-apis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ANVISA (Portal de APIs)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `anvisa-portal-de-apis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ANVISA (Portal de APIs)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "anvisa-portal-de-apis": {
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
