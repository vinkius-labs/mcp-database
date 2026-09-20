# Microsoft SharePoint MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/microsoft-sharepoint)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Explore SharePoint sites and read, search, create, and update the rows inside their lists — structured site data for any AI agent.

## Description
Connect your **SharePoint sites** to any AI agent through the Microsoft Graph API. SharePoint stores a huge amount of business data in lists — projects, requests, records, inventories — and this server lets an agent read and maintain that data without a browser.

### What you can do

- **Site Discovery** — List the sites the user can access and resolve a site by hostname, subsite path, or GUID
- **List Exploration** — See which lists a site contains, then read the rows with their field values
- **Row Search** — Search across all lists and documents of a site with one query
- **Row Creation & Updates** — Add new rows and change fields on existing rows using the exact column names

### How it works

1. Register an Entra application with Microsoft Graph delegated permissions (Sites.Read, Sites.ReadWrite, Sites.Manage)
2. Subscribe to this server and connect through OAuth 2.0
3. Point your agent at a site address and ask it to read or maintain the data — rows are paged so large lists never flood the context

### Who is this for?

- **Operations Teams** — keep request and task lists current, mark items progressed, and surface what changed without opening the portal
- **Analysts & Assistants** — pull structured site data for reporting, or find a specific record across dozens of lists


## Available Tools (8)
- **create_list_item**: The fields parameter is a JSON object mapping column internal names to values, for example {"Title":"Onboarding","Status":"Open"} — use list_lists and an existing item to learn the exact column names first. Lookup and person columns need special value shapes; when unsure, read a sample item and mirror its shape. The new item ID is returned for later updates.

Create a new row in a SharePoint list
- **list_sites**: Use for site discovery when the user is unsure which site holds the data. Page with top and skip when the tenant has many sites.

List the SharePoint sites the connected user has access to
- **get_site**: Use when the user names a SharePoint site by its hostname like contoso.sharepoint.com, by a sub-site path, or by its GUID. This is the starting point for any list work — it confirms the site resolves before drilling into its lists.

Get details for a SharePoint site
- **list_lists**: Use when the user wants to explore a site or to find the list that holds a piece of data before reading it. The site parameter is the same address form get_site accepts.

List the lists inside a SharePoint site
- **update_list_item**: Use to fix or progress a row found via list or search results. The item ID comes from those results, and column names follow the same shape as create_list_item fields.

Update fields on an existing SharePoint list item
- **get_list_item**: Use when a specific row was located via list_list_items or search_site_items and the user wants everything stored on that row. The item ID comes from those list/search results.

Read one SharePoint list item with all its fields
- **list_list_items**: Use when the user wants rows from a known list. The list parameter accepts the list display name or its ID. Add a CML filter expression to narrow rows, and page with top and skip for large lists.

Read items from a SharePoint list
- **search_site_items**: Use when the user describes data they cannot locate by walking lists. This is site-wide, not per-list, so it can be slower — cap results with top.

Search across the lists and documents of a SharePoint site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microsoft SharePoint** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the lists on the company site and show the 5 most recent items in the Tasks list."

**🤖 AI Agent:**
> The site has 12 lists: Tasks, Projects, Requests, Documents, Assets… In Tasks, the 5 most recently modified items are: #48 'Migrate invoice import to v2' (modified 2h ago, Status: Open), #45 'Update vendor contract' (1d ago, Done), #44 'Security questionnaire' (2d ago, In progress), #42 'Quarterly review deck' (3d ago, Open), #41 'Clean up stale access' (4d ago, Open).

---

**👤 You:**
> "Find everything mentioning 'Q3 budget' on the finance site."

**🤖 AI Agent:**
> Searched the finance site across all lists and documents. Found 3 rows in the Budgets list: #12 'Q3 budget plan v4' (updated 5 days ago, Owner: Dana), #9 'Q3 budget approvals' (updated 12 days ago, Status: In review), and a document 'Q3-budget-assumptions.xlsx' in the Shared Documents library. Want me to open the approvals row in full?

---

**👤 You:**
> "Mark item #44 in the Tasks list as Done and set the Status and CompletedBy fields."

**🤖 AI Agent:**
> I read item #44 to mirror its field shapes, then updated it: Status='Done', CompletedBy='Dana R.'. The row now shows Status Done, last modified just now. No other fields changed.


## ❓ FAQ

**Q: Which Microsoft Graph permissions does the app need?**
Delegated permissions: Sites.Read, Sites.ReadWrite and Sites.Manage, plus openid/profile/offline_access. You consent once at the OAuth step; the agent then works only inside the sites your account can access.

**Q: What address format does the site parameter accept?**
Three forms: the site hostname (contoso.sharepoint.com), a subsite path (contoso.sharepoint.com/sites/finance), or the site GUID returned by list_sites. Protocol and trailing slashes are stripped automatically.

**Q: Can the agent create and update rows?**
Yes — create_list_item adds a row and update_list_item changes fields on one row. Both take a JSON object keyed by the column's internal name; the agent should read a sample row first (get_list_item) to learn the exact shapes of lookup and person columns. Lookups use {Value}, persons {Value}/{DisplayName}, so mirroring an existing row's shape avoids errors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/microsoft-sharepoint](https://vinkius.com/en/ai-agent-connect/microsoft-sharepoint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microsoft SharePoint** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `microsoft-sharepoint` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microsoft SharePoint** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microsoft-sharepoint": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
