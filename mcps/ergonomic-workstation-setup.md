# Ergonomic Workstation Setup MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ergonomic-workstation-setup)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates precise workstation dimensions and ergonomic configurations based on user height and equipment.

## Description
This MCP server provides precise ergonomic calculations to prevent musculoskeletal strain. By using tools like `get_single_monitor_setup` and `get_dual_monitor_setup`, AI agents can determine optimal chair height, desk height, and monitor positioning based on a user's specific height and equipment. It also provides reach zone radii via `get_reach_zone_requirements` and lighting guidance through `get_lighting_and_glare_guidance` to ensure a healthy, compliant workspace.


## Available Tools (4)
- **get_dual_monitor_setup**: Calculates dimensions for a workstation utilizing two monitors
- **get_lighting_and_glare_guidance**: Provides specific lighting recommendations to prevent eye strain
- **get_reach_zone_requirements**: Determines the optimal placement area for peripherals
- **get_single_monitor_setup**: Calculates dimensions for a standard single-monitor workstation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ergonomic Workstation Setup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am 180cm tall and want a single monitor setup with a 27 inch monitor. What should my desk and chair height be?"

**🤖 AI Agent:**
> For a height of 180cm and a 27-inch monitor, your recommended chair height is 45cm, desk height is 72cm, and the monitor should be placed 65cm from your eyes.

---

**👤 You:**
> "I'm setting up a standing desk. I am 175cm tall and have a 32 inch monitor. What is the optimal desk height?"

**🤖 AI Agent:**
> For a standing setup at 175cm, your optimal desk height is 108cm to maintain a neutral elbow angle.

---

**👤 You:**
> "What is the best lighting for my workspace if it is currently very sunny?"

**🤖 AI Agent:**
> In a sunny environment, you should position your monitor to avoid direct window glare and aim for a target illumination of 500 Lux to maintain contrast.


## ❓ FAQ

**Q: How accurate are these ergonomic recommendations?**
The recommendations are based on standardized anthropometric scaling and ergonomic principles from OSHA and ANSI to ensure neutral posture.

**Q: Can I use this for a standing desk setup?**
Yes, by using `get_single_monitor_setup` with the `isStanding` parameter set to true, the tool calculates desk height aligned with your natural elbow height.

**Q: Does it support dual monitor configurations?**
Yes, the `get_dual_monitor_setup` tool specifically handles two-monitor layouts, including centered or primary-side alignments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ergonomic-workstation-setup](https://vinkius.com/en/ai-agent-connect/ergonomic-workstation-setup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ergonomic Workstation Setup** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ergonomic-workstation-setup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ergonomic Workstation Setup** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ergonomic-workstation-setup": {
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
