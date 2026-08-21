# Douyin & TikTok Retention Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/douyin-tiktok-retention-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Analyze video pacing, beat synchronization, and hook effectiveness to estimate viewer retention.

## Description
This MCP server provides deterministic tools to analyze short-form video pacing for platforms like Douyin and TikTok. Use `calculate_video_pacing` to evaluate visual rhythm, scene change frequency, and how well cuts align with the background music's tempo. Use `estimate_retention_performance` to predict the likely completion rate based on hook text length and the calculated pacing metrics. It helps creators optimize their visual stimulus and rhythmic synchronization to maximize audience attention.


## Available Tools (2)
- **calculate_video_pacing**: 
- **estimate_retention_performance**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Douyin & TikTok Retention Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pacing for a 15 second video with 10 scene changes and 120 BPM music."

**🤖 AI Agent:**
> The recommended hook duration is 3.0 seconds. The scene frequency is 0.67 changes per second, and the beat sync score is 100.

---

**👤 You:**
> "Estimate retention for a video with a 50 character hook, 0.5 scene frequency, and a 90 beat sync score."

**🤖 AI Agent:**
> The estimated completion rate is 75%.

---

**👤 You:**
> "Analyze a 60 second video with 5 scene changes and 100 BPM music."

**🤖 AI Agent:**
> The recommended hook duration is 3.0 seconds. The scene frequency is 0.08 changes per second, and the beat sync score is 0.


## ❓ FAQ

**Q: How is the beat sync score calculated?**
The `calculate_video_pacing` tool determines the score by checking if the total number of scene changes aligns perfectly with the rhythmic pulses of the background music's BPM.

**Q: Can I predict my video's completion rate?**
Yes, by using `estimate_retention_performance`, you can get a predicted percentage of viewers who will watch your video to the end based on your pacing and hook metrics.

**Q: What is the recommended hook duration?**
The tool follows the viral standard, recommending a fixed hook duration of 3.0 seconds to maximize initial viewer retention.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/douyin-tiktok-retention-calculator](https://vinkius.com/ai-agent-connect/douyin-tiktok-retention-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Douyin & TikTok Retention Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `douyin-tiktok-retention-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Douyin & TikTok Retention Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "douyin-tiktok-retention-calculator": {
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
