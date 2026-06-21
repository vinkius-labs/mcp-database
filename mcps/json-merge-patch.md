# JSON Merge Patch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/json-merge-patch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop losing data when updating massive files. Apply surgical JSON patches (RFC 7396) securely to large datasets.

## Description
If an AI Agent needs to update just 3 fields in a 5,000-line JSON configuration file, asking the LLM to rewrite the entire file often leads to truncated data or forgotten keys due to context limits. This MCP solves that by shifting the merge logic to the Edge.

### The Superpowers

- **Surgical Updates:** The LLM only generates the 'patch' (what changed), and the V8 engine merges it flawlessly with the original file.
- **RFC 7396 Compliant:** Uses official industry standards for JSON merging, ensuring zero data corruption during the patch.


## Available Tools (1)
- **apply_patch**: Pass the original and the patch as JSON strings. The engine applies deep merging deterministically.

Applies an RFC 7396 JSON Merge Patch deterministically. Allows LLMs to update massive JSON files by only sending the delta patch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSON Merge Patch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Merge this patch `{"status": "active"}` into the 3MB user database JSON."

**🤖 AI Agent:**
> ✅ **Patched Output:** Output cleanly updated without touching other keys.

---

**👤 You:**
> "Remove the `temporary_token` key from this payload by applying a null patch."

**🤖 AI Agent:**
> ✅ **Applied:** Key successfully deleted per RFC 7396 standard.


## ❓ FAQ

**Q: Can it delete keys?**
Yes, following RFC 7396, setting a key to `null` in the patch will remove it from the target.

**Q: Is this better than normal JS merge?**
Yes, it safely handles deep object merging and null-deletions which simple object spread (`...`) fails at.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/json-merge-patch](https://vinkius.com/mcp/json-merge-patch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSON Merge Patch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `json-merge-patch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSON Merge Patch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "json-merge-patch": {
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
