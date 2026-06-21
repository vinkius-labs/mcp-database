# MiiTel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/miitel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze phone conversations with AI that scores call quality, identifies sentiment, and provides coaching insights for sales teams.

## Description
Connect your **MiiTel** account to any AI agent and manage AI-powered speech analysis and call data through natural conversation.

### What you can do

- **Call Transcripts** — Access full text transcriptions of sales and support calls
- **Speech Analytics** — Analyze talk ratio, speech rate, overlaps, and silence
- **Recordings** — Retrieve call recording metadata and audio links
- **Agent Performance** — Monitor call volume, duration, and conversion rates
- **Emotion Analysis** — Track sentiment and energy levels during conversations

### How it works

1. Subscribe to this server
2. Enter your MiiTel Access Token
3. Start analyzing voice calls from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — review discovery calls and coach reps automatically
- **Customer Success** — monitor sentiment and identify churn risks
- **Quality Assurance** — ensure compliance on phone calls


## Available Tools
- **get_call_details**: Get details for a specific call
- **get_meeting_details**: Get details for a specific meeting
- **list_calls**: List MiiTel call history
- **list_synced_contacts**: List CRM contacts
- **list_online_meetings**: List online meeting history
- **list_miitel_users**: List MiiTel account users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MiiTel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show speech analytics for Mike's latest sales call."

**🤖 AI Agent:**
> Call ID: call_890 (Mike vs Acme Corp). Duration: 14m 20s. Talk Ratio: 45% Mike / 55% Customer (Excellent ✅). Speech Rate: 160 WPM. Interruptions: 2. Longest silence: 4.5s. Emotion: Positive trend at the end.

---

**👤 You:**
> "Get the transcript summary for call call_890."

**🤖 AI Agent:**
> Transcript (call_890): Mike asked discovery questions about Acme's current CRM setup. Customer mentioned 'Salesforce is too expensive'. Mike pitched the Pro Plan at $45/mo. Customer agreed to a follow-up demo next Tuesday. Competitor mentioned: Salesforce.

---

**👤 You:**
> "Show today's call volume and team performance."

**🤖 AI Agent:**
> Team Performance (Today): Total calls: 145. Total connected: 42 (28%). Avg duration: 4m 12s. Top performer: Sarah (18 connected, avg talk ratio 48%). Lowest talk ratio: John (85% talking - needs coaching ⚠️).


## ❓ FAQ

**Q: Can I access full call transcripts?**
Yes. Retrieve full text transcripts of calls, organized by speaker turns and timestamps.

**Q: How does MiiTel authentication work?**
MiiTel uses an **Access Token** (Bearer auth) against `revcomm.miitel.jp/api/v2`.

**Q: Does it analyze speech patterns?**
Yes. The API provides metrics like Talk/Listen ratio, interruptions, silences, and speaking speed (WPM).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/miitel](https://vinkius.com/mcp/miitel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MiiTel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `miitel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MiiTel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "miitel": {
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
