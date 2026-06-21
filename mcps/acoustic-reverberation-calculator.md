# Acoustic Reverberation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acoustic-reverberation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Estimate RT60 reverberation time and assess room acoustic suitability.

## Description
This MCP server provides professional-grade acoustic engineering tools. Use `calculate_reverberation_time` to estimate the RT60 decay time using the Sabine method based on room volume and surface materials. You can also use `evaluate_room_suitability` to compare your results against ideal targets for spaces like Acoustic Studios, Cinemas, or Concert Halls. The server includes a full catalog of acoustic materials with frequency-dependent absorption coefficients.


## Available Tools (3)
- **calculate_reverberation_time**: Calculates the estimated RT60 for a specific room configuration across all frequency bands
- **evaluate_room_suitability**: Compares calculated reverberation times against ideal acoustic targets
- **get_material_catalog**: Provides a complete list of all available materials and their absorption coefficients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acoustic Reverberation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate RT60 for a 500m3 room with 100m2 of Acoustic Foam and 400m2 of Concrete."

**🤖 AI Agent:**
> The estimated RT60 for the specified configuration is approximately 1.2 seconds at mid-frequencies.

---

**👤 You:**
> "Is a room with an RT60 of 2.5s suitable for an Acoustic Studio?"

**🤖 AI Agent:**
> No, a 2.5s decay time is too 'live' for an Acoustic Studio; you should add more absorptive materials.

---

**👤 You:**
> "List all available acoustic materials."

**🤖 AI Agent:**
> The catalog includes Acoustic Foam, Heavy Carpet, Glass, Wood Panel, and Concrete.


## ❓ FAQ

**Q: What is RT60?**
RT60 (Reverberation Time) is the time it takes for sound to decay by 60 decibels in a space.

**Q: How do I use the calculator?**
Provide the room volume and a JSON array of surfaces with their areas and material names to `calculate_reverberation_time`.

**Q: Which materials are supported?**
You can browse the full list of available materials using the `get_material_catalog` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acoustic-reverberation-calculator](https://vinkius.com/mcp/acoustic-reverberation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acoustic Reverberation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `acoustic-reverberation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acoustic Reverberation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acoustic-reverberation-calculator": {
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
