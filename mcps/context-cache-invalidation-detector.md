# Context Cache Invalidation Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/context-cache-invalidation-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Detects context loss and reasoning drift caused by aggressive prompt caching.

## Description
This MCP server provides diagnostic tools to identify when prompt caching or session management has caused the loss of critical reasoning, system instructions, or conversational continuity. It uses deterministic SHA-256 checksumming to monitor the 'Four Pillars of Context': System Prompt, CLAUDE_md Content, Conversation Summary, and the Last Reasoning Block. By comparing current checksums against expected states, it can detect if an AI agent's reasoning has been prematurely cleared or if instructions have been truncated. Use `check_context_integrity` to validate session health and `get_continuity_status` to quickly assess if a session is Healthy, Degraded, or Broken.


## Available Tools (3)
- **compute_pillar_checksums**: Generates unique fingerprints for the four pillars of context
- **get_continuity_status**: Assess session health based on continuity score
- **check_context_integrity**: Determines if the current session context is intact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Context Cache Invalidation Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my current session context is still valid."

**🤖 AI Agent:**
> The session is Healthy with a continuity score of 1.0. All context pillars are intact.

---

**👤 You:**
> "What is the current status of my session health?"

**🤖 AI Agent:**
> The session status is Degraded. The continuity score is 0.75, indicating one pillar has drifted.

---

**👤 You:**
> "Generate checksums for my current context."

**🤖 AI Agent:**
> {"systemPromptHash": "a1b2c3d4...", "mdContentHash": "e5f6g7h8...", "conversationSummaryHash": "i9j0k1l2...", "lastReasoningHash": "m3n4o5p6..."}


## ❓ FAQ

**Q: What is the purpose of the continuity score?**
The `context_continuity_score` represents the health of the session by calculating the ratio of matched checksums against the expected Four Pillars of Context.

**Q: How does it detect if reasoning was lost?**
It compares the hash of the `lastReasoningBlock` against the previously stored hash. If they do not match, it indicates the reasoning was cleared or altered.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/context-cache-invalidation-detector](https://vinkius.com/ai-agent-connect/context-cache-invalidation-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Context Cache Invalidation Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `context-cache-invalidation-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Context Cache Invalidation Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "context-cache-invalidation-detector": {
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
