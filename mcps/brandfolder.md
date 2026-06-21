# Brandfolder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brandfolder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Automate digital asset management with Brandfolder — search assets, check organizations, and browse collections from any AI agent.

## Description
Connect your **Brandfolder** environment to any AI agent and organize your entire digital asset repository organically through natural conversation.

### What you can do

- **Asset Discovery** — List, retrieve, and filter high-resolution brand assets across organizations
- **Collections** — Map active collections managing internal team sharing structures instantly
- **Organizations** — Check specific Brandfolder organization topologies

### How it works

1. Install this MCP Server
2. Authorize with your personal Brandfolder API Token
3. Leverage advanced search logic directly in Claude, Cursor, or any MCP-compatible environment

Eliminate messy folder trees and manual downloads. Let the AI serve links to the latest version of your branding files, precisely when you ask.

### Who is this for?

- **Marketing teams** — locate exact campaign logos and hero images without touching the user interface
- **Graphic Designers** — pull precise CDN-backed vectors into your workflow context instantly
- **Sales enablement** — serve pitch decks directly to the chat session requesting recent templates 
- **Software engineers** — verify asset CDN URLs validating collection permissions programmatic rules


## Available Tools (10)
- **create_cms_asset**: Inject a new digital asset (image, document, etc.) into a Brandfolder
- **wipe_media_asset**: Permanently delete a digital asset from Brandfolder
- **get_asset_details**: ` logic.

Retrieve extensive metadata for a specific digital asset
- **get_brandfolder_assets**: Search and retrieve digital assets within a specific Brandfolder
- **get_collection_assets**: Search and retrieve digital assets within a specific Collection
- **list_asset_attachments**: Retrieve the actual CDN delivery URLs and attachments stored behind an Asset
- **list_asset_tags**: Retrieve the exact structural matching verifying Tags attached to an asset
- **list_global_brandfolders**: Retrieve all Brandfolders (logical asset containers) in the workspace
- **list_platform_organizations**: Retrieve all top-level tenant organizations accessible by your API key
- **patch_cms_asset**: Update metadata attributes of an existing digital asset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brandfolder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the collections available in my main Brandfolder organization."

**🤖 AI Agent:**
> I've fetched 3 active collections under your organization. There's a 'Q3 Marketing Assets' and a 'Social Media Vectors' collection. Should I list the assets from any of them?

---

**👤 You:**
> "Search my assets for any PDF related to standard onboarding manuals."

**🤖 AI Agent:**
> I found an asset called 'Operations-Manual.pdf'. Here is the direct CDN download link provided natively over Brandfolder routing.

---

**👤 You:**
> "Double check my organization ID tied to the user profile."

**🤖 AI Agent:**
> Your active Brandfolder personal key maps to Organization ID xyz-123. The namespace is designated 'Global Enterprise Tier'.


## ❓ FAQ

**Q: Can it search for specific file types like PDFs or PNGs?**
Absolutely. Through the `list_assets` capability, the AI can parse queries finding exactly what format you need among your organization's total index.

**Q: Can the AI return download links for an asset?**
Yes. Upon locating an asset, you can ask the AI to provide the CDN URL representing the final high-resolution source file directly in the chat.

**Q: Is my API token secure during the requests?**
Yes. The API Token is encrypted at rest and dynamically injected strictly at the runtime limit inside a secure sandbox container. Keys are never exposed within chat interactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brandfolder](https://vinkius.com/mcp/brandfolder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brandfolder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brandfolder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brandfolder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brandfolder": {
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
