# Telebroad MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telebroad)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/telebroad-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/telebroad-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your business phone system with cloud PBX that includes auto-attendant, call queues, and voicemail-to-email transcription.

## Description
Connect your **Telebroad** business communication account to any AI agent and simplify how you manage your phone system, SMS outreach, and digital faxes through natural conversation.

### What you can do

- **Call Management** — Initiate voice calls, list active calls, and retrieve a complete history of incoming, outgoing, and missed calls.
- **SMS Automation** — List authorized SMS lines, query conversation threads, and send text messages directly via AI commands.
- **Fax Handling** — List received and sent faxes, and send PDF documents as digital faxes from your authorized lines.
- **Team Coordination** — Query the internal phone directory to find extensions and team member destinations.
- **Profile Oversight** — Retrieve detailed profile metadata including extensions, lines, and user settings.
- **Operational Tracking** — Monitor your cloud telephony and messaging activities in real-time.

### How it works

1. Subscribe to this server
2. Enter your Telebroad Username and Password
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & Support Teams** — quickly send SMS follow-ups and initiate calls via simple AI commands.
- **Office Managers** — coordinate extensions and verify call logs directly from the workspace.
- **Business Owners** — maintain an organized record of business communications and faxes via the AI assistant.


## Available Tools
- **get_profile**: Get the current Telebroad user profile
- **get_sms_messages**: Get messages from a specific SMS conversation
- **hangup_call**: Hang up an active call
- **list_active_calls**: List currently active calls
- **list_call_history**: List call history logs
- **list_faxes**: List faxes
- **list_phone_destinations**: List internal phone destinations (extensions)
- **list_sms_conversations**: List SMS conversations
- **list_sms_lines**: List available SMS lines
- **send_call**: Initiate a voice call
- **send_fax**: Send a fax
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telebroad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my recent call history."

**🤖 AI Agent:**
> I've retrieved your call log. You had 3 recent calls: 'Incoming from +15550199' (Missed), 'Outgoing to John Doe' (Success, 5m), and 'Incoming from Unknown' (Success, 2m). Would you like to return any of these calls?

---

**👤 You:**
> "Send an SMS from my line +15550100 to +15550188: 'Meeting at 2 PM'."

**🤖 AI Agent:**
> SMS sent! I've transmitted the message 'Meeting at 2 PM' from +15550100 to the recipient +15550188. Your message has been queued for delivery.

---

**👤 You:**
> "List all internal extensions in my company."

**🤖 AI Agent:**
> Fetching extensions... I found 5 internal destinations: 101 (Sales), 102 (Support), 103 (Finance), and 2 staff extensions. Which one would you like to call?


## Installation & Usage

To install and use the **Telebroad** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telebroad](https://vinkius.com/mcp/telebroad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
