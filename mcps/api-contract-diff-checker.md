# API Contract Diff Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/api-contract-diff-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Detect breaking and additive changes in OpenAPI and GraphQL schemas.

## Description
The API Contract Diff Checker is a specialized utility for identifying structural changes between two versions of API contracts. By comparing OpenAPI specifications or GraphQL SDL, it detects breaking changes like removed endpoints or type narrowing, as well as additive changes such as new fields. Use `diff_openapi` to analyze RESTful APIs, `diff_graphql` for GraphQL schemas, and `evaluate_version_bump` to receive a SemVer recommendation (MAJOR, MINOR, or PATCH) based on the detected impact.


## Available Tools (3)
- **diff_graphql**: Compares two GraphQL Schema Definition Language (SDL) strings to identify breaking and additive changes
- **diff_openapi**: Detects structural differences and compatibility impacts between two OpenAPI specification documents
- **evaluate_version_bump**: Analyzes a collection of identified changes to recommend a Semantic Versioning increment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **API Contract Diff Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two OpenAPI specs: baseSpec='{"openapi":"3.0.0","paths":{"/user":{"get":{}}}}' and targetSpec='{"openapi":"3.0.0","paths":{}}'"

**🤖 AI Agent:**
> Breaking changes detected: path '/user' was removed.

---

**👤 You:**
> "Check if adding a field to my GraphQL schema is breaking: baseSdl='type User { id: ID! }' and targetSdl='type User { id: ID!, email: String }'"

**🤖 AI Agent:**
> Additive changes detected: new field 'email' added to type 'User'.

---

**👤 You:**
> "What version bump should I use for these changes? JSON: '[{"severity": "BREAKING"}]'"

**🤖 AI Agent:**
> Recommendation: MAJOR. Reasoning: The detected changes include at least one breaking change.


## ❓ FAQ

**Q: What types of API contracts can I compare?**
You can compare OpenAPI specifications and GraphQL Schema Definition Language (SDL) strings.

**Q: How does the tool recommend a version bump?**
The `evaluate_version_bump` tool analyzes detected changes. A MAJOR bump is recommended for breaking changes, MINOR for additive changes, and PATCH for informational updates.

**Q: Can I detect type narrowing in OpenAPI?**
Yes, `diff_openapi` identifies type narrowing (e.g., changing a string to a specific regex pattern) as a breaking change.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/api-contract-diff-checker](https://vinkius.com/mcp/api-contract-diff-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **API Contract Diff Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `api-contract-diff-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **API Contract Diff Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "api-contract-diff-checker": {
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
