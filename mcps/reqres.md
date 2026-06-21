# Reqres MCP Server

Test your front-end against a real API — manage users, resources, and project records for prototyping and testing.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/reqres)

## Overview
**Category:** developer-tools
**Tools Count:** 25

## Description
Connect to **Reqres**, the industry-standard hosted REST-API, to simulate real-world data interactions without setting up a dedicated backend. Perfect for frontend developers, QA engineers, and AI agent builders.

### What you can do

- **User Management** — List, fetch, create, and update demo users to test your application's identity flows.
- **Resource Exploration** — Access Pantone color data and other resources to validate data fetching and UI rendering.
- **Project Records** — Perform full CRUD operations on custom project collections using slugs to simulate production databases.
- **Authentication Simulation** — Test login and registration flows with fixture users to receive valid tokens.
- **Agent Scenarios** — Trigger and monitor specific agent scenarios and orders for advanced workflow testing.

### How it works

1. Subscribe to this server
2. Enter your Reqres API Key or Session Token (optional for demo tools)
3. Start prototyping your API interactions from Claude, Cursor, or any MCP client

### Who is this for?

- **Frontend Developers** — quickly mock data and test UI components without waiting for backend deployment.
- **QA Engineers** — automate API testing scenarios and validate response structures.
- **AI Builders** — provide your agent with a sandbox environment to practice data manipulation and tool usage.


## Available Tools
- **agent_health**: Get Agent Sandbox health probe and rate-limit status
- **agent_orders**: Get orders with relational data from Agent Sandbox
- **agent_scenarios**: List available failure scenarios in Agent Sandbox
- **agent_users**: Get paginated users with cursor pagination from Agent Sandbox
- **create_app_record**: Create a user-scoped record in an app collection
- **create_record**: Create a record in a project collection
- **create_user**: Create a user (echoed) in Demo API
- **delete_record**: Delete a record from a project collection
- **delete_user**: Delete a user in Demo API
- **get_me**: Get current app user info
- **get_record**: Get a single record from a project collection
- **get_user**: Get a single user by ID from Demo API
- **list_app_records**: List user-scoped records in an app collection
- **list_colors**: List resource colors (Pantone) from Demo API
- **list_records**: List records in a project collection
- **list_users**: List users (paginated) from Demo API
- **login_demo**: Login with fixture users (returns token)
- **patch_record**: Partial update a record in a project collection
- **patch_user**: Partial update a user (echoed) in Demo API
- **register_demo**: Register with fixture users (returns id/token)
- **request_magic_link**: Request a magic link for App User login
- **trigger_scenario**: Trigger a specific failure scenario in Agent Sandbox
- **update_record**: Update a record (full replace) in a project collection
- **update_user**: Update a user (echoed) in Demo API
- **verify_magic_link**: Verify a magic link token to get a session token


## Installation & Usage

To install and use the **Reqres** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reqres](https://vinkius.com/mcp/reqres)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
