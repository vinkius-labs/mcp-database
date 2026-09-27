# NYC City Finance (OMB) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-city-finance-omb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Keyless NYC city-finance data: OMB expense budget by fiscal year, top agencies by adopted budget, the capital budget, the capital commitment plan and citywide energy cost projections — no API key.

## Description
New York City Office of the Mayor's Budget (OMB) records, keyless.

### What you can do
- **Expense budget** — OMB expense budget lines by fiscal year (2024–2027): agency, appropriation, object class and the adopted, modified and financial-plan amounts
- **Budget line count** — a fast count of expense lines for one fiscal year
- **Top agencies** — agencies ranked by their summed adopted budget for one fiscal year
- **Capital budget** — project budget lines with project type, budget-line title, funding source and per-year amounts
- **Capital commitment plan** — capital projects with funding source and per-year amounts over up to five fiscal years
- **Energy cost projections** — citywide energy cost projections by commodity and fiscal year (2020–2030)

### Who is this for
Budget and fiscal policy research, agency cost analysis and energy planning. The expense budget is always scoped to a fiscal year (defaults to 2026 when omitted); agency, appropriation and object-class filters are case-insensitive partial matches on the uppercase budget names.


## Available Tools (6)
- **count_expense_budget_lines**: Fiscal years 2024–2027 are published; fiscal_year defaults to 2026 when omitted. Use it to gauge how large a budget search will be.

Count NYC OMB expense budget lines for a fiscal year
- **get_energy_cost_projections**: Commodity values include "Gasoline", "Fuel Oil", "Heat, Light & Power", "HPD-In Rem / DAMP" and "HPD-Emergency Repairs". A small table (a few hundred rows, fiscal years 2020–2030); optionally pin one fiscal year or commodity.

NYC citywide energy cost projections
- **search_capital_budget**: Project-type, funding and budget-line-title values are free text; the filters are exact matches against the stored values. Pass a filter to bound the result.

Search the NYC OMB capital budget
- **search_capital_commitment**: Project-type, funding and budget-line values are free text; the filters are exact matches against the stored values. Pass a filter to bound the result.

Search the NYC OMB capital commitment plan
- **search_expense_budget**: Fiscal years 2024–2027 are published; fiscal_year defaults to 2026 when omitted. Agency, unit-appropriation and object-class names are stored uppercase (e.g. "DEPARTMENT OF EDUCATION"); the name filters are exact matches and the tool uppercases the inputs. Rows are sorted by the adopted budget amount, largest first.

Search the NYC OMB expense budget
- **top_agency_budgets**: Fiscal years 2024–2027 are published; fiscal_year defaults to 2026 when omitted. Each row is one agency with its summed adopted budget amount for that year.

Top NYC agencies by adopted expense budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC City Finance (OMB)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which NYC agencies have the largest expense budget in FY 2026?"

**🤖 AI Agent:**
> top_agency_budgets with fiscal_year: "2026" returns the agencies ranked by their summed adopted budget amount for the fiscal year.

---

**👤 You:**
> "Show me the education agency's expense budget lines for FY 2026."

**🤖 AI Agent:**
> search_expense_budget with agency_name: "Education" (case-insensitive partial match on the uppercase agency names) and fiscal_year: "2026" returns the matching budget lines sorted by the adopted amount, largest first.

---

**👤 You:**
> "What is the projected gasoline cost for FY 2030?"

**🤖 AI Agent:**
> get_energy_cost_projections with typ: "Gasoline" and fisc_yr: "2030" returns the citywide projected cost for that commodity and fiscal year.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Which fiscal years are published?**
The OMB expense budget publishes fiscal years 2024–2027; the tools default to FY 2026 when the fiscal year is omitted. The energy cost projections table runs fiscal years 2020–2030.

**Q: Why do the budget tools pin a fiscal year?**
The expense budget holds several fiscal years in one table. Every search, count and ranking is scoped to one fiscal year — fiscal_year defaults to "2026" when omitted — so the query stays bounded and fast.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-city-finance-omb](https://vinkius.com/en/ai-agent-connect/nyc-city-finance-omb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC City Finance (OMB)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-city-finance-omb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC City Finance (OMB)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-city-finance-omb": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
