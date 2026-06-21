# Robly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/robly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate email marketing via Robly — manage contacts, subscriber lists, and campaign stats with AI.

## Description
Connect your **Robly** account to any AI agent and take full control of your email marketing orchestration and audience management through natural conversation. Robly provides a powerful platform for reaching your subscribers, and this integration allows you to retrieve contact metadata, manage subscriber lists, and monitor campaign performance directly from your chat interface.

### What you can do

- **Subscriber & List Orchestration** — List, create, and organize subscriber lists programmatically to ensure your audience segments are always synchronized.
- **Contact Lifecycle Management** — Access and monitor your contact database and retrieve detailed profile metadata directly from the AI interface to keep your leads updated.
- **Campaign Intelligence** — Access available subscriber lists and monitor growth stats via natural language to drive better engagement.
- **Membership & Unsubscribe Control** — Manage contact unsubscribes and check membership status across multiple lists using simple AI commands.
- **Operational Monitoring** — Track system responses and manage list metadata to ensure your marketing stack is fully optimized.

### How it works

1. Subscribe to this server
2. Enter your Robly API ID and API Key from your account settings
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

No more manual CSV imports or list searching. Your AI acts as a dedicated marketing coordinator or audience analyst.

### Who is this for?

- **Email Marketers** — quickly retrieve subscriber counts and monitor list growth without switching between dashboard tabs.
- **Sales Teams** — automate the addition of new leads to specific subscriber lists via natural conversation.
- **Content Creators** — streamline the retrieval of contact metadata and monitor audience health directly within the chat.


## Available Tools
- **add_contact**: Add contact to list
- **check_list_membership**: Check if email is in list
- **clear_sub_list**: Clear list contacts
- **create_sub_list**: Create a new list
- **delete_sub_list**: Delete a sub-list
- **list_contacts**: List marketing contacts
- **list_sub_lists**: List all sub-lists
- **list_webhooks**: List account webhooks
- **rename_sub_list**: Rename a sub-list
- **search_contact**: Search contact by email
- **unsubscribe_contact**: Unsubscribe a contact
- **update_contact**: Update contact details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Robly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all subscriber lists in my Robly account."

**🤖 AI Agent:**
> I've retrieved your lists. You have 4 active sub-lists including 'Main Newsletter', 'Premium Customers', and 'Event Leads'. Which one would you like to see contacts for?

---

**👤 You:**
> "Show me the performance analytics for all email campaigns sent this month."

**🤖 AI Agent:**
> 12 email campaigns sent this month. Total sent: 45,600. Overall open rate: 28.4% (industry avg: 21%). Click rate: 4.8%. Unsubscribe rate: 0.12%. Top performer: "Flash Sale Alert" with 42% open rate and 8.9% click rate. "Weekly Newsletter #19" reached the largest audience (12,400 recipients). A/B test winner: Subject line B outperformed A by 34% on opens. Robly's OpenGen AI feature re-sent to non-openers and recovered 2,340 additional opens (5.1% recovery).

---

**👤 You:**
> "Create a new email campaign targeting subscribers who have not engaged in the last 30 days."

**🤖 AI Agent:**
> Re-engagement campaign created: "We Miss You!". Target segment: 3,456 subscribers with no opens or clicks in 30 days. Subject: "It's been a while - here's 20% off to welcome you back". Content: personalized with last purchased product category, 20% discount code COMEBACK20, and updated product highlights. Send schedule: Tomorrow 10 AM (optimal send time). OpenGen enabled: will auto-resend to non-openers 48 hours later with alternate subject line. Expected recovery: 12-15% re-engagement based on similar campaigns.


## ❓ FAQ

**Q: Can my AI automatically find if a specific email exists in a Robly subscriber list?**
Yes! Use the `exists_in_sub_list` tool. Provide the email and the `sub_list_id`, and your agent will return the membership status and subscription details instantly.

**Q: How do I find my Robly API ID and API Key?**
Log in to your Robly account, go to **My Account** (top right), and you will find your unique **API ID** and **API Key** listed in the account overview.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/robly](https://vinkius.com/mcp/robly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Robly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `robly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Robly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "robly": {
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
