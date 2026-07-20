# Code Clone Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/code-clone-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Identify exact and near-duplicate code blocks within your project.

## Description
The Code Clone Detector MCP server connects AI agents to your codebase to prevent logic duplication. It uses deterministic hashing and Levenshtein distance to find `identify_exact_duplicates` and `identify_near_matches`. By stripping comments, whitespace, and anonymizing variables via `generate_normalized_signature`, it ensures that even if variable names differ, the underlying structural similarity is detected.


## Available Tools (3)
- **generate_normalized_signature**: Provides a normalized, anonymized version of a code block
- **identify_exact_duplicates**: Finds blocks of code that are structurally identical after normalization
- **identify_near_matches**: Finds code blocks that are highly similar but not exact duplicates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Code Clone Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all exact duplicate code blocks in these files."

**🤖 AI Agent:**
> I found 2 clusters of exact matches in the provided file contents.

---

**👤 You:**
> "Are there any near-matches in this code with a similarity of at least 0.9?"

**🤖 AI Agent:**
> No near-matches were found above the 0.9 threshold.

---

**👤 You:**
> "Show me the normalized signature for this function."

**🤖 AI Agent:**
> $v_1 = $v_2 + 1


## ❓ FAQ

**Q: How does the tool detect duplicates?**
It uses `identify_exact_duplicates` to find identical structures via hashing and `identify_near_matches` for similar blocks using Levenshtein distance.

**Q: Can I see the normalized version of my code?**
Yes, you can use the `generate_normalized_signature` tool to see how your code looks after stripping comments and renaming variables.

**Q: What is the similarity threshold?**
The default threshold for `identify_near_matches` is 0.8, but you can adjust it between 0 and 1.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/code-clone-detector](https://vinkius.com/mcp/code-clone-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Code Clone Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `code-clone-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Code Clone Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "code-clone-detector": {
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
