# Timelapse Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/timelapse-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Plan precise timelapse sequences, storage needs, and golden hour windows.

## Description
The Timelapse Calculator MCP server is a precision utility for photographers and filmmakers. It bridges the gap between real-world events and cinematic playback by calculating exact camera settings. Use `compute_timelapse_plan` to determine your shot interval, total frames, and storage requirements based on your target clip duration and FPS. With `compute_playback_duration`, you can predict the final video length from a known sequence of shots. Additionally, use `lookup_golden_hour_window` to identify optimal lighting periods for specific geographic regions, ensuring your production captures the most aesthetic solar transitions.


## Available Tools (3)
- **lookup_golden_hour_window**: Provides solar transition durations for specific regions
- **compute_playback_duration**: Determines video playback duration based on captured images
- **compute_timelapse_plan**: Calculates how to configure a camera for a timelapse


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Timelapse Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to record a 30-minute sunset. I want my final video to be 20 seconds long at 24 FPS. Each photo is about 5MB. What should my interval be?"

**🤖 AI Agent:**
> To capture a 30-minute sunset for a 20-second clip at 24 FPS, you need to take a shot every 12.5 seconds. This will result in 144 frames and approximately 720 MB of storage used.

---

**👤 You:**
> "I have 300 photos taken at 5-second intervals. If I play them back at 30 FPS, how long will the video be?"

**🤖 AI Agent:**
> A sequence of 300 photos with a 5-second interval played at 30 FPS will result in a final clip duration of 50 seconds.

---

**👤 You:**
> "How long is the golden hour window in the US-WEST region?"

**🤖 AI Agent:**
> The expected golden hour duration for the US-WEST region is 45 minutes.


## ❓ FAQ

**Q: How do I calculate my storage needs?**
Use the `compute_timelapse_plan` tool. By providing your event duration, target clip length, and average frame size, it will output the total storage required in MB.

**Q: Can I plan for specific lighting conditions?**
Yes. Use `lookup_golden_hour_window` with a region code like 'EU-NORTH' to find the expected duration of the golden hour window for that area.

**Q: What if I already have a set number of photos?**
You can use `compute_playback_duration`. Input your shot interval and total shot count to see how long the resulting video will play at your chosen FPS.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timelapse-calculator](https://vinkius.com/mcp/timelapse-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Timelapse Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `timelapse-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Timelapse Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "timelapse-calculator": {
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
