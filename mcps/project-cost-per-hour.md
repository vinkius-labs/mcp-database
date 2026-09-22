# Project Cost Per Hour MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/project-cost-per-hour)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate project efficiency by analyzing cost per hour metrics.

## Description
This MCP server provides tools to analyze project efficiency by calculating the relationship between total expenditure and time investment. Use `get_project_cph` to find the cost per hour for a specific project, `compare_project_efficiency` to determine which of two projects was more cost-effective, or `list_high_cost_projects` to identify projects exceeding specific budget thresholds. It also offers `get_project_resource_summary` for a detailed breakdown of costs and hours.


## Available Tools (4)
- **list_high_cost_projects**: Identifies projects that exceed a specific cost-per-hour threshold
- **compare_project_efficiency**: Compares the cost-per-hour metrics of two different projects
- **get_project_cph**: Calculates the cost per hour for a specific project
- **get_project_resource_summary**: Provides a breakdown of total cost and total hours for a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Project Cost Per Hour** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cost per hour for project PROJ-123?"

**🤖 AI Agent:**
> The cost per hour for project PROJ-123 is $55.00, with a total cost of $5,500.00 over 100 hours.

---

**👤 You:**
> "Which project was more efficient: PROJ-A or PROJ-B?"

**🤖 AI Agent:**
> Project PROJ-A was more efficient with a cost per hour of $45.00 compared to $50.00 for PROJ-B.

---

**👤 You:**
> "Show me projects where the cost per hour is higher than $100."

**🤖 AI Agent:**
> The following projects exceed the $100 threshold: PROJ-999 ($120.00) and PROJ-888 ($150.00).


## ❓ FAQ

**Q: How is the cost per hour calculated?**
The cost per hour is calculated by dividing the total project cost by the total project hours recorded.

**Q: What does it mean if a project is 'more efficient'?**
A project is considered more efficient if it has a lower cost per hour, meaning less money was spent for every hour of work completed.

**Q: Can I identify projects that are over budget?**
Yes, you can use `list_high_cost_projects` to find all projects where the cost per hour exceeds a threshold you define.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/project-cost-per-hour](https://vinkius.com/en/ai-agent-connect/project-cost-per-hour)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Project Cost Per Hour** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `project-cost-per-hour` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Project Cost Per Hour** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "project-cost-per-hour": {
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
