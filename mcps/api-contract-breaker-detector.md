# API Contract Breaker Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/api-contract-breaker-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Detect breaking changes in API signatures and endpoints before they cause runtime failures.

## Description
The API Contract Breaker Detector prevents runtime failures in distributed systems by identifying modifications that violate existing API agreements. It uses deterministic AST parsing to scan codebases for FastAPI, Express, GraphQL, and TypeScript definitions. By building a persistent contract registry, it can compare current code against a known baseline to flag removed endpoints, altered paths, or changed parameter types. Use `register_api_contracts` to establish your baseline, `check_for_breaking_changes` to validate new code, and `query_contract_details` for deep inspection of specific endpoints.


## Available Tools (3)
- **check_for_breaking_changes**: Compares the current state of the codebase against the stored registry to identify any modifications that break existing contracts
- **query_contract_details**: Retrieves the full specific definition of a single contract from the registry for deep inspection
- **register_api_contracts**: You may optionally provide a list of framework types to prioritize.

Establishes the baseline "source of truth" by scanning the codebase and saving the current state of all API definitions into the registry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **API Contract Breaker Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you check if my recent changes broke any API contracts in the current directory?"

**🤖 AI Agent:**
> The check is complete. No breaking changes were detected; the current API state is compatible with the registry.

---

**👤 You:**
> "Register the API contracts in the /src/api folder."

**🤖 AI Agent:**
> API contracts have been successfully registered for the /src/api directory.

---

**👤 You:**
> "Show me the details for the endpoint 'GET /users/profile'."

**🤖 AI Agent:**
> The endpoint 'GET /users/profile' requires a 'user_id' string parameter and returns a JSON object containing 'username' and 'email'.


## ❓ FAQ

**Q: How do I start using this tool?**
First, run `register_api_contracts` to scan your codebase and create a baseline registry of your current API definitions.

**Q: What is considered a breaking change?**
A breaking change includes removing an endpoint, changing a URL path, renaming a parameter, changing a parameter type, or removing a field from a response body.

**Q: Does adding a new endpoint trigger a breaking change alert?**
No, adding new endpoints or adding optional parameters are not considered breaking changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/api-contract-breaker-detector](https://vinkius.com/ai-agent-connect/api-contract-breaker-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **API Contract Breaker Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `api-contract-breaker-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **API Contract Breaker Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "api-contract-breaker-detector": {
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
