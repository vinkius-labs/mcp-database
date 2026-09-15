# Wave-Selection-Priority MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wave-selection-priority)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Determine surfer priority, optimal takeoff zones, and wave-sharing potential.

## Description
This MCP server provides computational models to manage surf lineup dynamics. It allows AI agents to calculate right of way using `calculate_right_of_way`, identify the best locations to catch waves with `determine_takeoff_zone`, evaluate if multiple surfers can ride together via `assess_wave_sharing`, and monitor lineup density with `get_lineup_status`.


## Available Tools (4)
- **get_lineup_status**: Provides a summary of the current competition for a specific wave
- **calculate_right_of_way**: Determines which surfer holds the primary claim to a specific wave
- **determine_takeoff_zone**: Identifies the most efficient location for a surfer to catch the wave
- **assess_wave_sharing**: Evaluates if multiple surfers can safely ride the same wave


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave-Selection-Priority** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who has priority if I am at the peak and the wave is breaking left?"

**🤖 AI Agent:**
> The surfer at the peak has primary priority for the left-breaking wave.

---

**👤 You:**
> "Where should I position myself to catch the next wave if I am currently at the shoulder?"

**🤖 AI Agent:**
> The optimal takeoff zone is at the peak.

---

**👤 You:**
> "Can 3 surfers with tight spacing share a right-breaking wave?"

**🤖 AI Agent:**
> No, sharing is impossible due to the tight spacing and high interference risk at the peak.


## ❓ FAQ

**Q: How is priority determined in the lineup?**
Priority is primarily determined by position relative to the peak and wave direction. You can use `calculate_right_of_way` to find the primary claim holder.

**Q: Can I predict if a wave can be shared?**
Yes, the `assess_wave_sharing` tool evaluates the probability of safe wave sharing based on surfer count, spacing, and wave direction.

**Q: How do I find the best place to catch a wave?**
The `determine_takeoff_zone` tool calculates the most efficient location for takeoff based on your current position and paddling speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wave-selection-priority](https://vinkius.com/en/ai-agent-connect/wave-selection-priority)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave-Selection-Priority** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-selection-priority` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave-Selection-Priority** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-selection-priority": {
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
