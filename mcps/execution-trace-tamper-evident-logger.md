# Execution Trace Tamper-Evident Logger MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/execution-trace-tamper-evident-logger)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Creates immutable, cryptographic audit trails for agent execution steps using Merkle trees.

## Description
This MCP server provides a cryptographic layer for AI agent observability. It uses SHA-256 hashing and Merkle trees to create a tamper-evident log of every execution step. By using `log_execution_step`, you record discrete actions into a hierarchical hash structure. You can then use `verify_trace_integrity` to ensure the entire history remains unchanged, or `get_step_verification_proof` to extract specific audit paths. This ensures absolute provenance for agent workflows.


## Available Tools (3)
- **get_step_verification_proof**: Retrieves the cryptographic proof required to validate a specific step within the trace
- **log_execution_step**: Records a new step in the execution trace and updates the cryptographic integrity of the log
- **verify_trace_integrity**: Validates whether the current trace has been altered by comparing the calculated Merkle Root against a known trusted root


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Execution Trace Tamper-Evident Logger** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Log the current agent action."

**🤖 AI Agent:**
> Step logged successfully. The new Merkle root is 0x7f8e9d...

---

**👤 You:**
> "Check if the execution trace is still valid."

**🤖 AI Agent:**
> The trace is valid. No discrepancies detected in the Merkle root.

---

**👤 You:**
> "Get the proof for step hash 0xabc123."

**🤖 AI Agent:**
> Verification proof retrieved. The audit path contains 3 sibling hashes.


## ❓ FAQ

**Q: How does this ensure the logs haven't been changed?**
The server builds a Merkle tree where the root hash represents the entire trace. If any step is altered, the root hash will no longer match, which you can detect using `verify_trace_integrity`.

**Q: What is an execution step?**
An execution step is the atomic unit of an agent's activity, such as a single thought or action. You record these using `log_execution_step` to build the audit trail.

**Q: Can I verify a single step without checking the whole log?**
Yes, you can use `get_step_verification_proof` to retrieve the specific cryptographic proof needed to validate a single step hash against the Merkle root.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/execution-trace-tamper-evident-logger](https://vinkius.com/mcp/execution-trace-tamper-evident-logger)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Execution Trace Tamper-Evident Logger** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `execution-trace-tamper-evident-logger` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Execution Trace Tamper-Evident Logger** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "execution-trace-tamper-evident-logger": {
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
