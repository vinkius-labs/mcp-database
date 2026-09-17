# Novu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/novu)
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


## Available Tools (39)
- **delete_subscriber**: Specify the unique subscriber ID to delete.

Delete a subscriber
- **bulk_update_subscriber_preferences**: Provide the subscriber ID and array of preferences.

Bulk update subscriber preferences
- **create_environment_variable**: Supply both a unique name and its corresponding value.

Create an environment variable
- **create_integration**: Provide all required credentials and set the environment ID.

Create a new integration
- **create_layout**: Provide the required name and content. Variables are optional.

Create a new layout
- **create_subscriber**: Provide a unique subscriber ID and at least an email address.

Create a new subscriber
- **create_topic_subscriptions**: Provide the topic key and an array of subscriber IDs.

Create subscriptions for a topic
- **create_topic**: Supply both a unique key and a descriptive name for the topic.

Create a new topic
- **create_workflow**: Define the workflow name, description, and array of steps.

Create a new workflow
- **delete_integration**: Specify the integration ID to ensure correct deletion.

Delete an integration
- **delete_message**: Provide the unique message ID to delete the message.

Delete a message
- **delete_messages_by_transaction**: Use the transaction ID to identify messages.

Delete messages by transaction ID
- **delete_subscriber_credentials**: Specify both the subscriber ID and the provider ID.

Delete subscriber credentials
- **delete_topic_subscriptions**: Provide the topic key and the array of subscriber IDs.

Delete subscriptions from a topic
- **delete_topic**: Use the unique topic key for deletion.

Delete a topic
- **get_environment_variable_usage**: Supply the variable key.

Retrieve usage of an environment variable
- **get_subscriber_preferences**: Provide the subscriber ID.

Retrieve subscriber preferences
- **get_subscriber**: Only provide the subscriber ID.

Retrieve a subscriber by ID
- **list_active_integrations**: Do not require any parameters.

List active integrations
- **list_environment_variables**: Do not require any parameters.

List all environment variables
- **list_integrations**: Do not require any parameters.

List all integrations
- **list_messages**: Filter results using channel, subscriber, or transaction IDs.

List messages
- **list_topic_subscriptions**: Pass the topic key to retrieve the list.

List subscriptions for a topic
- **search_subscribers**: Use filters like email or name.

Search for subscribers
- **set_primary_integration**: Use the integration ID to set the primary status.

Set an integration as primary
- **trigger_broadcast**: Specify the workflow name and payload. Overrides are optional.

Send a notification to all existing subscribers
- **trigger_bulk_event**: Pass an array of event objects, ensuring the total count does not exceed 100.

Trigger multiple events in a single request
- **trigger_event**: Trigger a notification to one or more subscribers
- **update_environment_variable**: Must specify the variable key and provide the new value.

Update an environment variable
- **update_integration**: Must provide the integration ID to target the update.

Update an integration
- **update_subscriber_credentials**: Requires the subscriber ID and provider ID.

Update subscriber credentials
- **update_subscriber_preference**: Requires the subscriber ID and preference object.

Update a subscriber preference
- **update_subscriber**: Must provide the subscriber ID and at least one field to update.

Update an existing subscriber
- **update_topic**: Specify the topic key and the new name.

Update a topic
- **upsert_subscriber_credentials**: Provide the subscriber ID, provider ID, and credentials object.

Upsert subscriber credentials
- **cancel_trigger**: Provide the specific transaction ID to be canceled.

Cancel active or pending workflows (e.g., digests, delays)
- **check_topic_subscriber**: Supply the topic key and the external subscriber ID.

Check if a subscriber is subscribed to a topic
- **get_topic_subscription**: Provide the topic key and the specific subscription identifier.

Retrieve a topic subscription
- **get_topic**: Supply the required topic key.

Retrieve a topic by key


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

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/novu](https://vinkius.com/en/ai-agent-connect/novu)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `novu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
