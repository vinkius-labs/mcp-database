# Benefit Total Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/benefit-total-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Aggregate and analyze employee total compensation packages.

## Description
This MCP server provides tools to calculate the full economic value of employee compensation. It allows users to sum base salaries with various benefit categories to find the total reward. Use `calculate_total_compensation` to get a full breakdown, `get_category_totals` to see spending by type, `validate_benefit_structure` to check data integrity, and `find_highest_benefit_category` to identify the largest supplemental benefit.


## Available Tools (4)
- **calculate_total_compensation**: Calculate the total monetary value of an employee's full compensation package
- **find_highest_benefit_category**: Identify the benefit category with the highest cumulative sum
- **get_category_totals**: Get the total amount spent on each specific type of benefit
- **validate_benefit_structure**: Validate if the set of benefit values is formatted correctly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Benefit Total Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total compensation for an employee with a 100000 base salary and benefits: health 5000 and retirement 2000?"

**🤖 AI Agent:**
> The total compensation is 107000.

---

**👤 You:**
> "Show me the total spent on each benefit category for: health 5000, health 2000, and wellness 1000."

**🤖 AI Agent:**
> The totals are: health 7000 and wellness 1000.

---

**👤 You:**
> "Which benefit category is the largest for: insurance 3000, travel 5000, and gym 1000?"

**🤖 AI Agent:**
> The largest benefit category is travel.


## ❓ FAQ

**Q: How do I calculate the total compensation?**
You can use the `calculate_total_compensation` tool by providing the annual base salary and a list of benefit objects.

**Q: Can I check if my benefit data is valid?**
Yes, use the `validate_benefit_structure` tool to ensure your benefit objects contain the required category and amount fields.

**Q: How can I see which benefit is the most expensive?**
The `find_highest_benefit_category` tool will identify which category has the highest cumulative sum.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/benefit-total-calculator](https://vinkius.com/en/ai-agent-connect/benefit-total-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Benefit Total Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `benefit-total-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Benefit Total Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "benefit-total-calculator": {
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
