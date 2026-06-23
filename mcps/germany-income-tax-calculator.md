# Germany Income Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/germany-income-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate German income tax, social security contributions, and net take-home pay.

## Description
This MCP server provides a precise computation engine for determining German income tax liabilities. Using the `calculate_tax_breakdown` tool, you can input your annual gross salary to receive a detailed breakdown of progressive income tax, solidarity surcharge (Soli), and church tax based on your federal state. Additionally, it accounts for mandatory social security contributions--including health, pension, unemployment, and long-term care insurance--while respecting the statutory contribution assessment ceilings. You can also use `get_social_security_rates` to check current employee contribution percentages or `list_church_tax_regions` to identify which German states apply an 8% vs 9% church tax rate.


## Available Tools (3)
- **get_social_security_rates**: Retrieve current social security percentage rates
- **calculate_tax_breakdown**: Calculate German income tax breakdown
- **list_church_tax_regions**: List states by church tax rate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Germany Income Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will my net annual income be if I earn 60,000 EUR gross, am a church member, and live in Bavaria?"

**🤖 AI Agent:**
> With a gross annual income of 60,000 EUR in Bavaria, your estimated net annual income is approximately 38,450 EUR after all taxes and social security deductions.

---

**👤 You:**
> "Which German states have a 9% church tax rate?"

**🤖 AI Agent:**
> The states with a 9% church tax rate include Berlin, Brandenburg, Hesse, Lower Saxony, North Rhine-Westphalia, Rhineland-Palatinate, and Saxony.

---

**👤 You:**
> "What are the current employee rates for health insurance?"

**🤖 AI Agent:**
> The current employee share for health insurance is 7.3% (plus the specific additive contribution of your provider).


## ❓ FAQ

**Q: How do I calculate my net annual salary?**
Use the `calculate_tax_breakdown` tool by providing your annual gross income, whether you are a church member, and your German federal state.

**Q: Does this include social security deductions?**
Yes, the `calculate_tax_breakdown` tool calculates all mandatory contributions for health, pension, unemployment, and care insurance, respecting the annual contribution assessment ceilings.

**Q: How can I check the current social security rates?**
You can use the `get_social_security_rates` tool to retrieve the latest employee share percentages for all mandatory insurance components.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/germany-income-tax-calculator](https://vinkius.com/mcp/germany-income-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Germany Income Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `germany-income-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Germany Income Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "germany-income-tax-calculator": {
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
