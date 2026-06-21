# Landbot MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/landbot-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Build conversational landing pages and chatbot flows with a visual builder that replaces boring forms with engaging conversations.

## Description
Connect your **Landbot** account to any AI agent and manage chatbots through natural conversation.

### What you can do

- **Bot Management** — List bots, inspect configurations, and track performance
- **Conversation Tracking** — Browse conversations, read messages, and send replies
- **Customer Database** — List customers with engagement data and conversation history
- **Flow Monitoring** — Track chatbot flows and their conversion metrics
- **Channel Management** — Monitor WhatsApp, Web, and API channels
- **Analytics** — Access conversation metrics, response rates, and bot performance

### How it works

1. Subscribe to this server
2. Enter your Landbot API Token
3. Start managing chatbots from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing** — manage lead-generation bots and track conversions
- **Support** — monitor customer conversations and response quality
- **Growth** — analyze chatbot performance and optimize flows


## Available Tools
- **handoff_to_agent**: Assign to human
- **trigger_bot_flow**: Start bot flow
- **get_account_info**: Check API status
- **get_customer_details**: Get user profile
- **list_team_agents**: List support agents
- **list_active_bots**: List available bots
- **list_landbot_customers**: List chatbot users
- **list_message_hooks**: Get event configs
- **send_proactive_image**: Send chat image
- **send_proactive_text**: Send chat message
- **send_whatsapp_template**: Send WA template
- **update_customer_field**: Set user property


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Landbot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all bots with conversation counts and the latest customer conversations."

**🤖 AI Agent:**
> Bots: 4. 'Lead Qualifier' (1.2K conversations, Web, 34% conversion ⭐). 'Support Bot' (890, Web+WhatsApp, 4.2 min avg). 'Onboarding' (345, Web). 'WhatsApp Sales' (567, WhatsApp, 28% conversion). Latest: 1) Ana — Lead Qualifier, 'Interested in Pro plan' (5 min ago). 2) Mike — Support, 'Password reset help' (12 min ago). 3) Lisa — WhatsApp Sales, 'Pricing question' (20 min ago).

---

**👤 You:**
> "Show the conversation flow and analytics for the Lead Qualifier bot."

**🤖 AI Agent:**
> Lead Qualifier flow: 6 steps. 1) Welcome (98% reach). 2) Company Size (92%). 3) Budget Range (85%). 4) Timeline (78%). 5) Contact Info (62%). 6) Meeting Booking (34% ✅). Drop-off: Step 4→5 (16%, budget sensitivity). Avg completion: 2.1 min. Leads captured: 408 this month. Qualified: 246 (60%). MQL→SQL conversion: 42%.

---

**👤 You:**
> "List all customers and send a reply to Ana's conversation."

**🤖 AI Agent:**
> Customers: 2,834 total. Active (7 days): 145. Channels: Web (1,890), WhatsApp (944). Top by conversations: Ana Costa (8 conversations), Mike Torres (5), Lisa Park (4). Reply sent to Ana! ✅ 'Hi Ana, great to hear you are interested in Pro! I will have our sales team reach out within the hour. In the meantime, here is our pricing page.'


## ❓ FAQ

**Q: Can I manage bots and read conversations?**
Yes. List all bots with performance metrics, browse conversations with full message history, and send replies to customers.

**Q: How does Landbot authentication work?**
Landbot uses a **Token** header for authentication against `api.landbot.io/v1`. This differs from standard Bearer authentication.

**Q: Can I track chatbot conversion metrics?**
Yes. Monitor flow completion rates, drop-off points, lead capture rates, and conversation-to-conversion metrics per bot.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/landbot-alternative](https://vinkius.com/mcp/landbot-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Landbot** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `landbot-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Landbot** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "landbot-alternative": {
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
