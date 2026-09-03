# Steel Braced Frame Drift Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-braced-frame-drift-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates inter-story drift, drift ratios, and brace stiffness requirements for steel braced frames.

## Description
This MCP server provides structural engineering tools to analyze lateral displacement in steel braced frames. It calculates total horizontal displacement at specific levels using `calculate_story_drift`, determines brace geometry with `get_brace_geometry`, and evaluates compliance via `verify_stiffness_requirement`. It also allows for a detailed breakdown of deformation sources using `analyze_deformation_components` to identify the impact of brace elongation, column shortening, and connection deformation.


## Available Tools (4)
- **analyze_deformation_components**: Breaks down the total drift into its individual contributing factors
- **calculate_story_drift**: Calculates the total horizontal displacement at a specific level
- **get_brace_geometry**: Determines the geometric properties of the brace based on the frame dimensions
- **verify_stiffness_requirement**: Checks if the current brace configuration meets a specific stiffness threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Braced Frame Drift Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the story drift for a 4m story height, 6m bay width, 5000mm2 brace area, with a 50kN load in a 5-story building at the 3rd story."

**🤖 AI Agent:**
> The calculated story drift for the 3rd story is 12.45 mm, resulting in a drift ratio of 0.31%.

---

**👤 You:**
> "What is the length and angle of a brace for a frame with 3.5m story height and 5m bay width?"

**🤖 AI Agent:**
> The brace length is 4.30 meters and the brace angle is 35.54 degrees.

---

**👤 You:**
> "Is a brace with 200 kN/m stiffness compliant if the required stiffness is 150 kN/m?"

**🤖 AI Agent:**
> Yes, the brace is compliant with a stiffness margin of 50 kN/m.


## ❓ FAQ

**Q: How do I calculate the drift at a specific floor?**
Use the `calculate_story_drift` tool by providing the story height, bay width, brace area, applied load, total stories, and the target story level.

**Q: Can I check if my brace meets design requirements?**
Yes, use the `verify_stiffness_requirement` tool to compare your current brace stiffness against the minimum required stiffness.

**Q: What factors contribute to the total drift?**
Total drift is composed of brace elongation, column shortening, and connection deformation. You can use `analyze_deformation_components` to see the percentage contribution of each.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-braced-frame-drift-calculator](https://vinkius.com/ai-agent-connect/steel-braced-frame-drift-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Braced Frame Drift Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-braced-frame-drift-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Braced Frame Drift Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-braced-frame-drift-calculator": {
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
