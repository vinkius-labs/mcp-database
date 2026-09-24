# Assistive Equipment Selection Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/assistive-equipment-selection-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

A decision-support system for evaluating assistive technology against user constraints.

## Description
This MCP server provides specialized tools to evaluate assistive technology. Use `analyze_fit` to determine if equipment meets user profiles and environmental dimensions. Use `generate_vendor_inquiry` to clarify technical details, `create_trial_plan` to structure real-world testing, and `plan_acquisition` to outline the steps for purchase or lease.


## Available Tools (4)
- **generate_vendor_inquiry**: Creates a targeted list of questions for vendors to clarify ambiguities or confirm technical compatibility
- **plan_acquisition**: Outlines the logistical steps required to purchase or lease the equipment
- **analyze_fit**: Determines if specific equipment options meet the user's defined criteria and environmental constraints
- **create_trial_plan**: Formulates a structured schedule and checklist for testing the selected equipment in the user's real-world environment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Assistive Equipment Selection Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this wheelchair fits my needs."

**🤖 AI Agent:**
> The wheelchair meets your requirement for portability and fits through your 30-inch doorway.

---

**👤 You:**
> "What questions should I ask the vendor about the mobility aid?"

**🤖 AI Agent:**
> You should ask: 'Will the battery life support 12 hours of continuous use?' and 'Is the frame compatible with standard charging docks?'

---

**👤 You:**
> "Create a plan to test the new walker."

**🤖 AI Agent:**
> The trial will last 7 days. You should test the walker during morning walks and while navigating kitchen surfaces to ensure stability.


## ❓ FAQ

**Q: How does the tool evaluate equipment suitability?**
The `analyze_fit` tool compares equipment specifications against user-provided daily activities, environmental dimensions, and feature requirements.

**Q: Can I plan the purchase of the equipment?**
Yes, the `plan_acquisition` tool generates a logical sequence of steps for purchasing or leasing equipment within your budget.

**Q: How are trial periods managed?**
The `create_trial_plan` tool uses your specific trial terms and daily activities to create a structured testing schedule and checklist.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/assistive-equipment-selection-brief](https://vinkius.com/en/ai-agent-connect/assistive-equipment-selection-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Assistive Equipment Selection Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `assistive-equipment-selection-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Assistive Equipment Selection Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "assistive-equipment-selection-brief": {
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
