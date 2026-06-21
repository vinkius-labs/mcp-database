# Cardly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cardly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Send physical greeting cards via Cardly — automate personalized card sends, track orders, and manage contacts directly from any AI agent.

## Description
Connect your **Cardly** account to any AI agent and orchestrate your personalized gifting, customer appreciation, and physical mail workflows through natural conversation.

### What you can do

- **Order Management** — Place real orders for physical greeting cards with custom messages and designs directly from your workspace.
- **Design Oversight** — Browse your custom artwork library and retrieve detailed metadata for individual designs.
- **Order Preview** — Generate a watermarked PDF preview of your card to verify content and layout before sending.
- **Contact Coordination** — Access and manage your contact lists and add new recipients to your address book.
- **Global Shipping** — Send cards to recipients in the US, Australia, UK, and worldwide with automatic address validation.
- **API Verification** — Verify your connection and API key status instantly using the echo tool.

### How it works

1. Subscribe to this server
2. Enter your Cardly API Key (Test or Live)
3. Start sending physical cards from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing & HR Teams** — quickly send birthday or anniversary cards to employees and clients without manual portal work.
- **Sales Professionals** — automate follow-up thank you cards straight from their workflow tools.
- **Business Owners** — monitor gifting campaigns and verify artwork using natural language.


## Available Tools
- **add_contact_to_list**: Add a new contact to a specific list
- **find_contact**: Search for a contact in a list by email
- **get_account_info**: Retrieve core account information
- **get_artwork_details**: Get details of a specific piece of artwork
- **list_card_artwork**: List available greeting card designs/artwork
- **list_contact_lists**: List all contact lists in your account
- **place_greeting_card_order**: Place a real order for a physical greeting card
- **preview_greeting_card**: Generate a preview of a greeting card without placing a real order
- **verify_api_connection**: Verify connectivity and API key validity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cardly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the available greeting card designs in my account."

**🤖 AI Agent:**
> I've retrieved your artwork. You have several designs available, including 'Birthday Balloon' (ID: art_1) and 'Thank You Floral' (ID: art_2).

---

**👤 You:**
> "Preview a card with artwork art_1 and message 'Happy Birthday John!'."

**🤖 AI Agent:**
> Preview generated! You can view the card layout here: [Link]. It looks great! Would you like to place the actual order now?

---

**👤 You:**
> "Send a thank you card to Jane Smith in Australia."

**🤖 AI Agent:**
> I've initiated the order for Jane Smith. I'll need her full address in Australia and your preferred artwork ID to finalize the send.


## ❓ FAQ

**Q: Can I see a preview of the card before sending it?**
Yes! Use the `preview_greeting_card` tool with your message and artwork ID. Your agent will return a preview URL (usually a PDF) so you can verify everything looks perfect.

**Q: How do I find the correct artwork ID for a design?**
Simply ask the agent to `list_card_artwork`. It will retrieve all the available designs from your account, including their titles and unique IDs or slugs.

**Q: Does the integration support international shipping?**
Yes. When using the `place_greeting_card_order` action, you can specify the country code (e.g., 'UK', 'AU', 'US'). Cardly handles the local printing and postage automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cardly](https://vinkius.com/mcp/cardly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cardly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cardly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cardly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cardly": {
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
