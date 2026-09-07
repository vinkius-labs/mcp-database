# Twintip Buoyancy & Recovery Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/twintip-buoyancy-recovery-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [physics](../categories/physics.md)

Calculate board buoyancy, visibility, and recovery windows for lost surfboards.

## Description
This MCP server provides critical physics calculations for surfboard recovery planning. It allows AI agents to determine how well a board will float and how visible it will be in various sea states. Use `calculate_buoyancy_status` to find the float factor and submerged volume, `estimate_visibility_index` to assess visibility in waves, and `predict_recovery_window` to estimate how long a board stays afloat before sinking. You can also use `compare_configurations` to evaluate different material setups like wood cores and foam densities.


## Available Tools (4)
- **calculate_buoyancy_status**: Provides fundamental buoyancy metrics for a specific board configuration
- **compare_configurations**: Allows a user to compare two different material setups to see which provides better recovery outcomes
- **estimate_visibility_index**: Determines how visible the board will be in different sea states
- **predict_recovery_window**: Estimates how long a board will stay afloat before sinking or becoming unrecoverable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twintip Buoyancy & Recovery Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the buoyancy status for a 45L board weighing 3kg with a paulownia core and standard EPS foam?"

**🤖 AI Agent:**
> The board has a float factor of 1.45, with a submerged volume of 31.03L and 13.97L remaining above the waterline.

---

**👤 You:**
> "How visible will a board with a float factor of 1.2 be in 2-meter waves with clear water?"

**🤖 AI Agent:**
> The visibility score is 0.65.

---

**👤 You:**
> "How long will a board with a float factor of 1.5 stay afloat if water enters at 0.5L per minute in rough seas (intensity 2.0)?"

**🤖 AI Agent:**
> The estimated time remaining until the board loses buoyancy is 45.0 minutes.


## ❓ FAQ

**Q: How do I calculate the float factor?**
You can use the `calculate_buoyancy_status` tool by providing the board volume, weight, core material, and foam density.

**Q: Can I compare different board materials?**
Yes, the `compare_configurations` tool allows you to compare two different material setups to see which provides a better float factor.

**Q: How is visibility determined?**
Visibility is calculated using `estimate_visibility_index`, which considers the float factor, wave height, and water turbidity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/twintip-buoyancy-recovery-planner](https://vinkius.com/ai-agent-connect/twintip-buoyancy-recovery-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twintip Buoyancy & Recovery Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twintip-buoyancy-recovery-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twintip Buoyancy & Recovery Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twintip-buoyancy-recovery-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
