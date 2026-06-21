# Assertible MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/assertible)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/assertible-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/assertible-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate API testing and monitoring via Assertible — trigger deployments, run service tests, and sync specifications directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Assertible** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a deployment for service 'api-prod-123' version 'v2.1.0' in production."

**🤖 AI Agent:**
> I've initiated the deployment for version v2.1.0. Tests are now running against the production environment. I'll let you know the results shortly.

---

**👤 You:**
> "Run all tests for service ID '550e8400-e29b-41d4-a716-446655440000'."

**🤖 AI Agent:**
> Triggering all tests for the specified service. I'm monitoring the progress and will provide a summary of the pass/fail status once complete.

---

**👤 You:**
> "Validate this JSON payload against the standard schema."

**🤖 AI Agent:**
> I'll use the `validate_json` tool to check your document. Please provide the JSON content and the schema you'd like to validate it against.


## Installation & Usage

To install and use the **Assertible** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/assertible](https://vinkius.com/mcp/assertible)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
