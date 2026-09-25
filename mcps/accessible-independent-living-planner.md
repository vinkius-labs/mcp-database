# Accessible Independent Living Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-independent-living-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Transforms independence goals into autonomy-first action plans and support requests.

## Description
This MCP server provides a reasoning engine to convert personal independence goals into structured, autonomy-first action plans. It helps users navigate transitions by generating staged roadmaps, identifying necessary third-party requests, and calculating required support adjustments. By using `generate_action_plan`, users can create sequenced steps that respect their specific environmental constraints and permitted supports. The engine also includes `generate_decision_log` to ensure every step prioritizes the user's autonomy and consent, providing a clear record of why specific paths were chosen over traditional assistance models.


## Available Tools (5)
- **generate_decision_log**: Documents the logic behind the plan, specifically highlighting autonomy-driven decisions
- **identify_external_requests**: Identifies specific entities or individuals the user must contact to move the plan forward
- **calculate_support_adjustments**: Determines what changes are needed to current support systems to meet the new goal
- **create_review_checkpoints**: Generates a schedule of measurable milestones to track progress
- **generate_action_plan**: Converts the user's goal and constraints into a sequenced roadmap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Independent Living Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to move into my own apartment by December. I currently live with parents, have $5000 in savings, and can only accept physical help with moving heavy items."

**🤖 AI Agent:**
> To achieve your goal of moving by December, we will follow a three-stage plan: 1. Financial and Housing Search (securing the apartment and budgeting), 2. Logistics Preparation (arranging physical help for heavy items), and 3. Transition (the actual move).

---

**👤 You:**
> "Help me plan for increased independence in managing my own finances."

**🤖 AI Agent:**
> I will use `generate_action_plan` to create a roadmap for your financial independence, focusing on cognitive-administrative support and setting up review checkpoints to track your progress.

---

**👤 You:**
> "What changes do I need to make to my current support to live more independently?"

**🤖 AI Agent:**
> I will use `calculate_support_adjustments` to identify the specific shifts needed between your current arrangements and your target state, ensuring all changes align with your permitted supports.


## ❓ FAQ

**Q: How does this tool prioritize my autonomy?**
The engine uses `generate_decision_log` to document how every plan step and support adjustment respects your stated autonomy and consent priorities, ensuring your preferences take precedence over standard assistance models.

**Q: Can I limit what kind of help I receive?**
Yes. You define your 'permitted supports' during the planning process. The `identify_external_requests` tool will only suggest contacts that fall within those boundaries.

**Q: What is a staged action plan?**
A staged action plan is a sequential roadmap created by `generate_action_plan` that breaks your goal down into logical phases, such as preparation and implementation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-independent-living-planner](https://vinkius.com/en/ai-agent-connect/accessible-independent-living-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Independent Living Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-independent-living-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Independent Living Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-independent-living-planner": {
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
