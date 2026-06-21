# Localazy (AI Translation & Localization API) MCP Server

Manage software localization and translations via Localazy — list projects, import content, manage source keys, and handle glossary terms directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/localazy-ai-translation-localization-api)

## Overview
**Category:** developer-tools
**Tools Count:** 23

## Description
Connect your **Localazy** account to any AI agent to automate your localization workflows. This server allows you to manage projects, files, and translation keys through natural language.

### What you can do

- **Project Management** — List accessible projects and create new ones with specific source languages and tones.
- **Content Import/Export** — Import files in various formats and download translated content directly.
- **Key & Glossary Control** — Update source keys, set priorities, and manage glossary terms to ensure translation consistency.
- **Webhooks & Screenshots** — Manage webhooks for automation and upload screenshots for visual context.
- **CDN Metadata** — Retrieve metadata for content delivered via Localazy CDN.

### How it works

1. Subscribe to this server
2. Enter your Localazy Personal Access Token
3. Start localizing your apps from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate the sync of translation keys and files without leaving the terminal or IDE.
- **Localization Managers** — Quickly check project status, update glossary terms, and manage screenshots for translators.
- **Product Owners** — Ensure multi-language support is on track by querying project statistics and language coverage.


## Available Tools
- **create_glossary_term**: Create a new glossary term
- **create_project**: Create a new project inside the given organization
- **delete_glossary_term**: Delete a glossary term
- **delete_screenshot**: Delete a screenshot
- **delete_source_key**: Remove a key from the project
- **download_file**: Download the raw file content in the specified language
- **get_webhook_secret**: Get the webhook secret used for HMAC verification
- **import_content**: Import supported file formats including translations
- **list_cdn_metadata**: List metadata URLs for published release tags (CDN)
- **list_file_content**: Returns keys and translations for a specific language and file
- **list_files**: Returns a list of files in the project
- **list_glossary_terms**: List glossary terms for a project
- **list_import_formats**: List supported file types and their parameters
- **list_projects**: Use optional flags to include organization info or language statistics.

List projects accessible with the current token
- **list_screenshots**: List screenshots in a project
- **list_webhooks**: List configured webhooks for a project
- **set_key_priority**: Batch operation to set priority for keys
- **set_key_tags**: Batch operation to set tags for keys (Max 1,000 keys)
- **update_glossary_term**: Update an existing glossary term
- **update_screenshot**: Update metadata for a screenshot (link phrases, tags)
- **update_source_key**: Modify properties of a source key
- **update_webhooks**: Update webhook configurations for a project
- **upload_screenshot**: Upload a new screenshot (Base64 encoded image)


## Installation & Usage

To install and use the **Localazy (AI Translation & Localization API)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/localazy-ai-translation-localization-api](https://vinkius.com/mcp/localazy-ai-translation-localization-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
