# Directory State Fingerprinter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/directory-state-fingerprinter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate and verify deterministic cryptographic fingerprints of directory states.

## Description
The Directory State Fingerprinter MCP provides a way to ensure environmental integrity by creating immutable snapshots of file contents. Using the `generate_fingerprint` tool, you can create a Merkle-tree-like root hash that represents the exact state of a provided list of files. You can also use `compare_fingerprints` to detect any unauthorized changes between two different states. This is essential for security-sensitive workflows where verifying that files have not been altered by external actors is critical.


## Available Tools (2)
- **compare_fingerprints**: Compares two fingerprints for identity
- **generate_fingerprint**: The tool will compute the Merkle root hash and return a map of file hashes.

Generates a deterministic fingerprint of a file list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Directory State Fingerprinter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a fingerprint for these files: [{'filePath': 'config.json', 'content': '{"version": "1.0"}'}]"

**🤖 AI Agent:**
> The generated Merkle root hash is [REDACTED].

---

**👤 You:**
> "Compare these two fingerprint objects to see if they are identical."

**🤖 AI Agent:**
> The comparison shows that the fingerprints are not identical, indicating a change in the directory state.

---

**👤 You:**
> "Check if my current file list matches the previously recorded hash."

**🤖 AI Agent:**
> The verification process confirms that the current state matches the expected cryptographic signature.


## ❓ FAQ

**Q: How does the fingerprinting process work?**
The tool sorts all provided files by path, computes a SHA-256 hash for each file's content, and then aggregates these into a single Merkle root hash.

**Q: Can I use this to detect unauthorized file changes?**
Yes, by using `compare_fingerprints` on two different snapshots, you can immediately see if the state of your files has changed.

**Q: What format should the input be in?**
The `generate_fingerprint` tool expects a JSON string representing an array of objects, each containing a `filePath` and `content`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/directory-state-fingerprinter](https://vinkius.com/mcp/directory-state-fingerprinter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Directory State Fingerprinter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `directory-state-fingerprinter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Directory State Fingerprinter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "directory-state-fingerprinter": {
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
