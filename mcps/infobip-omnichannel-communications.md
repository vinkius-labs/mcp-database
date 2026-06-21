# Infobip (Omnichannel Communications) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/infobip-omnichannel-communications)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Send SMS, WhatsApp, and Email via Infobip — manage omnichannel messages and customer profiles in People CDP.

## Description
Connect your **Infobip** account to any AI agent and take full control of your global communications and customer engagement through natural conversation.

### What you can do

- **Omnichannel Messaging** — Send high-priority SMS, WhatsApp Business messages, and HTML emails directly from your agent to international destinations securely
- **Delivery Intelligence** — Track real-time delivery reports and inspect deep proxy logs to ensure your messages reach terminal carriers accurately
- **Customer CDP** — Manage audience profiles in Infobip People, including creating, updating, and retrieving detailed nested traits for personalized engagement
- **Compliance & GDPR** — Execute irreversible data erasure requests for specific CDP profiles to maintain privacy regulations and clean communication queues
- **Activity Audit** — Enumerate recently sent messages and retrieve cost reports to monitor your communication spending and channel performance
- **WhatsApp Business** — Dispatch verified WhatsApp messages using session parameters and omnichannel arrays for professional customer support

### How it works

1. Subscribe to this server
2. Enter your Infobip Base URL and API Key
3. Start communicating globally from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Leads** — dispatch rapid customer updates via WhatsApp or SMS through natural conversation during incidents
- **Marketing Operations** — manage audience profiles and monitor delivery rates across multiple communication channels
- **Developers** — test omnichannel messaging and audit API logs without writing manual scripts or using Postman


## Available Tools
- **upsert_crm_person**: 164 bindings tracking real UUID attributes natively establishing marketing profiles inherently.

Bootstrap an entirely empty structural Contact vector inside People CDP
- **delete_crm_person**: Irreversibly vaporize explicit CDP profiles securing GDPR deletes natively
- **get_delivery_reports**: Inspect deep internal metrics tracking global SMS handoffs
- **get_person_details**: Retrieve the exact structural matching verifying InfoBip Person arrays
- **list_sms_logs**: Retrieve explicit Cloud logging tracing sent SMS bounds over past days
- **list_crm_people**: Enumerate explicitly attached structured profiles identifying entire Audiences
- **dispatch_html_email**: Perform structural extraction of properties spanning the Infobip Email API
- **dispatch_sms_message**: 164 parameters executing international drops securely.

Provision a highly-available JSON Payload routing natively into Infobip SMS
- **dispatch_whatsapp_message**: Identify bounded routing spaces converting JSON texts towards Meta Whatsapp APIs
- **update_person_name**: Mutate global Web CRM parameters modifying explicit People identifiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infobip (Omnichannel Communications)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +123456789: 'Your verification code is 5544'"

**🤖 AI Agent:**
> Dispatching SMS… I've sent the message to +123456789. The Message ID is 'sms-abc-123'. I can monitor the delivery report for you if you'd like to confirm it was received.

---

**👤 You:**
> "List all people in our CDP with the first name 'Alex'"

**🤖 AI Agent:**
> I've scanned your People CDP and found 3 profiles matching 'Alex': 1) Alex Smith (ID: p-123), 2) Alex Johnson (ID: p-456), and 3) Alex Rivera (ID: p-789). Would you like the full details for any of them?

---

**👤 You:**
> "Show me the delivery reports for today's SMS campaign"

**🤖 AI Agent:**
> Retrieving delivery reports… For today's messages, 92% were successfully delivered, 5% are still pending, and 3% failed due to invalid numbers. I can provide the exact Message IDs for the failures if you need to audit them.


## ❓ FAQ

**Q: Can I send a WhatsApp message using my agent?**
Yes. Use the `dispatch_whatsapp_message` tool. You'll need to provide your verified WhatsApp Business number and the target recipient's phone number. Your agent will handle the omnichannel routing to deliver the text instantly.

**Q: How do I check if an SMS was actually delivered?**
The `get_delivery_reports` tool allows your agent to pull raw status updates from Infobip. You can see if terminal carriers processed the text accurately and identify if any packets bounced or failed.

**Q: Can I manage customer profiles in People CDP through a conversation?**
Absolutely. Use tools like `upsert_crm_person` and `list_crm_people` to manage your audience database. Your agent can create new marketing profiles or update existing ones with structured traits directly from your chat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infobip-omnichannel-communications](https://vinkius.com/mcp/infobip-omnichannel-communications)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infobip (Omnichannel Communications)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `infobip-omnichannel-communications` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infobip (Omnichannel Communications)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infobip-omnichannel-communications": {
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
