# Vinyl Speed Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vinyl-speed-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate adjusted playback durations when changing vinyl RPM speeds.

## Description
This MCP server provides precise calculations for vinyl record enthusiasts and technicians. By using tools like `convert_playback_duration`, you can determine exactly how long a track will play when transitioning between standard rotational speeds such as 33, 45, or 78 RPM. It also includes utilities to `get_speed_ratio` and `validate_rpm_standard` to ensure all calculations remain within industry standards.


## Available Tools (4)
- **convert_playback_duration**: Calculates how long a record will play if the rotational speed is changed from a known speed to a target speed
- **get_speed_ratio**: Determines the mathematical relationship (ratio) between two different playback speeds
- **list_standard_speeds**: Provides a list of all supported rotational speeds for the converter
- **validate_rpm_standard**: Checks if a given numerical value corresponds to one of the three industry-standard vinyl speeds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vinyl Speed Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If a record plays for 180 seconds at 33 RPM, how long will it play at 45 RPM?"

**🤖 AI Agent:**
> The record will play for 133.33 seconds at 45 RPM.

---

**👤 You:**
> "What is the speed ratio between 78 RPM and 45 RPM?"

**🤖 AI Agent:**
> The ratio between 78 RPM and 45 RPM is approximately 1.73.

---

**👤 You:**
> "Is 50 RPM a valid standard speed?"

**🤖 AI Agent:**
> No, 50 RPM is not a recognized industry-standard vinyl speed.


## ❓ FAQ

**Q: What RPM speeds are supported?**
The converter supports the three industry standards: 33, 45, and 78 RPM.

**Q: How do I calculate the new time for a record played at a different speed?**
You can use the `convert_playback_duration` tool by providing the original RPM, the target RPM, and the original duration in seconds.

**Q: Can I verify if a specific speed is a standard?**
Yes, the `validate_rpm_standard` tool allows you to check if a numerical value is a recognized vinyl speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vinyl-speed-converter](https://vinkius.com/en/ai-agent-connect/vinyl-speed-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vinyl Speed Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vinyl-speed-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vinyl Speed Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vinyl-speed-converter": {
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
