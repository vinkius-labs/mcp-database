# Markdown Frontmatter Harvester MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/markdown-frontmatter-harvester)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Scan local Obsidian or Hugo vaults and extract all YAML frontmatter (tags, dates, status) into a single structured JSON. Let your AI query your scattered notes metadata instantly.

## Description
If you use a Knowledge Management system like Obsidian, Logseq, or Hugo, you likely use YAML 'frontmatter' at the top of your markdown files to track metadata like `status: draft`, `tags: [idea, research]`, or `date: 2024-01-01`.

When you ask Claude, 'Which of my notes are marked as drafts and never published?', it fails because it can't read thousands of local files quickly. This MCP solves that by acting as a hyper-fast metadata librarian. It recursively scans your local folder, rips out only the YAML frontmatter from every file, and aggregates it into a clean JSON index. The AI can then instantly filter, sort, and query your entire knowledge base.

### The Superpowers

- **Vault-Wide Indexing:** Turns scattered local markdown metadata into a unified database.
- **Lightning Fast:** Uses `fast-glob` and `gray-matter` to scan 1,000+ files in milliseconds.
- **Zero Config:** Just give the AI the absolute path to your notes folder.
- **100% Air-Gapped Privacy:** Your private journal entries and business notes never leave your machine.


## Available Tools (1)
- **harvest_markdown_frontmatter**: Provide the absolute directory path.

Scan a local directory of Markdown files (Obsidian/Hugo) and extract all YAML frontmatter tags, dates, and metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Markdown Frontmatter Harvester** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan my Obsidian vault at C:/Notes and list all files that have the tag 'urgent'."

**🤖 AI Agent:**
> I found 5 notes with the tag 'urgent'. Here are their filenames: ProjectX.md, MeetingNotes.md...

---

**👤 You:**
> "Harvest the frontmatter from my blog repo and tell me which posts are still marked as 'status: draft'."

**🤖 AI Agent:**
> Based on the frontmatter, you have 12 posts still marked as 'draft'. Would you like the list?

---

**👤 You:**
> "Count how many notes I created in the year 2023 based on the YAML 'date' field."

**🤖 AI Agent:**
> According to the metadata, you created exactly 142 notes in 2023.


## ❓ FAQ

**Q: Does it send my entire note content to the AI?**
No. To protect your privacy and save context tokens, it strictly extracts ONLY the YAML metadata block between the `---` delimiters. The actual body text of your note is ignored.

**Q: Will this alter my Obsidian files?**
Not at all. The parser operates in a strict read-only mode. It reads the files into memory to extract the metadata and never writes back to the disk.

**Q: Does it work with nested folders?**
Yes! The engine uses recursive globbing to scan every single folder and sub-folder inside the path you provide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markdown-frontmatter-harvester](https://vinkius.com/mcp/markdown-frontmatter-harvester)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Markdown Frontmatter Harvester** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `markdown-frontmatter-harvester` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Markdown Frontmatter Harvester** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "markdown-frontmatter-harvester": {
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
