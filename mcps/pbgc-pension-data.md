# PBGC Pension Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pbgc-pension-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access official US Pension Benefit Guaranty Corporation data — query single and multiemployer plans, ERISA 4044 rates, and financial assistance records.

## Description
Connect to the **PBGC (Pension Benefit Guaranty Corporation)** open data repository and empower your AI agent to analyze US pension plan health and regulatory metrics through natural conversation.

### What you can do

- **Single-Employer Plans** — List and filter active plans by EIN, Plan Number, or State to monitor corporate pension landscapes.
- **Multiemployer Plans** — Retrieve comprehensive lists of active multiemployer plans insured by the PBGC.
- **ERISA 4044 Rates** — Access critical interest assumptions (select and ultimate rates) used for determining the present value of annuities.
- **Financial Assistance** — Track and analyze financial assistance payments made by the PBGC to multiemployer plans by fiscal year.

### How it works

1. Subscribe to this server
2. Enter your PBGC Open Data API Key (or public token)
3. Start querying pension datasets directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — quickly gather data on pension plan premiums and financial assistance trends.
- **Actuaries & Legal Professionals** — retrieve ERISA 4044 interest assumptions for valuation and compliance without manual spreadsheet lookups.
- **Policy Researchers** — analyze the distribution of pension plans across different states and fiscal years.


## Available Tools (4)
- **list_erisa_4044_rates**: Get ERISA 4044 Interest Assumptions
- **list_financial_assistance**: List financial assistance payments
- **list_multiemployer_plans**: List active multiemployer pension plans
- **list_single_employer_plans**: List active single-employer pension plans


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PBGC Pension Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active single-employer pension plans in California."

**🤖 AI Agent:**
> I've retrieved the active single-employer plans for California. There are several plans listed, including [Plan Name] (EIN: [Number]). Would you like to see the full list or details for a specific EIN?

---

**👤 You:**
> "What are the ERISA 4044 interest rates for 2023, Q4?"

**🤖 AI Agent:**
> For Q4 2023, the ERISA 4044 select interest rate was [Rate]% and the ultimate rate was [Rate]%. These are used for determining the present value of annuities in terminations.

---

**👤 You:**
> "Show me multiemployer plans insured by PBGC."

**🤖 AI Agent:**
> I've fetched the list of active multiemployer plans insured by PBGC. I found [Number] plans. Notable entries include [Plan A] and [Plan B]. Do you need details on a specific plan?


## ❓ FAQ

**Q: How can I filter single-employer pension plans for a specific state?**
You can use the `list_single_employer_plans` tool and provide the two-letter state code (e.g., 'NY' or 'CA') in the `state` parameter to get localized results.

**Q: Can I retrieve ERISA 4044 interest rates for a specific year and quarter?**
Yes! The `list_erisa_4044_rates` tool accepts optional `year` and `quarter` parameters to fetch the exact interest assumptions you need for valuation.

**Q: Is it possible to see financial assistance payments by fiscal year?**
Absolutely. Use the `list_financial_assistance` tool and specify the `fiscal_year` (e.g., 2023) to see all payments made to multiemployer plans during that period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pbgc-pension-data](https://vinkius.com/mcp/pbgc-pension-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PBGC Pension Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pbgc-pension-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PBGC Pension Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pbgc-pension-data": {
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
