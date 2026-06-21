# Levo.ai (API Security & Observability) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/levoai-api-security-observability)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Secure your APIs via Levo.ai — audit endpoints, monitor sensitive data (PII/PHI), and manage OWASP vulnerabilities.

## Description
Connect your **Levo.ai** account to any AI agent and take full control of your API security posture and runtime observability through natural conversation.

### What you can do

- **Endpoint Orchestration** — List all auto-discovered API endpoints (REST, GraphQL, gRPC) and identify undocumented shadow or zombie APIs directly from your agent
- **Sensitive Data Audit** — Query categorizations for endpoints exposing regulated data flows including PII (names, emails), PHI (medical), and financial boundaries
- **Vulnerability Management** — Monitor active API security vulnerabilities validating against OWASP boundaries, including BOLA instances and broken authentication
- **OpenAPI Generation** — Export live, precisely accurate OpenAPI specifications derived immediately from actual observed traffic rather than static manual definitions
- **Behavioral Monitoring** — Analyze runtime API traffic patterns and anomalous observations detected by live sensors indicating unexpected schema drift
- **Diagnostic Investigation** — Retrieve detailed diagnostic exploitation evidence for specific vulnerabilities to understand root causes and remediation steps

### How it works

1. Subscribe to this server
2. Enter your Levo.ai API Token and Organization ID
3. Start monitoring your API security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — hunt for API threats and monitor sensitive data exposure through natural conversation without manual log filtering
- **Backend Developers** — audit API endpoint schemas and verify build-time security results to ensure only secure APIs reach production
- **Compliance Officers** — automate the auditing of regulated data flows and report on global API security posture across different environments


## Available Tools
- **list_applications**: List all API applications (services) tracked by Levo.ai
- **list_catalog_endpoints**: Identifies REST, GraphQL, gRPC, and SOAP endpoints — including undocumented shadow and zombie APIs mapped dynamically.

List all discovered API endpoints in the Levo.ai catalog
- **get_endpoint_details**: Get deep detailed schema structure for a specific discovered API endpoint
- **list_environments**: List deployment boundaries environments monitored by Levo active sensors
- **export_openapi_spec**: Export a live auto-generated OpenAPI payload specification for an application
- **get_observation**: Get details of a specific runtime anomalous observation
- **get_vulnerability**: Get detailed diagnostic exploitation evidence for a specific API vulnerability
- **list_observations**: List runtime API behavior observations detected by Levo sensors
- **list_sensitive_data**: List categorized API endpoints exposing sensitive or regulated data flows
- **list_vulnerabilities**: List active API security vulnerabilities discovered across all applications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Levo.ai (API Security & Observability)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all discovered API endpoints in our Levo catalog"

**🤖 AI Agent:**
> I've found 24 total endpoints across 3 applications. Highlights include '/v1/users' (REST), '/graphql' (GraphQL), and 5 undocumented shadow APIs discovered in the 'Payments' service. Would you like to inspect the sensitive data status for these?

---

**👤 You:**
> "Show me the active OWASP vulnerabilities for the 'Checkout' application"

**🤖 AI Agent:**
> Retrieving vulnerabilities for 'Checkout'… I've identified 2 High impact issues: 1) BOLA (Broken Object Level Authorization) on '/api/v1/orders/{id}', 2) Broken User Authentication. I can provide the diagnostic exploitation evidence for both.

---

**👤 You:**
> "Generate a live OpenAPI spec for the 'User Management' service"

**🤖 AI Agent:**
> Generating OpenAPI spec based on live traffic… Done. I've successfully exported the specification for the User Management service. It includes 12 verified endpoints and mapped request/response schemas. Would you like the JSON payload?


## ❓ FAQ

**Q: Can Levo.ai identify undocumented APIs in my environment?**
Yes. Use the `list_catalog_endpoints` tool to see the full inventory auto-discovered by Levo sensors. Your agent can highlight 'Shadow' or 'Zombie' APIs that exist in your infrastructure but are missing from official documentation.

**Q: How do I check which endpoints are exposing PII or sensitive data?**
The `list_sensitive_data` tool allows your agent to query endpoints categorized by regulated data flows. You'll see which paths are transmitting names, emails, SSNs, or financial data, helping you prioritize compliance audits.

**Q: Can my agent generate a live OpenAPI specification for an existing service?**
Absolutely. Use the `export_openapi_spec` tool with a specific App ID. Your agent will retrieve a specification derived from actual observed traffic, providing a more accurate reflection of your live API than static files.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/levoai-api-security-observability](https://vinkius.com/mcp/levoai-api-security-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Levo.ai (API Security & Observability)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `levoai-api-security-observability` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Levo.ai (API Security & Observability)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "levoai-api-security-observability": {
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
