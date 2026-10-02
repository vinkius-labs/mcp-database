# Family Photo Print Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-photo-print-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize photo print quantities and costs based on albums, recipients, and budget.

## Description
This MCP server provides a planning engine to manage photo printing projects. It allows AI agents to coordinate print quantities from various albums, account for recipient needs, and optimize spending against a specific budget. Using tools like `query_available_albums`, `query_print_pricing`, `query_frame_options`, and `calculate_print_plan`, an agent can determine the best combination of print sizes and frames to satisfy as many people as possible while staying within financial constraints.


## Available Tools (4)
- **calculate_print_plan**: 
- **query_frame_options**: 
- **query_available_albums**: 
- **query_print_pricing**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Photo Print Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 5 albums and I want to give prints to 10 people. My budget is $50. What is the best plan using 4x6 prints?"

**🤖 AI Agent:**
> You can provide 10 prints of size 4x6 for a total cost of $42.00, which fits within your $50 budget.

---

**👤 You:**
> "What are the available frame options and their prices?"

**🤖 AI Agent:**
> The available frames are: Classic Wood ($5.00), Modern Black ($4.00), and Minimalist White ($3.50).

---

**👤 You:**
> "List all available albums."

**🤖 AI Agent:**
> The available albums are: 'Summer 2023' (50 photos), 'Family Reunion' (120 photos), and 'Birthday Party' (30 photos).


## ❓ FAQ

**Q: How does the budget optimization work?**
The system uses `calculate_print_plan` to prioritize recipient satisfaction by selecting the best print sizes and frame options that fit within your specified budget.

**Q: Can I see which albums are available for printing?**
Yes, you can use the `query_available_albums` tool to list all registered photo collections and their contents.

**Q: Does the plan include frame costs?**
Yes, if you set the includeFrames parameter to true in `calculate_print_plan`, the engine will attempt to include frames in the optimal plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-photo-print-planner](https://vinkius.com/en/ai-agent-connect/family-photo-print-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Photo Print Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-photo-print-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Photo Print Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-photo-print-planner": {
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
