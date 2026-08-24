# Celestial Navigation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/celestial-navigation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Perform deterministic celestial sight reduction to calculate intercept and azimuth.

## Description
This MCP server provides precise tools for celestial navigation. It allows AI agents to perform sight reduction by calculating the intercept and true azimuth from observed celestial bodies like the Sun, Moon, or stars. Using `calculate_sight_reduction`, agents can determine the distance from an assumed position. The server also provides `get_correction_factors` to account for atmospheric dip, refraction, parallax, and semidiameter, and `verify_position_validity` to ensure geographical plausibility of observations.


## Available Tools (3)
- **calculate_sight_reduction**: Calculates the intercept and true azimuth for a celestial body sight
- **get_correction_factors**: Retrieves the necessary atmospheric and physical correction values for a specific observation
- **verify_position_validity**: Validates if an assumed position is geographically plausible for the given observation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Celestial Navigation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the intercept and azimuth for the Sun at 45.0 N, 30.0 W, with an observed altitude of 40.0 degrees and GHA of 120.0 degrees and declination of 15.0 degrees."

**🤖 AI Agent:**
> The calculated altitude (Hc) is 38.45 degrees, the intercept is 12.5 nautical miles towards the Sun, and the true azimuth (Zn) is 145.2 degrees.

---

**👤 You:**
> "Check if an observation of a star at 10.0 degrees altitude is valid for a position at 0.0 latitude and 0.0 longitude."

**🤖 AI Agent:**
> The position and altitude are valid for this observation.

---

**👤 You:**
> "What are the correction factors for a Moon observation at 20 degrees altitude with an eye height of 5 meters?"

**🤖 AI Agent:**
> The correction factors are: dip: -0.04 degrees, refraction: 0.03 degrees, parallax: 0.01 degrees, and semidiameter: 0.26 degrees.


## ❓ FAQ

**Q: What is a sight reduction?**
Sight reduction is the process of calculating the intercept and azimuth to determine a vessel's position based on the observed altitude of a celestial body.

**Q: How do I handle atmospheric corrections?**
You can use the `get_correction_factors` tool to retrieve specific values for dip, refraction, parallax, and semidiameter based on your observation.

**Q: Can I use this for Moon observations?**
Yes, the tool supports the Sun, Moon, and stars, including specific parallax corrections required for lunar observations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/celestial-navigation-calculator](https://vinkius.com/ai-agent-connect/celestial-navigation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Celestial Navigation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `celestial-navigation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Celestial Navigation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "celestial-navigation-calculator": {
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
