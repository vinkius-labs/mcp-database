# Contractor Safety Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/contractor-safety-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-management](../categories/risk-management.md)

Manage contractor safety compliance, risk tiering, and monitoring requirements.

## Description
This MCP server provides tools to manage contractor safety programs by evaluating qualifications and risk exposure. Use `get_prequalification_status` to verify if a contractor is eligible for a specific scope of work. Generate inspection schedules with `calculate_monitoring_plan` and track safety metrics using `get_contractor_performance_score`. For high-risk tasks, use `evaluate_high_risk_exposure` to identify hazards and mandatory mitigations.


## Available Tools (4)
- **calculate_monitoring_plan**: Defines how often and in what manner a contractor must be inspected
- **get_prequalification_status**: Determines if a contractor is eligible to perform a specific scope of work
- **evaluate_high_risk_exposure**: Identifies specific safety hazards and required precautions for a proposed engagement
- **get_contractor_performance_score**: Retrieves a quantitative assessment of a contractor safety performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contractor Safety Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is contractor C-123 eligible for the upcoming electrical maintenance task?"

**🤖 AI Agent:**
> The contractor is Approved for this scope of work.

---

**👤 You:**
> "What are the safety risks for the confined space entry task (SOW-99)?"

**🤖 AI Agent:**
> The risk level is High. Identified hazards include oxygen deficiency and toxic fumes. Mandatory mitigations include atmospheric testing and continuous ventilation.

---

**👤 You:**
> "What was the safety score for contractor C-456 from 2023-01-01 to 2023-12-31?"

**🤖 AI Agent:**
> The safety score for contractor C-456 is 92, with 0 incidents and a 98% compliance rate.


## ❓ FAQ

**Q: How do I check if a contractor can perform a specific task?**
You can use the `get_prequalification_status` tool to determine if a contractor meets the safety requirements for a given scope of work.

**Q: Can I see the safety performance of a contractor?**
Yes, the `get_contractor_performance_score` tool provides safety scores, incident counts, and compliance rates for a specified period.

**Q: How are inspection frequencies determined?**
The `calculate_monitoring_plan` tool calculates inspection frequency and required permits based on the risk level and contractor profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/contractor-safety-management](https://vinkius.com/en/ai-agent-connect/contractor-safety-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contractor Safety Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contractor-safety-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contractor Safety Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contractor-safety-management": {
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
