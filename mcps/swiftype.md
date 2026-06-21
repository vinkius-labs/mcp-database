# Swiftype MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swiftype)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/swiftype-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/swiftype-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your AI to Elastic Swiftype. Query your search engines, manage documents, and retrieve deep analytical insights natively from the terminal.

## Description
Empower your conversational AI with robust enterprise search capabilities by securely integrating the **Swiftype (Elastic)** MCP connector. Stop navigating web dashbaords to manage indexing logic; allow your LLM to act as a direct data architect interacting with your core Swiftype endpoints natively. With full support for reading, creating, and deleting JSON documents on the fly, inspecting live search engine queries, and querying direct analytical metrics like top clicks—this connector brings headless search administration straight to your preferred prompt environment.

### What you can do

- **Headless Search & Suggestions** — Execute strict queries interrogating custom content engines running `st.post_search` and provide predictive autocompletes processing `st.post_suggest`.
- **CRUD Document Indexing** — Pull exact active records from isolated data maps using `st.list_documents`, inject new payload structures in bulk operating `st.create_documents`, or vaporize explicit keys commanding `st.delete_documents`.
- **Architectural Discovery** — Browse registered core scopes applying `st.list_engines` and parse schema blueprints identifying object hierarchies with `st.list_doc_types`.
- **Search Analytics & CTR** — Uncover real-world operational user conversion intent evaluating actual volume via `st.analytics_top_searches` and calculating active hit paths invoking `st.analytics_top_clicks`.

### How it works

1. Append the Swiftype MCP agent structurally within your Vinkius integration configuration variables.
2. Configure explicit authorization binding your `SWIFTYPE_API_KEY` (available via the Elastic Swiftype Administrative Profile) to enable encrypted access restrictions.
3. Request immediate execution: "List my active semantic engines, search the 'help-center' engine for 'billing support', and let me know the top clicked documents for this month."

### Who is this for?

- **Search Architecture Engineers** — Investigate live JSON REST indices flawlessly executing bulk CRUD tasks resolving map limits seamlessly within the terminal.
- **Content Marketing Managers** — Parse real-world analytics, quickly discovering top searched queries and high-conversion clicks avoiding tedious web portal logins.
- **Data Reliability Analysts** — Audit structured mapping constraints discovering isolated index bugs securely testing search queries programmatically via AI-assisted CLI.


## Available Tools
- **st.create_documents**: Enumerate explicitly attached structured rules exporting active Billing
- **st.delete_documents**: json` eliminating cached pages permanently erasing bounds metrics from search.

Dispatch an automated validation check routing explicit Gateway history
- **st.list_documents**: json` dumping all stored metadata physically tracking IDs per document type.

Irreversibly vaporize explicit validations extracting rich Churn flags
- **st.list_domains**: json` verifying automated crawler limits mapped inside explicit index scopes.

Identify precise active arrays spanning native Gateway auth
- **st.list_engines**: json` extracting all active isolated Elastic indices bound per tenant.

Identify bounded CRM records inside the Headless Swiftype Platform
- **st.post_search**: json` firing raw queries into the specific Engine returning faceted JSON hierarchies.

Perform structural extraction of properties driving active Account logic
- **st.post_suggest**: json` bounding predictive keys and spelling tolerant matches decoupled from main indexing.

Provision a highly-available JSON Payload generating hard Customer bindings
- **st.analytics_top_clicks**: Identify precise active arrays spanning native Hold parsing
- **st.analytics_top_searches**: Inspect deep internal arrays mitigating specific Plan Math
- **st.list_doc_types**: json` extracting schema blueprints enforcing exact map types correctly.

Retrieve explicit Cloud logging tracing explicit Vault limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swiftype** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my available Swiftype search engines, then run a search for 'documentation' on the most relevant one and show me the top 3 analytics clicks it generated last week."

**🤖 AI Agent:**
> Connecting natively to Swiftype... I found 2 engines: 'prod-store-engine' and 'internal-docs'.
Running `st.post_search` on 'internal-docs' explicitly for 'documentation'.
Found 15 documents. Now fetching CTR metrics (`st.analytics_top_clicks`)...

**Top Converging Documentation Documents**:
1. '/docs/api/endpoints' - 145 Clicks
2. '/help/getting-started' - 93 Clicks
3. '/support/auth-faqs' - 42 Clicks

---

**👤 You:**
> "List all active engines in our Swiftype account."

**🤖 AI Agent:**
> Scanning Elastic instances ('list_engines')...
Found 3 active engines:
1. 'Global-Help-Center' (Language: EN)
2. 'Ecommerce-Catalog-US' (Language: EN)
3. 'Internal-Company-Wiki' (Language: EN)

Let me know if you want me to index new documents into any of these.

---

**👤 You:**
> "Run a test suggestion for 'passw' in the internal wiki engine."

**🤖 AI Agent:**
> Executing `post_suggest` constraint on 'Internal-Company-Wiki'...
The engine suggests the following completions based on hits:
1. 'password reset policy'
2. 'password manager installation'
3. 'passport visa procedures'


## Installation & Usage

To install and use the **Swiftype** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swiftype](https://vinkius.com/mcp/swiftype)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
