# Podium MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/podium)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Win more local customers with review generation, webchat, text marketing, and payment collection from one inbox.

## Description
Connect your **Podium** account to any AI agent and take full control of your local business communication and reputation orchestration through natural conversation. Podium provides a premier platform for managing customer interactions, and this integration allows you to retrieve conversation metadata, monitor online reviews, and manage customer contacts directly from your chat interface.

### What you can do

- **Unified Messaging Orchestration** — List all managed conversations and send new messages programmatically across various locations and channels to ensure your customer outreach is always synchronized.
- **Reputation & Review Intelligence** — Access and monitor business reviews and send automated review invitations to satisfied customers directly from the AI interface.
- **Contact Lifecycle Management** — Create and update customer contacts and retrieve detailed profile metadata via natural language to maintain a high-fidelity CRM.
- **Location & Operational Control** — List business locations and retrieve organization-level metadata to ensure your communication hub is always optimized.
- **Operational Monitoring** — Track system activity and manage webhook metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Podium Access Token from your developer settings
3. Start managing your local business communications from Claude, Cursor, or any MCP-compatible client

No more manual dashboard navigation for simple replies. Your AI acts as a dedicated communication manager or customer success coordinator.

### Who is this for?

- **Local Business Owners** — quickly retrieve customer feedback and monitor location performance without switching apps.
- **Customer Success Teams** — automate the retrieval of message history and respond to queries via natural conversation.
- **Marketing Operations** — streamline the retrieval of review metadata and monitor organizational health directly within the chat.


## Available Tools
- **create_contact**: Create a new customer contact
- **get_contact_details**: Get details for a specific contact
- **get_location_details**: Get details for a specific location
- **get_current_user**: Get authenticated user profile
- **get_organization_info**: Get current organization details
- **send_review_invitation**: Send a review invitation
- **list_contacts**: List customers contacts
- **list_conversations**: List conversations for a location
- **list_locations**: List business locations
- **list_reviews**: List business reviews
- **list_webhooks**: List configured webhooks
- **send_message**: Requires location ID and message body.

Send a message to a contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Podium** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my business locations in Podium."

**🤖 AI Agent:**
> I've retrieved your locations. You have 2 active environments: 'Downtown Office' (ID: loc_123) and 'Westside Branch'. Which one would you like to see reviews for?

---

**👤 You:**
> "Show me all unread customer messages from today across all communication channels."

**🤖 AI Agent:**
> 34 unread messages today across your channels. SMS: 18 messages (12 new inquiries, 4 appointment confirmations, 2 review responses). Google Business: 8 messages (5 questions about hours/services, 3 quote requests). Facebook Messenger: 5 conversations. Web chat: 3 live requests. Average response time today: 12 minutes. 6 messages are flagged as urgent based on sentiment analysis, including a billing complaint from a VIP customer.

---

**👤 You:**
> "Send a review request via text message to the 15 customers who completed service today."

**🤖 AI Agent:**
> Review requests sent to 15 customers. Message: "Thanks for choosing us today! We'd love your feedback. Leave a review here: [review_link]". Delivery status: 14 delivered, 1 pending. Based on historical data, you can expect 5-6 reviews (38% response rate). Your current Google rating: 4.7 stars from 234 reviews. These review requests typically boost monthly review volume by 40%.


## ❓ FAQ

**Q: Can my AI automatically find the latest reviews for a specific business location?**
Yes! Use the `list_reviews` tool with the Location ID. Your agent will respond with the most recent customer reviews and their ratings in seconds.

**Q: How do I find my Podium Location ID?**
Ask the AI agent to run the `list_locations` tool. It will retrieve all your business locations along with their unique IDs for you to use in other commands.

**Q: Can I send an SMS invitation for a review via the AI?**
Absolutely. Use the `send_review_invitation` tool. Provide the customer details and the location ID, and the agent will trigger the invitation via Podium immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/podium](https://vinkius.com/mcp/podium)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Podium** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `podium` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Podium** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "podium": {
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
