# Localazy (AI Translation & Localization API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/localazy-ai-translation-localization-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage software localization and translations via Localazy — list projects, import content, manage source keys, and handle glossary terms directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Localazy (AI Translation & Localization API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Localazy projects and include language statistics."

**🤖 AI Agent:**
> I've retrieved your projects. You have 'Mobile App' (ID: 123) with 95% completion in 5 languages, and 'Web Dashboard' (ID: 456) with 80% completion in 3 languages.

---

**👤 You:**
> "Show me the content of file 'strings.json' (ID: f789) for the French (fr) language in project 'p123'."

**🤖 AI Agent:**
> Fetching content for 'strings.json' in French... I found 10 keys. For example, 'login_button' is translated as 'Se connecter' and 'welcome_msg' as 'Bienvenue'.

---

**👤 You:**
> "Add a new glossary term 'Workspace' with the description 'The primary area for user collaboration' to project 'p456'."

**🤖 AI Agent:**
> The glossary term 'Workspace' has been successfully created in project 'p456' with the provided description to help your translators.


## ❓ FAQ

**Q: How can I check which file formats are supported for import?**
You can use the `list_import_formats` tool. It will return a comprehensive list of all supported file types and their specific parameters for the Localazy API.

**Q: Can I update the context or character limit for a specific translation key?**
Yes! Use the `update_source_key` tool. You can modify properties like the character limit, context comments, and even mark keys as hidden or deprecated.

**Q: How do I retrieve the translations for a specific file in a target language?**
Use the `list_file_content` tool by providing the Project ID, File ID, and the target language code. It will return the keys and their corresponding translations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/localazy-ai-translation-localization-api](https://vinkius.com/mcp/localazy-ai-translation-localization-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Localazy (AI Translation & Localization API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `localazy-ai-translation-localization-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Localazy (AI Translation & Localization API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "localazy-ai-translation-localization-api": {
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
