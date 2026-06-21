# Levo.ai (API Security & Observability) MCP Server

Secure your APIs via Levo.ai — audit endpoints, monitor sensitive data (PII/PHI), and manage OWASP vulnerabilities.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/levoai-api-security-observability)

## Overview
**Category:** developer-tools
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Levo.ai (API Security & Observability)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/levoai-api-security-observability](https://vinkius.com/mcp/levoai-api-security-observability)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
