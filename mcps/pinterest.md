# Pinterest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pinterest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Pinterest profile — audit boards and pins via AI.

## Description
Empower your AI agent to orchestrate your entire visual discovery ecosystem on **Pinterest**, the platform for inspiration and creative ideas. By connecting Pinterest to your agent, you transform board management and pinning into a natural conversation. Your agent can instantly list your boards, audit your pin library, and create new content without you ever touching a dashboard. Whether you are a content curator or a brand marketer, your agent acts as a real-time creative assistant, ensuring your visual catalog is always organized and inspiration is captured.

### What you can do

- **Board Auditing** — List all boards in your account and retrieve detailed metadata, including descriptions and IDs.
- **Pin Management** — Create new pins with titles, descriptions, and destination links directly through natural language.
- **Library Oversight** — Query pins for any specific board to maintain a clear view of your visual categorization.
- **Governance Controls** — Autonomously delete pins or boards that no longer fit your aesthetic or strategy.
- **Account Intelligence** — Retrieve detailed user account information to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your Pinterest Access Token
3. Start managing your visual assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Visual Creators** — publish new pins and manage boards straight from your design workflow.
- **Content Marketers** — verify if new products have been correctly pinned and linked for maximum traffic.
- **Curators** — perform rapid audits of visual libraries and organize content into new boards without manual logins.
- **Operations Leads** — automate visual data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **create_board**: Create a new board
- **create_pin**: Create a new pin
- **delete_board**: Delete a specific board
- **delete_pin**: Delete a specific pin
- **get_board**: Get details for a specific board
- **get_me**: Get authenticated Pinterest user account info
- **list_boards**: List all boards for the authenticated user
- **list_pins**: Optional: filter by board ID.

List pins. Optional: filter by board ID
- **get_pin**: Get details for a specific pin


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinterest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Pinterest boards."

**🤖 AI Agent:**
> I've retrieved your boards. You have 5 active boards, including 'Home Decor' and 'Travel Goals'. Which one would you like to audit for pins?

---

**👤 You:**
> "Create a new pin in 'Travel Goals' titled 'Summer in Italy'."

**🤖 AI Agent:**
> Pin created! 'Summer in Italy' is now live on your 'Travel Goals' board. I've recorded the pin ID for your audit.

---

**👤 You:**
> "Show me the pins in my 'Home Decor' board."

**🤖 AI Agent:**
> I've found 12 pins in that board. Notable entries include 'Modern Kitchen' and 'Minimalist Living Room'. Would you like the links for any of them?


## ❓ FAQ

**Q: How do I find my Pinterest Access Token?**
Go to the [**Pinterest App Console**](https://developers.pinterest.com/apps/), create an App, and generate a token with the necessary scopes (boards:read, pins:read, pins:write, etc.). Copy and paste it below.

**Q: Can the agent create new boards?**
Yes. Use the `create_board` tool providing a name and optional description. Your agent will create the board and return its unique ID instantly.

**Q: Is it possible to pin from an image URL?**
Yes. The `create_pin` tool requires a `media_source_url`. Your agent will use this URL to generate the pin on your target board.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pinterest](https://vinkius.com/mcp/pinterest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pinterest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pinterest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pinterest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pinterest": {
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
