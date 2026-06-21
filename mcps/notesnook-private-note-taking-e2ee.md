# Notesnook (Private Note Taking & E2EE) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/notesnook-private-note-taking-e2ee)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/notesnook-private-note-taking-e2ee-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/notesnook-private-note-taking-e2ee-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage encrypted notes via Notesnook — create secure entries, sync your vault, and audit private notebooks.

## Description
Connect your **Notesnook** account to any AI agent and take full control of your privacy-first knowledge base, zero-knowledge note taking, and secure vault synchronization through natural conversation.

### What you can do

- **Encrypted Orchestration** — List all secure notes and retrieve detailed encrypted payloads including raw text and binary history directly from your agent
- **Vault Synchronization** — Trigger a full sync with the Notesnook server to resolve encrypted state changes and ensure your local representation is up-to-date
- **Secure Note Injection** — Instantly create and attach brand new encrypted notes to your vault, securely pushing plaintext into persistent encrypted envelopes natively
- **Notebook Navigation** — Explore hierarchical notebook groupings to understand your knowledge organization and categorize secure notes across project boundaries
- **Metadata & Tag Audit** — Enumerate cross-cutting categorical tags and classification indices to identify related information through metadata parameters securely
- **Attachment Visibility** — List encapsulated binary attachments mapping images, PDFs, and embedded blobs stored persistently inside your encrypted notes
- **Lifecycle Management** — Update partial strings within existing notes or irreversibly delete specific entries to maintain a clean and relevant secure workspace

### How it works

1. Subscribe to this server
2. Enter your Notesnook Sync URL and Auth Token
3. Start managing your private vault from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Privacy-Conscious Users** — organize sensitive thoughts and research through natural conversation without exposing data to third-party providers
- **Knowledge Workers** — manage technical documentation and project snippets directly from your IDE while maintaining full zero-knowledge security
- **Researchers** — retrieve rapid summaries of favorited notes and audit large collections of encrypted information efficiently


## Available Tools
- **sync_items**: Yields encrypted binary objects based on the last sync timestamp boundaries.

Trigger a full sync with the Notesnook server resolving vault state
- **list_notes**: Indispensable for discovering target node IDs prior to fetching decryption contexts.

List all encrypted notes securely stored in the Notesnook vault
- **get_note**: Retrieve the underlying encrypted cipher payload of a single note
- **create_note**: This will securely push plaintext into an encrypted envelope stored persistently in the Notesnook sync server.

Create and inject a brand new encrypted note into the vault
- **update_note**: Updates synchronization timelines and forces re-encryption across the specific item payload.

Modify partial strings within a pre-existing encrypted vault note
- **delete_note**: Destroys the node logic completely inside the encrypted persistence layer.

Irreversibly delete a specific encrypted note from the server
- **list_notebooks**: Critical for correlating hierarchical IDs before exploring note clusters.

List boundary organizing Notebooks spanning the vault
- **list_tags**: List cross-cutting categorical classification Tags indexing Notes
- **list_trash**: Identifies tracking records physically slated for permanent erasure.

List nodes trapped inside the local vault waste bin
- **list_favorites**: List high-priority specific notes flagged as favorites
- **list_attachments**: List encapsulated binary attachments mapped against notes
- **get_user**: Validate the authenticated Notesnook user security identity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Notesnook (Private Note Taking & E2EE)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 encrypted notes in my vault"

**🤖 AI Agent:**
> I've retrieved your recent encrypted notes. Highlights include 'Project Alpha Strategy' (ID: note-123), 'Meeting Notes: Backend' (ID: note-456), and 'Research Snippets'. Would you like me to fetch the encrypted payload for the strategy note?

---

**👤 You:**
> "Create a new private note called 'Ideas 2026' with content 'Automated note generation via AI'"

**🤖 AI Agent:**
> New encrypted note 'Ideas 2026' has been successfully created and injected into your persistent vault. The note is now synced and secured with end-to-end encryption. New Note ID: 'note-98765'.

---

**👤 You:**
> "Show me all my classified tags in Notesnook"

**🤖 AI Agent:**
> Retrieving tags… I've identified 4 cross-cutting categories in your vault: 'Confidential', 'Drafts', 'Research', and 'Personal'. I can help you list all notes associated with the 'Confidential' tag if you'd like.


## Installation & Usage

To install and use the **Notesnook (Private Note Taking & E2EE)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/notesnook-private-note-taking-e2ee](https://vinkius.com/mcp/notesnook-private-note-taking-e2ee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
