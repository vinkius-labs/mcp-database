# RenderMe MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/renderme)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate video generation via RenderMe (re.video) templates directly from your AI agent.

## Description
Connect your **RenderMe** (re.video) account to any AI agent and take full control of your automated video production and media orchestration through natural conversation. RenderMe provides a powerful API for rendering professional videos from motion templates, allowing you to trigger render jobs, manage deployments, and track media assets directly from your chat interface.

### What you can do

- **Automated Video Rendering** — Trigger video generation jobs using deployment IDs and dynamic variables (text, images, colors) programmatically.
- **Job Lifecycle Management** — Monitor the status of your rendering requests and retrieve final result URLs directly from the AI interface.
- **Template & Deployment Control** — List all available video templates and access detailed technical metadata to ensure your visual content is always on-brand.
- **Asset & Folder Oversight** — Manage your video projects, uploaded media, and organizational folders via natural language.
- **Operational Monitoring** — Track account statistics and monitor system health using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your RenderMe (re.video) API Key from your dashboard settings
3. Start generating video content from Claude, Cursor, or any MCP-compatible client

No more manual editing or complex media processing. Your AI acts as a dedicated video producer or technical media coordinator.

### Who is this for?

- **Social Media Managers** — quickly generate branded video snippets and monitor production queues without switching apps.
- **Marketing Teams** — automate the creation of personalized video assets for email campaigns or social ads.
- **Operations Teams** — streamline the management of cloud assets and monitor organizational media health directly within the chat.


## Available Tools
- **check_api_health**: Verify RenderMe API connectivity
- **get_template_details**: Get details for a specific video template
- **get_render_job_status**: Check status of a render job
- **get_current_user**: Get authenticated user profile
- **get_account_render_stats**: Get account usage and render statistics
- **list_uploaded_assets**: List all uploaded images and media
- **list_video_templates**: List all video templates (deployments)
- **list_asset_folders**: List asset organization folders
- **list_recent_render_jobs**: List recent video render jobs
- **list_video_projects**: List all video projects
- **list_configured_webhooks**: List active webhooks
- **create_video_render_job**: Trigger a new video rendering job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RenderMe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my video deployments in RenderMe."

**🤖 AI Agent:**
> I've retrieved your deployments. You have 3 active video templates: 'Social Intro', 'Ad Campaign v1' (ID: dep_123), and 'Product Showcase'. Which one would you like to render?

---

**👤 You:**
> "Render a batch of 50 personalized certificate images for our training program graduates."

**🤖 AI Agent:**
> Batch rendering initiated: 50 personalized certificates. Template: "Professional Certificate Gold". Dynamic fields: graduate name, course title, completion date, instructor signature, unique certificate ID. Progress: 50/50 completed (100%). All certificates generated in PDF (print-ready, 300 DPI) and PNG (web) formats. Average render time: 1.2 seconds per certificate. Download link generated for the ZIP archive (124 MB). Email delivery option available for direct distribution to graduates.

---

**👤 You:**
> "Show me the rendering statistics and API usage for my account this month."

**🤖 AI Agent:**
> Monthly rendering statistics. Total renders: 3,456. Successful: 3,421 (99.0%). Failed: 35 (1.0%, mostly timeout on complex templates). API calls: 4,890. Average render time: 2.1 seconds. Peak usage: Tuesday at 2 PM (234 renders/hour). By format: PNG 58%, PDF 32%, JPG 10%. Storage used: 2.3 GB of 10 GB. Plan limit: 5,000 renders/month (69.1% used). Estimated overage at current pace: none.


## ❓ FAQ

**Q: Can my AI automatically find my RenderMe templates?**
Yes! Use the `list_deployments` tool. Your agent will respond with complete metadata for all your video templates, including their IDs and technical specifications in seconds.

**Q: How do I find my RenderMe (re.video) API Key?**
Log in to your RenderMe account at app.re.video, navigate to the **Settings** or **API** section, and you will find your unique secret token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/renderme](https://vinkius.com/mcp/renderme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RenderMe** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `renderme` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RenderMe** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "renderme": {
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
