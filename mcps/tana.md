# Tana MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tana)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect your AI to Tana. Build intelligent knowledge graphs, define supertags, and capture dynamic nested nodes directly from the prompt.

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


## Available Tools (10)
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
- **add_checkbox_task**: Optionally set initial done status.

Creates a checkbox/todo item in the Tana inbox


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tana** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a new conceptual outline to my Inbox. The main title should be 'Quarterly Product Strategy', and it should contain three specific child nodes functioning as checkable tasks."

**🤖 AI Agent:**
> Processing graph entry natively...
Executing `add_node_with_children` with root name: 'Quarterly Product Strategy'.
Child items initialized safely as text nodes temporarily...
Converting children to executable tasks sequentially using `add_checkbox_task` targeting the new node parent ID. The workflow is completed synchronously in your Inbox.

---

**👤 You:**
> "Create a new node 'Meeting Notes format' structured in our weekly workspace."

**🤖 AI Agent:**
> Compiling cognitive envelope using `create_node`...
New node 'Meeting Notes format' instantiated successfully in the weekly workspace.
Node ID generated: `node-7bx9`. You can now map sub-nodes or supertags to this base.

---

**👤 You:**
> "Search my Tana knowledge base for nodes tagged with '#project'."

**🤖 AI Agent:**
> Querying your graph environment ('search_nodes')...
Found 4 operational nodes bearing the `#project` supertag:
- 'Website Redesign'
- 'Q3 Marketing Push'
- 'API Deprecation'
- 'Cloud Migration'


## ❓ FAQ

**Q: Can it apply Supertags with pre-filled fields?**
Yes. Use `add_node_with_fields` to create a node with a specific Supertag and populate its attributes in a single call.

**Q: Are there limits on nested hierarchies?**
No practical limits beyond your token window. The `add_node_with_children` tool accepts arrays of child nodes and populates the hierarchy in a single request.

**Q: Which Tana plan is required?**
API access is available on Tana Plus and Pro plans. Free accounts do not have API tokens. Generate your token from Workspace Settings in the Tana web app.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tana](https://vinkius.com/mcp/tana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tana** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tana` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tana** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tana": {
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
