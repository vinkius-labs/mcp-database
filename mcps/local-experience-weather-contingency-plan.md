# Local Experience Weather Contingency Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-experience-weather-contingency-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Evaluate outdoor activities against weather thresholds and provider rules to generate actionable contingency plans.

## Description
This MCP server provides a decision-support engine for managing outdoor activities. It evaluates planned experiences against user-defined weather thresholds and provider cancellation policies. Using tools like `analyze_contingency_status` and `generate_communication_templates`, it determines whether to proceed, pivot to an indoor alternative, or cancel entirely. It also calculates financial implications and provides ready-to-use communication templates for participants and providers.


## Available Tools (2)
- **analyze_contingency_status**: Determines if the current plan is still viable based on weather and provider rules
- **generate_communication_templates**: Provides ready-to-use messages for participants and providers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Experience Weather Contingency Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My hiking trip is threatened by rain. Should I go or cancel?"

**🤖 AI Agent:**
> Based on the forecast of heavy rain and your threshold, the status is 'Change'. You should pivot to the indoor botanical garden visit instead of hiking.

---

**👤 You:**
> "The wind speed is too high for our boat tour. What should I do?"

**🤖 AI Agent:**
> The status is 'Cancel'. Since the provider offers a full refund for weather-related cancellations, you should contact them immediately before the decision deadline.

---

**👤 You:**
> "It's going to be 35 degrees Celsius today. Is my picnic okay?"

**🤖 AI Agent:**
> The status is 'Go'. The temperature is within your defined threshold for outdoor activities.


## ❓ FAQ

**Q: How does the tool decide if I should cancel?**
The `analyze_contingency_status` tool compares your weather forecast against your personal thresholds and the provider's specific weather policies to determine the best course of action.

**Q: Can I get messages ready to send to my group?**
Yes, once a status is determined, you can use `generate_communication_templates` to create messages for both participants and providers based on the required tone.

**Q: Does it handle refund calculations?**
Yes, the engine evaluates provider rules to calculate expected recovery or potential loss during a cancellation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-experience-weather-contingency-plan](https://vinkius.com/en/ai-agent-connect/local-experience-weather-contingency-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Experience Weather Contingency Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-experience-weather-contingency-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Experience Weather Contingency Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-experience-weather-contingency-plan": {
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
