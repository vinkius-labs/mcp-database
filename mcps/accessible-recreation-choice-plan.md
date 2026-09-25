# Accessible Recreation Choice Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-recreation-choice-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

An intelligent decision engine that matches accessibility needs and interests to actionable recreation plans.

## Description
This MCP server provides a specialized decision engine for planning accessible recreation. It uses `get_eligible_activities` to filter options based on mandatory constraints like cost and accessibility features. Once eligible options are found, `generate_activity_plan` selects the best match based on user interests and pace. The server also includes `get_alternative_options` for fallback choices and `validate_participation_readiness` to ensure users have the necessary equipment and support for their chosen activity.


## Available Tools (4)
- **generate_activity_plan**: Selects the best activity from the eligible list and generates a plan
- **get_alternative_options**: Provides fallback options when the primary plan cannot be fully met
- **get_eligible_activities**: Identifies which recreation options satisfy all user-defined mandatory constraints
- **validate_participation_readiness**: Checks if the user's equipment and companion status are sufficient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Recreation Choice Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to go to a park. I need wheelchair access and my budget is $20."

**🤖 AI Agent:**
> The local Central Park is available for $0 and features full wheelchair access via the north entrance.

---

**👤 You:**
> "Suggest a high-intensity activity for someone interested in nature."

**🤖 AI Agent:**
> The Mountain Trail Hike is a great high-intensity option that matches your interest in nature.

---

**👤 You:**
> "Am I ready for the adaptive skiing trip with my current gear?"

**🤖 AI Agent:**
> You are missing the required adaptive skis; please ensure you have them or book them in advance.


## ❓ FAQ

**Q: How does the engine ensure activities meet my accessibility needs?**
The `get_eligible_activities` tool filters all available options against your mandatory criteria, such as specific accessibility features or cost limits, to ensure only suitable activities are considered.

**Q: Can I check if I have the right equipment before I go?**
Yes, you can use `validate_participation_readiness` to compare your current equipment and companion availability against the requirements of your selected activity.

**Q: What happens if my first choice doesn't match all my interests?**
If the primary plan doesn't meet all your preferences, you can use `get_alternative_options` to find other activities that still respect your mandatory accessibility requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-recreation-choice-plan](https://vinkius.com/en/ai-agent-connect/accessible-recreation-choice-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Recreation Choice Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-recreation-choice-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Recreation Choice Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-recreation-choice-plan": {
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
