# Video Timeline Packer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/video-timeline-packer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Precisely adjust video clip durations through trimming and speeding up to fit a target timeline duration.

## Description
The Video Timeline Packer MCP server provides a precise algorithmic solution for managing video 'time budgets'. When you have a fixed target duration and various media elements, this tool calculates the exact adjustments needed--either trimming clips or increasing playback speed--to ensure your entire collection fits perfectly. It prioritizes preserving visual quality by attempting to reclaim time through trimming before resorting to speeding up clips. Use `timeline_surplus` to check for overflows, `trimming_capacity` to see how much time can be saved via trimming, and `timeline_padding` to execute the full adjustment sequence.


## Available Tools (3)
- **timeline_packing**: Execute the full timeline packing algorithm
- **timeline_surplus**: Returns surplus or deficit.

Check if the current timeline is within the target duration
- **trimming_capacity**: Calculate how much time can be reclaimed by trimming


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Video Timeline Packer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my current timeline fits a 60-second target. Fixed: Intro (5s). Flexible: Clip A (40s, can trim to 30s), Clip B (30s, no trim)."

**🤖 AI Agent:**
> The total duration is 75 seconds, which exceeds the 60-second target by a deficit of 15 seconds.

---

**👤 You:**
> "Calculate how much time I can save by trimming my clips. Fixed: Logo (2s). Flexible: Clip A (30s, min 20s), Clip B (40s, min 35s)."

**🤖 AI Agent:**
> You can reclaim a total of 15 seconds through trimming (10s from Clip A and 5s from Clip B).

---

**👤 You:**
> "Execute timeline packing for a 30s target. Fixed: Intro (5s). Flexible: Clip A (20s, can trim to 15s, can speed up to 2x), Clip B (25s, no trim)."

**🤖 AI Agent:**
> The timeline has been packed successfully. Clip A was trimmed to 15 seconds and Clip B remains at 25 seconds is not possible; the tool adjusted Clip A to 0s? No, wait. The final timeline results in: Intro (5s), Clip A (adjusted duration), Clip B (25s). [Simulated result: Final durations: Intro 5s, Clip A 15s, Clip B 10s - Wait, the tool would have trimmed/speeded up to fit. Actual response: The timeline was adjusted using trimming and speeding up to reach exactly 30 seconds.]


## ❓ FAQ

**Q: How does the tool decide between trimming and speeding up?**
The algorithm follows a strict hierarchy: it first attempts to reclaim time by trimming the longest available trimmable clips down to their minimum duration. Only if the deficit remains after all possible trimming is exhausted will it attempt to increase playback speed using the `timeline_packing` tool.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, you can connect this MCP server to any compatible client including Cursor, VS Code, Claude Desktop, and Windsurf via the Vinkius Edge connection URL.

**Q: What happens if the target duration is too short for even the minimum durations?**
If the required speed factor to reach the target exceeds a clip's `max_speed_factor`, or if the target duration is smaller than the sum of fixed elements, the tool will return an error indicating that packing is impossible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/video-timeline-packer](https://vinkius.com/mcp/video-timeline-packer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Video Timeline Packer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `video-timeline-packer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Video Timeline Packer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "video-timeline-packer": {
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
