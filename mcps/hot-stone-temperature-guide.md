# Hot Stone Temperature Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hot-stone-temperature-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Professional guidance for safe and effective hot stone therapy parameters.

## Description
This MCP server provides professional guidance for setting safe and effective hot stone therapy parameters. It helps therapists determine optimal temperatures, heating times, and treatment rhythms. Use `get_target_settings` to calculate specific temperature and timing for a stone, `validate_safety_parameters` to ensure client safety, `get_heating_requirements` for equipment needs, and `get_treatment_protocol_summary` to plan the treatment pace.


## Available Tools (4)
- **get_heating_requirements**: Calculate specific heating environment needs based on stone mass
- **get_target_settings**: Determine specific temperature and timing parameters for a single stone application
- **get_treatment_protocol_summary**: Provide a high-level summary of how a treatment should be paced
- **validate_safety_parameters**: Verify if proposed temperature and timing settings are safe for a specific client profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hot Stone Temperature Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the settings for a medium stone for a relaxation treatment on a client with moderate tolerance on their back?"

**🤖 AI Agent:**
> For a medium stone used for relaxation on the back with moderate tolerance, the target temperature is 45°C. It requires 25 minutes of heating, a 5-minute cooling period, and a placement duration of 10 minutes.

---

**👤 You:**
> "Is a temperature of 55°C safe for a client with low tolerance on their abdomen?"

**🤖 AI Agent:**
> No, 55°C is not safe for a client with low tolerance on the abdomen. It exceeds the safety threshold for that area and sensitivity level.

---

**👤 You:**
> "What is the recommended pace for a deep tissue treatment using large stones?"

**🤖 AI Agent:**
> For deep tissue treatments with large stones, the recommended pace is active and moving, involving more frequent stone changes to maintain therapeutic effect.


## ❓ FAQ

**Q: How do I know if a temperature is safe for my client?**
You can use the `validate_safety_parameters` tool to check if a specific temperature is safe based on the client's heat tolerance and the body area being treated.

**Q: Can I use this for different stone sizes?**
Yes, the `get_target_settings` tool accounts for small, medium, and large stone sizes to provide accurate heating and placement data.

**Q: Does it help with equipment selection?**
Yes, by using `get_heating_requirements`, you can determine if you need a standard heater or a high-capacity warmer based on the stone size.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hot-stone-temperature-guide](https://vinkius.com/en/ai-agent-connect/hot-stone-temperature-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hot Stone Temperature Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hot-stone-temperature-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hot Stone Temperature Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hot-stone-temperature-guide": {
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
