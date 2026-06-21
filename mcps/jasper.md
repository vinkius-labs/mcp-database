# Jasper MCP Server

Equip your AI agent with direct access to Jasper — generate marketing copy, manage brand voices, and orchestrate content campaigns without opening the Jasper app.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jasper)

## Overview
**Category:** productivity
**Tools Count:** 20

## Description
Connect **Jasper** to your AI agent and supercharge your marketing content production pipeline.

### What you can do

- **Content Generation** — Generate blog posts, ad copy, social media captions, email sequences, and landing page copy with brand-consistent voice.
- **Brand Voice Management** — Access and apply your configured brand voices, tone guidelines, and style rules to all generated content.
- **Template Library** — Browse and execute Jasper's template library for specific content types (PAS framework, AIDA, email subject lines).
- **Campaign Orchestration** — Generate multi-channel content variations from a single brief — ads, emails, and social posts in one request.

### How it works

1. Subscribe to the Jasper integration on the marketplace.
2. Generate an API token from your Jasper account (Settings → Dev Tools → API Tokens → Generate).
3. Ask your AI agent to generate copy, apply brand voices, or create campaign content.

### Who is this for?

- **Marketing Teams** — Produce channel-specific copy at scale without context-switching between tools.
- **Content Strategists** — Generate first drafts for blog posts, landing pages, and email campaigns in seconds.
- **Growth Teams** — Create A/B test variants for ads and emails programmatically from your AI agent.


## Available Tools
- **get_usage**: Requires start/end dates in ISO format and granularity (day, week, hour).

Get API usage statistics
- **list_templates**: Each template includes its input schema for use with run_template.

List content templates
- **run_template**: Retrieve template input schemas via list_templates first, then pass the required inputs as JSON.

Run a specific template
- **run_command**: Pass a command (prompt) and optional context for grounding. Supports voice IDs for brand-consistent output and output language selection.

Generate AI content with Jasper
- **list_voices**: Use voice IDs with run_command or run_task for brand-consistent content.

List brand voices
- **get_voice**: Get voice details
- **list_knowledge**: Use knowledge IDs with run_command or run_task for grounded output.

List knowledge items
- **list_styles**: List style guides
- **list_documents**: Supports filtering by name, status, and date range.

List workspace documents
- **get_document**: Get document details
- **list_tasks**: Each task includes context items (input fields) required for execution.

List agent tasks
- **get_task**: Get agent task details
- **run_task**: Pass context items as a JSON array. Each item needs either {id, value} for predefined items or {name, question, answer} for custom context. Retrieve task input schema via get_task first.

Run an agent task
- **list_users**: List workspace users
- **get_template**: Get template details
- **get_knowledge_item**: Get knowledge item details
- **search_knowledge**: Matches by meaning and context, not just keywords.

Search knowledge base
- **get_style**: Get style guide details
- **list_audiences**: Use audience IDs with run_task for targeted content.

List target audiences
- **get_audience**: Get audience details


## Installation & Usage

To install and use the **Jasper** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jasper](https://vinkius.com/mcp/jasper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
