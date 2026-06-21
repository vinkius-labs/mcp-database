# Crowdin MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crowdin)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crowdin-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crowdin-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to manage localization projects, files, and translations directly via the Crowdin API.

## Description
Integrate **Crowdin**, the leading localization management platform, directly into your AI workflow. Manage your translation projects, monitor file statuses, and track localization tasks using natural language.

### What you can do

- **Project Management** — List and retrieve detailed settings and statuses for all your localization projects.
- **File Operations** — Monitor files within projects and retrieve specific file metadata.
- **Task & Workflow Tracking** — Track translation and proofreading tasks to ensure timely delivery.
- **Resource Insights** — Access glossaries, translation memories, and supported language lists via chat.

### How it works

1. Connect the Crowdin integration to your AI assistant.
2. Authorize using your Crowdin Personal Access Token (found in your account settings).
3. Manage your global localization strategy through intuitive conversation.

### Who is this for?

- **Localization Managers** — Quickly check project progress and task statuses on the go.
- **Developers** — Audit project files and translation memories via chat.
- **Content Strategists** — Explore glossaries and supported languages during internationalization planning.


## Available Tools
- **list_supported_languages**: Resolves language codes, human-readable names, and locale identifiers.

List all languages supported by Crowdin
- **list_projects**: Resolves project names, IDs, source languages, and target languages for localization workflows.

List all localization projects in your Crowdin account
- **list_project_reports**: Resolves report names, types (Translation Costs, Progress), and creation timestamps.

List generated reports for a specific project
- **list_project_screenshots**: Resolves screenshot IDs, tags, and linked string identifiers used for visual context.

List all screenshots uploaded to a project for context
- **list_project_tasks**: Resolves task titles, types (Translation, Proofreading), status, and assigned linguist references.

List translation and proofreading tasks for a project
- **list_translation_memories**: Resolves TM names, IDs, and segment counts for reuse in future translations.

List all translation memories (TMs) available
- **get_file_details**: Touches file structure, revision history, and per-language translation status boundaries.

Get metadata for a specific file in a project
- **get_project_details**: Touches source/target language settings and project-level activity summary boundaries.

Get detailed settings and status for a project
- **list_project_files**: Resolves file names, IDs, paths, and current translation progress metrics.

List all files within a specific project
- **list_glossaries**: Resolves glossary names, IDs, and language pairs used for terminology management.

List all glossaries available in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crowdin** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all localization projects in my account."

**🤖 AI Agent:**
> I've found 5 localization projects, including 'Mobile App', 'Marketing Website', and 'Documentation Portal'. Would you like to see the file status for any of these?

---

**👤 You:**
> "What is the status of files in project 'Mobile App'?"

**🤖 AI Agent:**
> Project 'Mobile App' (ID: 123) contains 15 files. 'en.json' is 100% translated, while 'notifications.xml' is at 85%. Should I list the pending tasks for this project?

---

**👤 You:**
> "List all active translation tasks for my projects."

**🤖 AI Agent:**
> I've retrieved 3 active tasks: 'Translate UI Strings' (due June 15), 'Review Help Docs' (due June 20), and 'Proofread Marketing Copy'. Would you like the details for a specific task?


## Installation & Usage

To install and use the **Crowdin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crowdin](https://vinkius.com/mcp/crowdin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
