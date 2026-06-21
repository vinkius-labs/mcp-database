# Flodesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flodesk-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Design gorgeous email campaigns with intuitive templates that grow your audience and reflect your brand without design skills.

## Description
Connect your **Flodesk** account to any AI agent and take full control of your email marketing and subscriber workflows through natural conversation.

### What you can do

- **Audience Orchestration** — List and manage your complete database of email subscribers, including retrieving detailed metadata and performing search lookups
- **Segment Intelligence** — Create and manage subscriber segments (lists) programmatically to maintain a high-fidelity organization of your audience
- **Automation Control** — Monitor your marketing workflows and programmatically add subscribers to automated sequences directly through your agent
- **Subscriber Lifecycle** — Create or update subscriber profiles and manage their opt-in status to ensure compliance and engagement
- **CRM Personalization** — Access and manage custom fields to store unique data points for every subscriber in your account

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Flodesk account (Settings > Integrations > API keys)
3. Start managing your email marketing and automation from Claude, Cursor, or any MCP client

No more manual subscriber lookups or complex segment navigation. Your AI acts as your dedicated email marketing and automation coordinator.

### Who is this for?

- **Content Creators & Influencers** — instantly check subscriber growth and manage newsletters using natural language queries
- **Marketing Managers** — automate lead nurturing by adding new subscribers to specific workflows without leaving your workspace
- **SaaS Founders** — monitor audience segments and update subscriber details through simple AI commands


## Available Tools (10)
- **add_subscriber_to_segment**: Add a subscriber to a segment
- **add_subscriber_to_workflow**: Trigger a workflow for a subscriber
- **create_segment**: Create a new segment
- **get_segment**: Get details for a segment
- **get_subscriber**: Get details for a subscriber
- **list_custom_fields**: List subscriber custom fields
- **list_segments**: List all subscriber segments
- **list_subscribers**: List all Flodesk subscribers
- **list_workflows**: List all workflows
- **upsert_subscriber**: Requires email.

Create or update a subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flodesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Flodesk segments."

**🤖 AI Agent:**
> I've retrieved your segments. You have 3 active lists: 'Weekly Newsletter' (ID: seg_1), 'Beta Testers' (ID: seg_2), and 'Lead Magnet' (ID: seg_3). Which one should I provide details for?

---

**👤 You:**
> "Find subscriber details for 'hello@example.com'."

**🤖 AI Agent:**
> I've located the profile for hello@example.com. They are an 'Active' subscriber and belong to the 'Weekly Newsletter' segment. Would you like to see their custom field values?

---

**👤 You:**
> "Add subscriber 'user@example.com' to the 'Welcome Flow' workflow."

**🤖 AI Agent:**
> Action complete! I've successfully added 'user@example.com' to the 'Welcome Flow' (ID: wflow_123). They will start receiving your automation sequence immediately.


## ❓ FAQ

**Q: How do I find my Flodesk API Key?**
Log in to your Flodesk account, navigate to **Settings** > **Integrations** > **API keys**, and click **Generate new key**.

**Q: Can I search for a subscriber by email?**
Yes! Use the `get_subscriber` tool and provide the email address to retrieve their profile, segments, and status.

**Q: How do I trigger an automation for a subscriber?**
Use the `add_subscriber_to_workflow` tool by providing the unique `workflow_id` and the subscriber's ID or email address.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flodesk-alternative](https://vinkius.com/mcp/flodesk-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flodesk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flodesk-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flodesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flodesk-alternative": {
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
