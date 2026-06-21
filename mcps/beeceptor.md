# Beeceptor MCP Server

Mock APIs, intercept requests, and manage proxy rules directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/beeceptor)

## Overview
**Category:** developer-tools
**Tools Count:** 29

## Description
Connect **Beeceptor** to your AI agent to build, manage, and monitor mock APIs and HTTP proxies through natural language.

### What you can do

- **Endpoint Management** — Configure CORS, request logging, and authentication for your subdomains using `update_settings`.
- **Mock Rules** — Create, update, and reorder rules via `create_rule` and `reorder_rules` to simulate complex API behaviors.
- **Request Inspection** — List and inspect incoming HTTP requests in real-time with `list_requests` to debug webhooks or integrations.
- **API Specifications** — Upload OpenAPI or Swagger specs using `upload_spec` to automatically generate mock endpoints.
- **State Management** — Maintain state across mock calls using key-value storage tools like `upsert_state` and `get_state_item`.

### How it works

1. Subscribe to this server
2. Enter your Beeceptor API Key
3. Start mocking and debugging APIs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — quickly mock backend dependencies without writing server code.
- **QA Engineers** — simulate edge cases, timeouts, and error responses to test application resilience.
- **Backend Developers** — debug webhooks and third-party callbacks by inspecting payloads in real-time.


## Available Tools
- **add_certificate**: Add mTLS certificate
- **bulk_replace_rules**: Bulk replace mock rules
- **create_rule**: Create mock rule
- **delete_all_rules**: Delete all mock rules
- **delete_certificate**: Delete mTLS certificate
- **delete_request**: Delete single request
- **delete_requests**: Delete request history
- **delete_rule**: Delete mock rule
- **delete_spec**: Delete specification
- **delete_state_item**: Delete single state item
- **delete_state**: Delete state items (Bulk)
- **download_multipart**: Download multipart file
- **get_job_status**: Get spec upload job status
- **get_request**: Get single request
- **get_rule**: Get single mock rule
- **get_settings**: Get endpoint settings
- **get_spec_details**: Get specification details
- **get_state_item**: Get single state item
- **list_certificates**: List mTLS certificates
- **list_requests**: Get request history
- **list_rules**: Get all mock rules
- **list_state**: Get all state
- **reorder_rules**: Reorder mock rules
- **update_rule_full**: Update mock rule (Full)
- **update_rule_partial**: Update mock rule (Partial)
- **update_settings**: Update endpoint settings
- **upload_blob**: Upload binary blob
- **upload_spec**: Upload API specification
- **upsert_state**: Upsert state (Bulk)


## Installation & Usage

To install and use the **Beeceptor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beeceptor](https://vinkius.com/mcp/beeceptor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
