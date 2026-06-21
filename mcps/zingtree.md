# Zingtree MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zingtree)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze decision trees, workflows, and user session data via the Zingtree API.

## Description
Connect your **Zingtree** account to any AI agent to streamline your interactive workflows and decision tree management. This MCP server enables your agent to interact with trees, nodes, and detailed user session data directly from natural language.

### What you can do

- **Tree Oversight** — List all interactive trees in your organization and retrieve their hierarchical structures
- **Content Search** — Search for specific text, keywords, or labels across all your nodes and workflows
- **Session Analysis** — Access detailed path data, browser info, and interaction history for any user session
- **Form Data Extraction** — Retrieve all values and answers entered by users during their tree interactions
- **Historical Tracking** — List sessions for specific trees within any date range to monitor performance and usage

### How it works

1. Subscribe to this server
2. Enter your Zingtree API Key
3. Start managing your decision trees and session data from Claude, Cursor, or any MCP client

### Who is this for?

- **Support Managers** — Analyze customer interaction paths and common friction points via natural language
- **Product Owners** — Quickly query tree structures and variables without opening the designer
- **Operations Teams** — Automate the retrieval of form data and session reports for audit or analysis


## Available Tools (8)
- **get_session_form_data**: Get all form data entered during a session
- **search_all_trees**: Search for text within all decision trees
- **get_clean_session_path**: Get a clean linear path for a user session
- **get_session_details**: Get detailed data for a specific user session
- **list_tree_sessions**: List sessions for a tree within a date range
- **get_tree_structure**: Get the full structure of a specific tree
- **list_tree_variables**: List all variables used in a tree
- **list_trees**: List all interactive trees in the organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zingtree** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all decision trees in my Zingtree account."

**🤖 AI Agent:**
> I've retrieved your trees. You have 5 active workflows, including 'Customer Troubleshooting', 'Sales Intake', and 'Product FAQ'. Which one would you like to explore?

---

**👤 You:**
> "Show me the structure for tree ID '12345'."

**🤖 AI Agent:**
> I've fetched the structure for tree 12345. It contains 12 nodes, starting with 'Welcome' and branching into 'Technical Issue' or 'Billing Question'. Would you like to see the content of a specific node?

---

**👤 You:**
> "Get the form data for session ID 'XYZ-987-ABC'."

**🤖 AI Agent:**
> I found the form data for session XYZ-987-ABC. The user provided: Name: 'John Smith', Email: 'john@example.com', and Issue: 'Product Defect'.


## ❓ FAQ

**Q: How do I find my Zingtree API Key?**
Log in to Zingtree and go to Account > Organizations and Billing to find your unique API Key.

**Q: Can I see the path a specific user took in a tree?**
Yes, the `get_session_details` or `get_clean_session_path` tools provide the exact sequence of nodes visited by a user during their session.

**Q: Is it possible to retrieve answers entered in forms?**
Absolutely. Use the `get_session_form_data` tool with a session ID to extract all field values submitted by the user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zingtree](https://vinkius.com/mcp/zingtree)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zingtree** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zingtree` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zingtree** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zingtree": {
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
