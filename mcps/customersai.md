# Customers.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/customersai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identify anonymous website visitors by name and turn them into leads with AI-powered visitor identification and outreach automation.

## Description
Connect your **Customers.ai** (formerly MobileMonkey) account to any AI agent and take full control of your automated messaging and B2B identity resolution workflows through natural conversation.

### What you can do

- **Contact Orchestration** — List and search your contact database programmatically, retrieving detailed metadata from identity resolution pipelines like X-Ray Pixel
- **Multichannel Engagement** — Programmatically dispatch plain text or high-fidelity JSON messages (including galleries and buttons) across SMS and chat channels
- **Identity Resolution Intelligence** — Access leads identified through website visits to prioritize high-intent prospects and maintain a high-fidelity sales pipeline
- **Attribute Management** — Programmatically update custom contact attributes and manage audience segments through dynamic tagging directly from your agent
- **Lead Discovery** — Find contacts by email, phone, or external identifiers to perfectly coordinate your multichannel outreach and follow-ups

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Customers.ai dashboard (Settings > API)
3. Start managing your lead engagement from Claude, Cursor, or any MCP client

No more manual scrubbing through identified visitor logs. Your AI acts as your dedicated growth engineer and messaging coordinator.

### Who is this for?

- **Marketing Operations** — instantly retrieve lists of identified website visitors and trigger nurturing sequences using natural language commands
- **Sales Development (SDRs)** — automate the personalized outreach to high-intent leads without leaving your workspace
- **Growth Marketers** — integrate identity resolution data and automated messaging into custom performance workflows through simple AI queries


## Available Tools
- **add_tag_to_contact**: Add a tag to a contact
- **get_contact**: Get contact profile details
- **list_xray_leads**: List identified website visitors
- **remove_tag_from_contact**: Remove a tag from a contact
- **search_contacts**: Search for contacts in Customers.ai
- **send_rich_message**: Send a structured JSON message
- **send_text_message**: Send a text message to a contact
- **update_contact_attributes**: Update attributes for a contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customers.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 leads identified via X-Ray Pixel."

**🤖 AI Agent:**
> I've retrieved your recent X-Ray leads. I found 5 identified visitors, including profiles for managers at 'Acme Corp' and 'Global Tech'. Would you like the detailed attributes for any of them?

---

**👤 You:**
> "Find the contact with email 'jane.doe@example.com'."

**🤖 AI Agent:**
> I've located Jane Doe's profile (ID: 1024). She has 15 custom attributes and is currently tagged as 'Hot Lead'. Shall I send her a follow-up text message?

---

**👤 You:**
> "Add the 'Q2 Campaign' tag to contact ID '1024'."

**🤖 AI Agent:**
> Action complete! Contact 1024 has been successfully tagged with 'Q2 Campaign'. This update can now trigger your automated nurturing sequences. Need help with other tags?


## ❓ FAQ

**Q: How do I find my Customers.ai API Key?**
Log in to your dashboard, navigate to **Settings** > **API**, and generate or copy your unique API Key.

**Q: What is the X-Ray Pixel?**
The X-Ray Pixel is a tool that identifies anonymous website visitors and resolves their identity into actionable lead profiles.

**Q: Can I send rich JSON messages?**
Yes! Use the `send_rich_message` tool and provide a JSON payload containing image URLs, buttons, or gallery structures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/customersai](https://vinkius.com/mcp/customersai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Customers.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `customersai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Customers.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "customersai": {
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
