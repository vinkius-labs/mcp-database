# GraphQL Schema Breaking Change Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/graphql-schema-breaking-change-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [testing](../categories/testing.md)

Identify breaking changes in GraphQL schemas by comparing SDL strings.

## Description
The GraphQL Schema Breaking Change Detector is a specialized utility designed to prevent regressions during API evolution. By providing two versions of your GraphQL SDL, the `compare_schemas` tool performs a deterministic analysis to identify deletions, type mutations, and nullability changes that would break existing clients. The server also provides `validate_syntax` to ensure structural correctness before comparison and `inspect_schema` to reveal the parsed internal structure of your types and fields. This ensures that every change to your schema is evaluated for compatibility, protecting your ecosystem from unexpected failures.


## Available Tools (3)
- **compare_schemas**: Compare two GraphQL schemas for breaking changes
- **inspect_schema**: Inspect GraphQL schema structure
- **validate_syntax**: Validate GraphQL SDL syntax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GraphQL Schema Breaking Change Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this GraphQL schema is syntactically valid: 'type User { id: ID! }'"

**🤖 AI Agent:**
> The syntax is valid.

---

**👤 You:**
> "Compare these two schemas for breaking changes: Base: 'type User { id: ID! }' Next: 'type User { id: String! }'"

**🤖 AI Agent:**
> A breaking change was detected: the type of field `User.id` changed from ID to String.

---

**👤 You:**
> "Show me the structure of this schema: 'type Query { user: User } type User { id: ID! }'"

**🤖 AI Agent:**
> The schema contains 2 types: `Query` (fields: `user`) and `User` (fields: `id`).


## ❓ FAQ

**Q: What constitutes a breaking change in this tool?**
A breaking change is any modification that violates the existing contract, such as removing a type or field, changing an argument, or transitioning a field from nullable to non-null.

**Q: Can I use this to verify my new schema before deployment?**
Yes, by using `compare_schemas` with your current production schema as the base and your proposed changes as the next version, you can identify all potential regressions.

**Q: Does it support all GraphQL features?**
The tool parses and compares types, fields, arguments, and enums. It specifically monitors nullability constraints and type mutations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/graphql-schema-breaking-change-detector](https://vinkius.com/mcp/graphql-schema-breaking-change-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GraphQL Schema Breaking Change Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `graphql-schema-breaking-change-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GraphQL Schema Breaking Change Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "graphql-schema-breaking-change-detector": {
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
