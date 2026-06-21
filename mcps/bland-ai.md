# Bland AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bland-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Automate phone calls via Bland AI — dispatch voice agents, analyze call transcripts, and manage inbound phone numbers directly from your AI agent.

## Description
Connect your **Bland AI** API key to your AI agent and take full programmatic control over enterprise-grade telephony and conversational voice workflows.

### What you can do

- **Automated Calling** — Dispatch individual conversational voice agents to specific phone numbers, or scale up with bulk telecom batch dispatching.
- **Call Management & Analysis** — Retrieve full historical call logs, pull raw transcripts, end live calls instantly, and forcefully interrogate recordings to extract goal completion statuses.
- **Inbound & WebRTC** — View your purchased PSTN numbers for inbound routing and effortlessly spawn decoupled internet-based WebRTC signaling sockets for browser audio.
- **Media Extraction** — Pull native MP3/WAV recording files directly for quality assurance or CRM logging.

### How it works

1. Subscribe to this server
2. Enter your Bland AI API Key
3. Start dispatching and managing voice agents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & Operations** — instantly fire off batch campaigns, query transcript logs, and determine lead qualification status seamlessly.
- **Customer Support** — monitor inbound numbers, listen to specific raw call recordings, and evaluate voice-agent performance.
- **Developers** — debug live conversational flows, disconnect rogue calls, and test WebRTC fallback channels without leaving the IDE.


## Available Tools
- **analyze_call**: Interrogate an active recording querying direct goal completion status
- **end_call**: Force an immediate disconnect disrupting a live AI call
- **get_batch**: Retrieve aggregations profiling the concurrent status of a Bulk Batch
- **get_call_details**: Retrieve explicit variables and exact transcript logic for a completed call
- **list_inbound**: Identify available inbound phone numbers currently bridged to an AI agent
- **list_calls**: Retrieve the full historical log of AI phone calls
- **get_recording**: Retrieve raw native MP3/WAV links logging exact raw audio
- **send_batch**: Dispatch multiple AI agents concurrently scaling bulk telecom arrays
- **send_call**: Dispatch an automated conversational AI agent to a phone number
- **create_web_call**: Spawn a decoupled internet-based WebRTC signaling socket logic stream


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bland AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Please analyze call ID `c-12345` with the goal query 'Was the customer interested in a demo?'"

**🤖 AI Agent:**
> I ran the targeted analysis over the raw transcript for call `c-12345`. The extracted goal status is TRUE. The customer stated 'they would love to see how the dashboard works next Thursday'.

---

**👤 You:**
> "End the currently active phone call ID `c-99999` immediately."

**🤖 AI Agent:**
> The command has been processed. A synchronous interrupt flag was sent to Bland AI, and the telecom session has been successfully shut down.

---

**👤 You:**
> "List all my purchased inbound phone numbers on Bland AI."

**🤖 AI Agent:**
> Here are the PSTN numbers currently bridged to your AI routing logic: 1. +1 (555) 012-3456 (Status: Active), 2. +1 (555) 987-6543 (Status: Inactive).


## ❓ FAQ

**Q: Can my agent determine if a sales phone call was successful?**
Yes. By providing the specific Call ID and a structured goal query (e.g., 'Did they buy?'), your AI agent triggers the 'analyze_call' tool, running a targeted LLM pass exactly over that transcript to extract the explicit boolean outcome.

**Q: What if a voice agent goes off-script on a live call?**
You can instruct your agent to forcefully disrupt the conversation. Using the 'end_call' tool, it will immediately pass an interrupt flag and drop the active telecom connection without waiting for the other party.

**Q: Can I make AI agent calls directly through the browser instead of standard telephony?**
Absolutely. Your agent can execute the 'create_web_call' tool, which bypasses PSTN billing entirely and opens a pure WebRTC signaling socket for direct in-app or browser audio interactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bland-ai](https://vinkius.com/mcp/bland-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bland AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bland-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bland AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bland-ai": {
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
