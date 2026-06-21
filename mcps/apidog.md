# Apidog MCP Server

Sync your Apidog workspace with your AI agent — list projects, fetch endpoint schemas, and export full OpenAPI specifications instantly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/apidog)

## Overview
**Category:** productivity
**Tools Count:** 5

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


## Installation & Usage

To install and use the **Apidog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apidog](https://vinkius.com/mcp/apidog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
