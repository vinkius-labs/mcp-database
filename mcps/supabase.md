# Supabase MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/supabase)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Connect your AI to Supabase. Execute database queries, manage users, and trigger PostgreSQL functions directly from your terminal.

## Description
Integrate the comprehensive backend infrastructure of **Supabase** straight into your conversational LLM workflows. By securely authenticating with your `service_role` key, your AI assistant bypasses row-level security constraints, operating as a fully-privileged database administrator. Query rows, invoke complex PL/pgSQL functions via RPC, evaluate the authenticated user roster, and audit your active storage buckets all through simple natural language commands, accelerating debugging and environment iterations without leaving the terminal.

### What you can do

- **Database Interactions** — Actively query datasets using `db_select`, seamlessly add new rows executing `db_insert`, and modify existing data structures applying `db_update` or `db_delete`.
- **Custom Functional Logic** — Invoke pre-compiled database procedures and PL/pgSQL functions securely utilizing `db_rpc` with dynamic JSON arguments.
- **Authentication Tracking** — Audit your userbase and confirm authentication statuses instantly fetching native rosters through `list_auth_users`.
- **Storage Diagnostics** — Inspect configured object storage containers mapping file architectures securely invoking `list_storage_buckets`.

### How it works

1. Enable the Supabase MCP plugin as an active integration inside your configuration.
2. In the parameter matrix, bind your exact `SUPABASE_URL` and authenticate the AI utilizing your powerful `SUPABASE_SERVICE_ROLE_KEY`.
3. Instruct your AI securely: "Retrieve the last 10 users from the 'subscribers' table where the status is 'active', and verify if our 'profiles' storage bucket is operational."

### Who is this for?

- **PostgreSQL Database Administrators** — Run complex validation queries and invoke custom RPCs flawlessly parsing responses directly during analytical review workflows.
- **Backend Developers** — Iterate database structures, mock rapid insertions, and securely alter state without opening external platforms or writing repetitive query scripts.
- **Full-Stack Engineers** — Seamlessly query backend storage or resolve user authorization bugs directly tracking the root dependencies visually connected inside the IDE/CLI environment.


## Available Tools
- **delete_auth_user**: Requires service_role key. This action is irreversible.

Delete an authenticated user permanently
- **create_storage_bucket**: Optionally make it public for unauthenticated reads.

Create a new storage bucket
- **delete_storage_file**: Provide a comma-separated list of file paths.

Delete files from a storage bucket
- **get_auth_user**: Get detailed information about a specific authenticated user
- **list_auth_users**: List authenticated users from Supabase Auth
- **db_count**: Useful for pagination and analytics.

Count rows in a database table with optional filters
- **db_delete**: A match_query is mandatory. This action is irreversible.

Delete rows from a database table
- **db_insert**: Provide the payload as a JSON string.

Insert a new row into a database table
- **db_rpc**: Provide the function name and optional JSON arguments.

Execute a Supabase Postgres Function (RPC)
- **db_select**: For filters, use match_query (e.g. "id=eq.1"). Defaults to 50 rows.

Query records from any PostgreSQL database table using PostgREST syntax
- **db_update**: A match_query is required to target specific rows (e.g. "id=eq.123").

Update existing rows in a database table
- **list_storage_buckets**: List all available storage buckets
- **list_storage_files**: List files inside a storage bucket


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Supabase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the 'inventory_products' table sequentially effectively correctly querying all products labeled 'out-of-stock'."

**🤖 AI Agent:**
> Confirming connections internally locally effectively...
**Records Accessed Matrix (`db_select`)**:
- Target table: `inventory_products`
- Applying filtering natively: `status=eq.out-of-stock`

Returning 12 distinct entries reliably safely. Execution successful locally.

---

**👤 You:**
> "Trigger the custom stored procedure 'restock_items' using `db_rpc` to replenish the inventory of IDs 12 and 15 natively."

**🤖 AI Agent:**
> Preparing RPC execution parameter payload locally...
Calling `db_rpc` mapped to 'restock_items' with arguments: `{"ids": [12, 15]}` naturally.
Response matrix from PostgreSQL indicates correct execution cleanly dynamically successfully. Items restocked securely.

---

**👤 You:**
> "Check all registered accounts dynamically applying `list_auth_users` for recent logins natively securely."

**🤖 AI Agent:**
> Authenticating logic cleanly verifying parameters...
**Supabase Auth Operatives Located (`list_auth_users`)**:
- 15 total authentications indexed.
- Latest user confirmed successfully natively.
Task complete organically.


## ❓ FAQ

**Q: Why do I need to use the service role key instead of the safe public anon key?**
The MCP integration operates inherently as an administration module properly securely autonomously. Utilizing the `service_role` actively gracefully securely circumvents logical Row Level Security settings globally, empowering correct system manipulation properly dynamically successfully without error friction organically.

**Q: Is there a safety measure preventing unintended whole table destructive deletions?**
Yes. Commands mutating or destroying rows, such as accurately calling `db_delete`, rigorously mandate explicit logical matching definitions (like exact ID tracking) seamlessly inherently systematically mitigating risk effectively fully locally organically efficiently properly.

**Q: Can the AI call custom PostgreSQL functions (RPC)?**
Yes. Use `db_rpc` to invoke any server-side PL/pgSQL function by name, passing JSON arguments. This lets the AI trigger stored procedures, computed views, or custom business logic directly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supabase](https://vinkius.com/mcp/supabase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Supabase** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `supabase` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Supabase** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supabase": {
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
