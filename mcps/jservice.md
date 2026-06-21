# Jservice MCP Server

Access the Jeopardy! clue database — fetch clues by category, value, or date, and get random trivia for your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jservice)

## Overview
**Category:** knowledge-management
**Tools Count:** 4

## Description
Connect to the **Jservice** API and bring the world of Jeopardy! trivia to your AI agent. This server allows you to query thousands of historical clues, explore categories, and generate random trivia challenges directly through natural conversation.

### What you can do

- **Clue Retrieval** — Fetch specific clues filtered by dollar value, category ID, or date ranges using the `get_clues` tool.
- **Random Trivia** — Generate random clues to create quizzes or test general knowledge with `get_random_clues`.
- **Category Exploration** — Browse through the extensive list of Jeopardy! categories and their associated IDs using `get_categories`.
- **Deep Category Inspection** — Retrieve all clues belonging to a specific category for focused study or gaming via `get_category`.

### How it works

1. Subscribe to this server
2. No API key is required as Jservice is a public trivia database
3. Start querying trivia data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — building trivia apps or testing LLM knowledge retrieval with real-world data
- **Educators** — creating engaging quizzes based on historical Jeopardy! clues
- **Trivia Enthusiasts** — exploring the vast history of the game show through natural conversation


## Available Tools
- **get_categories**: Limited to 100 at a time.

Get a list of categories
- **get_category**: Get a specific category and its associated clues
- **get_clues**: Can be filtered by value, category, date, and offset.

Get a list of clues based on filter criteria
- **get_random_clues**: Limited to 100 at a time.

Get a random set of clues


## Installation & Usage

To install and use the **Jservice** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jservice](https://vinkius.com/mcp/jservice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
