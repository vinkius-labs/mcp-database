# Flodesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flodesk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage email subscribers, segments, and workflows via AI agents with Flodesk.

## Description
Connect your **Flodesk** account to any AI agent and automate your email marketing and audience management through the Model Context Protocol (MCP). Flodesk is designed for creators and businesses that want to build stunning emails and automate their sales funnels with ease. Now, you can manage your subscribers, organize your segments, and trigger automated workflows directly through natural conversation.

### What you can do

- **Subscriber Management** — List all email subscribers, fetch detailed profile data, and create or update subscriber records instantly.
- **Audience Segmentation** — Access and list your segments, and add subscribers to specific groups to ensure targeted messaging.
- **Workflow Automation** — List your automated email sequences and trigger specific workflows for new or existing subscribers.
- **Opt-out Handling** — Unsubscribe users directly through the agent to maintain a clean and compliant mailing list.
- **Custom Data Fields** — List and create custom subscriber fields to store specific metadata (e.g., interests, purchase history).
- **Form Oversight** — Retrieve a list of all your opt-in forms to monitor where your audience is coming from.
- **Account Insights** — Fetch your Flodesk account metadata to ensure your agent has the correct context for your branding.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flodesk API Key (found in your Settings > Integrations)
3. Start managing your email marketing operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Creators & Solopreneurs** — quickly add a new lead to a specific segment or trigger a welcome sequence after a meeting.
- **Marketing Managers** — get a real-time overview of subscriber counts and active workflows through simple AI commands.
- **E-commerce Brands** — automate the synchronization of customer data and segments for more personalized outreach.


## Available Tools (12)
- **add_to_segment**: Add subscriber to segment
- **trigger_workflow**: Start workflow for user
- **create_subscriber**: Add a subscriber
- **get_account_details**: Get account info
- **get_subscriber**: Get subscriber details
- **list_custom_fields**: List custom subscriber fields
- **list_forms**: List opt-in forms
- **list_segments**: List segments
- **list_subscribers**: List email subscribers
- **list_workflows**: List automation workflows
- **unsubscribe_subscriber**: Unsubscribe a user
- **create_custom_field**: Create custom field


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flodesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 10 most recent email subscribers."

**🤖 AI Agent:**
> Fetching subscribers... I found your 10 most recent contacts, including 'alice@example.com' and 'bob@test.com'. Would you like to see the segments they belong to?

---

**👤 You:**
> "Add 'hello@newlead.com' to my 'Welcome' segment and trigger the 'Onboarding' workflow."

**🤖 AI Agent:**
> Actions completed! I've added the subscriber to your 'Welcome' segment and successfully triggered the 'Onboarding' email sequence for them.

---

**👤 You:**
> "Show me all my active automation workflows."

**🤖 AI Agent:**
> Retrieving workflows... You have 3 active workflows: 'Weekly Newsletter', 'Post-Purchase Survey', and 'Holiday Special'. Which one should I manage for you?


## ❓ FAQ

**Q: How do I add a new subscriber to a specific segment using the agent?**
You can use the 'add_to_segment' tool. Provide the subscriber's email or ID and the specific Segment ID. The agent will immediately associate the contact with that segment in your Flodesk account.

**Q: Can I trigger an automated email sequence for a user?**
Yes! The 'trigger_workflow' tool allows you to start a subscriber on any of your active Flodesk workflows. Simply provide the Workflow ID and the subscriber's email address.

**Q: How do I check if a contact is active or unsubscribed?**
Use the 'get_subscriber' tool and provide the contact's email address. The agent will retrieve the profile details, including their current status (e.g., 'active', 'unsubscribed', or 'bounced').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flodesk](https://vinkius.com/mcp/flodesk)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `flodesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flodesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flodesk": {
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
