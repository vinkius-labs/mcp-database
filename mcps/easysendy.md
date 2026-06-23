# EasySendy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/easysendy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Send high-volume email campaigns through multiple delivery servers with list hygiene tools that protect your sender score.

## Description
Connect your **EasySendy** account to any AI agent and take full control of your email marketing lists and subscriber engagement workflows through natural conversation.

### What you can do

- **Audience Orchestration** — Create and manage email subscriber lists programmatically, including retrieving detailed metadata and custom tags
- **Subscriber Lifecycle** — Programmatically add, update, or remove subscribers from lists and manage detailed profiles directly from your agent
- **Batch Intelligence** — Perform large-scale subscriber imports and batch operations to streamline your high-volume marketing campaigns
- **Engagement Control** — Programmatically unsubscribe users or manage opt-in types (single/double) to ensure high-fidelity list hygiene and compliance
- **Field Customization** — Retrieve and manage custom contact fields and tags to maintain a structured and personalized communication ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **Public API Key** from your EasySendy dashboard (Profile > APIs)
3. Start managing your email marketing lists from Claude, Cursor, or any MCP client

No more manual subscriber management or complex CSV exports in the dashboard. Your AI acts as your dedicated email marketing and list coordinator.

### Who is this for?

- **Growth Marketers** — instantly retrieve list details and manage segments using natural language queries
- **Marketing Operations** — automate lead ingestion and track custom tags across multiple lists without leaving your workspace
- **Business Owners** — monitor audience growth and manage subscriber lifecycles through simple AI commands


## Available Tools (11)
- **add_multiple_subscribers**: Input should be an array of subscriber objects.

Add multiple subscribers to a list
- **add_subscriber**: Requires the List UID and at least an EMAIL address.

Add a single subscriber to a list
- **create_list**: Create a new subscriber list
- **delete_list**: Delete a subscriber list
- **delete_subscriber**: Delete a subscriber from a list
- **get_list_fields**: Get custom fields/tags for a list
- **get_subscriber_details**: Get details for a specific subscriber
- **list_all_lists**: List all subscriber lists
- **unsubscribe_user**: Unsubscribe a user from a list
- **update_list**: Update an existing subscriber list
- **update_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EasySendy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email subscriber lists in EasySendy."

**🤖 AI Agent:**
> I've retrieved your email lists. You currently have 3 active lists: 'Newsletter 2026' (UID: abc-123), 'Product Leads', and 'Beta Testers'. Which one should we manage?

---

**👤 You:**
> "Add subscriber 'john.doe@example.com' to list UID 'abc-123'."

**🤖 AI Agent:**
> Done! John Doe has been successfully added to the 'Newsletter 2026' list. They will now receive your scheduled campaigns for this list.

---

**👤 You:**
> "Find subscriber details for 'sarah@example.com' in list 'abc-123'."

**🤖 AI Agent:**
> I've located Sarah's profile in the specified list. She is currently 'Confirmed' and joined on 2024-03-15. Her tags include 'Premium' and 'Loyalty'. Would you like to see her custom field values?


## ❓ FAQ

**Q: How do I find my EasySendy API Key?**
Log in to your EasySendy account, click on your profile (top right), select **APIs**, and copy your Public API Key.

**Q: Can I search for a subscriber by email?**
Yes! Use the `get_subscriber_details` tool and provide the List UID and the subscriber's email address to retrieve their full profile.

**Q: How do I import multiple subscribers at once?**
Use the `add_multiple_subscribers` tool and provide a JSON array containing the subscriber details (EMAIL, FNAME, LNAME, etc.).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/easysendy](https://vinkius.com/mcp/easysendy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EasySendy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `easysendy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EasySendy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "easysendy": {
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
