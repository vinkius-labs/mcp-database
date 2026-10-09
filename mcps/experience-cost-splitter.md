# Experience Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/experience-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Split the cost of shared experiences like tours or classes equally among participants.

## Description
This MCP server provides tools to manage shared expenses for group activities. You can use `calculate_individual_shares` to determine exactly what each person owes, `validate_experience_budget` to check if a cost fits within budget, mid-range, or luxury tiers, and `calculate_per_person_savings` to see how much the group saves compared to solo pricing. It ensures mathematical precision for every split.


## Available Tools (4)
- **calculate_individual_shares**: 
- **calculate_per_person_savings**: 
- **get_participant_summary**: 
- **validate_experience_budget**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Experience Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We spent $150 on a cooking class for 4 people. How much does each person owe?"

**🤖 AI Agent:**
> Each person owes $37.50.

---

**👤 You:**
> "Is a $250 guided tour within the luxury budget tier?"

**🤖 AI Agent:**
> No, the cost exceeds the limit for the luxury tier.

---

**👤 You:**
> "A solo museum visit is $40, but a group of 5 can do it for $100 total. How much does each person save?"

**🤖 AI Agent:**
> Each person saves $32.00.


## ❓ FAQ

**Q: How does the tool handle remainders when splitting costs?**
The `calculate_individual_shares` tool uses rounding logic to ensure the sum of all individual shares equals the original total cost exactly.

**Q: Can I check if my tour fits my budget?**
Yes, you can use `validate_experience_budget` to check if your planned cost falls within the budget, mid-range, or luxury tiers.

**Q: What AI clients can I use with this server?**
You can connect this server to Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/experience-cost-splitter](https://vinkius.com/en/ai-agent-connect/experience-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Experience Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `experience-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Experience Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "experience-cost-splitter": {
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
