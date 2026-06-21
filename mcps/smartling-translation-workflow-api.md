# Smartling (Translation Workflow API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smartling-translation-workflow-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Automate translation workflows via Smartling — manage projects, create jobs, upload content, and download translations directly from any AI agent.

## Description
Connect your **Smartling** account to any AI agent to orchestrate complex translation and localization workflows through natural language.

### What you can do

- **Project Management** — List and inspect translation projects to understand your localization landscape.
- **Job Orchestration** — Create new translation jobs and group content to streamline the workflow for linguists.
- **Content Handling** — Upload source files (JSON, XML, HTML, etc.) and download completed translations for specific locales.
- **Visual Context** — Upload screenshots or HTML context to help translators provide more accurate localized strings.
- **Automation** — Automatically authorize content for translation during the upload process.

### How it works

1. Subscribe to this server
2. Enter your Smartling User Identifier and User Secret
3. Start managing your global content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Localization Managers** — monitor job progress and create translation tasks without leaving the chat interface.
- **Developers** — automate the upload of resource files and download of translations directly from the IDE.
- **Content Teams** — ensure translators have the right context by attaching visual references to strings.


## Available Tools (7)
- **add_content_to_job**: Add content to an existing translation job
- **create_job**: Create a new translation job in a project
- **download_translated_file**: Download a translated file
- **get_project**: Get details for a specific Smartling project
- **list_projects**: List Smartling projects
- **upload_context**: Upload visual context for translators
- **upload_file**: Upload a file for translation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smartling (Translation Workflow API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Smartling projects."

**🤖 AI Agent:**
> I've retrieved your projects. You have access to 'Mobile App Localization' (ID: a1b2c3d4) and 'Web Platform' (ID: e5f6g7h8). Which one would you like to manage?

---

**👤 You:**
> "Create a new translation job called 'Spring Release' in project a1b2c3d4."

**🤖 AI Agent:**
> The job 'Spring Release' has been successfully created in project a1b2c3d4 with UID 'job_98765'. You can now start adding content to it.

---

**👤 You:**
> "Download the French translation for 'strings.json' from project a1b2c3d4."

**🤖 AI Agent:**
> I've downloaded the 'fr-FR' version of 'strings.json'. The content is ready for use. Would you like me to display the translated strings?


## ❓ FAQ

**Q: Can I upload a file and have it immediately ready for translation?**
Yes! When using the `upload_file` tool, set the `authorize` parameter to true. This will automatically authorize the content for translation in your project.

**Q: How do I group multiple files into a single translation task?**
First, use `create_job` to create a new translation job. Then, use `add_content_to_job` for each file URI you want to associate with that specific job UID.

**Q: Can I provide visual context to help translators?**
Absolutely. Use the `upload_context` tool to send visual references (like screenshots or HTML) to your project, ensuring higher translation quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smartling-translation-workflow-api](https://vinkius.com/mcp/smartling-translation-workflow-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smartling (Translation Workflow API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smartling-translation-workflow-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smartling (Translation Workflow API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smartling-translation-workflow-api": {
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
