# Assertible MCP Server

Automate API testing and monitoring via Assertible — trigger deployments, run service tests, and sync specifications directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/assertible)

## Overview
**Category:** developer-tools
**Tools Count:** 7

## Description
Connect your **Assertible** account to any AI agent to streamline your API testing and monitoring workflows through natural conversation.

### What you can do

- **Deployments & Testing** — Create deployments and trigger automated test runs for specific environments using `create_deployment`.
- **Service Monitoring** — Run all tests for a service or target specific tests by ID to ensure uptime and reliability with `run_service_tests` and `run_specific_test`.
- **Spec Synchronization** — Keep your tests updated by syncing OpenAPI, Swagger, or Postman specifications using `sync_specification`.
- **Status Visibility** — Retrieve embeddable status badges and markdown for services and individual tests via `get_service_status_badge`.
- **JSON Validation** — Validate JSON documents against Schema Draft 4 directly within your workflow using `validate_json`.

### How it works

1. Subscribe to this server
2. Enter your Assertible API Token (and optionally your Sync Token)
3. Start managing your API quality and monitoring from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — Automate deployment tracking and post-deploy test triggers directly from the CLI or chat.
- **QA Engineers** — Run specific test suites and verify API health without leaving the development environment.
- **Backend Developers** — Validate JSON schemas and sync API specifications as soon as code changes are made.


## Available Tools
- **create_deployment**: Create a deployment and trigger tests
- **get_service_status_badge**: Get the status badge URL and markdown for a service
- **get_test_status_badge**: Get the status badge URL and markdown for a specific test
- **run_service_tests**: Run all tests for a service
- **run_specific_test**: Run a specific test
- **sync_specification**: Requires ASSERTIBLE_SYNC_TOKEN.

Sync a specification (OpenAPI, Swagger, Postman)
- **validate_json**: No authentication required.

Validate a JSON document against a JSON Schema Draft 4


## Installation & Usage

To install and use the **Assertible** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/assertible](https://vinkius.com/mcp/assertible)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
