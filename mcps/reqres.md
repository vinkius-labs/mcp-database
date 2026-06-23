# Reqres MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/reqres)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Test your front-end against a real API — manage users, resources, and project records for prototyping and testing.

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


## Available Tools (25)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reqres** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the users on the second page of the demo API."

**🤖 AI Agent:**
> I've retrieved the users from page 2. You have users like Michael Lawson (ID: 7) and Lindsay Ferguson (ID: 8). Would you like the details for a specific user ID?

---

**👤 You:**
> "Create a new user named 'Alice' with the job 'Senior Developer'."

**🤖 AI Agent:**
> User 'Alice' has been successfully created (simulated). The API returned ID 452 with a creation timestamp of today. The job is set to 'Senior Developer'.

---

**👤 You:**
> "Fetch all records from the 'inventory' collection slug."

**🤖 AI Agent:**
> Querying the 'inventory' collection... I found 3 records. They include 'Item A', 'Item B', and 'Item C'. Would you like to see the full JSON data for any of these?


## ❓ FAQ

**Q: How can I see the list of available demo users?**
You can use the `list_users` tool. It supports pagination, so you can specify which `page` you want to retrieve from the demo database.

**Q: Can I test authentication flows like login and registration?**
Yes! Use `login_demo` or `register_demo` with fixture emails (like 'eve.holt@reqres.in') to simulate successful authentication and receive a token.

**Q: How do I manage custom data for my specific project?**
Use the Project API tools like `list_records` and `create_record`. You just need to provide a `slug` to identify your collection and the JSON data payload.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reqres](https://vinkius.com/mcp/reqres)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reqres** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reqres` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reqres** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reqres": {
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
