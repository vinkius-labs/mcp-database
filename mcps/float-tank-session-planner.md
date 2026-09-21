# Float Tank Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/float-tank-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Personalized sensory environments and preparation protocols for float therapy.

## Description
This MCP server provides specialized tools to design customized float therapy experiences. It uses `plan_session_parameters` to generate complete session roadmaps, including recommended durations and sensory configurations. Users can use `validate_sensory_config` to ensure light and sound settings are safe for their experience level, `get_preparation_checklist` for pre-float physical tasks, and `calculate_integration_schedule` to determine necessary post-float downtime.


## Available Tools (4)
- **calculate_integration_schedule**: Determines the necessary downtime after a session to prevent disorientation
- **get_preparation_checklist**: Provides a specific list of physical preparations based on the user's goal
- **plan_session_parameters**: Generates a complete, customized float session roadmap
- **validate_sensory_config**: Checks if a specific light and sound combination is safe and effective


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Float Tank Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a novice looking for a relaxation session. Can you plan my float?"

**🤖 AI Agent:**
> For your relaxation session, I recommend a 60-minute duration with soft blue light and ambient nature sounds. Please ensure you hydrate well and shower before entering the tank.

---

**👤 You:**
> "I want deep meditation. I am an expert. What should my settings be?"

**🤖 AI Agent:**
> As an expert, you can utilize total sensory deprivation. I recommend 90 minutes of complete darkness and silence for your meditation goal.

---

**👤 You:**
> "What should I do to prepare for a session focused on pain management?"

**🤖 AI Agent:**
> To prepare for pain management, please focus on staying hydrated and performing some gentle stretching before your session.


## ❓ FAQ

**Q: How does the planner handle beginners?**
For novice users, the `validate_sensory_config` tool ensures that sensory anchors like light or ambient sound are included to prevent sensory shock and maintain comfort.

**Q: Can I request specific music or lighting?**
Yes, you can include specific requests in the `plan_session_parameters` tool, which will then be validated for safety and effectiveness.

**Q: What happens after my session?**
The `calculate_integration_schedule` tool provides a recommended transition period and activity suggestions to help you reintegrate safely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/float-tank-session-planner](https://vinkius.com/en/ai-agent-connect/float-tank-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Float Tank Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `float-tank-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Float Tank Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "float-tank-session-planner": {
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
