# Showpad MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/showpad)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to radically infiltrate your Showpad enablement platform. Search sales collateral, fetch user profiles, track channels, and extract asset metadata.

## Description
Grant your AI agent (like Claude or Cursor) absolute administrative observability over your Showpad sales enablement environment. The **Showpad MCP** equips your LLM to act as a fully autonomous vault auditor. Forget manually opening platform channels and endless folders—now you can interrogate asset libraries, audit user hierarchies, and extract direct sales collateral exclusively via natural conversational prompts interacting deeply with your dedicated API.

### What you can do

- **Massive Collateral Infiltration** — Rip through your organizational asset vault via `list_assets` and `search_assets`. Found the brochure you need? Drill down violently with `get_asset_details` to extract all underlying metadata
- **User & Division Surveillance** — Audit seller hierarchies invoking `list_users` and pull their raw profiles via `get_user_details`. Scope out overarching structures using `list_divisions` to forecast alignment without opening a single dashboard
- **Taxonomy & Channel Cartography** — Interrogate the categorization mechanics applying `list_tags` and map the publishing pipelines by extracting `list_channels`

### How it works

1. Anchor this core interface directly within your native MCP agent framework natively
2. Safely entrench your `SHOWPAD_ACCESS_TOKEN` and `SHOWPAD_SUBDOMAIN` matrix inside the workspace to lock down security boundaries
3. Engage your agent pragmatically: "Search all assets tagged with 'Q3 Launch' and check which division they belong to based on their publisher!"


## Available Tools (8)
- **list_users**: Lists all Showpad users
- **get_user_details**: Retrieves details for a specific user
- **list_divisions**: Lists all organizational divisions
- **list_tags**: Lists all tags used for content classification
- **list_assets**: Returns asset IDs and metadata.

Lists all content assets in Showpad
- **get_asset_details**: Retrieves details for a specific asset
- **search_assets**: Searches for assets by keyword
- **list_channels**: Lists all content channels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Showpad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all resources mentioning 'Product Roadmap' and fetch details on the first one."

**🤖 AI Agent:**
> Executing `search_assets` robustly with query 'Product Roadmap'. Unearthed 4 collateral objects. Sequentially executing `get_asset_details` passively on asset 0cd3f-9... Discovered a 12-page presentation tagged aggressively with internal permissions and managed exclusively under the executive division structure heavily.

---

**👤 You:**
> "List users systematically and check to see how many sit under the 'EMEA Enterprise' division."

**🤖 AI Agent:**
> Initiating deep retrieval invoking `list_users` sequentially cross-referenced strictly traversing boundaries mapped via `list_divisions`. Count indicates approximately 34 individual internal representations actively bound beneath the EMEA Enterprise namespace structural label directly without active restrictions explicitly.

---

**👤 You:**
> "List content channels available actively within my organization boundaries."

**🤖 AI Agent:**
> Initiating raw matrix extraction accessing `list_channels` passively exclusively. Extracted 5 heavily prominent publishing funnels spanning structurally from direct marketing hubs, explicitly targeted external reseller networks, and localized sales hubs uniformly distributing collateral without disruption natively efficiently systematically.


## ❓ FAQ

**Q: Can the integration alter, upload, or delete assets directly?**
By structural design, this module is strictly bound as an observational and auditing lens. Operations such as `search_assets`, `list_channels`, and `get_user_details` parse and extract massive contextual architecture. It explicitly omits write mechanisms preventing your autonomous agent from accidentally sabotaging or permanently deleting valid organizational sales assets.

**Q: Why construct this manually over downloading platform-provided CSVs?**
Static extracts decay instantly upon creation implicitly blinding observers. The MCP parameter configuration hands your prompt active, unadulterated runtime authority to scan real-time hierarchies, pull active tags, and interrogate asset metadata aggressively instantly. It creates dynamic query dialogue natively routing structural truths.

**Q: Are specific domain aliases required for the query logic?**
Yes exactly. Because Showpad physically partitions tenants distinctively, providing and solidifying the `SHOWPAD_SUBDOMAIN` variable string guarantees the underlying path execution targets explicitly your organizational API backbone (`your-subdomain.showpad.biz`) ruthlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/showpad](https://vinkius.com/mcp/showpad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Showpad** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `showpad` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Showpad** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "showpad": {
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
