# Postman MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postman)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/postman-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/postman-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Bring your Postman API lifecycle to your AI — orchestrate collections, environments, API mocks, and check workspace health seamlessly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postman** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any Mock servers currently simulating our Auth API?"

**🤖 AI Agent:**
> I checked your Postman configurations and found 1 active mock server tied to 'User Onboarding Flows'. It exposes exactly 4 static JSON responses for `/login` and `/token` and operates at URL `https://c123.mock.pstmn.io`. Shall I pull its schema details?

---

**👤 You:**
> "Download our core API Collection. Tell me exactly what parameters I need to submit to the Create User endpoint."

**🤖 AI Agent:**
> I extracted Collection `col-x71...`, the 'Create User' endpoint (POST `/api/v2/users`) expects a JSON body containing `email` (string, required), `role` (string, defaults to 'viewer'), and `department_id` (number, required). Would you like me to write a Javascript snippet invoking it?

---

**👤 You:**
> "Did any of our scheduled Postman monitors fail over the weekend?"

**🤖 AI Agent:**
> Looking at the `list_monitors` data, your 'Checkout Flow Monitor' failed consecutively on Saturday morning. The internal log indicates an assertion error mapping a `502 Bad Gateway` status on step 3 (`POST /cart`). All other monitors are currently healthy and passing.


## Installation & Usage

To install and use the **Postman** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postman](https://vinkius.com/mcp/postman)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
