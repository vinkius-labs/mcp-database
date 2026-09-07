# Wave Refraction Effect MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wave-refraction-effect)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Calculates wave refraction, breaking points, and point break intensity based on bathymetry.

## Description
This MCP server provides computational models to analyze how seafloor topography influences ocean swells. By processing bathymetry contours and swell parameters, it determines how waves bend (refraction) and where they will impact the coast. Use `get_refraction_profile` to map direction changes, `predict_breaking_zone` to find the physical breaking location, `analyze_point_break_intensity` to identify high-quality surf spots, and `calculate_section_dynamics` to measure the total surf zone length.


## Available Tools (4)
- **analyze_point_break_intensity**: Identifies if specific underwater features will create high-quality, concentrated "point breaks."
- **calculate_section_dynamics**: Computes the total length of the surf zone affected by the refracted swell
- **get_refraction_profile**: Calculates the change in wave direction at specific depths based on the seafloor shape
- **predict_breaking_zone**: Determines the physical location and characteristics of where waves will break on the shore


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Refraction Effect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the wave refraction profile for a swell of 120 degrees with a 10s period and these depths: [20, 15, 10, 5, 2]."

**🤖 AI Agent:**
> The refraction profile shows a direction change of 15 degrees with energy concentration increasing at the 5m contour.

---

**👤 You:**
> "Where will the waves break if the beach angle is 5 degrees and the refraction profile is provided?"

**🤖 AI Agent:**
> The waves will break at a point shifted 12 meters from the deep-water path, with a section length of 45 meters.

---

**👤 You:**
> "Is there a point break at these coordinates with a 14s wave period?"

**🤖 AI Agent:**
> Yes, the analysis indicates a high-intensity point break at the third contour point.


## ❓ FAQ

**Q: How do I calculate the breaking point shift?**
You must first call `get_refraction_profile` to generate a profile, then pass that profile into `predict_breaking_zone` to determine the shift.

**Q: Can this tool identify point breaks?**
Yes, use `analyze_point_break_intensity` with bathymetry contours and swell direction to identify concentrated energy zones.

**Q: What inputs are required for the refraction profile?**
The `get_refraction_profile` tool requires bathymetry contours, swell direction, and the wave period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wave-refraction-effect](https://vinkius.com/ai-agent-connect/wave-refraction-effect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave Refraction Effect** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-refraction-effect` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave Refraction Effect** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-refraction-effect": {
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
