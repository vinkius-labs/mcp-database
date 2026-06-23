# Gong MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gong-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Analyze sales conversations with AI that reveals winning patterns, coach reps with data, and forecast revenue with precision.

## Description
Connect your **Gong** account to any AI agent and unlock conversation intelligence insights through natural conversation.

### What you can do

- **Call Management** — List all recorded calls, filter by user or date range, and inspect individual call metadata with participants and topics
- **Transcripts** — Retrieve full speaker-labeled transcripts for any recorded call
- **Team Analytics** — List all team members with roles and activity metrics, and drill into per-user call statistics
- **Scorecard Evaluation** — Browse scoring rubrics and retrieve call quality scores for coaching
- **Deal Pipeline** — View deal stages, amounts, and associated calls for pipeline visibility
- **Coaching Library** — Access curated calls saved to the Gong coaching library for training
- **Aggregate Statistics** — Retrieve org-wide call metrics: total calls, duration, talk ratios

### How it works

1. Subscribe to this server
2. Enter your Gong Access Key and Access Key Secret from Company Settings > API
3. Start analyzing your conversations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — review call recordings, track rep performance, and identify coaching opportunities
- **Revenue Operations** — correlate deal pipeline data with conversation patterns to forecast accurately
- **Sales Enablement** — curate best-practice calls in the coaching library and evaluate with scorecards


## Available Tools (14)
- **check_gong_status**: Verify connectivity
- **get_call**: Get call details
- **get_call_stats**: Get call statistics
- **get_transcript**: Get call transcript
- **get_user_stats**: Get user stats
- **get_user**: Get user details
- **list_call_scores**: Get call scores
- **list_calls_by_date**: List calls by date range
- **list_calls_by_user**: List calls by user
- **list_calls**: List calls
- **list_deals**: List deals
- **list_library_calls**: List library calls
- **list_scorecards**: List scorecards
- **list_users**: List users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gong** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all calls from this week and the transcript for the longest one."

**🤖 AI Agent:**
> Found 28 calls this week. The longest was 'Enterprise Demo — Acme Corp' (call_7891, 52 minutes, 4 participants). Speakers: Sarah Chen (rep, 58% talk time), John Miller (prospect, 35%), Lisa Park (SE, 7%). Key topics discussed: pricing tiers, SSO integration, data migration timeline. Action items: 1) Send SOW by Friday. 2) Schedule security review. 3) Provide reference customers. Would you like to see the scorecard evaluation or the full transcript?

---

**👤 You:**
> "Compare the call performance of Sarah and Mike this quarter using their stats and scorecards."

**🤖 AI Agent:**
> Sarah Chen (user_201): 89 calls, avg duration 34 min, talk ratio 52/48 (ideal), avg scorecard: 8.4/10. Top strength: discovery questions (9.1). Area to improve: closing technique (7.2). Mike Torres (user_205): 72 calls, avg duration 28 min, talk ratio 65/35 (over-talking), avg scorecard: 7.1/10. Top strength: product knowledge (8.8). Area to improve: active listening (5.9). Recommendation: Mike could benefit from Sarah's coaching library calls on discovery methodology. Would you like to see the library calls?

---

**👤 You:**
> "Show the deal pipeline and highlight deals that have had no calls in the last 2 weeks."

**🤖 AI Agent:**
> Deal pipeline: 24 active deals totaling $1.2M. Stage breakdown: Prospecting (8, $280K), Discovery (6, $340K), Demo (5, $290K), Negotiation (3, $190K), Closing (2, $100K). ⚠️ 4 deals have had no calls in 14+ days: 1) 'DataFlow Inc' ($45K, Negotiation, last call 18 days ago). 2) 'CloudSync' ($30K, Discovery, 16 days). 3) 'FinTrack' ($25K, Demo, 15 days). 4) 'LogiPro' ($20K, Prospecting, 21 days). These are at risk of going cold. Would you like to check the last call transcripts?


## ❓ FAQ

**Q: Can I access the full transcript of a recorded sales call?**
Yes. Use `list_calls` to browse all recorded calls, then call `get_transcript` with the Call ID to retrieve the full speaker-labeled transcript. Each segment includes the speaker name, timestamp, and spoken text. Use `get_call` for additional metadata like topics discussed and action items.

**Q: Does Gong require two separate credentials?**
Yes. Gong uses HTTP Basic Authentication with an **Access Key** and an **Access Key Secret**. Both are generated in **Company Settings > Ecosystem > API > API Keys**. The credentials are Base64-encoded and sent in the Authorization header. You must be a Technical Administrator to generate API keys.

**Q: Can I track deal pipeline data alongside call recordings?**
Yes. The `list_deals` tool retrieves your deal pipeline with stages, amounts, and associated calls. Cross-reference with `list_calls` and `get_call` to understand which conversations influenced deal progression. Use `get_call_stats` for aggregate metrics like total call volume and talk ratios.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gong-alternative](https://vinkius.com/mcp/gong-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gong** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gong-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gong** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gong-alternative": {
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
