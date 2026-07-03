# Crossfade Time Subtractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crossfade-time-subtractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise video durations and required raw footage lengths when using overlapping transitions.

## Description
The Crossfade Time Subtractor MCP server provides essential calculations for video editors working with overlapping transitions. When clips crossfade, the total timeline duration is shorter than the sum of individual clip lengths because segments occupy the same space. This tool allows you to use `get_true_duration` to find the actual visible length of a sequence, `get_required_raw_sum` to determine how much raw footage is needed for a target duration, and `get_overlap_impact_report` to analyze time lost to junctions.


## Available Tools (3)
- **get_overlap_impact_report**: Provides a breakdown of time lost to transitions
- **get_required_raw_sum**: Calculates the total sum of raw clip lengths needed for a target duration
- **get_true_duration**: Determines the actual length of the final video sequence after all crossfades have been applied


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crossfade Time Subtractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have three clips that are 5000ms, 7000ms, and 4500ms long. If I use a 500ms crossfade between them, what is the final video duration?"

**🤖 AI Agent:**
> The final visible duration of your video will be 15500ms.

---

**👤 You:**
> "I need a final video to be exactly 30 seconds (30000ms) using 5 clips with a 1000ms crossfade. How much total raw footage do I need?"

**🤖 AI Agent:**
> To achieve a 30000ms final duration with 5 clips and 1000ms crossfades, you need a total raw sum of 34000ms.

---

**👤 You:**
> "Analyze the impact of transitions for clips with durations: [2000, 3000, 2500] and a crossfade of 400ms."

**🤖 AI Agent:**
> The total time lost to transitions is 800ms across 2 junctions.


## ❓ FAQ

**Q: How does the duration calculation work?**
The tool calculates the total sum of all clip durations and then subtracts the cumulative time lost at each junction. The number of junctions is always one less than the number of clips.

**Q: Can I use this to plan my footage requirements?**
Yes, by using `get_required_raw_sum`, you can determine exactly how much raw clip length is needed to hit a specific target duration after all crossfades are applied.

**Q: What happens if the crossfade duration is too large?**
If the `crossfadeDuration` exceeds the length of any clip in your sequence, the tool will return an error to prevent invalid calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crossfade-time-subtractor](https://vinkius.com/mcp/crossfade-time-subtractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crossfade Time Subtractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crossfade-time-subtractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crossfade Time Subtractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crossfade-time-subtractor": {
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
