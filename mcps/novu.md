# Novu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/novu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate multi-channel notifications via Novu — trigger workflows, manage subscribers, and handle preferences directly from any AI agent.

## Description
Connect your **Novu** account to any AI agent and take full control of your notification infrastructure through natural conversation.

### What you can do

- **Triggering & Events** — Trigger single, bulk, or broadcast notifications across Email, SMS, Push, and Chat using workflow identifiers.
- **Subscriber Management** — Create, retrieve, update, and search for subscribers to maintain an up-to-date communication database.
- **Preference Controls** — Inspect and update subscriber-specific notification preferences to ensure compliance and user satisfaction.
- **Workflow Cancellation** — Cancel active or pending workflows, such as digests or delayed notifications, using transaction IDs.
- **Tenant Context** — Manage notifications within specific tenant contexts for multi-tenant applications.

### How it works

1. Subscribe to this server
2. Enter your Novu Secret Key
3. Start triggering and managing notifications from Claude, Cursor, or any MCP-compatible client

No more manual API calls to test your notification flows. Your AI acts as a dedicated communications engineer.

### Who is this for?

- **Developers** — test notification triggers and subscriber updates directly from the code editor without switching to Postman.
- **Product Managers** — verify workflow payloads and inspect subscriber preferences to troubleshoot delivery issues.
- **Growth Teams** — automate broadcast notifications for marketing campaigns through simple natural language commands.


## Available Tools
- **bulk_update_subscriber_preferences**: Bulk update subscriber preferences
- **cancel_trigger**: Cancel active or pending workflows (e.g., digests, delays)
- **check_topic_subscriber**: Check if a subscriber is subscribed to a topic
- **create_environment_variable**: Create an environment variable
- **create_integration**: Create a new integration
- **create_layout**: Create a new layout
- **create_subscriber**: Create a new subscriber
- **create_topic_subscriptions**: Create subscriptions for a topic
- **create_topic**: Create a new topic
- **create_workflow**: Create a new workflow
- **delete_integration**: Delete an integration
- **delete_message**: Delete a message
- **delete_messages_by_transaction**: Delete messages by transaction ID
- **delete_subscriber_credentials**: Delete subscriber credentials
- **delete_subscriber**: Delete a subscriber
- **delete_topic_subscriptions**: Delete subscriptions from a topic
- **delete_topic**: Delete a topic
- **get_environment_variable_usage**: Retrieve usage of an environment variable
- **get_subscriber_preferences**: Retrieve subscriber preferences
- **get_subscriber**: Retrieve a subscriber by ID
- **get_topic_subscription**: Retrieve a topic subscription
- **get_topic**: Retrieve a topic by key
- **list_active_integrations**: List active integrations
- **list_environment_variables**: List all environment variables
- **list_integrations**: List all integrations
- **list_messages**: List messages
- **list_topic_subscriptions**: List subscriptions for a topic
- **search_subscribers**: Search for subscribers
- **set_primary_integration**: Set an integration as primary
- **trigger_broadcast**: Send a notification to all existing subscribers
- **trigger_bulk_event**: Trigger multiple events in a single request
- **trigger_event**: Trigger a notification to one or more subscribers
- **update_environment_variable**: Update an environment variable
- **update_integration**: Update an integration
- **update_subscriber_credentials**: Update subscriber credentials
- **update_subscriber_preference**: Update a subscriber preference
- **update_subscriber**: Update an existing subscriber
- **update_topic**: Update a topic
- **upsert_subscriber_credentials**: Upsert subscriber credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Novu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Trigger the 'welcome-onboarding' workflow for subscriber 'user_99' with the payload { "name": "Alice" }."

**🤖 AI Agent:**
> I've triggered the 'welcome-onboarding' event for subscriber 'user_99'. The transaction has been initiated successfully.

---

**👤 You:**
> "Search for a subscriber with the email 'support@example.com'."

**🤖 AI Agent:**
> I found a subscriber matching that email. The ID is 'sub_5544' and the name is 'Support Team'. Would you like to see their full preferences?

---

**👤 You:**
> "Cancel the notification trigger with transaction ID 'tx_abc123'."

**🤖 AI Agent:**
> The workflow execution for transaction 'tx_abc123' has been successfully cancelled.


## ❓ FAQ

**Q: Can I send a notification to all my subscribers at once?**
Yes! Use the `trigger_broadcast` tool with your workflow name. This will initiate a notification event for every existing subscriber in your Novu environment.

**Q: How do I find a subscriber if I only have their email address?**
You can use the `search_subscribers` tool and provide the email as a parameter. The agent will return the subscriber's full profile, including their unique `subscriberId`.

**Q: Is it possible to stop a notification that is currently in a 'delay' or 'digest' state?**
Yes. By using the `cancel_trigger` tool with the corresponding `transactionId`, you can halt any active or pending workflow execution before it reaches the final delivery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/novu](https://vinkius.com/mcp/novu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Novu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `novu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Novu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "novu": {
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
