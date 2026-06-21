# Google Firestore Collection MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-firestore-collection)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-firestore-collection-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-firestore-collection-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it manages documents in a single Google Firestore Collection. That's its only function, and nothing else. Incredible for giving your AI a secure NoSQL database.

## Description
This server strips away dangerous global GCP permissions. It gives your AI agent one surgical superpower: **the ability to query, insert, and update documents inside one specific Firestore Collection.**

By strictly scoping access, your AI can safely manage structured data, store chat histories, and process complex NoSQL queries without ever touching your critical cloud databases.

### The Superpowers

- **Absolute Containment:** The agent is locked to a single collection. It cannot query other collections or drop your production data.
- **Native Firestore Integration:** Direct interactions with Firestore, supporting rich document structures and filters.
- **Plug & Play Database:** Instantly gives your agent a scalable NoSQL database to store structured memories and application state.


## Available Tools
- **delete_document**: Delete a document from the Google Firestore collection
- **get_document**: Read a document from the configured Google Firestore collection
- **set_document**: If the document exists, fields are updated.

Create or update a document in the Google Firestore collection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Firestore Collection** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the document with ID 'task-99'."

**🤖 AI Agent:**
> I've retrieved document 'task-99'. The fields indicate its status is currently 'in-progress'.

---

**👤 You:**
> "Save this workflow result to a new document 'result-123': {"status": "done", "score": 95}."

**🤖 AI Agent:**
> I've successfully written the JSON data to the document 'result-123' in the collection.

---

**👤 You:**
> "Delete the temporary 'draft-01' document."

**🤖 AI Agent:**
> The document 'draft-01' has been deleted successfully.


## Installation & Usage

To install and use the **Google Firestore Collection** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-firestore-collection](https://vinkius.com/mcp/google-firestore-collection)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
