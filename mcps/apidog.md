# Apidog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apidog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Sync your Apidog workspace with your AI agent — list projects, fetch endpoint schemas, and export full OpenAPI specifications instantly.

## Description
Connect your **Apidog** account to your AI agent and seamlessly access your API specifications, data models, and documentation through natural conversation.

### What you can do

- **Discover Projects & Endpoints** — Browse your active projects and list all HTTP routes without opening the Apidog client
- **Inspect Endpoint Schemas** — Fetch the complete anatomy of any route, including its HTTP method, dynamic path params, headers, and request/response body schemas
- **Understand Data Models** — Query active reusable schemas (DTOs, entities) defined throughout your API
- **Export OpenAPI Specs** — Extract the complete OpenAPI 3.0 JSON specification from your team’s project to give your AI maximum context for testing or code generation

### How it works

1. Subscribe to this server
2. Enter your Personal Apidog API Access Token
3. Interface with your API contracts using Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **Backend Developers** — quickly review endpoints or export a full OpenAPI spec so the LLM can safely scaffold controllers or unit tests
- **Frontend Engineers** — ask the AI to inspect an Apidog endpoint schema and generate the corresponding TypeScript interfaces or API service layers
- **QA Automation Teams** — fetch expected response payloads automatically to construct robust integration tests


## Available Tools
- **list_projects**: List all API projects in the connected Apidog organization
- **list_endpoints**: List all API endpoints defined within a specific Apidog project
- **get_endpoint**: Fetch the complete schema of a single API endpoint
- **list_schemas**: List all data model schemas (DTOs, entities) defined in an Apidog project
- **export_openapi**: Export the full OpenAPI 3.0 specification of an Apidog project as JSON


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apidog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in our Apidog organization."

**🤖 AI Agent:**
> I've retrieved your workspace projects. You have 'E-commerce API' (ID: 39420) and 'Internal Admin Portal' (ID: 10429). Which one would you like to explore?

---

**👤 You:**
> "Write a TypeScript interface for the response schema of the /users endpoint in the E-commerce project."

**🤖 AI Agent:**
> I analyzed the response schema for `/users`. Here is the exact TypeScript interface matching the backend's contract:

```typescript
export interface UserResponse {
  id: number;
  email: string;
  status: 'active' | 'suspended';
}
```

---

**👤 You:**
> "Export the full OpenAPI JSON for the E-commerce project so we can generate unit tests."

**🤖 AI Agent:**
> The complete OpenAPI 3.0 specification has been imported into my context. The project defines 42 endpoints and 18 global schemas. Looking at the /cart endpoints, which of its constraints would you like me to test first?


## ❓ FAQ

**Q: Can I import a complete OpenAPI spec into an AI chat session?**
Yes. Instruct the agent to run the `export_openapi` tool. It downloads the JSON metadata and safely passes it into your context. Given its size, the agent can use this massive reference guide to rapidly write tests, endpoints, or data models perfectly mimicking your production systems.

**Q: How can I check the payload requirements for a single specific route?**
If you know the general area of the project, use `list_endpoints` to verify the ID. Then query `get_endpoint`. It brings back the specific HTTP verbs, query arguments, path definitions, and expected JSON body — letting your agent craft exact functional requests to external systems.

**Q: Will my Apidog tokens expire?**
When generating your Personal Access Token in Apidog, you dictate the validity duration (e.g. 30 days, 1 year or never expire). If you choose a finite span, you will need to come back, generate a new token and insert it once more to reconnect the MCP server successfully.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apidog](https://vinkius.com/mcp/apidog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apidog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apidog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apidog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apidog": {
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
