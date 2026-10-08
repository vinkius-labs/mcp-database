# Raise Negotiation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/raise-negotiation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the real impact of salary increases, bonuses, and benefits on your take-home pay.

## Description
This MCP server provides precise financial modeling for professional compensation negotiations. Use `calculate_current_compensation` to establish your baseline, then use `compare_raise_proposals` to evaluate different salary and bonus scenarios. You can also use `check_target_attainment` to see if a proposal meets your specific percentage goals, or `simulate_benefit_impact` to understand how changes in benefit packages affect your total compensation package.


## Available Tools (4)
- **calculate_current_compensation**: Establishes the baseline financial state before any negotiation occurs
- **check_target_attainment**: Determines if a specific raise proposal meets a user's predefined percentage goal
- **compare_raise_proposals**: Evaluates multiple potential salary or bonus increases against the current baseline
- **simulate_benefit_impact**: Analyzes how changing benefit packages shifts the total compensation and net pay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Raise Negotiation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I currently earn $100,000 salary, $10,000 bonus, and $5,000 in benefits with a 25% tax rate. What is my current monthly take-home pay?"

**🤖 AI Agent:**
> Your current net monthly pay is $6,750.00.

---

**👤 You:**
> "If I get a raise to $120,000 salary and $15,000 bonus with the same 25% tax rate, how much will my monthly pay increase?"

**🤖 AI Agent:**
> Your net monthly pay will increase by $1,875.00.

---

**👤 You:**
> "I want a 15% increase in total compensation. If my current total compensation is $115,000, will a $130,000 salary and $5,000 bonus meet my goal?"

**🤖 AI Agent:**
> Yes, that proposal meets your target. The actual percentage increase is 17.39%.


## ❓ FAQ

**Q: How do I calculate my current baseline?**
Use the `calculate_current_compensation` tool by providing your current annual salary, bonus, benefits value, and tax rate.

**Q: Can I compare multiple different raise offers?**
Yes, use `compare_raise_proposals` to evaluate how different combinations of salary and bonus affect your net monthly pay and total compensation.

**Q: Does this tool account for taxes?**
Yes, the tools use the tax rate you provide to calculate the difference between gross income and your actual net monthly take-home pay.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/raise-negotiation-calculator](https://vinkius.com/en/ai-agent-connect/raise-negotiation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Raise Negotiation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `raise-negotiation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Raise Negotiation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "raise-negotiation-calculator": {
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
