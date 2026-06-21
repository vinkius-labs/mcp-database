# Supabase MCP Server

Connect your AI to Supabase. Execute database queries, manage users, and trigger PostgreSQL functions directly from your terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/supabase)

## Overview
**Category:** loved-by-devs
**Tools Count:** 13

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


## Installation & Usage

To install and use the **Supabase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supabase](https://vinkius.com/mcp/supabase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
