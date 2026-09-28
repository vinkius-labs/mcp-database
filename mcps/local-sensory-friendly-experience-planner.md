# Local Sensory-Friendly Experience Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-sensory-friendly-experience-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Evaluate event compatibility and generate personalized sensory support plans.

## Description
This MCP server provides a decision-support engine for individuals with sensory sensitivities. It connects AI agents to specialized tools that analyze event environments against personal sensory profiles. Use `analyze_participation_feasibility` to determine if an event is safe, `generate_preparation_plan` to prepare for sensory load, `assign_support_roles` to define duties for companions, and `create_exit_protocol` to design calm departure strategies.


## Available Tools (4)
- **analyze_participation_feasibility**: Determine if an event is compatible with a user's sensory profile
- **assign_support_roles**: Define specific duties for support persons
- **create_exit_protocol**: Design a low-friction departure strategy
- **generate_preparation_plan**: Create a proactive plan to reduce sensory overwhelm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Sensory-Friendly Experience Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this concert safe for someone sensitive to loud noises?"

**🤖 AI Agent:**
> The concert has a high decibel rating of 95dB, which exceeds your sensitivity threshold. Participation is not recommended without active mitigation.

---

**👤 You:**
> "Help me prepare for a museum visit with bright lights."

**🤖 AI Agent:**
> To prepare, you should bring polarized sunglasses and plan to arrive during the low-light morning hours.

---

**👤 You:**
> "What should my support person do at the festival?"

**🤖 AI Agent:**
> Your support person should act as a Sound Monitor to track decibel levels and a Space Manager to ensure personal space is maintained.


## ❓ FAQ

**Q: How do I know if an event is safe for me?**
You can use the `analyze_participation_feasibility` tool to compare your specific sensory sensitivities against the published venue conditions.

**Q: Can this help me prepare for a crowded event?**
Yes, the `generate_preparation_plan` tool creates concrete steps and lists specific tools to bring to mitigate sensory load.

**Q: What if I need to leave an event early?**
The `create_exit_protocol` tool designs a low-friction departure strategy based on your exit preferences and the venue's ticket terms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-sensory-friendly-experience-planner](https://vinkius.com/en/ai-agent-connect/local-sensory-friendly-experience-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Sensory-Friendly Experience Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-sensory-friendly-experience-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Sensory-Friendly Experience Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-sensory-friendly-experience-planner": {
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
