# Chorus.ai (ZoomInfo) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chorusai-zoominfo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Analyze sales conversations and meetings via Chorus.ai — track transcripts, identify key moments, and monitor team performance directly from any AI agent.

## Description
Connect your **Chorus.ai (ZoomInfo)** account to any AI agent and take full control of your conversation intelligence through natural conversation. Streamline how you review and coach your sales team's interactions.

### What you can do

- **Meeting Oversight** — List and retrieve details for all recorded meetings and calls natively
- **Transcription Intelligence** — Access full text transcripts for any engagement to review customer dialogue flawlessly
- **Moment Analysis** — Retrieve AI-identified key moments, such as next steps or pain points, securely
- **Team Management** — List all users and team members to manage access and review performance flawlessly
- **Engagement Visibility** — Monitor active and past engagements to understand sales cycle progress in real-time
- **Market Insights** — List tracked competitors mentioned in conversations to identify market trends flawlessly
- **Shared Knowledge** — Access shared meeting playlists to facilitate team learning directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Chorus.ai API Token (obtained from Personal Settings)
3. Start managing your conversation intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — review team meetings and identify coaching opportunities using natural language
- **Account Executives** — quickly look up previous call transcripts and AI-identified moments without opening the dashboard
- **Revenue Ops** — audit meeting volumes and competitor mentions straight from their chat interface
- **Product Managers** — verify customer feedback and pain points discussed in sales calls


## Available Tools (8)
- **get_my_chorus_profile**: Retrieve information about the currently authenticated session
- **get_meeting_details**: Get detailed information for a specific meeting
- **get_meeting_moments**: Retrieve AI-identified key moments for a meeting
- **get_meeting_transcript**: Retrieve the full text transcript for a meeting
- **list_tracked_competitors**: List competitors being tracked in conversations
- **list_chorus_meetings**: ai.

List recent meetings and calls
- **list_meeting_playlists**: List all shared meeting playlists
- **list_chorus_users**: List all users and team members in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chorus.ai (ZoomInfo)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my meetings from today in Chorus.ai."

**🤖 AI Agent:**
> Retrieving today's meetings... I found 3 recordings: 'Intro Call with Acme', 'Q2 Review - Global Corp', and 'Product Feedback Session'. All are fully processed and transcribed.

---

**👤 You:**
> "What were the key moments in the 'Intro Call with Acme'?"

**🤖 AI Agent:**
> Checking AI moments for the Acme call... I identified 4 key moments: 2 Next Steps (Follow up next Tuesday), 1 Competitor Mention (referencing 'Competitor X'), and 1 Pricing Discussion.

---

**👤 You:**
> "Who are the members of the 'EMEA Sales' team?"

**🤖 AI Agent:**
> Retrieving user list... I found 5 members in the EMEA Sales group: Sarah Miller (Team Lead), Mike Scott, John Doe, Jane Smith, and Bob Black.


## ❓ FAQ

**Q: Can I see the transcript of a meeting through the agent?**
Yes! Use the `get_meeting_transcript` tool with the meeting ID. The agent will return the full text transcript of the conversation directly from Chorus.ai.

**Q: How do I find 'Next Steps' or key moments identified by AI?**
Use the `get_meeting_moments` tool. Your agent will fetch the AI-curated insights for that meeting, which typically include action items, questions, and other relevant moments.

**Q: Where do I find my Chorus.ai API Token?**
Log in to your Chorus.ai account, navigate to your **Personal Settings**, and look for the API or Integration section to generate and copy your token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chorusai-zoominfo](https://vinkius.com/mcp/chorusai-zoominfo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chorus.ai (ZoomInfo)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chorusai-zoominfo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chorus.ai (ZoomInfo)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chorusai-zoominfo": {
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
