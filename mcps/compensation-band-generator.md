# Compensation Band Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/compensation-band-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate structured compensation packages including base salary, bonus targets, and equity ranges based on global market data.

## Description
The Compensation Band Generator connects AI agents to precise market data for professional roles. By using tools like `calculate_base_salary`, `calulate_bonus_target`, and `calculate_equity_range`, you can determine the annual fixed cash, variable bonus targets, and equity grant ranges for specific job levels (IC1-IC6, M1-M4).


## Available Tools (3)
- **calculate_base_salary**: Calculate the annual base salary for a role
- **calculate_bonus_target**: Calculate the annual variable cash bonus target
- **calculate_equity_range**: Calculate the annual equity grant range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Compensation Band Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the base salary for a Software Engineer (IC3) in San Francisco at the 75th percentile?"

**🤖 AI Agent:**
> $185,000

---

**👤 You:**
> "What is the expected bonus target for an M2 level manager?"

**🤖 AI Agent:**
> 20%

---

**👤 You:**
> "Calculate the equity range for a Principal Engineer (IC6) in London at the 90th percentile."

**🤖 AI Agent:**
> £120,000 - £180,000


## ❓ FAQ

**Q: How do I calculate the base salary for a specific role?**
Use the `calculate_base_salary` tool by providing the job title, seniority level (e.g., IC3), city, and target market percentile (50th, 75th, or 90th).

**Q: Can I determine the bonus percentage for management roles?**
Yes, use the `calculate_bonus_target` tool. It calculates the expected annual variable cash bonus as a percentage of base salary based on the employee's level.

**Q: How is the equity range calculated?**
The `calculate_equity_range` tool identifies the baseline value for a specific level and adjusts it based on the selected percentile and geographic location.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/compensation-band-generator](https://vinkius.com/mcp/compensation-band-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Compensation Band Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `compensation-band-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Compensation Band Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "compensation-band-generator": {
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
