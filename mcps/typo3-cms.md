# TYPO3 CMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typo3-cms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [content-management](../categories/content-management.md)

Automate content management via TYPO3 CMS — retrieve page structures, create Extbase entities, update fields, and audit configurations seamlessly.

## Description
Connect your **TYPO3 CMS** backend to any AI agent and take full enterprise control over global content operations mapping, backend Extbase entity tracking, and site hierarchy inspection.

### What you can do

- **Page Structuring** — Query an entire hierarchical navigation mesh grabbing exact IDs to isolate sub-folder content via the API organically
- **Extbase Data Entry** — Perform high-volume CRUD patterns by instantiating new raw custom JSON configurations mapped flawlessly onto defined backend tables
- **Global Constant Audit** — Ping initial states tracking configurations directly looking through the system Constants to bypass heavy configuration modules
- **Direct Node Removal** — Programmatically obliterate or forcefully mutate an outdated content record via native endpoint requests securely

### How it works

1. Subscribe manually to this core server context
2. Introduce your REST API's external TYPO_BASE_URL accompanied by your TYPO3 Authorization Bearer
3. Engage directly your preferred AI model on cursor ensuring full architectural discovery limits

Drop PHP dependency injection debugging just to update a node value. You describe the change, the agent fires the protocol payload over REST effortlessly.

### Who is this for?

- **CMS Platform Engineers** — automate routine node setups requesting tree structures from LLMs avoiding constant IDE window switches 
- **Digital Editors** — prompt the agent to bulk-view lists of localized backend items skipping complicated table drill-downs natively 
- **Web Architects** — confirm internal route stability extracting pure JSON rendering on top-priority pages to find syntax breaks


## Available Tools (10)
- **create_cms_entity**: Provide the entity name and data as a JSON object.

Creates a new TYPO3 Extbase entity or content element
- **delete_cms_entity**: This action is irreversible.

Permanently deletes a TYPO3 record
- **get_initial_boot**: Retrieves global configuration and root page schema from TYPO3
- **get_navigation_tree**: Retrieves the hierarchical navigation menu starting from a page
- **get_rendered_page**: Provide a numeric ID or canonical path.

Retrieves a structured representation of a rendered TYPO3 page
- **get_single_record**: Retrieves a single TYPO3 record by ID
- **list_backend_records**: Provide the entity name and optional query parameters.

Lists records for a specific TYPO3 entity or route
- **list_typoscript_globals**: Lists global TypoScript settings and constants
- **ping_rest_api**: Verifies connectivity to the TYPO3 REST API
- **update_cms_entity**: Provide entity name, record ID, and JSON updates.

Updates fields of an existing TYPO3 record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TYPO3 CMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check the current initial boot configuration of our TYPO3 project?"

**🤖 AI Agent:**
> Initial boot grabbed: System sits at version v12.4 LTS. Found core default routing mappings in context alongside basic site language configurations spanning EN and DE arrays.

---

**👤 You:**
> "List standard backend records available on the custom entity table 'tx_myext_domain_model_item'."

**🤖 AI Agent:**
> Under 'tx_myext_domain_model_item', 8 distinct entries were listed. Records IDs #23 and #40 seem recently added. Would you like me to deeply inspect the payload geometry of element #23?

---

**👤 You:**
> "Permanently delete the CMS entity under ID 644 on 'pages'."

**🤖 AI Agent:**
> Action confirmed. Record ID 644 inside the 'pages' entity has been wiped through a deletion mutation payload. It has been successfully removed from visibility.


## ❓ FAQ

**Q: Can it retrieve both the navigation tree and single rendered pages autonomously?**
Yes. Command the LLM to 'get_navigation_tree' from ID 1, revealing the layout. Finding a curious page, you can instruct it to 'get_rendered_page' supplying its new ID to dissect content instantly.

**Q: How does the assistant handle adding complex backend module data like Extbase records?**
Using the 'create_cms_entity' endpoint tool, you just tell the AI the physical target database component and pass your JSON. TYPO3 resolves it server-side identically as if inserted from the admin view.

**Q: Is there a fast way to verify if my TYPO3 API authentication block is working?**
Run a request with the 'ping_rest_api' capability. It triggers a lightweight, zero-payload call directly returning successful metadata from your host validating you have unbridled authorization natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typo3-cms](https://vinkius.com/mcp/typo3-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TYPO3 CMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `typo3-cms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TYPO3 CMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "typo3-cms": {
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
