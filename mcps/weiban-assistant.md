# Weiban Assistant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weiban-assistant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Customer relationship management for WeCom — manage leads, customers, and group chats via AI.

## Description
Empower your AI agent to orchestrate your customer relationship within the WeCom ecosystem with **Weiban Assistant**, the leading CRM solution for business WeChat. By connecting Weiban to your agent, you transform complex customer tracking and group chat management into a natural conversation. Your agent can instantly list your customers, retrieve detailed lead information, monitor group chat activity, and even provide staff behavior statistics without you ever needing to navigate the web interface. Whether you are managing high-volume customer inquiries or complex sales pipelines, your agent acts as a real-time sales and service assistant, keeping your data accurate and your team responsive.

### What you can do

- **Customer Orchestration** — List and retrieve detailed information about your WeCom customers and external users.
- **Pipeline Management** — Manage sales leads with full support for listing and creating new prospects.
- **Group Chat Monitoring** — List active group chats and retrieve detailed information about participation and activity.
- **Staff Analytics** — Monitor staff behavior statistics and performance metrics across the organization.
- **Activity Auditing** — Browse chat records and retrieve high-level summaries of organization-wide WeCom engagement.

### How it works

1. Subscribe to this server
2. Enter your Weiban Corp ID and Secret
3. Start managing your WeCom ecosystem through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — track lead progress and monitor team responsiveness through natural language queries.
- **Customer Success Teams** — manage customer relationships and monitor group chat activity directly from your AI-powered workspace.
- **Operations Leads** — oversee organization-wide WeCom metrics and staff behavior statistics through a unified AI interface.
- **WeCom Power Users** — integrate your existing Weiban CRM workflows into your AI-driven daily routines.


## Available Tools
- **create_lead**: Create a new lead
- **get_customer_details**: Get customer details
- **get_group_chat**: Get group chat details
- **get_org_summary**: Get organization activity summary
- **get_staff_stats**: Get staff behavior statistics
- **list_chat_records**: List chat histories
- **list_customers**: List WeCom customers
- **list_group_chats**: List WeCom group chats
- **list_leads**: List sales leads
- **list_staff**: List organization staff


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weiban Assistant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my WeCom customers from Weiban."

**🤖 AI Agent:**
> I've retrieved your WeCom customers. You have 150 total customers, including 12 high-value accounts marked with specific tags. Would you like to view the details of the most active ones?

---

**👤 You:**
> "Show me the behavior statistics for staff user 'Mario'."

**🤖 AI Agent:**
> I've listed the performance stats for Mario. Today, he has handled 42 customer messages with an average response time of 2 minutes. His customer satisfaction score is currently 4.9/5.0.

---

**👤 You:**
> "Check the activity summary for our group chats."

**🤖 AI Agent:**
> I've retrieved the group chat summary. There are 25 active groups with a total of 1,200 participants. The 'VIP Customers' group is currently the most active. Would you like a detailed breakdown of engagement per group?


## ❓ FAQ

**Q: How do I find my Weiban Corp ID and Secret?**
Log in to your Weiban administration backend, go to [App Center] → [Open Platform], and you will find your Corp ID and Secret there. Ensure you have the necessary permissions enabled.

**Q: Can I see chat records through this server?**
Yes. Use the `list_chat_records` tool to retrieve historical chat between staff members and customers. This is essential for auditing service quality and tracking sales conversations.

**Q: Is it possible to monitor group chat activity?**
Yes! You can use the `list_group_chats` tool to see all active groups and `get_group_chat` with a specific ID to retrieve detailed information about participation and engagement levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weiban-assistant](https://vinkius.com/mcp/weiban-assistant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weiban Assistant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `weiban-assistant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weiban Assistant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weiban-assistant": {
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
