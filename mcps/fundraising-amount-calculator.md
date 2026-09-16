# Fundraising Amount Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fundraising-amount-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate optimal capital requirements, runway extensions, and dilution impact.

## Description
This MCP server provides strategic financial planning tools for startups. It connects AI agents to critical fundraising calculations, including determining the total capital needed via `get_target_raise`, calculating runway extensions with `get_runway_extension`, predicting equity impact using `estimate_dilution`, and identifying the ideal fundraising window with `calculate_fundraising_timing`.


## Available Tools (4)
- **calculate_fundraising_timing**: Identifies the strategic window for when the company should begin the fundraising process
- **estimate_dilution**: Predicts the impact of a fundraising round on existing equity holders
- **get_runway_extension**: Calculates how much additional time the company gains by raising a specific amount of capital
- **get_target_raise**: Determines the total capital required to satisfy the runway target and reach defined milestones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fundraising Amount Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much should I raise if my monthly burn is $50,000, I want 18 months of runway, and I have a milestone costing $100,000 in 6 months? Use a 10% buffer."

**🤖 AI Agent:**
> To cover 18 months of burn ($900,000) and the $100,000 milestone with a 10% buffer, your target raise is $1,100,000.

---

**👤 You:**
> "If I have $200,000 in cash and a monthly burn of $40,000, how many months of runway do I have?"

**🤖 AI Agent:**
> You currently have 5 months of runway.

---

**👤 You:**
> "I own 20% of my company. If I raise $2,000,000 at a $10,000,000 post-money valuation, what will my new ownership be?"

**🤖 AI Agent:**
> Your new ownership stake will be 16%.


## ❓ FAQ

**Q: How do I calculate my target raise?**
You can use the `get_target_raise` tool by providing your monthly burn, desired runway months, and any upcoming milestones.

**Q: Can I estimate how much my ownership will decrease?**
Yes, the `estimate_dilution` tool allows you to predict the impact of a new funding round on your current equity percentage.

**Q: How do I know when to start fundraising?**
The `calculate_fundraising_timing` tool identifies the strategic window to start your raise based on current cash and expected duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fundraising-amount-calculator](https://vinkius.com/en/ai-agent-connect/fundraising-amount-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fundraising Amount Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fundraising-amount-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fundraising Amount Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fundraising-amount-calculator": {
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
