# Bynder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bynder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Empower your asset strategy via Bynder — list media banks, filter collections, and retrieve digital download links with your AI agent.

## Description
Connect your **Bynder** Digital Asset Management platform to any AI agent and organize your enterprise brand resources through natural conversation.

### What you can do

- **Deep Media Exploration** — Query massive media banks fetching specific branded visuals filtering by keyword or raw native asset IDs
- **Collection Management** — Navigate explicit user collections inspecting curated groups of files rapidly
- **Instant Retrievals** — Directly output public and secure downloading URLs for immediate use without digging in browser galleries
- **Taxonomy Editing** — Inspect and patch internal asset metadata mapping schema attributes seamlessly

### How it works

1. Subscribe to this server
2. Enter your Permanent Bynder token and integration domain base
3. Start fetching and sharing creative data directly through Claude, Cursor, or any MCP-compatible smart interface

No manual searches inside cluttered visual portals. Your AI agent digs up the exact brand elements on command.

### Who is this for?

- **Marketing Specialists** — bypass platform navigation finding recent campaign launch visuals directly in the chat window
- **Graphic Agencies** — confirm a master brand asset's internal metadata correctly mirrors current external directives swiftly
- **Automated Workflows** — empower scripts mapping vast amounts of raw image IDs checking against current catalog taxonomies


## Available Tools
- **list_collections**: List all media collections
- **list_smart_filters**: List configured smart filters
- **list_tags**: List all asset tags
- **list_users**: List all portal users
- **patch_asset_metadata**: Update metadata for an asset
- **get_asset**: Get details of a specific asset
- **get_collection**: Get details of a specific collection
- **get_download_link**: Get a direct download URL for an asset
- **get_account_usage**: Retrieve account storage and traffic usage
- **list_assets**: List digital assets from the DAM


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bynder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List standard assets in our repository matching the word 'logomark'."

**🤖 AI Agent:**
> I queried your DAM structure. You currently maintain 4 specific image files labeled 'logomark'. Options range from PNG cutouts to full AI vectors. Would you like me to generate precise download links for any of them?

---

**👤 You:**
> "What exact metadata properties exist right now for asset ID ABC-1234?"

**🤖 AI Agent:**
> Asset 'ABC-1234' is mapped to the 'Summer Promo' taxonomy branch natively. The copyright field details 'External Studio Use Only', while color tags span red and yellow variants. Shall I patch those internal bounds?

---

**👤 You:**
> "Generate a solid download URL for asset 'DEF-5522'."

**🤖 AI Agent:**
> I submitted a retrieval to the core platform. Your robust download pipeline is open: [Download Asset DEF-5522]. Let me know if you need to extract alternative media sizes.


## ❓ FAQ

**Q: Can the AI generate a native download link for a large video asset?**
Yes. Once the agent identifies the particular asset ID from a list command, you can request a direct download link. It invokes the platform's specific get_download_link route avoiding manual gallery searching.

**Q: Will it discover collections created by other members of my team?**
Yes. The list_user_collections endpoint enables cross-inspections returning aggregated folders that exist on Bynder infrastructure letting you know precisely which assets were curated by designers.

**Q: Does the integration allow altering taxonomy and metadata fields?**
Yes. Using the patch_asset_metadata functionality, you can ask your AI to append missing SEO properties natively directly inside your Bynder catalog records.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bynder](https://vinkius.com/mcp/bynder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bynder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bynder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bynder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bynder": {
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
