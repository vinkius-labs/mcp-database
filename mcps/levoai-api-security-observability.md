# Levo.ai (API Security & Observability) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/levoai-api-security-observability)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/levoai-api-security-observability-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/levoai-api-security-observability-mcp)
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


## Installation & Usage

To install and use the **Levo.ai (API Security & Observability)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/levoai-api-security-observability](https://vinkius.com/mcp/levoai-api-security-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
