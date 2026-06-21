# Teachable (Extended) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/teachable-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your Teachable school — list courses, manage users, track transactions, and monitor webhooks directly from your AI agent.

## Description
Connect your **Teachable** school to any AI agent to streamline your course management and student operations through natural conversation.

### What you can do

- **Course Management** — List all courses, filter by name, author, or publication status to keep track of your curriculum.
- **User Operations** — List, create, and update users. Search for students by email and manage their profiles without leaving your chat.
- **Financial Tracking** — Query transactions to monitor sales, refunds, and chargebacks across specific courses or users.
- **Pricing & Plans** — Access available pricing plans to understand your school's offer structure.
- **Webhook Monitoring** — List registered webhooks to ensure your external integrations are correctly configured.

### How it works

1. Subscribe to this server
2. Enter your Teachable API Key
3. Start managing your e-learning platform from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Course Creators** — quickly check enrollment numbers and student details while planning content.
- **Support Teams** — update student names or find transaction records instantly to resolve tickets.
- **School Administrators** — monitor the health of the school through transaction and webhook audits.


## Available Tools
- **list_courses**: Can be filtered by name, publish status, or author.

List all courses in the Teachable school
- **create_user**: Email is required.

Create a new user in the Teachable school
- **list_pricing_plans**: List pricing plans in the Teachable school
- **list_transactions**: Can be filtered by user, course, affiliate, dates, or refund/chargeback status.

List transactions in the Teachable school
- **update_user**: Update an existing user in the Teachable school
- **list_users**: Can be filtered by email. Use search_after for pagination beyond 10,000 records.

List all users in the Teachable school
- **list_webhooks**: List all registered webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Teachable (Extended)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all courses that are currently published in my school."

**🤖 AI Agent:**
> I've retrieved your published courses. You have 3 active courses: 'Mastering MCP' (ID: 101), 'AI for Beginners' (ID: 102), and 'Advanced React' (ID: 103). Would you like more details on any of these?

---

**👤 You:**
> "Create a new user with the email 'newstudent@example.com' and name 'John Doe'."

**🤖 AI Agent:**
> User 'John Doe' has been successfully created with ID 987654. They are now registered in your Teachable school.

---

**👤 You:**
> "Show me the recent transactions for course ID 554433."

**🤖 AI Agent:**
> I found 2 recent transactions for course 554433. One for $99.00 (User: 123) and another for $99.00 (User: 456). Neither has been refunded.


## ❓ FAQ

**Q: Can I search for a specific student using their email address?**
Yes! Use the `list_users` tool and provide the email address as a filter. The agent will return the user's details, including their ID and signup information.

**Q: Is it possible to see if a transaction has been refunded?**
Absolutely. The `list_transactions` tool allows you to filter by `is_fully_refunded`. You can also filter by course ID or user ID to narrow down your search.

**Q: Can I update a user's name if they made a typo during registration?**
Yes. Use the `update_user` tool with the student's `user_id` and the new `name`. The agent will process the update and confirm the changes in your Teachable school.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/teachable-extended](https://vinkius.com/mcp/teachable-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Teachable (Extended)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `teachable-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Teachable (Extended)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "teachable-extended": {
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
