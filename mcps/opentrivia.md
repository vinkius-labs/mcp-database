# OpenTrivia MCP Server

Access a massive database of trivia questions — fetch quizzes by category, manage session tokens, and track global question statistics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/opentrivia)

## Overview
**Category:** learning-training
**Tools Count:** 6

## Description
Connect to the **Open Trivia Database** (OpenTDB) and transform any AI agent into a trivia master or educational assistant. This server provides seamless access to thousands of verified user-contributed questions.

### What you can do

- **Fetch Questions** — Retrieve trivia questions with granular filters for amount (up to 50), category, difficulty (easy, medium, hard), and type (multiple choice or true/false).
- **Session Management** — Use session tokens to ensure you never receive the same question twice within a 6-hour window.
- **Category Discovery** — Browse the full list of trivia categories and their corresponding IDs to target specific knowledge areas.
- **Database Insights** — Query real-time statistics on question counts per category or global database health (verified vs. pending questions).
- **Token Control** — Request and reset session tokens to manage long-running trivia sessions or restart a quiz cycle.

### How it works

1. Subscribe to this server
2. Use the tools to fetch categories or start a session
3. Generate quizzes directly in your AI chat interface

### Who is this for?

- **Developers** — Build trivia bots, games, or learning apps without managing a backend database.
- **Educators** — Instantly generate classroom quizzes or study materials across dozens of subjects.
- **Trivia Fans** — Challenge yourself or others with fresh questions from a community-driven source.


## Available Tools
- **get_categories**: Lookup all trivia categories
- **get_category_count**: Get question count for a category
- **get_global_count**: Get global question count
- **get_questions**: Retrieve trivia questions
- **request_token**: Tokens expire after 6 hours of inactivity.

Retrieve a session token
- **reset_token**: Reset a session token


## Installation & Usage

To install and use the **OpenTrivia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opentrivia](https://vinkius.com/mcp/opentrivia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
