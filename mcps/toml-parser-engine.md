# TOML Parser Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/toml-parser-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Convert TOML config files to JSON and back. Essential for Rust (Cargo.toml), Python (pyproject.toml), and Cloudflare (wrangler.toml).

## Description
When an AI Agent edits Cargo.toml, pyproject.toml, or wrangler.toml, it needs to understand TOML syntax perfectly — nested tables, arrays of tables, inline tables, and datetime values. This MCP converts bidirectionally with zero data loss.

### The Superpowers

- **Bidirectional:** TOML to JSON and JSON to TOML with full round-trip fidelity.
- **Full TOML 1.0 Spec:** Nested tables, arrays of tables, inline tables, datetime, and multiline strings.


## Available Tools
- **parse_toml**: Pass the raw TOML or JSON content and the direction ("toml-to-json" or "json-to-toml"). The engine handles nested tables, arrays of tables, inline tables, and datetime values deterministically.

Converts TOML configuration files to JSON and vice versa. Essential for Rust (Cargo.toml), Python (pyproject.toml), and Cloudflare (wrangler.toml) workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TOML Parser Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert this Cargo.toml to JSON so I can inspect the dependencies."

**🤖 AI Agent:**
> TOML Conversion: JSON output generated with all nested tables preserved.

---

**👤 You:**
> "Generate a valid wrangler.toml from this JSON config."

**🤖 AI Agent:**
> TOML Conversion: Valid wrangler.toml generated.

---

**👤 You:**
> "Parse this pyproject.toml and extract the project metadata as JSON."

**🤖 AI Agent:**
> TOML Conversion: Project metadata extracted with name, version, and dependencies.


## ❓ FAQ

**Q: Does it support TOML 1.0 spec?**
Yes. @iarna/toml fully supports the TOML 1.0 specification including all edge cases like nested tables, inline tables, and datetime values.

**Q: Can I convert JSON back to TOML?**
Yes. Use direction "json-to-toml" to serialize a JSON object back into valid TOML format with proper sections and formatting.

**Q: What files does this commonly work with?**
Cargo.toml (Rust), pyproject.toml (Python), wrangler.toml (Cloudflare Workers), Hugo config.toml, and any TOML-based configuration file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/toml-parser-engine](https://vinkius.com/mcp/toml-parser-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TOML Parser Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `toml-parser-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TOML Parser Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "toml-parser-engine": {
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
