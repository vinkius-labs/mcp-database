# Single Point Mooring (SPM) Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/single-point-mooring-spm-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design Single Point Mooring systems for tanker loading and unloading operations.

## Description
This MCP server provides specialized engineering tools for designing Single Point Mooring (SPM) systems. It allows engineers to calculate peak tension forces using `calculate_mooring_loads`, determine necessary buoy dimensions with `size_buoy`, select appropriate mooring lines via `determine_hawser_specs`, and verify operational safety with `validate_approach_departure`. The system accounts for vessel displacement, environmental conditions like wave height and wind speed, and water depth to ensure stable tanker mooring.


## Available Tools (4)
- **calculate_mooring_loads**: Calculate peak tension forces acting on the buoy and mooring system
- **determine_hawser_specs**: Select the appropriate hawser properties for the tanker connection
- **size_buoy**: Determine the required physical characteristics of the floating buoy
- **validate_approach_departure**: Assess if the design allows for safe tanker approach and departure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Single Point Mooring (SPM) Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the mooring loads for a tanker with 150,000 tons displacement, 4m wave height, 15 knots wind, and 2 knots current."

**🤖 AI Agent:**
> The peak tension is 4500 kN with a safety factor of 1.8.

---

**👤 You:**
> "What are the hawser specifications for a VLCC with a peak tension of 5000 kN and a safety margin of 2.5?"

**🤖 AI Agent:**
> The required minimum breaking strength is 12500 kN and the recommended material is Polyester.

---

**👤 You:**
> "Is it safe for a tanker with 12m draft to approach if the max wave height is 3m and current is 1.5 knots?"

**🤖 AI Agent:**
> Yes, the operation is safe under these environmental conditions.


## ❓ FAQ

**Q: What parameters are needed to calculate mooring loads?**
You need to provide the vessel displacement, significant wave height, wind speed, and water current speed to `calculate_mooring_loads`.

**Q: Can I check if a tanker can safely approach the buoy?**
Yes, use the `validate_approach_departure` tool by providing the vessel draft, maximum wave height, and current speed.

**Q: How is the buoy size determined?**
The `size_buoy` tool calculates the required displacement and diameter based on the target peak tension, water depth, and vessel displacement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/single-point-mooring-spm-design](https://vinkius.com/en/ai-agent-connect/single-point-mooring-spm-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Single Point Mooring (SPM) Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `single-point-mooring-spm-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Single Point Mooring (SPM) Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "single-point-mooring-spm-design": {
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
