# VTuber Clip Highlight Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vtuber-clip-highlight-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-creation](../categories/content-creation.md)

A deterministic engine to evaluate the viral potential of VTuber stream clips.

## Description
This MCP server provides a deterministic scoring engine designed to evaluate the viral potential of VTuber stream clips. By analyzing engagement metrics like Super Chat counts, chat velocity, and laugh emotes, it calculates a precise highlight score and normalizes it into a Score Per Minute (SPM). The engine then classifies clips into viral tiers (S, A, B, or C) to help content managers prioritize high-impact moments. Use `calculate_highlight_potential` to determine the viral tier and `validate_clip_metrics` to ensure engagement data is logically sound before scoring.


## Available Tools (3)
- **calculate_highlight_potential**: Evaluates the viral intensity of a specific clip segment
- **get_tier_thresholds**: Retrieves the current business rules for viral tier classifications
- **validate_clip_metrics**: Verifies that the provided engagement metrics are logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VTuber Clip Highlight Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the highlight potential for a 60-second clip with 5 Super Chats, 120 chat messages per minute, and 10 laugh emotes."

**🤖 AI Agent:**
> The clip has a highlight score of 81.0, a score per minute of 81.0, and is classified as B-Tier.

---

**👤 You:**
> "What is the viral tier for a clip with a score per minute of 550?"

**🤖 AI Agent:**
> A score per minute of 550 results in an S-Tier classification.

---

**👤 You:**
> "Check if these metrics are valid: 10 Super Chats, 50 chat velocity, and -5 laugh emotes."

**🤖 AI Agent:**
> The metrics are invalid because laugh emote count cannot be negative.


## ❓ FAQ

**Q: How is the viral tier determined?**
The viral tier is determined by the Score Per Minute (SPM). Tiers are classified as S (Legendary), A (High Engagement), B (Moderate), or C (Standard) based on specific intensity thresholds.

**Q: What metrics are used for scoring?**
The engine uses Super Chat counts, chat velocity (messages per minute), and laugh emote counts to calculate the total highlight score.

**Q: Can I validate my data before scoring?**
Yes, you can use the `validate_clip_metrics` tool to ensure your engagement data is logically sound and non-negative before running the full scoring process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vtuber-clip-highlight-scorer](https://vinkius.com/ai-agent-connect/vtuber-clip-highlight-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VTuber Clip Highlight Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vtuber-clip-highlight-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VTuber Clip Highlight Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vtuber-clip-highlight-scorer": {
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
