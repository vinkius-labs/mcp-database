# BLS Wages — OEWS Occupational Employment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bls-wages-oews-occupational-employment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

The holy grail of HR data. Use Occupational Employment and Wage Statistics (OEWS) to extract exact median earnings broken down by detailed professions and states.

## Description
If you need to know exactly how much a 'registered nurse in Texas' or a 'software engineer in Illinois' earns, OEWS is your required dataset.

### What you can find
- **Median / Average Pay** — Discover true wage distributions percentiles.
- **Occupation Codes** — Maps hundreds of distinct professions.
- **State Comparisons** — Compare geographic locations for job offers.


## Available Tools (1)
- **query_bls**: Use this instead of specific endpoints if you intimately know the underlying numerical code. Up to 50 concurrent lookbacks allowed.

Generic BLS v2 api timeseries query. Requires explicit BLS Series IDs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BLS Wages — OEWS Occupational Employment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the median salary for Software Developers in Texas versus California?"

**🤖 AI Agent:**
> Software Developers in California enjoy a median wage upward of $150,000, whereas the median in Texas is closer to $120,000.

---

**👤 You:**
> "Tell me the hourly wage differences for Registered Nurses nationally."

**🤖 AI Agent:**
> Registered Nurses nationally see an average hourly boundary of roughly $42.80, with highs well past $60 in coastal markets.

---

**👤 You:**
> "Compare top 90th percentile to bottom 10th for Accountants."

**🤖 AI Agent:**
> Entry-level (10th percentile) Accountants run near $48,000 yearly, standing in stark contrast to the top executive counterparts (90th percentile) pushing toward $135,000+.


## ❓ FAQ

**Q: How reliable is OEWS compared to private job boards?**
Extremely. OEWS pulls directly from true tax and payroll disclosures to the government, eliminating inflated self-reported figures typical on private job sites.

**Q: Is a Key required?**
Only one single Key is required from the registration page. Simply plug it into the settings page and access the entire 20-year catalog of wage distribution profiles globally.

**Q: Why is wage data a unique server?**
Because querying compensation brackets specific to states and detailed codes (like separating Senior vs Junior codes horizontally) takes specialized tool structures optimally tailored here.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bls-wages-oews-occupational-employment](https://vinkius.com/mcp/bls-wages-oews-occupational-employment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BLS Wages — OEWS Occupational Employment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bls-wages-oews-occupational-employment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BLS Wages — OEWS Occupational Employment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bls-wages-oews-occupational-employment": {
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
