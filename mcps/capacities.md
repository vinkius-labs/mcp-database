# Capacities MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/capacities)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/capacities-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/capacities-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Empower your AI agents to build knowledge graphs, append daily notes, and save weblinks directly into your Capacities spaces.

## Description
Connect your **Capacities** account to any AI agent and take full control of your object-based personal knowledge management through natural conversation.

### What you can do

- **Spaces & Structures** — Enumerate your personal spaces and discover the exact object type structures mapping your active environment.
- **Object Instantiation** — Build new typed graph objects complying precisely with the predefined structure parameters.
- **Daily Note Appends** — Send quick thoughts, summaries, and Markdown text directly into your mapped daily note log.
- **Content Lookups** — Execute rapid keyword searches targeting explicit object hierarchies to track down active nodes.
- **Rich Link Saving** — Parse and inject web URLs dynamically into your space as Weblink objects, triggering automatic previews.
- **Media & Tagging** — Attach images and add tags to existing objects to organize your graph relations instantly.

### How it works

1. Subscribe to this server
2. Navigate to your Capacities app Settings to grab your Personal Token
3. Start fetching and creating deep knowledge blocks dynamically from Claude or Cursor

### Who is this for?

- **Researchers & Writers** — Instantly instruct your agent to capture weblinks or draft quick notes straight into today’s daily log without switching context.
- **Developers** — Allow AI coding assistants to document system architectures automatically by injecting structured Markdown objects.
- **Knowledge Workers** — Command the agent to search your Capacities workspace and extract specific object properties to brief you before a meeting.


## Available Tools
- **list_spaces**: List all personal spaces in the Capacities account. Spaces are top-level containers for organizing objects, notes, and knowledge
- **get_space_info**: Retrieve detailed information about a Capacities space including all object types (structures), their property definitions, and configuration
- **get_structures**: Get all object type definitions (structures) within a Capacities space exposing exact metadata parameters limitlessly
- **lookup**: Search for content across a specific Capacities space by title or explicit keywords tracking exact nodes
- **save_weblink**: Save a web URL as a Weblink object dynamically tracking automatic preview generation natively
- **save_to_daily_note**: Append strict Markdown textual payloads to the dynamically mapped daily note explicitly linking content blocks
- **create_object**: Create a new typed object in a Capacities space bounded by specific graph rules instantiating entities
- **get_object**: Retrieve a specific full explicit object by ID accessing its root graph data traversing properties internally
- **save_media**: Locate and attach an explicit Media payload explicitly binding it directly onto existing specific record scopes
- **add_tag**: Add a structural categorical Tag linking explicitly dynamically grouping related Graph items via relations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Capacities** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my 'Work' space for the product launch meeting notes and summarize them."

**🤖 AI Agent:**
> I queried the space and found the object 'Q1 Product Launch Sync' (ID: O90s...). The object contains 5 key updates. Briefly, the marketing campaign goes live on Tuesday, and dev-ops completed the staging environment. Let me know if you want me to tag this as 'Completed'.

---

**👤 You:**
> "Save this URL https://example.com to my 'Research' space as a new Weblink."

**🤖 AI Agent:**
> Weblink creation initiated. Capacities successfully received the URL linking it into 'Research' space (ID: X74n...). The dynamic preview and native metadata will populate automatically via their backend.

---

**👤 You:**
> "Append the code I just wrote to my daily note to remember the bugfix."

**🤖 AI Agent:**
> I've appended your block of Python code and a quick summary as Markdown directly into today's daily note in your primary space. It’s logged permanently mapping your bugfix securely in Capacities.


## Installation & Usage

To install and use the **Capacities** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/capacities](https://vinkius.com/mcp/capacities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
