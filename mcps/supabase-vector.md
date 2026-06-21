# Supabase Vector MCP Server

Connect your AI to Supabase Vector. Execute pgvector semantic searches, manage embeddings, and run relational database queries directly from your terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/supabase-vector)

## Overview
**Category:** loved-by-devs
**Tools Count:** 7

## Description
Integrate the powerful AI-native PostgreSQL extensions of **Supabase Vector** straight into your conversational LLM workflows. By authenticating your environment natively with the `service_role` key, your AI assistant bypasses row-level security constraints to operate as an unrestricted database administrator. Perform advanced similarity searches using the pgvector extension, parse and manipulate multi-dimensional embeddings, and execute foundational CRUD operations via simple natural language commands. Streamline RAG (Retrieval-Augmented Generation) setups and semantic engineering directly, avoiding the need for external dashboards or manual SQL querying.

### What you can do

- **Semantic Vector Matching** — Seamlessly query unstructured contextual similarities performing embedding comparisons by executing `match_vectors` utilizing custom postgres RPC parameters locally.
- **Database Structural Interaction** — Systematically browse schema availability utilizing `list_tables` and extract specific data arrays effortlessly through `query_table_rows`.
- **Content State Manipulations** — Seamlessly orchestrate data inputs invoking `insert_table_rows` or explicitly clear legacy assignments logically mapping identifiers with `delete_table_rows`.
- **Custom Functional Logic** — Launch sophisticated PL/pgSQL algorithms statically configured in your Supabase backend directly with `call_postgres_function`.

### How it works

1. Set up the Supabase Vector MCP module as an active integration inside your CLI environment.
2. In the configuration matrix, bind your exact deployed `SUPABASE_URL` alongside your powerful validation `SUPABASE_SERVICE_KEY`.
3. Instruct your AI securely: "Match the current context to my 'documents_embeddings' function extracting the 5 most similar articles, then call the active review RPC."

### Who is this for?

- **AI & Data Engineers** — Rapidly iterate embedding architectures testing embedding models and distance metrics strictly without opening external validation platforms.
- **PostgreSQL Database Administrators** — Diagnose semantic accuracy directly from the prompt line configuring inputs organically and adjusting values via conversational arrays.
- **Backend Developers** — Evaluate robust vector databases quickly debugging your semantic infrastructure and RAG deployments natively directly in your active workspace.


## Available Tools
- **delete_table_rows**: This action is irreversible.

Deletes rows from a table based on a column value
- **get_table_row**: Retrieves a specific row by matching a column value
- **insert_table_rows**: Provide a JSON array of row objects.

Inserts new rows into a specific table
- **list_tables**: Lists all tables in the Supabase project
- **match_vectors**: Requires a valid RPC function name and an embedding array.

Performs a vector similarity search via Postgres RPC
- **query_table_rows**: Provide table name and optional select/limit.

Queries rows from a specific table
- **call_postgres_function**: Calls a custom Postgres function (RPC) with parameters


## Installation & Usage

To install and use the **Supabase Vector** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supabase-vector](https://vinkius.com/mcp/supabase-vector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
