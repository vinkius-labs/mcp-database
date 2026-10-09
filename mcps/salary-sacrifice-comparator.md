# Salary Sacrifice Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/salary-sacrifice-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Compare cash compensation against salary sacrifice benefits to find your true total compensation.

## Description
This MCP server provides a suite of financial tools to evaluate the impact of salary sacrifice arrangements. It models how giving up gross salary for benefits like pensions or electric vehicles affects your monthly take-home pay and overall wealth. Use `compare_cash_vs_sacrifice` to see immediate cash flow changes, `calculate_tax_burden` to model progressive taxation, `evaluate_pension_impact` to project retirement growth, and `get_effective_total_compensation` to determine your true total wealth including benefits and employer contributions.


## Available Tools (4)
- **calculate_tax_burden**: Calculates total annual tax liability based on income and brackets
- **compare_cash_vs_sacrifice**: Compares monthly take-home pay between cash salary and salary sacrifice
- **evaluate_pension_impact**: Evaluates annual pension growth and net cost of sacrifice
- **get_effective_total_compensation**: Calculates the holistic annual total compensation value


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salary Sacrifice Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I earn £50,000. If I sacrifice £5,000 for an electric vehicle worth £6,000 and my employer adds £1,000, what is my monthly take-home pay difference?"

**🤖 AI Agent:**
> Your monthly take-home pay will decrease by £320, but your total monthly value gain will be £450 when accounting for the vehicle and employer contribution.

---

**👤 You:**
> "What is the impact of sacrificing £2,000 into my pension if my employer matches £500 and I save £400 in tax?"

**🤖 AI Agent:**
> Your annual pension growth will be £2,500, and the net cost of this sacrifice is only £1,600.

---

**👤 You:**
> "Calculate my total compensation if my net pay is £35,000, my benefits are worth £5,000, and employer contributions are £3,000."

**🤖 AI Agent:**
> Your annual total value is £43,000.


## ❓ FAQ

**Q: How does salary sacrifice affect my monthly take-home pay?**
By using `compare_cash_vs_sacrifice`, you can see how reducing your gross salary to pay for a benefit changes your net monthly income after taxes and social security are applied.

**Q: Can I calculate my total wealth including benefits?**
Yes, the `get_effective_total_compensation` tool calculates your holistic value by summing net take-home pay, the value of benefits, and employer contributions.

**Q: How do I model different tax brackets?**
You can use `calculate_tax_burden` by providing a JSON array of tax thresholds and rates to model progressive taxation accurately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/salary-sacrifice-comparator](https://vinkius.com/en/ai-agent-connect/salary-sacrifice-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salary Sacrifice Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salary-sacrifice-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salary Sacrifice Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salary-sacrifice-comparator": {
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
