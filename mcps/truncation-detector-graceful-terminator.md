# Truncation Detector & Graceful Terminator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/truncation-detector-graceful-terminator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Detects and repairs truncated LLM outputs to restore structural integrity.

## Description
This MCP server provides essential diagnostic and recovery tools for handling incomplete Large Language Model (LLM) responses. It identifies if an output was cut off due to token limits by checking for mid-word cutoffs, missing terminal punctuation, or unclosed structural elements like brackets and braces. Using `detect_truncation`, you can confirm if a response is incomplete. The `repair_truncated_text` tool uses a deterministic stack-based approach to append the necessary closing characters, ensuring JSON or Markdown structures are syntactically valid. Additionally, `validate_structural_integrity` allows for verifying the completeness of text in plain_text, json, or markdown formats.


## Available Tools (3)
- **detect_truncation**: 
- **repair_truncated_text**: 
- **validate_structural_integrity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Truncation Detector & Graceful Terminator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this text is truncated: {"name": "item", "value": 10"

**🤖 AI Agent:**
> {"name": "item", "value": 10}

---

**👤 You:**
> "Is this sentence complete? The weather is very"

**🤖 AI Agent:**
> The weather is very.

---

**👤 You:**
> "Validate the integrity of this markdown: # Title

This is a test"

**🤖 AI Agent:**
> The markdown structure is valid.


## ❓ FAQ

**Q: How does the tool detect if a response is truncated?**
The `detect_truncation` tool checks for missing terminal punctuation, mid-word cutoffs, and unmatched opening symbols like braces or brackets.

**Q: Can I use this to fix broken JSON outputs?**
Yes, `repair_truncated_text` is designed to append the correct closing sequences to restore the structural validity of JSON, Markdown, and other formats.

**Q: What formats are supported for validation?**
The `validate_structural_integrity` tool supports plain_text, json, and markdown formats.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/truncation-detector-graceful-terminator](https://vinkius.com/mcp/truncation-detector-graceful-terminator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Truncation Detector & Graceful Terminator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `truncation-detector-graceful-terminator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Truncation Detector & Graceful Terminator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "truncation-detector-graceful-terminator": {
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
