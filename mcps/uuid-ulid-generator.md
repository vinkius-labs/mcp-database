# UUID & ULID Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uuid-ulid-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate and validate UUID (v1, v3, v4, v5, v7) and ULID identifiers with timestamp extraction.

## Description
This MCP server provides a complete toolkit for working with modern unique identifiers. You can use `generate_uuid` to create specific UUID versions like the time-ordered v7 or random v4. The `generate_ulid` tool produces lexicographically sortable ULIDs using Crockford's Base32 encoding. For existing IDs, `validate_identifier` checks if a string is a valid UUID or ULID format, while `extract_timestamp` allows you to retrieve the embedded creation date from temporal identifiers like UUID v1, UUID v7, and ULID.


## Available Tools (4)
- **extract_timestamp**: Retrieves the original creation timestamp embedded within time-based identifiers
- **generate_uuid**: For v3 and v5, namespace and name are required.

Generates a new UUID based on a specified version
- **validate_identifier**: Determines if a provided string is a valid UUID or ULID
- **generate_ulid**: Generates a new, valid ULID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UUID & ULID Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a random UUID v4."

**🤖 AI Agent:**
> f47ac10b-58cc-4372-a567-0e02b2c3d479

---

**👤 You:**
> "Is this a valid ULID: 01H7X9K6B5V8N2M4P7R3D5F6G7?"

**🤖 AI Agent:**
> Yes, the identifier is a valid ULID.

---

**👤 You:**
> "Extract the timestamp from this UUID v7: 018d2f3a-4b5c-7d6e-8f9a-0b1c2d3e4f5g"

**🤖 AI Agent:**
> 2025-02-14T10:30:00Z


## ❓ FAQ

**Q: What UUID versions are supported?**
The `generate_uuid` tool supports v1, v3, v4, v5, and v1.

**Q: Can I extract the date from a ULID?**
Yes, using the `extract_timestamp` tool on a valid ULID will return its creation time in ISO 8601 format.

**Q: How do I check if a string is a valid identifier?**
You can use the `validate_identifier` tool to check if a string follows the UUID or ULID specification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uuid-ulid-generator](https://vinkius.com/mcp/uuid-ulid-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UUID & ULID Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uuid-ulid-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UUID & ULID Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uuid-ulid-generator": {
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
