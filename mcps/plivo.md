# Plivo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plivo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Equip AI with native telecom powers. Send SMS, manage SIP trunks, and audit voice calls autonomously.

## Description
Grant your AI agent the absolute capacity to bridge code into the global telecommunications network via **Plivo**. Circumvent visual dashboards entirely. You can instruct your personal LLM (Cursor, Claude) to dispatch real SMS text messages, bridge live VoIP calls across E.164 formats, or pull heavy financial billing limits proactively from the console.

### What you can do

- **Live SMS Outbound** — Instruct your bot to dynamically dispatch `send_sms` payloads mapping precise strings to specific international destination variables without writing boilerplate bindings.
- **Voice Operations** — Push strict XML logic routing into active PSTN grids. Initiate (`make_call`), actively trace connection lengths (`get_call`), or vaporize stuck voice sessions (`cancel_call`).
- **Telecom Auditing** — Dive into messaging analytics. Query `list_messages` extracting exact 5xx delivery failures, retrieving explicitly why a telecom carrier rejected the frame (`get_message`).
- **Inventory & Capacity** — Force the agent to interrogate your account for its exact active DID numbers (`list_numbers`), map VoIP registration footprints (`list_endpoints`), and monitor billing funds natively (`get_account`).

### How it works

1. Enable the explicit Plivo integration module on Vurb
2. Supply your Plivo Auth ID alongside its Auth Token
3. Start dictating telecom operations exclusively via AI chat prompts

### Who is this for?

- **DevOps Engineers** — script your local LLM to run diagnostics, ping `get_account` to evaluate low balances, and instantly message admins on their phone.
- **Backend Architects** — verify SMS integrations dynamically by demanding the AI send you test payloads bridging directly to your mobile device.
- **Telecom Ops** — purge phantom active calls stuck in loop states by conversing directly using `list_calls` followed by sweeping `cancel_call` operations.


## Available Tools (10)
- **terminate_call**: Hang up an active call
- **get_account_info**: Get Plivo account details
- **get_call_details**: Get specific call details
- **get_message_details**: Get details for a specific message
- **list_calls**: List recent voice calls
- **list_sip_endpoints**: List SIP endpoints
- **list_messages**: List sent and received messages
- **list_plivo_numbers**: List phone numbers in the account
- **make_voice_call**: Initiate an outbound voice call
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check Plivo account status and let me know my remaining wallet balance."

**🤖 AI Agent:**
> Retrieval confirmed via `get_account`. Primary Plivo account is active securely. Current remaining balance mapped to `$412.55`. Would you like me to ping the `list_calls` node to verify active expenses burning constraints right now?

---

**👤 You:**
> "Send an SMS message to `15551234567` from our main `15559876543` local number saying the servers are online."

**🤖 AI Agent:**
> Action logged and sent. Executed the mutation `send_sms` seamlessly passing source E.164 and target destinations simultaneously. Plivo acknowledged payload receipt queue mapping it successfully holding object UUID: `a7d-22r9`. I will monitor the background if required.

---

**👤 You:**
> "Check Plivo network to list all presently active voice phone calls."

**🤖 AI Agent:**
> Query deployed against the active telecom trunk node (`list_calls`). Result: Empty array bounding currently parsed instances. The network endpoints are clean, reporting identically 0 concurrent routing states or phantom SIP loops tied to your active parameters.


## ❓ FAQ

**Q: Can my AI directly check why a specific SMS message failed to send?**
Yes. When anomalous delivery states occur, the AI can query `list_messages` identifying problematic entries. Then, executing `get_message` feeding the discrete UUID returns explicit structural insights straight from Plivo’s carrier networks (e.g., 'Destination Not Found', 'Blocked by telecom firewall').

**Q: Is it possible to terminate a live stuck call from my text prompt?**
Absolutely. If you detect logic loops keeping Voice trunks active in `list_calls`, instruct the agent to issue the `cancel_call` action. Supplying the precise UUID forces the HTTP architecture to literally send a `DELETE` tear-down protocol, instantly vaporizing the connection physically.

**Q: Can the agent interact with my billing limits to warn me?**
Correct. Plivo natively exposes account architecture. Prompting the system to fetch `get_account` pulls cash balances, available capacity boundaries, and current currency mapping logic. It allows your Agent to perform autonomous diagnostics warning you natively before critical telecom endpoints shutdown due to zero-balance errors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plivo](https://vinkius.com/mcp/plivo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plivo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plivo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plivo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plivo": {
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
