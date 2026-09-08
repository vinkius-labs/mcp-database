# Royalty Calculation Mining MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/royalty-calculation-mining)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates mining royalty obligations using ad valorem and unit-based methods.

## Description
This MCP server provides specialized tools for mining operations to determine royalty payments. It handles both ad valorem calculations based on market value and unit-based calculations for fixed rates. Use `calculate_gross_royalty` to find initial amounts, `calculate_net_royalty` to subtract deductions, and `generate_royalty_schedule` to project payments over multiple periods.


## Available Tools (4)
- **calculate_gross_royalty**: Determines the initial royalty amount before any deductions are applied
- **calculate_net_royalty**: Determines the final payment amount after subtracting allowed costs
- **generate_royalty_schedule**: Projects royalty payments across multiple production periods or volume tiers
- **validate_royalty_parameters**: Verifies that all provided mining data adheres to logical constraints before calculation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Royalty Calculation Mining** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the gross royalty for 500 units at a metal price of 150 with a 5% ad valorem rate."

**🤖 AI Agent:**
> 3750

---

**👤 You:**
> "What is the net royalty if the gross royalty is 1000 and deductions are 200?"

**🤖 AI Agent:**
> 800

---

**👤 You:**
> "Calculate a unit-based royalty for 100 units at a rate of 10 per unit."

**🤖 AI Agent:**
> 1000


## ❓ FAQ

**Q: What is the difference between ad valorem and unit-based royalties?**
Ad valorem royalties are a percentage of the mineral's market value, while unit-based royalties are a fixed amount per unit produced. You can use `calculate_gross_royalty` to compute either type.

**Q: How do I account for operational costs?**
After calculating the initial amount, use `calculate_net_royalty` to subtract your allowable deductions from the gross total.

**Q: Can I project future payments?**
Yes, the `generate_royalty_schedule` tool allows you to input series of production volumes and metal prices to project payments over time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/royalty-calculation-mining](https://vinkius.com/ai-agent-connect/royalty-calculation-mining)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Royalty Calculation Mining** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `royalty-calculation-mining` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Royalty Calculation Mining** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "royalty-calculation-mining": {
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
