# Cryptographic Action Attestor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cryptographic-action-attestor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Creates a tamper-proof audit trail of every agent action using SHA-256 hashing.

## Description
The Cryptographic Action Attestor MCP server provides an immutable, append-only ledger for tracking agent activities. By using SHA-256 hashing, it ensures that every action--including the tool name, parameters, and timestamp--is cryptographically linked to its predecessor. Use `attest_action` to record new events and `get_audit_log_status` to verify that the entire history remains untampered. This server is essential for building autonomous systems where provenance and accountability are critical.


## Available Tools (2)
- **attest_action**: This will compute a SHA-256 hash and append it to the log.

Creates a tamper-proof audit trail of an action
- **get_audit_log_status**: Checks the integrity and size of the audit log


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cryptographic Action Attestor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record that I just used the 'search_web' tool with parameters {'query': 'weather in London'} at timestamp 1715683200."

**🤖 AI Agent:**
> Action recorded successfully. Action ID: act_98234, Hash: [REDACTED], Integrity Valid: true

---

**👤 You:**
> "Check if the audit log is still valid and hasn't been tampered with."

**🤖 AI Agent:**
> The audit log integrity is valid. Total entries in the ledger: 12.

---

**👤 You:**
> "Show me the recent actions recorded in the system."

**🤖 AI Agent:**
> The following actions were found: 1. tool: search_web, timestamp: 1715683200; 2. tool: calculate_sum, timestamp: 1715683500.


## ❓ FAQ

**Q: How does the server ensure the log hasn't been tampered with?**
The server uses SHA-256 hashing to create a cryptographic fingerprint for every action. When you call `get_audit_log_status`, the system recomputes all hashes in the log and compares them against the stored values to detect any unauthorized changes.

**Q: What information is recorded during an attestation?**
The `attest_action` tool records the name of the tool used, the specific parameters passed to it, and a Unix timestamp.

**Q: Can I see previous actions in the log?**
Yes, you can use the history retrieval tools to view the sequence of recorded events in the ledger.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cryptographic-action-attestor](https://vinkius.com/mcp/cryptographic-action-attestor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cryptographic Action Attestor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cryptographic-action-attestor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cryptographic Action Attestor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cryptographic-action-attestor": {
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
