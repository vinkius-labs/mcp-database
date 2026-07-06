# WeChat Official Accounts / 微信公众号 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wechat-official-accounts)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's dominant social messaging platform — manage subscribers, broadcast messages, and menus via AI.

## Description
Empower your AI agent to orchestrate your social ecosystem and subscriber engagement with **WeChat Official Accounts** (微信公众号), the dominant communication platform in China. By connecting WeChat to your agent, you transform complex user management, template-based broadcasting, and menu orchestration into a natural conversation. Your agent can instantly retrieve subscriber profiles, send direct customer service messages, publish custom navigation menus, and audit permanent materials without you ever needing to navigate the comprehensive WeChat MP portal. Whether you are automating customer support or coordinating a content marketing blast, your agent acts as a real-time social operations assistant, providing accurate and reliable results from a single, unified source.

### What you can do

- **Subscriber Orchestration** — Retrieve detailed user profiles, list subscribers, and manage user segments using OpenIDs.
- **Messaging Control** — Send direct custom text messages or structured template alerts to your followers.
- **Menu Management** — Create, retrieve, and delete custom navigation menus for your official account interface.
- **Material Auditing** — Browse permanent media assets and news articles stored in your material library.
- **Operational Insights** — Monitor material counts and account connectivity status to ensure system-wide reliability.

### How it works

1. Subscribe to this server
2. Enter your WeChat AppID and AppSecret
3. Start managing your social ecosystem through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Social Media Managers** — manage menus and audit content libraries through natural language queries.
- **Customer Support Teams** — send direct messages and verify user identities directly from your AI-powered workspace.
- **Developers** — integrate professional WeChat MP capabilities into your AI-driven daily routines.
- **WeChat Power Users** — integrate your existing social workflows into your AI-driven daily routines.


## Available Tools (10)
- **delete_custom_menu**: Delete custom menu
- **get_account_status**: Check account connectivity
- **get_custom_menu**: Retrieve custom menu
- **get_material_count**: Get material totals
- **get_user_info**: Get user profile information
- **list_articles**: List permanent articles
- **list_users**: List subscribers
- **send_custom_text**: Send custom text message
- **send_template_message**: Send template message
- **create_custom_menu**: Create custom menu


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WeChat Official Accounts / 微信公众号** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the profile for user with OpenID 'o88210934...'."

**🤖 AI Agent:**
> I've retrieved the user profile. The user is nicknamed 'Zhang San', based in Shanghai, China. They are a male subscriber. Would you like to send them a direct message or check their interaction history?

---

**👤 You:**
> "Show me the current custom menu for our account."

**🤖 AI Agent:**
> I've retrieved your current menu configuration. You have 3 main buttons: 'Products', 'Support', and 'About Us'. Each button leads to specific sub-menus or external links. Would you like to modify any of these entries?

---

**👤 You:**
> "Send a template message to 'o992018...' using template ID 'TEMP_8821'."

**🤖 AI Agent:**
> I've sent the template message to the specified user. The transaction ID is `88210934`. The user will receive the structured notification on their WeChat app immediately. Should I check the delivery status?


## ❓ FAQ

**Q: How do I find my WeChat AppID and Secret?**
Log in to the [WeChat Official Accounts Platform](https://mp.weixin.qq.com/), navigate to [Settings] -> [Development] -> [Basic Configuration] to find your unique AppID and generate your AppSecret.

**Q: What is an OpenID?**
An OpenID is a unique identifier for a specific user relative to your Official Account. It is required for most user-specific operations like sending messages or retrieving profiles.

**Q: Can I send messages to anyone?**
Custom messages can only be sent to users who have interacted with your account in the last 48 hours. Template messages can be sent at any time but must follow specific structured formats and use-cases defined by WeChat.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wechat-official-accounts](https://vinkius.com/mcp/wechat-official-accounts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WeChat Official Accounts / 微信公众号** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wechat-official-accounts` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WeChat Official Accounts / 微信公众号** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wechat-official-accounts": {
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
