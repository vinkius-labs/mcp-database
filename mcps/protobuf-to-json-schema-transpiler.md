# Protobuf to JSON Schema Transpiler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/protobuf-to-json-schema-transpiler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Convert Protocol Buffer (.proto) definitions into valid JSON Schema objects deterministically.

## Description
The Protobuf to JSON Schema Transpiler bridges the gap between gRPC/Protobuf schemas and AI agents by providing a way to validate data without needing a full Protobuf compiler. Using `transpile_proto_to_json_schema`, you can transform raw .proto strings into structured JSON Schemas, mapping types like int3 32 to integer and handling repeated fields as arrays. It also allows for quick inspection of schemas using `summarize_message_definitions` and detecting complexity with `scan_for_complex_elements`.


## Available Tools (3)
- **scan_for_complex_elements**: Identifies the presence of advanced Protobuf features
- **summarize_message_definitions**: Provides a high-level summary of all messages found within a schema
- **transpile_proto_to_json_schema**: proto definitions and maps them to standard JSON Schema types.

Converts a Protobuf schema string into a JSON Schema object


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Protobuf to JSON Schema Transpiler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert this proto definition to JSON Schema: 'message User { string name = 1; int32 id = 2; }'"

**🤖 AI Agent:**
> {"type": "object", "properties": {"name": {"type": "string"}, "id": {"type": "integer"}}, "required": ["name", "id"]}

---

**👤 You:**
> "How many messages are in this proto: 'message A { string s = 1; } message B { int32 i = 1; }'"

**🤖 AI Agent:**
> There are 2 messages identified in the provided schema.

---

**👤 You:**
> "Does this proto have nested messages: 'message Outer { message Inner { string x = 1; } }'"

**🤖 AI Agent:**
> Yes, the scan detected 1 nested message structure.


## ❓ FAQ

**Q: What does the `transpile_proto_to_json_schema` tool do?**
It takes a raw Protobuf string and converts it into a functional JSON Schema, identifying messages, fields, and types.

**Q: Can I check for repeated fields in my schema?**
Yes, you can use the `scan_for_complex_elements` tool to detect if your schema contains repeated fields or nested structures.

**Q: How can I get a quick overview of my message definitions?**
Use the `summarize_message_definitions` tool to retrieve a list of all identified message names and the total field count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/protobuf-to-json-schema-transpiler](https://vinkius.com/mcp/protobuf-to-json-schema-transpiler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Protobuf to JSON Schema Transpiler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `protobuf-to-json-schema-transpiler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Protobuf to JSON Schema Transpiler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "protobuf-to-json-schema-transpiler": {
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
