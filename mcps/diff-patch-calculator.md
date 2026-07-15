# Diff & Patch Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/diff-patch-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Compute line-level and word-level diffs, generate unified patches, and calculate text similarity.

## Description
The Diff & Patch Calculator MCP connects AI agents to precise text comparison utilities. Using the Myers algorithm, it identifies structural changes at both line and word granularity. You can use `generate_line_diff` to see added or removed lines in a unified diff format, `analyze_word_changes` for fine-grained token mutations, `apply_patch_operation` to transform text using an existing patch, and `evaluate_similarity` to quantify content overlap between two blocks.


## Available Tools (4)
- **analyze_word_changes**: Perform word-level comparison for specific lines
- **apply_patch_operation**: Transform a base text block using a provided unified diff patch
- **evaluate_similarity**: Provide a high-level similarity metric between two text blocks
- **generate_line_diff**: Identify structural changes between two blocks of text at the line level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diff & Patch Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two lines and tell me what changed: 'Hello world' and 'Hello brave new world'."

**🤖 AI Agent:**
> The words 'brave' and 'new' were added to the line.

---

**👤 You:**
> "Generate a line diff between 'Line 1
Line 2' and 'Line 1
Line 2
Line 3'."

**🤖 AI Agent:**
> The unified diff shows one line added: '+Line 3'.

---

**👤 You:**
> "How similar are 'Apple' and 'Apple Inc.'?"

**🤖 AI Agent:**
> The similarity percentage is approximately 50%.


## ❓ FAQ

**Q: What algorithm does this server use for diffing?**
This server implements the Myers diff algorithm to find the shortest edit script for both line and word-level comparisons.

**Q: Can I apply a patch to an existing text block?**
Yes, you can use the `apply_patch_operation` tool to take a target text and a unified diff patch to produce the updated version.

**Q: How is similarity calculated?**
The `evaluate_similarity` tool calculates a percentage (0-100) representing the degree of content overlap between two text blocks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/diff-patch-calculator](https://vinkius.com/mcp/diff-patch-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Diff & Patch Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `diff-patch-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Diff & Patch Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "diff-patch-calculator": {
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
