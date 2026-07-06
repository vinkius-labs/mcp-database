# Brevo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brevo-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Engage customers across email, SMS, and chat with marketing campaigns and transactional messaging that scale with you.

## Description
Connect your **Brevo** account to any AI agent and take full control of your marketing automation and transactional communication workflows through natural conversation.

### What you can do

- **Contact Orchestration** — List and manage your contact database programmatically, retrieving detailed high-fidelity profiles and synchronizing custom attributes in real-time
- **Campaign Intelligence** — Create and monitor high-fidelity email marketing campaigns and retrieve detailed performance reports directly through your agent
- **Transactional Messaging** — Programmatically dispatch single transactional emails via Brevo SMTP to ensure perfectly coordinated customer notifications
- **Audience Discovery** — Access complete directories of contact lists and manage segmentations to maintain high-fidelity targeting for your digital outreach
- **Operational Monitoring** — Access account-level metadata, verified senders, and real-time SMTP delivery statistics for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** (v3) from your Brevo dashboard (SMTP & API settings)
3. Start managing your communication pipeline from Claude, Cursor, or any MCP client

No more manual toggling between campaign tables or digging through SMTP logs. Your AI acts as your dedicated CRM and marketing operations coordinator.

### Who is this for?

- **Digital Marketers** — instantly retrieve campaign engagement metrics and update contact lists using natural language commands
- **Growth Teams** — automate the ingestion of new leads and monitor transactional email health without leaving your workspace
- **Developers** — integrate high-speed email marketing and SMTP features into custom workflows through simple AI queries


## Available Tools (11)
- **get_account**: Get Brevo account details
- **create_email_campaign**: Create an email campaign
- **list_senders**: List approved senders
- **create_contact**: Create a new contact
- **get_contact**: Get details for a specific contact
- **get_contact_list**: Get details for a specific list
- **get_smtp_statistics**: Get SMTP delivery statistics
- **list_email_campaigns**: List email campaigns
- **list_contacts**: List Brevo contacts
- **list_contact_lists**: List contact lists
- **send_email**: Send a transactional email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brevo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contacts in my Brevo database."

**🤖 AI Agent:**
> I've retrieved your contact directory. You currently have 150 active subscribers, including @user1 and @user2. Would you like to see the detailed attributes for a specific contact?

---

**👤 You:**
> "Send a transactional email to 'test@example.com' with subject 'Order Confirmed'."

**🤖 AI Agent:**
> Email dispatched! I've successfully sent the 'Order Confirmed' notification to test@example.com via Brevo SMTP. Need help tracking the delivery status?

---

**👤 You:**
> "Show my email campaign engagement statistics."

**🤖 AI Agent:**
> Fetching historical performance... Your last campaign 'Spring Sale' had a 24% open rate and 5% clicks. Total successful deliveries: 4,500. Shall I retrieve the detailed sender metadata for your next run?


## ❓ FAQ

**Q: How do I find my Brevo API Key?**
Log in to your account, navigate to **Settings** > **SMTP & API**, and generate a new v3 API Key.

**Q: Can I send transactional emails via AI?**
Yes! The `send_email` tool allows your agent to dispatch single SMTP messages by providing sender and recipient details programmatically.

**Q: How do I check SMTP delivery statistics?**
Use the `get_smtp_statistics` tool to retrieve high-fidelity reports on transactional email performance directly from the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brevo-alternative](https://vinkius.com/mcp/brevo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brevo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brevo-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brevo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brevo-alternative": {
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
