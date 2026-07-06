# Kit (ConvertKit) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kit-convertkit-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate your creator marketing — manage subscribers, tags, and forms via AI.

## Description
Empower your AI agent to orchestrate your entire creator ecosystem with **Kit** (formerly ConvertKit), the leading platform for professional creators. By connecting Kit to your agent, you transform audience engagement into a natural conversation. Your agent can instantly audit subscriber growth, assign targeted tags, and manage email sequences without you ever touching a dashboard. Whether you are launching a new lead magnet or maintaining a large community, your agent acts as a real-time audience manager, ensuring your marketing is always automated and personal.

### What you can do

- **Subscriber Management** — List, retrieve, and update subscriber profiles to maintain a deep understanding of your audience.
- **Tagging & Segmentation** — Create and assign tags to subscribers instantly to organize your list for targeted broadcasts.
- **Form & Sequence Control** — Monitor signup forms and email sequences to ensure your lead generation funnels are active.
- **Account Auditing** — Quickly retrieve account-wide metadata and authorized access to maintain control.
- **Unsubscribe Handling** — Process unsubscriptions through natural language to respect audience preferences automatically.

### How it works

1. Subscribe to this server
2. Enter your Kit API Key and API Secret
3. Start automating your creator marketing through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Professional Creators** — monitor subscriber growth and manage tags straight from your workflow.
- **Digital Marketers** — verify if subscribers are correctly entering sequences and receiving tags from lead magnets.
- **Community Managers** — perform rapid audience audits and update member profiles without manual dashboard logins.
- **Operations Leads** — automate audience querying to orchestrate cross-functional creator teams smoothly.


## Available Tools (12)
- **get_subscriber**: Get details for a specific subscriber
- **list_forms**: List all Kit forms
- **list_sequences**: List all Kit email sequences
- **list_subscribers**: List Kit subscribers
- **list_tags**: List all Kit tags
- **remove_tag_from_subscriber**: Remove a tag from a subscriber
- **subscribe_to_form**: Subscribe an email to a form
- **tag_subscriber**: Add a tag to a subscriber
- **unsubscribe_subscriber**: Unsubscribe a subscriber
- **update_subscriber**: Update a Kit subscriber
- **create_tag**: Create a new tag
- **get_account**: Get Kit account details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kit (ConvertKit)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my tags in Kit."

**🤖 AI Agent:**
> I've retrieved your tags. You have 8 active tags, including 'VIP', 'Newsletter', and 'Event-2024'. Which tag would you like to explore further?

---

**👤 You:**
> "Subscribe 'user@example.com' to my main newsletter form."

**🤖 AI Agent:**
> Processing the subscription... 'user@example.com' has been successfully added to your newsletter form. I've also confirmed their profile is active.

---

**👤 You:**
> "Get details for subscriber ID 98765."

**🤖 AI Agent:**
> I've fetched the profile for ID 98765. The subscriber is 'Marcus R.', currently active and associated with 3 tags. Would you like to see their custom fields?


## ❓ FAQ

**Q: Where do I find my Kit API Key and Secret?**
Go to your Kit account settings, navigate to the **Advanced** tab, and you will find both your API Key and API Secret there.

**Q: Can I automatically tag new subscribers via the agent?**
Yes. Use the `tag_subscriber` tool by providing the Tag ID and the subscriber's email. Your agent will confirm the association instantly.

**Q: Is it possible to see which email sequences are active?**
Yes. The `list_sequences` tool retrieves all your email sequences, allowing your agent to audit their status and subscriber counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kit-convertkit-alternative](https://vinkius.com/mcp/kit-convertkit-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `kit-convertkit-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kit (ConvertKit)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kit-convertkit-alternative": {
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
