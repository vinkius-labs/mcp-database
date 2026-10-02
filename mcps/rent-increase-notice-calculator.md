# Rent Increase Notice Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rent-increase-notice-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify the financial and legal impact of rent increase notices.

## Description
This MCP server provides tools to analyze the impact of rent increases. Use `calculate_impact` to find the monthly and total cost increase, `get_milestones` to map out key dates, `verify_compliance` to check if notice periods meet legal requirements, or `analyze_lease_scenario` for a complete overview of the financial and temporal impact.


## Available Tools (4)
- **analyze_lease_scenario**: Provides a high-level summary of the financial and temporal impact for decision making
- **calculate_impact**: Determines the immediate and long-term financial consequences of the proposed rent increase
- **get_milestones**: Maps out the timeline of the rent change process
- **verify_compliance**: Checks if the notice was provided with enough lead time to be legally valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rent Increase Notice Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am paying $2000 and my landlord wants to increase it to $2200. I have 6 months left on my lease. What is the impact?"

**🤖 AI Agent:**
> The monthly increase is $200, and the total increase for the remaining 6 months of your lease is $1,200.

---

**👤 You:**
> "My notice was given on 2024-01-01 and the increase starts on 2024-02-15. Is this compliant if the law requires 30 days notice?"

**🤖 AI Agent:**
> No, the notice period provided is 45 days, which meets the 30-day requirement. Wait, let me re-calculate: from Jan 1 to Feb 15 is 45 days. Since 45 is greater than 30, it is compliant.

---

**👤 You:**
> "Show me the timeline for a notice issued on 2024-05-01, effective 2024-06-01, with the lease ending 2024-12-31."

**🤖 AI Agent:**
> The notice was issued on 2024-05-01, the increase takes effect on 2024-06-01, and your lease ends on 2024-12-31. The notice period was 31 days.


## ❓ FAQ

**Q: How can I calculate the total cost of a rent increase?**
You can use the `calculate_impact` tool by providing the current rent, the proposed rent, and the number of months remaining in your lease.

**Q: Can this tool check if my landlord gave enough notice?**
Yes, the `verify_compliance` tool allows you to check if the notice period meets the minimum days required by your local laws.

**Q: What dates do I need for a full scenario analysis?**
To use `analyze_lease_scenario`, you will need the current rent, proposed rent, remaining lease months, notice date, effective date, and lease end date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rent-increase-notice-calculator](https://vinkius.com/en/ai-agent-connect/rent-increase-notice-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rent Increase Notice Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rent-increase-notice-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rent Increase Notice Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rent-increase-notice-calculator": {
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
