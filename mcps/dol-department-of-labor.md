# DOL (Department of Labor) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dol-department-of-labor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access US Department of Labor data including OSHA inspections, MSHA safety records, and wage compliance directly from your AI agent.

## Description
Access comprehensive labor data from the **U.S. Department of Labor (DOL)**. This server provides tools to query critical datasets including workplace safety inspections, mine safety violations, wage compliance records, and employment training statistics.

### What you can do

- **OSHA Inspections** — Retrieve health and safety inspection records via `get_osha_inspections` to monitor workplace compliance.
- **MSHA Safety** — Access mine safety inspection data (`get_msha_inspections`) and violation records (`get_msha_violations`) to ensure industrial safety standards.
- **WHD Compliance** — Query Wage and Hour Division data via `get_whd_compliance` regarding labor law investigations and compliance history.
- **ETA Statistics** — Fetch labor market data and information on job training programs using `get_eta_data`.

### How it works

1. Subscribe to this server
2. Enter your DOL API Key
3. Query public labor data using natural language in any MCP-compatible client

### Who is this for?

- **Compliance Officers** — Monitor safety records and regulatory adherence across industries.
- **Data Researchers** — Analyze labor market trends and workplace safety statistics.
- **Legal Professionals** — Investigate wage and hour compliance history for specific entities.


## Available Tools (5)
- **get_eta_data**: Get ETA employment and training data
- **get_msha_inspections**: Get MSHA inspection data
- **get_msha_violations**: Get MSHA violations data
- **get_osha_inspections**: Get OSHA inspection data
- **get_whd_compliance**: Get WHD compliance data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DOL (Department of Labor)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the top 5 OSHA inspections in New York."

**🤖 AI Agent:**
> I've retrieved the 5 most recent OSHA inspections for New York. The records include inspections for 'BuildRight Construction' and 'SafeLogistics Hub' with details on inspection types and dates.

---

**👤 You:**
> "Show me recent MSHA violations ordered by date."

**🤖 AI Agent:**
> Fetching MSHA violation records... I found several recent entries. The most recent violation was recorded at 'DeepRock Mine' on October 12th regarding ventilation standards.

---

**👤 You:**
> "Get wage and hour compliance data for the state of Texas."

**🤖 AI Agent:**
> Querying WHD compliance data for Texas... I have compiled the investigation records, including case IDs and findings related to the Fair Labor Standards Act (FLSA) for various employers in the region.


## ❓ FAQ

**Q: Can I filter OSHA inspection data by a specific state?**
Yes! You can use the `filter` parameter in the `get_osha_inspections` tool with OData syntax, such as `state_code eq 'CA'` for California.

**Q: What kind of information does the ETA data tool provide?**
The `get_eta_data` tool fetches information regarding employment and training programs, as well as various labor market statistics managed by the Employment and Training Administration.

**Q: How can I limit the number of results returned from a query?**
All tools, such as `get_msha_violations` or `get_whd_compliance`, include a `top` parameter. Simply specify a number to limit the results to that amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dol-department-of-labor](https://vinkius.com/mcp/dol-department-of-labor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DOL (Department of Labor)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dol-department-of-labor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DOL (Department of Labor)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dol-department-of-labor": {
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
