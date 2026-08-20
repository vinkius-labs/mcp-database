# Douyin Engagement Algorithm MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/douyin-engagement-algorithm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate precise video engagement scores and viral potential for Douyin and TikTok content.

## Description
This MCP server provides deterministic tools to quantify video performance in the Douyin and TikTok ecosystems. It calculates a weighted engagement score normalized per 1,000 views, allowing for fair comparison across different video scales. Use `calculate_engagement_score` to determine raw quality, `predict_viral_potential` to find the growth tier, `calculate_posting_adjustment` to account for freshness decay, and `estimate_view_multiplier` to forecast future reach.


## Available Tools (4)
- **calculate_engagement_score**: Determine the raw engagement quality of a video relative to its reach
- **calculate_posting_adjustment**: Adjust the expected engagement based on the time elapsed since the video was posted
- **estimate_view_multiplier**: Forecast the potential reach of a video based on its current performance
- **predict_viral_potential**: Categorize a video's growth trajectory into a standardized index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Douyin Engagement Algorithm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the engagement score for a video with 5000 views, 80% completion rate, 200 likes, 50 comments, 30 shares, and 10 saves."

**🤖 AI Agent:**
> The calculated engagement score is 34.5 per 1,000 views.

---

**👤 You:**
> "What is the viral potential for a video with an engagement score of 85?"

**🤖 AI Agent:**
> The video has a Viral Potential Index of 92 and is in the 'Explosive' growth tier.

---

**👤 You:**
> "Estimate the view multiplier for a video with 10,000 views and an engagement score of 40."

**🤖 AI Agent:**
> The predicted view multiplier is 5.2, suggesting significant growth potential.


## ❓ FAQ

**Q: How is the engagement score calculated?**
The score is calculated using a weighted formula: (completion_rate × 0.4) + (shares × 0.3) + (saves × 0.15) + (comments × 0.1) + (likes × 0.05), all normalized per 1,000 views.

**Q: Can I predict if a video will go viral?**
Yes, by using the `predict_viral_potential` tool, you can obtain a Viral Potential Index from 0 to 100 and a specific growth tier.

**Q: Does the algorithm account for video age?**
Yes, the `calculate_posting_adjustment` tool applies a historical decay rate to adjust engagement scores based on the hours elapsed since upload.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/douyin-engagement-algorithm](https://vinkius.com/ai-agent-connect/douyin-engagement-algorithm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Douyin Engagement Algorithm** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `douyin-engagement-algorithm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Douyin Engagement Algorithm** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "douyin-engagement-algorithm": {
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
