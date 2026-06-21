# SleekFlow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sleekflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage omnichannel customer conversations — read messages, check contacts, and send replies across WhatsApp, Instagram, and more directly from your AI agent.

## Description
Connect your **SleekFlow** platform to any AI agent to power up your conversational support, sales, and marketing. Read real-time chat threads spanning across multiple digital channels and dispatch replies without leaving your chat interface.

### What you can do

- **Unified Conversations** — Track and retrieve ongoing chat histories across WhatsApp, Instagram, Telegram, and WeChat
- **Direct Messaging** — Compose and send outbound responses or proactive messages back to customers seamlessly
- **Contact Management** — List all synced contacts and get their deep profile metadata including CRM ties
- **Chat Segmentation** — View categorization labels to segment hot leads or identify VIP support customers
- **Automation Overviews** — Retrieve a list of your configured automation workflows and active chatbot trees

### How it works

1. Subscribe to this server
2. Provide your SleekFlow API Key
3. Use Claude, Cursor, or any MCP-compatible client to start responding to leads or monitoring your omnichannel inbox

Stop switching between WhatsApp Web, Facebook Business, and your internal tools. Your AI agent acts as your super-powered central inbox.

### Who is this for?

- **Sales Development Reps (SDRs)** — ask your agent to retrieve new hot leads from WhatsApp and draft high-converting proposals
- **Support Teams** — read a frustrated customer's recent WeChat log and formulate a deeply personalized resolution instantly
- **CRM Managers** — run audits on customer labels and active automation chat flows straight from the terminal


## Available Tools
- **list_contacts**: Lists all contacts in SleekFlow
- **get_contact_details**: Retrieves details for a specific contact
- **list_conversations**: Lists all conversations across channels
- **send_message**: Sends a message in a conversation
- **list_channels**: Lists all connected communication channels
- **list_automation_flows**: Lists available automation flows
- **list_contact_labels**: Lists all labels used for contact categorization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SleekFlow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all unread conversations from this weekend."

**🤖 AI Agent:**
> You have 14 unread conversations since Saturday:
- 6 from WhatsApp (3 refund requests, 2 product inquiries, 1 complaint)
- 5 from Instagram DM (all product inquiries)
- 3 from Telegram (support questions)
Would you like me to draft responses for the refund requests first?

---

**👤 You:**
> "Send a reply to conversation conv-xxxx saying 'Your refund has been processed. It will appear in 3-5 business days.'"

**🤖 AI Agent:**
> Reply sent to conversation conv-xxxx (WhatsApp).
- Contact: Maria Silva (+55 11 9xxxx-xxxx)
- Message: 'Your refund has been processed. It will appear in 3-5 business days.'
- Status: delivered ✓


## ❓ FAQ

**Q: Can my AI automatically reply to an agitated customer on WhatsApp?**
Yes. If you point your AI to an active conversation ID, the agent can analyze the raw message history to gauge the emotion. It will draft a polite, perfectly-toned de-escalation message, and if you approve it, it'll trigger the `send_message` tool pointing directly to the customer's WhatsApp payload.

**Q: Can I bulk analyze all incoming conversations over the weekend?**
Absolutely. You can request your agent to invoke the `list_conversations` command. Your agent can read the active, unassigned threads, categorize them by user intent (e.g., 'refund query', 'feature request'), and provide you a summary dashboard right inside your IDE or markdown interface.

**Q: How does the AI know if a customer has an automation flow attached?**
Your agent can call `list_automation_flows` as well as query the specific `get_contact_details` tool. This cross-references whether the phone number currently triggers out of an existing flow ID, preventing your AI from interrupting an active bot onboarding session accidentally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sleekflow](https://vinkius.com/mcp/sleekflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SleekFlow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sleekflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SleekFlow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleekflow": {
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
