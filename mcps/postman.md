# Postman MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postman)
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


## ❓ FAQ

**Q: Can the AI automatically write code using my internal API documentation?**
Absolutely. If you use `get_collection` the AI unpacks the entire Postman hierarchy. Combine this by asking the AI to 'write a Python script to hit my Users Endpoint' and it will natively respect your headers, payload requirements, and auth settings without any context copy-pasting.

**Q: How does the agent handle environments like production vs staging variables?**
The agent can call `list_environments` exposing active configurations inside your workspace. If a collection points to `{{base_url}}`, the AI reads your environments array to resolve exactly what URLs or access keys map to staging versus production natively.

**Q: Can I query test success rates via AI instead of dashboards?**
Yes. The `list_monitors` connection unrolls the cron checks tied to your Postman collections. The AI inherently sees whether the latest automated integration tests succeeded or failed, making status reports conversational.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postman](https://vinkius.com/mcp/postman)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postman** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `postman` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postman** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postman": {
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
