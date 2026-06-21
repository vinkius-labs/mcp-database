# Heyzine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heyzine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Transform PDFs into interactive flipbooks with page-turn animations, embedded media, and sharing analytics for digital publishing.

## Description
Connect your **Heyzine** account to any AI agent and take full control of your digital publishing and flipbook distribution through natural conversation.

### What you can do

- **Instant Conversion** — Seamlessly convert PDF, DOCX, or PPTX links into professional, interactive digital flipbooks programmatically
- **Design Customization** — Update flipbook design settings, titles, and backgrounds directly through natural language instructions
- **Digital Bookshelves** — Organize and manage collections of flipbooks using virtual bookshelves to streamline your digital library
- **Access Control** — Manage download permissions and privacy settings for each flipbook to ensure secure distribution
- **Usage Monitoring** — Track your account subscription limits and API health status directly through your agent

### How it works

1. Subscribe to this server
2. Enter your Heyzine API Key (Bearer token) from your dashboard
3. Start creating and managing interactive publications from Claude, Cursor, or any MCP client

No more manual uploads or configuration through complex web editors. Your AI acts as your dedicated digital publishing assistant.

### Who is this for?

- **Digital Publishers** — quickly convert and distribute magazines, catalogs, and brochures via automated workflows
- **Marketing Teams** — create branded digital flipbooks for lead generation and high-impact sales collateral
- **Content Managers** — organize large digital libraries using bookshelves without leaving your workspace


## Available Tools
- **add_flipbook_to_bookshelf**: Add a flipbook to a collection
- **check_api_status**: Verify Heyzine API status
- **convert_pdf_to_flipbook**: Returns the flipbook URL and ID.

Convert a PDF URL to an interactive flipbook
- **delete_flipbook**: Delete a flipbook
- **get_account_info**: Get Heyzine account information
- **get_bookshelf_details**: Get details for a bookshelf
- **get_flipbook_details**: Get details for a specific flipbook
- **list_all_flipbooks**: List all flipbooks in the account
- **list_bookshelf_flipbooks**: List flipbooks in a bookshelf
- **list_available_templates**: List flipbook templates
- **remove_flipbook_from_bookshelf**: Remove a flipbook from a collection
- **update_flipbook_design**: Update flipbook design or settings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heyzine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert this PDF to a flipbook: https://example.com/catalog.pdf"

**🤖 AI Agent:**
> Conversion started! I've successfully triggered the Heyzine engine for your PDF. Your new interactive flipbook will be available shortly at: https://heyzine.com/flip-book/ig_123. Would you like to update its title now?

---

**👤 You:**
> "List all flipbooks in my 'Spring 2026' bookshelf."

**🤖 AI Agent:**
> I've retrieved 5 flipbooks from the 'Spring 2026' collection. Notable titles include 'Q1 Product Guide' and 'Regional Brochure'. Which one should we manage or share?

---

**👤 You:**
> "Update the title of flipbook ID 'ig_123' to 'Summer Promo'."

**🤖 AI Agent:**
> Done! I've updated the title for flipbook 'ig_123' to 'Summer Promo' in your Heyzine account. The changes are now live on the public link.


## ❓ FAQ

**Q: How do I find my Heyzine API key?**
Log in to your Heyzine account and navigate to the **API** section in your dashboard to generate or copy your unique Bearer token.

**Q: What file formats can be converted into flipbooks?**
Heyzine currently supports PDF, DOCX, and PPTX files for seamless conversion into professional interactive digital publications.

**Q: Can I manage bookshelves through this AI integration?**
Yes! Use the `list_bookshelves` and `add_to_bookshelf` tools to organize your flipbooks into collections for easier access and distribution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heyzine](https://vinkius.com/mcp/heyzine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heyzine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `heyzine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heyzine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heyzine": {
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
