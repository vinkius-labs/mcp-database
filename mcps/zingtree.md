# Zingtree MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zingtree)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zingtree-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zingtree-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Zingtree** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zingtree](https://vinkius.com/mcp/zingtree)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
