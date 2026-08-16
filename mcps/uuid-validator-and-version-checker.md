# UUID Validator and Version Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/uuid-validator-and-version-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validate UUID structure and extract version numbers instantly.

## Description
This MCP server provides precise tools for inspecting Universally Unique Identifiers (UUIDs). Use `check_uuid_validity` to verify if a string adheres to the RFC 4122 format, including correct hex character layout and variant bits. The `get_uuid_version` tool allows you to quickly identify whether a UUID is version 1, 2, 3, 4, or 5. For deep inspection, `list_uuid_metadata` provides a comprehensive breakdown of the identifier's properties. It acts as a bridge for AI agents in Cursor, VS Code, Claude Desktop, and Windsurf to handle identity strings with high precision.


## Available Tools (3)
- **check_uuid_validity**: Validates if a string is a valid RFC 4122 UUID
- **get_uuid_version**: Extracts the UUID version from a valid UUID string
- **list_uuid_metadata**: Provides a full breakdown of UUID metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UUID Validator and Version Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is '550e8400-e29b-41d4-a716-446655440000' a valid UUID?"

**🤖 AI Agent:**
> Yes, the string is a valid RFC 4122 compliant UUID.

---

**👤 You:**
> "What version is this UUID: '6ba7b810-9dad-11d1-80b4-00c04fd430c8'?"

**🤖 AI Agent:**
> The extracted UUID version is 1.

---

**👤 You:**
> "Give me the metadata for 'f47ac10b-58cc-4372-a567-0e02b2c3d479'."

**🤖 AI Agent:**
> The UUID is valid, version 4, with the correct variant bits and hex structure.


## ❓ FAQ

**Q: What UUID versions are supported?**
The server supports extraction and validation for UUID versions 1, 2, 3, 4, and 5.

**Q: How can I check if a specific string is a valid UUID?**
You can use the `check_uuid_validity` tool by providing the raw string to be inspected.

**Q: Does this tool work with Claude Desktop?**
Yes, by connecting via Vinkius Edge, you can use these tools in Claude Desktop and other MCP clients.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/uuid-validator-and-version-checker](https://vinkius.com/ai-agent-connect/uuid-validator-and-version-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UUID Validator and Version Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uuid-validator-and-version-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UUID Validator and Version Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uuid-validator-and-version-checker": {
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
