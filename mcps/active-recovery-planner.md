# Active Recovery Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/active-recovery-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates personalized active recovery sessions based on training load and fatigue.

## Description
This MCP server provides an intelligent planning engine for athletes and fitness enthusiasts. It uses physiological data like previous workout intensity, muscle groups trained, and fatigue levels to design optimal recovery sessions. By using tools like `get_recovery_plan` and `get_modality_suitability`, it ensures that recovery activities promote blood flow and metabolic clearance without adding structural stress. It can also determine the best timing via `validate_recovery_window` and specific metabolic targets using `get_intensity_guidelines`.


## Available Tools (4)
- **get_intensity_guidelines**: Provides the specific metabolic or heart rate intensity targets for a session
- **get_modality_suitability**: Determines how well a specific activity aligns with the user's recovery needs
- **get_recovery_plan**: Generates a complete active recovery session plan based on the user's current state and constraints
- **validate_recovery_window**: Checks if the user is attempting to recover too soon or too late after a workout


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Active Recovery Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just finished a high intensity leg workout and I'm feeling a 7/10 on fatigue. I have 30 minutes. What should I do?"

**🤖 AI Agent:**
> Based on your high fatigue and leg training, a 25-minute low-impact swimming session is recommended to promote blood flow without stressing your lower body.

---

**👤 You:**
> "Is running a good idea for recovery after a heavy upper body session?"

**🤖 AI Agent:**
> Yes, running is a suitable recovery activity after upper body training as it provides low impact to your targeted muscle groups.

---

**👤 You:**
> "What intensity zone should I aim for if I'm very exhausted after a moderate workout?"

**🤖 AI Agent:**
> Since your fatigue is high, you should stay within Zone 1 (Recovery), which focuses on extremely light effort primarily for blood flow.


## ❓ FAQ

**Q: How does the planner decide which activity to recommend?**
The planner uses `get_modality_suitability` to match your preferred activity with the muscle groups you trained, ensuring the chosen movement minimizes additional stress.

**Q: Can I specify my preferred exercise?**
Yes, you can provide a preferred modality like cycling or swimming, and the tool `get_recovery_plan` will evaluate its suitability for your current recovery needs.

**Q: How do I know if I am recovering at the right time?**
You can use the `validate_recovery_window` tool to check if the time elapsed since your last workout is optimal for an active recovery session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/active-recovery-planner](https://vinkius.com/en/ai-agent-connect/active-recovery-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Active Recovery Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `active-recovery-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Active Recovery Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "active-recovery-planner": {
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
