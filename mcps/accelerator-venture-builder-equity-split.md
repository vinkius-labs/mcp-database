# Accelerator Venture Builder Equity Split MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-venture-builder-equity-split)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate optimal equity distributions, vesting schedules, and governance rights for venture builders.

## Description
This MCP server provides specialized tools for venture builders and entrepreneurs to model equity structures. It balances founder contributions against institutional support to determine fair ownership. Use `calculate_equity_split` to model ownership based on idea origin and IP status, `generate_vesting_schedule` to define time-based equity earning, and `determine_governance_rights` to establish decision-making frameworks.


## Available Tools (3)
- **calculate_equity_split**: Determine the recommended percentage of ownership for both the Founder and the Venture Builder
- **determine_governance_rights**: Establish the decision-making framework and control rights for the venture
- **generate_vesting_schedule**: Propose a time-based schedule for how equity is earned


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Venture Builder Equity Split** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate an equity split where the founder contributes 60%, the builder contributes 40%, the idea is external, and the founder owns the IP."

**🤖 AI Agent:**
> The recommended equity split is 60% for the Founder and 40% for the Venture Builder.

---

**👤 You:**
> "Generate a 4-year vesting schedule with a 1-year cliff for 100% of the equity."

**🤖 AI Agent:**
> The vesting schedule includes a 12-month cliff, after which equity is earned monthly. The total duration is 48 months.

---

**👤 You:**
> "Determine governance rights for a split of 70% founder and 30% builder where the builder is an institutional entity."

**🤖 AI Agent:**
> The founder holds primary voting control, but the institutional builder maintains shared control and specific oversight rights.


## ❓ FAQ

**Q: How does the tool handle IP ownership in equity calculations?**
The `calculate_equity_split` tool applies a premium to the builder's equity if the IP is owned by the builder, reflecting the value of the intellectual property being transferred to the venture.

**Q: Can I generate a vesting schedule for all equity?**
Yes, you can use `generate_vesting_schedule` by providing the total equity pool, the desired vesting period in years, and the cliff period in months.

**Q: What determines the governance rights?**
Governance is determined via `determine_governance_rights`, which evaluates the equity split and whether the builder is an institutional entity with fiduciary duties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-venture-builder-equity-split](https://vinkius.com/ai-agent-connect/accelerator-venture-builder-equity-split)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Venture Builder Equity Split** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-venture-builder-equity-split` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Venture Builder Equity Split** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-venture-builder-equity-split": {
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
