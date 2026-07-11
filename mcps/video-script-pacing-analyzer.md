# Video Script Pacing Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/video-script-pacing-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [advertising](../categories/advertising.md)

Analyze video and ad scripts for timing, hook strength, and rhythmic pacing.

## Description
Optimize your video content for maximum viewer retention. This MCP server provides specialized tools to evaluate the structural rhythm of scripts. Use `analyze_script_timing` to determine total spoken duration and CTA placement, `evaluate_hook_retention` to check information density in the critical first 8 seconds, `calculate_pacing_variance` to detect monotonous or overly rapid segments, and `assess_audio_rhythm` to ensure natural breathability through pause analysis.


## Available Tools (4)
- **calculate_pacing_variance**: Analyze the variance in script segment durations
- **assess_audio_rhythm**: Analyze the rhythm and breathability of the script
- **evaluate_hook_retention**: Evaluate how well the script hooks viewers in early windows
- **analyze_script_timing**: Analyze timing and CTA placement in a video script


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Video Script Pacing Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this script: 'Stop scrolling! This is the secret to better pacing. [pause] You need to watch until the end for the CTA.' at 150 WPM."

**🤖 AI Agent:**
> The total estimated duration is approximately 12 seconds, with the Call to Action located at 83% of the script length.

---

**👤 You:**
> "Check the hook strength for: 'Welcome to the show. Today we are talking about pacing. It is very important for creators.'"

**🤖 AI Agent:**
> The 3-second window contains 4 words, the 5-second window contains 7 words, and the 8-second window contains 12 words.

---

**👤 You:**
> "Does this script have good breathability? 'Running fast... [pause] breathing hard... [pause] stop.'"

**🤖 AI Agent:**
> The pause to word ratio is 0.67, indicating a high level of breathability and intentional pauses.


## ❓ FAQ

**Q: How does the tool calculate script duration?**
The `analyze_script_timing` tool calculates duration by dividing the total word count of your script by a provided Words Per Minute (WPM) rate.

**Q: What is considered a strong hook?**
A strong hook is measured by information density in the first 3, 5, and 8 seconds. You can use `evaluate_hook_retention` to see if your script captures attention immediately.

**Q: Can I detect if my script is too fast for viewers?**
Yes, `calculate_pacing_variance` flags segments that exceed your specified words-per-second threshold, helping you avoid rapid speech that might confuse the audience.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/video-script-pacing-analyzer](https://vinkius.com/mcp/video-script-pacing-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Video Script Pacing Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `video-script-pacing-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Video Script Pacing Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "video-script-pacing-analyzer": {
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
