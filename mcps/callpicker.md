# Callpicker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/callpicker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Track and analyze inbound calls with attribution data that shows which marketing channels drive your best phone leads.

## Description
Connect your **Callpicker** account to any AI agent and take full control of your cloud-based business telephony and virtual PBX workflows through natural conversation.

### What you can do

- **Call Orchestration** — Programmatically initiate high-fidelity phone calls from your virtual PBX numbers to any destination worldwide directly through your agent
- **Communication Intelligence** — Monitor real-time incoming and outgoing call history and retrieve detailed logs and high-fidelity Call Detail Records (CDR)
- **Recording Management** — Access and retrieve secure download URLs for call recordings to maintain high-fidelity oversight of customer interactions
- **PBX & Extension Architecture** — Access your complete directory of virtual phone numbers and PBX extensions to coordinate your internal communication structure
- **Operational Monitoring** — Check real-time system status and generate performance reports over specific date ranges directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **Client ID** and **Client Secret** from the Callpicker Portal (Configuration > API)
3. Start managing your business voice pipeline from Claude, Cursor, or any MCP client

No more manual logging of phone results or digging through complex PBX portals. Your AI acts as your dedicated telephony engineer and voice coordinator.

### Who is this for?

- **Sales & Support Teams** — instantly initiate calls to leads and retrieve conversation recordings using natural language commands
- **Operations Managers** — monitor PBX system health and automate call log analysis without leaving your workspace
- **Developers** — integrate high-speed virtual calling and CDR data into custom workflows through simple AI queries


## Available Tools
- **get_call_details**: Get details for a specific call
- **get_cdr_report**: Get Call Detail Records (CDR)
- **get_pbx_system_status**: Check PBX system status
- **get_recording_url**: Get the download URL for a recording
- **list_call_logs**: List recent call logs
- **list_pbx_extensions**: List PBX extensions
- **list_virtual_numbers**: List virtual phone numbers
- **list_call_recordings**: List available call recordings
- **make_call**: Initiate a phone call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Callpicker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Initiate a call to '+1234567890' from my virtual number '+0987654321'."

**🤖 AI Agent:**
> Call triggered! I've successfully initiated the outgoing call via Callpicker. The PBX is now bridging the connection to +1234567890. Shall I notify you when the call completes?

---

**👤 You:**
> "Show the last 5 call logs with duration and status."

**🤖 AI Agent:**
> Accessing call logs... Your last 5 interactions include 3 answered calls (avg 5m 12s) and 2 missed. The most recent was a 12-minute consultation. Need the high-fidelity CDR report for these?

---

**👤 You:**
> "Get the download link for call recording ID '789'."

**🤖 AI Agent:**
> Link generated! You can download the recording for interaction 789 here: [recording_url]. The link is secure and valid for 24 hours. Would you like a summary of the PBX status?


## ❓ FAQ

**Q: How do I find my Callpicker Client ID and Secret?**
Log in to the [**Callpicker Portal**](https://admin.callpicker.com/), navigate to **Configuration** > **API**, and generate your credentials.

**Q: Can I retrieve call recordings via AI?**
Yes! The `get_recording_url` tool provides a temporary secure link to play or download any recorded interaction in your account.

**Q: How do I check my virtual numbers?**
Use the `list_virtual_numbers` tool to retrieve your complete directory of active virtual phone numbers programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/callpicker](https://vinkius.com/mcp/callpicker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Callpicker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `callpicker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Callpicker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "callpicker": {
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
