# Kit (ConvertKit) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kit-convertkit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enable your AI agent to manage email subscribers, organize tags, and monitor broadcast campaigns via the Kit API.

## Description
Integrate your AI assistant with **Kit** (formerly ConvertKit), the email marketing platform for creators.

### What you can do

- **Subscriber Management** — Retrieve subscriber profiles, add emails to lists, and check engagement metrics.
- **Tag Organization** — List audience tags or apply specific markers to user segments.
- **Broadcast Monitoring** — Check open rates, click-through metrics, and campaign statuses.

### How it works

1. Add the Kit integration to your AI toolset.
2. Provide your Kit API Secret (found in Settings > Advanced).
3. Manage your email audiences via natural language commands.

### Who is this for?

- **Digital Creators** — Track funnel sign-ups and tag audience members from chat.
- **Marketing Managers** — Pull open rates and campaign performance instantly.
- **Customer Support** — Check if a user received an onboarding email without accessing the dashboard.


## Available Tools (10)
- **add_subscriber_to_form**: Subscribe a person to a form
- **get_account_growth_summary**: Retrieve a high-level summary of your subscriber count
- **get_subscriber_details**: Get details for a specific subscriber
- **list_optin_forms**: List all opt-in forms
- **list_email_sequences**: List automated email sequences
- **list_subscribers**: List your email subscribers
- **list_all_tags**: List all audience tags
- **search_subscriber_by_id**: Retrieve a subscriber by their numeric ID
- **apply_tag_to_subscriber**: Apply a tag to a subscriber by email
- **update_subscriber**: Update subscriber metadata or custom fields


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kit (ConvertKit)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the profile and tags for 'john.doe@example.com'."

**🤖 AI Agent:**
> Subscriber 'John Doe' is active. Tags: 'Welcome Sequence Completed', 'VIP Customers'. Last broadcast interaction: 3 days ago.

---

**👤 You:**
> "Show the open rate and clicks from my latest broadcast."

**🤖 AI Agent:**
> Your latest broadcast 'Monthly Creator Tips' was sent to 14,500 subscribers. Open rate: 42.1% (6,104 opens). Unique clicks: 1,215 (CTR: 8.3%). Want me to check the top performing link?

---

**👤 You:**
> "List all tags available in my Kit account so I can categorize new leads."

**🤖 AI Agent:**
> I've retrieved 12 tags from your account, including 'Newsletter Subscriber', 'Ebook Download', and 'Webinar-2024-Attendee'. Which tag should we apply to the current segment?


## ❓ FAQ

**Q: How do I find my Kit API Secret?**
Log in to Kit, go to **Settings > Advanced**. Under 'API', click **Show** next to API Secret, copy the string, and paste it below.

**Q: Why is the API Secret required instead of the standard API Key?**
The API Key only provides read access to public forms. The API Secret grants full access to manage subscribers, tags, and broadcast data as needed by this integration.

**Q: Can the agent send broadcast emails?**
No. For safety, the integration is read/manage only. The agent can check campaign metrics and manage tags, but actual email sending must be done via the Kit dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kit-convertkit](https://vinkius.com/mcp/kit-convertkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kit (ConvertKit)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kit-convertkit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kit (ConvertKit)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kit-convertkit": {
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
