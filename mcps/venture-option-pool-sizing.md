# Venture Option Pool Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-option-pool-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate necessary option pool sizes, dilution impact, and hiring runway.

## Description
This MCP server provides essential financial modeling tools for managing employee equity. Use `calculate_pool_requirements` to determine the total equity needed for future hires and retention. You can use `estimate_dilution_impact` to see how new pools affect current shareholders, `project_hiring_runway` to predict how long your equity will last, and `calculate_net_pool_adjustment` to account for departures and unvested option forfeitures.


## Available Tools (4)
- **calculate_pool_requirements**: Calculate pool requirements
- **estimate_dilution_impact**: Estimate dilution
- **project_hiring_runway**: Project runway
- **calculate_net_pool_adjustment**: Adjust pool


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Option Pool Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required option pool for a company with 10 employees, 5 planned hires, 2% ungranted options, 1% refresh need, and a 15% benchmark."

**🤖 AI Agent:**
> The recommended pool size is 16.0%, with a total equity requirement of 16.0% and a buffer of 1.0%.

---

**👤 You:**
> "If I have 20% ownership and create a new 10% option pool, what will my new ownership be?"

**🤖 AI Agent:**
> Your post-dilution ownership will be 18.18%, representing a dilution factor of 0.91%.

---

**👤 You:**
> "How many months of hiring runway do I have if I have 5% available pool, an average grant of 0.5% per hire, and plan to hire 2 people per month?"

**🤖 AI Agent:**
> You have 5.0 months of runway, which supports a total of 10 hires.


## ❓ FAQ

**Q: How do I calculate the total equity needed for my next funding round?**
You can use the `calculate_pool_requirements` tool. It takes into account your current employees, planned hires, ungranted options, and industry benchmarks to provide a recommended pool size.

**Q: Can I predict how long my current option pool will last?**
Yes, the `project_hiring_runway` tool allows you to predict how many months or hiring cycles your available pool can sustain based on your planned hiring rate and average grants.

**Q: How does creating a new pool affect my ownership?**
You can use `estimate_dilution_impact` to calculate the reduction in ownership percentage for existing shareholders caused by the creation of a new option pool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-option-pool-sizing](https://vinkius.com/en/ai-agent-connect/venture-option-pool-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Option Pool Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-option-pool-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Option Pool Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-option-pool-sizing": {
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
