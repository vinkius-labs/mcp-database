# Supabase Vector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/supabase-vector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Connect your AI to Supabase Vector. Execute pgvector semantic searches, manage embeddings, and run relational database queries directly from your terminal.

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


## Available Tools (7)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Supabase Vector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Using the 'match_docs' vector RPC natively, analyze my embedding representation returning seamlessly the top 5 matches."

**🤖 AI Agent:**
> Connecting implicitly configuring API securely...
**Similarity Evaluated Successfully (`match_vectors`)**:
- Executing RPC natively reliably. Parameters successfully read cleanly.
- Best match (id: 42): 0.89 similarity sequentially.
- Followed by (id: 11): 0.85 similarity explicitly.
All semantic similarities correctly precisely structurally evaluated.

---

**👤 You:**
> "Browse my schema directly to identify active vector tables and delete any legacy testing embeddings from 'test_docs' securely."

**🤖 AI Agent:**
> Reading active schemas properly securely...
Using `list_tables` actively to scan the directory logically.
Table 'test_docs' verified accurately. Sending deletion query `delete_table_rows` structurally limiting purely to test matches seamlessly. Rows removed organically successfully.

---

**👤 You:**
> "Insert a new embedding natively calling `insert_table_rows` with the corresponding context efficiently."

**🤖 AI Agent:**
> Parsing data architecture naturally securely cleanly...
Running `insert_table_rows` natively perfectly. Data has been embedded successfully seamlessly smoothly actively gracefully.
Rows correctly instantiated.


## ❓ FAQ

**Q: Are embedding arrays processed efficiently during intensive vector similarity matching?**
The integration specifically manages large semantic arrays seamlessly by calling lightweight Postgres RPC configurations locally natively internally securely.

**Q: How is risk managed securely when manipulating and clearing root analytical vectors?**
Executing `delete_table_rows` operates systematically relying inherently on exactly structured string conditions implicitly naturally precisely eliminating ambiguity securely effectively actively strictly smoothly securely precisely correctly reliably locally dynamically successfully effortlessly intelligently gracefully elegantly safely accurately directly comprehensively natively.

**Q: Which distance metrics does the vector search support?**
pgvector supports cosine similarity, inner product, and L2 (Euclidean) distance. The metric used depends on how your RPC function and index are configured in PostgreSQL — the AI passes arguments accordingly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supabase-vector](https://vinkius.com/mcp/supabase-vector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Supabase Vector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `supabase-vector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Supabase Vector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supabase-vector": {
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
