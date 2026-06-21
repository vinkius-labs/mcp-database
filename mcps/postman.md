# Postman MCP Server

Bring your Postman API lifecycle to your AI — orchestrate collections, environments, API mocks, and check workspace health seamlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/postman)

## Overview
**Category:** loved-by-devs
**Tools Count:** 6

## Description
Connect your **Postman** developer keys to any AI agent and bring the power of collaborative API design, testing, and monitoring into a pure LLM conversational context.

### What you can do

- **Collections & Endpoints** — Extract complete internal JSON schemas of your Postman Collections to teach your AI exactly how internal APIs work
- **Workspaces & Environments** — Map development environments (Staging/Prod) and expose scoped variables autonomously
- **Mock Servers** — List active API endpoints serving simulated JSON responses, crucial for checking decoupled front-ends
- **Health Monitors** — Retrieve scheduled cron checks tracking test success and failure histories out-of-the-box

### How it works

1. Subscribe to this server
2. Enter your Postman Developer API Key
3. Start mapping REST definitions natively in Claude, Cursor, or any MCP client

No exporting JSONs or jumping back and forth to read raw cURL formats. Ask the AI how to hit an endpoint, and it reads your collection.

### Who is this for?

- **Backend Engineers** — quickly check if staging environment URLs differ from production without navigating the Postman app
- **Frontend Devs** — ask the AI to retrieve exact HTTP payloads and Mock server URLs when building your UI bindings
- **QA Testers** — monitor failing API scenarios actively reporting through Postman Scheduled Monitors


## Available Tools
- **list_collections**: List all available API Collections on the connected Postman account
- **list_workspaces**: List all available engineering team workspaces in Postman
- **list_environments**: List development environments (Staging, Prod) and their variables configured in Postman
- **list_mocks**: List configured Mock Servers on Postman to simulate API responses and test Front-Ends
- **list_monitors**: List API health monitors, showing their schedules and last run status (Success/Failure)
- **get_collection**: Download the complete internal schema of a Postman Collection. Exposes all API Endpoints, HTTP Methods, Headers, and Request Bodies for AI learning


## Installation & Usage

To install and use the **Postman** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postman](https://vinkius.com/mcp/postman)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
