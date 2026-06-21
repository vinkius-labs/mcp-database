# Tana MCP Server

Connect your AI to Tana. Build intelligent knowledge graphs, define supertags, and capture dynamic nested nodes directly from the prompt.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tana)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Translate your AI conversation into structured personal knowledge management seamlessly with the **Tana** MCP connector. Evolve your LLM into a dedicated ontological architect capable of pushing rich, contextual data fragments straight into your workspace. Bypass tedious manual entry by programming your assistant to dynamically categorize thoughts, mint native ontological classes (Supertags), and instantiate multi-level hierarchies inside your Tana graph while maintaining maximum focus in your local environment.

### What you can do

- **Node Structuring** — Swiftly inject clean data fragments anywhere by defining paths invoking `add_node` or securely drop ideations asynchronously into your capture zone utilizing `add_to_inbox`.
- **Ontology & Metadata** — Formalize data classifications mapping real-world objects using `define_supertag` and instantiate them powerfully utilizing `add_tagged_node` and `add_node_with_fields`.
- **Hierarchy & Linking** — Push whole outline structures programmatically executing `add_node_with_children` and enforce complex bi-directional network paths executing `add_node_reference`.
- **Specialized Datatypes** — Effortlessly instantiate formatted daily operations leveraging `add_checkbox_task`, temporal entries mapping `add_date_node`, or external resources resolving via `add_url_bookmark`.

### How it works

1. Append the generic Tana matrix module correctly inside your Vinkius connective logic workspace.
2. Obtain an active `TANA_API_TOKEN` (reserved to Tana Plus/Pro accounts) within Workspace Settings and enforce its security parameter within your local environment.
3. Prompt graph inputs naturally: "Send a structured meeting note to my inbox with the 'Agenda' supertag, and include three checkbox tasks as its children."

### Who is this for?

- **Knowledge Workers** — Programmatically dispatch asynchronous memos, capturing multi-tiered references avoiding heavy manual logging friction.
- **Productivity Systems Engineers** — Solidify operational ontologies strictly managing Supertag instantiations verifying schemas systematically.
- **Researchers & Analysts** — Build deep graph linkages seamlessly tying bookmarks, date blocks, and deep nested lists via streamlined prompt interactions.


## Available Tools
- **add_checkbox_task**: Optionally set initial done status.

Creates a checkbox/todo item in the Tana inbox
- **add_date_node**: Format: YYYY-MM-DD.

Creates a date-typed node in the Tana inbox
- **add_node**: Provide a target node ID (or "INBOX", "LIBRARY") and the node name.

Creates a new node in a specific Tana location
- **add_node_reference**: Provide a label and the target node ID.

Creates a reference node linking to an existing node
- **add_tagged_node**: g. #meeting, #person). Requires the supertag ID from Tana schema.

Creates a new node with a supertag applied
- **add_to_inbox**: Quickly adds a new node directly to the Tana Inbox
- **add_url_bookmark**: Creates a URL-typed node in Tana
- **add_node_with_children**: Provide a name and comma-separated children.

Creates a parent node with multiple child nodes
- **add_node_with_fields**: Provide name, supertag ID, and field data as a JSON object.

Creates a supertagged node with structured field values
- **define_supertag**: Provide a name and description.

Defines a new supertag in the Tana schema


## Installation & Usage

To install and use the **Tana** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tana](https://vinkius.com/mcp/tana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
