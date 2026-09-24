# Accessible Transport Disruption Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-transport-disruption-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Automated contingency protocols for users with accessibility needs during transport disruptions.

## Description
This MCP server provides critical contingency management for users with mobility requirements. It allows AI agents to manage transport failures by generating disruption triggers, contact orders, and replacement actions. Use `get_disruption_plan` to generate contingency responses, `validate_journey_parameters` to ensure accessibility compliance, `get_provider_status` to monitor delays, and `simulate_fallback_sequence` to test the viability of fallback rules.


## Available Tools (4)
- **get_disruption_plan**: Generates a complete contingency response for a specific journey when a disruption occurs
- **get_provider_status**: Checks the current availability or delay status of a specific transport provider
- **simulate_fallback_sequence**: Tests a user's fallback rules against a hypothetical disruption to ensure the plan is viable
- **validate_journey_parameters**: Ensures a new recurring journey configuration is logically sound and meets accessibility requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Transport Disruption Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My primary transport provider is delayed by 20 minutes. What is the contingency plan?"

**🤖 AI Agent:**
> The disruption trigger has been activated. The system will notify your primary contact via SMS and then attempt to book your secondary provider, Provider B.

---

**👤 You:**
> "Check if my current transport provider is available for my 10:00 AM trip."

**🤖 AI Agent:**
> Provider Alpha is currently available and is running on schedule for your 10:00 AM trip.

---

**👤 You:**
> "Is my new journey configuration valid for someone using a wheelchair?"

**🤖 AI Agent:**
> The journey configuration is valid. All selected pickup points are marked as accessible and the fallback providers are correctly prioritized.


## ❓ FAQ

**Q: How does the system handle a provider delay?**
The system uses `get_disruption_plan` to evaluate if a delay exceeds the user's maximum acceptable limit and then triggers the pre-defined fallback rules.

**Q: Can I test my fallback rules before a real disruption occurs?**
Yes, you can use the `simulate_fallback_sequence` tool to run hypothetical failure scenarios and verify that the replacement actions are viable.

**Q: How are accessibility requirements enforced?**
The `validate_journey_parameters` tool ensures that all pickup points are explicitly marked as accessible and that the journey configuration is logically sound.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-transport-disruption-plan](https://vinkius.com/en/ai-agent-connect/accessible-transport-disruption-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Transport Disruption Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-transport-disruption-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Transport Disruption Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-transport-disruption-plan": {
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
