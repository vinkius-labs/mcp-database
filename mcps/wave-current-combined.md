# Wave-Current Combined MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wave-current-combined)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Calculates the combined influence of wave and current velocities on surf conditions.

## Description
This MCP server provides tools to analyze how wave and current velocities interact. By using vector addition, it determines the effective wave speed, calculates changes in breaking intensity, and assesses overall surf quality. It helps surfers and oceanographers understand if a current is following or opposing the waves and how that affects the rideability of the surf.


## Available Tools (4)
- **assess_surf_quality**: Provides a qualitative assessment of the surfing conditions based on the combined wave-current profile
- **calculate_breaking_intensity**: Quantifies how much the current modifies the intensity of the wave breaking
- **calculate_effective_velocity**: Determines the resultant speed of the wave when moving through a current
- **get_interaction_summary**: Provides a high-level overview of the wave and current relationship for a quick user briefing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave-Current Combined** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the effective wave speed if the wave is 5 m/s at 90 degrees and the current is 2 m/s at 270 degrees?"

**🤖 AI Agent:**
> The effective wave speed is 3.0 m/s.

---

**👤 You:**
> "How will a 1 m/s following current affect a 4 m/s wave?"

**🤖 AI Agent:**
> The following current will increase the effective wave speed and reduce the breaking intensity.

---

**👤 You:**
> "Give me a summary of the interaction for a 6 m/s wave at 0 degrees and a 3 m/s current at 180 degrees."

**🤖 AI Agent:**
> The primary effect is an increase in wave intensity due to a directly opposing current.


## ❓ FAQ

**Q: How does this tool help with surf forecasting?**
It uses `calculate_effective_velocity` to find the true speed of waves moving through currents, which is critical for predicting when waves will break.

**Q: Can I determine if a current will make waves steeper?**
Yes, the `calculate_breaking_intensity` tool quantifies how much an opposing current increases wave steepness.

**Q: What determines the final surf rating?**
The `assess_surf_quality` tool evaluates the effective speed and intensity factor to provide a rating from Poor to Excellent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wave-current-combined](https://vinkius.com/ai-agent-connect/wave-current-combined)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave-Current Combined** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-current-combined` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave-Current Combined** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-current-combined": {
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
