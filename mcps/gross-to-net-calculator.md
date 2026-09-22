# Gross-to-Net Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gross-to-net-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise take-home pay by applying fixed and percentage-based deductions to gross income.

## Description
This MCP server provides a suite of financial tools to accurately determine net pay. Users can use `calculate_net_pay` to find the final take-home amount after all subtractions, `validate_deduction_limit` to ensure deductions stay within a healthy percentage of income, `get_deduction_summary` to see a breakdown of fixed versus percentage costs, and `simulate_tax_impact` to model how changing a specific tax or fee affects the final result.


## Available Tools (4)
- **calculate_net_pay**: Calculates the final net pay for an individual based on a provided gross amount and a list of deductions
- **get_deduction_summary**: Provides a breakdown of how much was taken out via fixed amounts versus percentage-based amounts
- **simulate_tax_impact**: Determines how much the net pay would change if a specific percentage-based deduction was increased or decreased
- **validate_deduction_limit**: Checks if a proposed set of deductions exceeds a predefined maximum percentage of the gross income


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gross-to-Net Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my net pay for a gross income of 5000 with a 200 fixed fee and a 10% tax."

**🤖 AI Agent:**
> Your net pay is 4300.00. Total deductions were 700.00.

---

**👤 You:**
> "Show me a summary of these deductions: a 50 fixed fee and a 5% health insurance fee."

**🤖 AI Agent:**
> The summary includes 1 fixed deduction totaling 50.00 and 1 percentage deduction totaling 5.00% of the gross amount.

---

**👤 You:**
> "What happens to my 4000 net pay if my 15% tax increases to 18%?"

**🤖 AI Agent:**
> Increasing the tax from 15% to 18% will reduce your net pay by 120.00.


## ❓ FAQ

**Q: How do I calculate my final take-home pay?**
You can use the `calculate_net_pay` tool by providing your gross income and a list of your deductions.

**Q: Can I see how a tax increase will affect my paycheck?**
Yes, the `simulate_tax_impact` tool allows you to adjust a specific percentage-based deduction to see the resulting change in net pay.

**Q: How can I check if my deductions are too high?**
Use the `validate_deduction_limit` tool to check if your total deductions exceed a specific percentage of your gross pay.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gross-to-net-calculator](https://vinkius.com/en/ai-agent-connect/gross-to-net-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gross-to-Net Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gross-to-net-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gross-to-Net Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gross-to-net-calculator": {
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
