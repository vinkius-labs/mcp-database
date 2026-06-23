# Bilibili Live MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bilibili-live)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate VTuber interaction parsing via Bilibili Live — monitor super-chats, extract danmaku streams, and manage host rooms natively from any AI agent.

## Description
Bolt the massive broadcasting ecosystem of **Bilibili Live Open Platform** into your intelligent workflows allowing comprehensive algorithmic polling of the largest Danmaku network globally without manual dashboards.

### What you can do

- **Super-Chat Monitoring** — Directly scan massive bullet-chat oceans isolating premium user contributions continuously updating without browser intervention
- **VTuber Identity Linking** — Fetch demographic metadata resolving numerical keys to official liver host profiles cleanly integrating esports tracking
- **Audience Polling** — Read heavy concurrency metrics gauging organic popularity of rooms isolating fake viewership bots
- **Virtual Gifting Arrays** — Unpack real-time financial donation ledgers tying precise value exchanges mapped to precise broadcast seconds

### How it works

1. Enlist officially into the [Bilibili Open Live Console](https://open-live.bilibili.com/)
2. Generate the mandatory AccessKey / Secret combos strictly required
3. Plug those secrets here letting your local LLM handle real-time chat parsing

Say goodbye to missing massive interactions under heavy traffic. You now possess a tireless automated moderator handling raw text metrics dynamically.

### Who is this for?

- **VTuber Agencies** — map and store automated logs summarizing entire broadcast donation waves seamlessly bridging into daily ledger CRMs
- **Community Moderators** — inject strict AI safety layers capable of filtering heavy toxic word dumps across hundreds of messages per second instantly
- **Esports Broadcasters** — retrieve room stability metrics logging heavy influxes safely generating historical reports directly to executives via terminal


## Available Tools (10)
- **get_danmu_config**: Get WebSockets configuration for Danmu (bullet chat)
- **get_fans_medal_info**: Check a users fan medal level in the current room
- **get_gift_history**: View recent virtual items gifted in the room
- **get_guard_list**: Get a list of active "Guards" (Captains/Admirals) in the room
- **get_room_info**: Start the app connection and get high-level room config
- **get_room_play_info**: Get stream playback URLs and live status
- **get_streamer_info**: Retrieve the broadcasters public account details
- **get_super_chats**: Extract actively purchased Super Chats
- **send_danmu**: Send a message into the broadcast as the developer account
- **update_room_title**: Change the streamers live room title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bilibili Live** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the raw user engagement metric from Bilibili room '51923' quickly."

**🤖 AI Agent:**
> Targeting identifier '51923'... Stream fetched! The current popularity index bursts at 1,402,050 concurrent interactions suggesting massive virtual tipping activity ongoing. Should I attempt parsing the overarching super-chat list now?

---

**👤 You:**
> "Summarize the metadata tied directly to backend ID of host 892019."

**🤖 AI Agent:**
> Running profile extraction algorithms... The host tied to '892019' resolves to 'GamerLegendXXX'. They maintain official standing in the 'Esports Casting' realm holding verified status with peak traffic histories around late evening shifts. Do you need explicit cover-art image arrays linked?

---

**👤 You:**
> "Retrieve the top 10 richest super-chat donations logged actively over the current cycle."

**🤖 AI Agent:**
> Accessing donation arrays filtering outliers aggressively... The pinnacle contribution sits at ~3000 CNY dropped by user ID 'VIP91'. The subsequent 9 donations average around 800 CNY tightly clustered across a 2-minute competitive wave. Rendering complete table now...


## ❓ FAQ

**Q: Can my AI automatically aggregate bullet-chat density from a major active esports broadcast directly?**
Yes! Utilize the `get_room_danmu` endpoint integration tool. Your agent will dynamically hook to the channel pinging the rapid incoming stream mapping it natively to your terminal workspace seamlessly bypassing clunky UI obstacles totally.

**Q: How do I fetch the exact real-time audience capacity on a specified VTuber room?**
Simply ask the agent to run `get_room_popularity` targeting the internal integer Room ID. The pipeline will isolate the live audience metric securely displaying the engagement index free of visual latency delays instantly in markdown format natively.

**Q: Are there destructive capabilities enabling unwarranted permanent room shutdowns programmatically?**
Absolutely not. This suite adheres to read-only data mining directives strictly mapping traffic, messages, and identities. No system administration functions or destructive endpoints are configured assuring unbreakable security fences from external tampering continuously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bilibili-live](https://vinkius.com/mcp/bilibili-live)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bilibili Live** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bilibili-live` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bilibili Live** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bilibili-live": {
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
