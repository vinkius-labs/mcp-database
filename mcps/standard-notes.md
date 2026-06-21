# Standard Notes MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/standard-notes)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Connect your AI to the Standard Notes encrypted ecosystem. Sync items natively, modify protected notes, and manage tags seamlessly.

## Description
Seamlessly integrate your highly secure **Standard Notes** environments directly into your local AI workflows. Eliminate the friction of manually transferring encrypted data or research logs into your conversational interface. Empower your assistant to execute encrypted synchronizations, draft new secure notes, and systematically organize your knowledge base with precise tag management across your entire architecture.

### What you can do

- **Knowledge Retrieval** — Securely list your encrypted notes via `list_notes` or retrieve specific detailed payloads using the `get_item_details` routine.
- **Automated Drafting** — Command the agent to generate new structural content and save it securely via `create_note`, or surgically update existing drafts through `update_note`.
- **Vault Maintenance** — Maintain a clean workspace by permanently removing deprecated assets via `delete_item`, and keep local context synchronized with the official server using `sync_items`.
- **Taxonomy & Organization** — Streamline categorization by generating new organizational folders with `create_tag`, retrieving current structures with `list_tags`, and associating tags to specific items utilizing `tag_note`.

### How it works

1. Attach the Standard Notes MCP integration securely to your AI terminal.
2. Configure your endpoint URL (Official Cloud or Self-Hosted) along with your valid JWT Access Token.
3. Instruct your AI: "Retrieve the 'Project Alpha' note, update its contents with today's action items, and assign it the 'Priority' tag."

### Who is this for?

- **Privacy-focused Researchers** — Aggregate massive data logs using AI to pull notes, summarize them locally, and append new research securely without compromising client-side architecture.
- **Knowledge Architects & PKM Users** — Orchestrate seamless taxonomy alignments by instructing the AI to methodically analyze and map untagged notes.
- **System Administrators** — Automate the documentation of server incidents or deployment logs directly into a self-hosted encrypted database.


## Available Tools (10)
- **create_note**: Provide plaintext title and text; encryption is handled by the sync layer.

Creates a new encrypted note
- **create_tag**: Creates a new tag
- **delete_item**: This action is irreversible.

Permanently deletes an item (note, tag, or extension) by UUID
- **get_auth_parameters**: Retrieves authentication parameters for an account email
- **get_item_details**: Retrieves a specific item (note, tag, or extension) by UUID
- **list_notes**: Note content remains encrypted until decrypted with user keys.

Lists all encrypted notes
- **list_tags**: Lists all tags defined in the account
- **sync_items**: Use the sync_token from the previous response.

Performs a Standard Notes sync operation
- **tag_note**: Requires both the tag UUID and the note UUID.

Associates a tag with a note
- **update_note**: Updates an existing note by UUID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Standard Notes** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active tags in my vault. Next, read out the title and UUID strings of my notes so I can assign categorizations properly."

**🤖 AI Agent:**
> Securely querying local Standard Notes indexes...

**Tag Taxonomies (`list_tags`)**:
- `Personal Infrastructure` (UUID: a1b2...)
- `Work Configurations` (UUID: c3d4...)
- `Project Research` (UUID: x8z1...)

**Vault Notes Retrieved (`list_notes`)**:
- Title: "Architecture Decisions 2026" [UUID: 99x1...]
- Title: "NGINX Routing Documentation" [UUID: 88z2...]

Please clarify which specific item you would like me to dissect using `get_item_details`.

---

**👤 You:**
> "Write a completely new structured document titled 'Q3 Marketing Directives'. Save it to my records mentioning our emphasis on standardizing B2B outreach."

**🤖 AI Agent:**
> Generating structured output through the `create_note` implementation...

- **Metadata Title**: *Q3 Marketing Directives*
- **Generated Body Content**: *This quarter demands a robust standardization of our B2B pipeline strategies. Client outreach synchronization will be prioritized...*

**STATUS: VAULT RECORD SAVED ✅**
The isolated item UUID generated from the central server was successfully registered locally.

---

**👤 You:**
> "System cleanup required. Permanently delete the draft attached to UUID 'note-xyz1' leveraging the standard removal procedures."

**🤖 AI Agent:**
> Verifying constraints for permanent destruction. Transmitting standard secure vectors across endpoints matching target ID to `delete_item` protocols... Targeted File: `note-xyz1`.

**PERMANENT ERASURE CONFIRMED 🗑️**
The item correlating to your input parameter UUID has been entirely removed from the persistent repository securely.


## ❓ FAQ

**Q: If I am self-hosting Standard Notes on my own server, can this integration still connect to it?**
Absolutely. The `SN_SERVER_URL` parameter allows complete flexibility. You can use the official `https://api.standardnotes.com` endpoint, or simply provide the custom domain pointing to your private server infrastructure.

**Q: Are my encrypted notes fully exposed to the AI model during a query?**
The server passes local encrypted blocks down to the MCP layer. While `list_notes` primarily retrieves metadata and structural UUIDs, executing an extraction using `get_item_details` or writing entirely new content via `create_note` will securely transmit standard text directly to the model's localized context.

**Q: What is the purpose of the 'sync_items' functionality?**
Standard Notes employs a client-side database synchronization architecture. The `sync_items` module retrieves exclusively the differences or modifications made since the execution of your last tracked `sync_token`. It ensures local operational states match the remote vault natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/standard-notes](https://vinkius.com/mcp/standard-notes)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Standard Notes** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `standard-notes` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Standard Notes** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "standard-notes": {
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
