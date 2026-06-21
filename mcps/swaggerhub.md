# SwaggerHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swaggerhub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your AI to SwaggerHub. Read OpenAPI specifications, explore domains, and manage your API design lifecycle natively from the terminal.

## Description
Integrate **SwaggerHub**, the enterprise platform for API design and documentation, directly into your conversational workflows with the intelligent MCP connector. Transform your LLM into an active technical architect, empowering it to securely index, validate, and retrieve full OpenAPI specifications directly from your organizational directories. Eradicate context-switching by verifying CI/CD integration pipelines, scanning centralized API definitions, and pulling structural component domains intuitively without having to hunt through graphical interfaces.

### What you can do

- **API Cataloging & Specs** — Query an entire organizational API roster using `list_apis` and pull exact OpenAPI JSON configurations cleanly calling `get_api_version_spec`.
- **Component Reusability Insights** — Investigate generic shared definitions executing `list_domains` and fetch core parameters seamlessly via `get_domain_details`.
- **Project & Lifecycle Control** — Map team infrastructures inspecting groupings natively with `list_projects` and verify operational logic by calling `get_project_details`.
- **Ecosystem Verification** — Audit backend dependencies natively invoking `list_api_integrations` to test GitHub, AWS, and GitLab sync parameters tied to your specs.

### How it works

1. Append the SwaggerHub MCP framework natively within your operational intelligence environment.
2. Configure access safely by mapping your personal or organizational `SWAGGERHUB_KEY` into your credentials setup.
3. Instruct your AI directly: "Check the 'PaymentsAPI' definition owned by my organization, retrieve version '2.0.0', and list all shared domains it might depend on."

### Who is this for?

- **API Architects & Backend Engineers** — Query exact spec configurations seamlessly and retrieve JSON OpenAPI schemas natively to structure robust code generation logic.
- **DevOps & CI/CD Leads** — Guarantee your pipelines match deployed definitions rapidly mapping integration synchronization via CLI conversational checks.
- **Technical Writers** — Examine Swagger endpoints efficiently drafting high-quality structured documentation parsing correct definitions smoothly.


## Available Tools (10)
- **get_api_details**: Retrieves metadata for a SwaggerHub API definition
- **get_api_version_spec**: Retrieves a specific version of a SwaggerHub API definition (OpenAPI spec)
- **get_domain_details**: Retrieves metadata for a SwaggerHub domain
- **get_project_details**: Retrieves details of a SwaggerHub project
- **list_apis**: List all API definitions owned by a SwaggerHub user or organization
- **list_domains**: Lists all shared domains (reusable components) owned by a user or org
- **list_api_integrations**: Lists all CI/CD integrations configured for a SwaggerHub API
- **list_projects**: Lists all projects in a SwaggerHub organization
- **list_api_templates**: Lists all available API templates on SwaggerHub
- **search_apis**: Search all public APIs on SwaggerHub by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SwaggerHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for public API specifications related to 'payment gateway' on SwaggerHub."

**🤖 AI Agent:**
> Accessing public registries ('search_apis')...
Found 3 matches for 'payment gateway':
- 'AcmeCorp-Payments' (Version: v1.2.0)
- 'OpenPay-Gateway' (Version: v3.0.0)
- 'SecureTx-API' (Version: v1.0.1)

Let me know if you want me to fetch the OpenAPI specs for any of these results natively.

---

**👤 You:**
> "List all active projects in our SwaggerHub organization."

**🤖 AI Agent:**
> Mapping team clusters ('list_projects')...
I found 2 core organizational projects:
1. 'Billing-Infrastructure' (4 underlying APIs)
2. 'User-Authentication-Systems' (2 shared domains and 1 API configuration)

---

**👤 You:**
> "Ensure that the 'Acme-Billing' API has AWS API Gateway integration synced currently."

**🤖 AI Agent:**
> Interrogating pipeline bounds ('list_api_integrations')...
The specified API 'Acme-Billing' v1.0.0 currently returns 1 active integration:
- Type: AWS API Gateway Sync
- Status: Synced & Configured Successfully
- Last Run: 25 minutes ago.


## ❓ FAQ

**Q: Can the agent interact with public APIs outside my specific organizational ecosystem?**
Yes. Beyond listing your own API configurations, the integration includes powerful global metadata tools like `search_apis` allowing you to query keyword structures discovering public interfaces readily.

**Q: How securely does the system parse potentially heavy or oversized API configurations locally?**
Yes. The integration parses large JSON configurations securely and natively, ensuring large multi-megabyte API definitions are safely parsed without memory timeouts.

**Q: Can the AI modify or publish new API specifications?**
The integration is primarily read-oriented — it retrieves specs, domains, projects, and integration configs. To publish or edit specs you would use the SwaggerHub editor or its write API endpoints separately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swaggerhub](https://vinkius.com/mcp/swaggerhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SwaggerHub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swaggerhub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SwaggerHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swaggerhub": {
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
