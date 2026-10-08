# Salary Offer Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/salary-offer-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Compare job offers by normalizing salary, taxes, cost of living, and lifestyle factors.

## Description
This MCP server provides a comprehensive framework for evaluating job offers. It allows AI agents to perform side-by-side comparisons using `compare_offers` to identify the best financial and lifestyle choice. Users can determine the true value of their time with `calculate_effective_hourly_rate`, quantify quality of life improvements via `evaluate_lifestyle_impact`, and calculate purchasing power using `estimate_net_disposable_income` which accounts for local cost of living and tax burdens.


## Available Tools (4)
- **calculate_effective_hourly_rate**: Determines the true value of an offer by accounting for all hours worked, including commuting
- **estimate_net_disposable_income**: Calculates the actual cash remaining after taxes for a specific location
- **evaluate_lifestyle_impact**: Quantifies the impact of remote work, commute, and working hours on the overall quality of life
- **compare_offers**: Provide a JSON string of offer objects and optionally specify a primary metric to rank by.

Performs a direct side-by-side comparison of multiple job offers to identify the best financial and lifestyle choice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salary Offer Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare two offers: Offer A is $100k with 2 days remote, and Offer B is $110k with 0 days remote. Which is better for lifestyle?"

**🤖 AI Agent:**
> Offer A provides a higher lifestyle score due to the remote work flexibility, even though Offer B has a higher nominal salary.

---

**👤 You:**
> "What is my effective hourly rate if I earn $120,000, have a $10,000 bonus, and work 40 hours plus 5 hours of commuting per week?"

**🤖 AI Agent:**
> $41.38 per hour.

---

**👤 You:**
> "Calculate my net disposable income for a $150,000 salary in a city with a 30% tax rate and a 1.2 cost of living index."

**🤖 AI Agent:**
> Your net disposable income is $105,000, with a cost of living adjusted income of $87,500.


## ❓ FAQ

**Q: How does the tool account for different cities?**
The tool uses `estimate_net_disposable_income` to adjust income based on a local cost of living index, showing the actual purchasing power in different regions.

**Q: Can I compare multiple offers at once?**
Yes, you can use the `compare_offers` tool to provide multiple offer profiles and rank them by metrics like net income or lifestyle score.

**Q: Does it include commute time in the calculations?**
Yes, `calculate_effective_hourly_rate` factors in weekly commute hours to determine the true hourly value of your time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/salary-offer-comparator](https://vinkius.com/en/ai-agent-connect/salary-offer-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salary Offer Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salary-offer-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salary Offer Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salary-offer-comparator": {
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
