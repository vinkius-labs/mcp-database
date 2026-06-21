# Creatomate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/creatomate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to automate video generation, rendering, and asset management via the Creatomate API.

## Description
Integrate **Creatomate**, the powerful video automation platform, directly into your AI workflow. Generate high-quality videos from templates, manage your media assets, and monitor rendering tasks using natural language.

### What you can do

- **Automated Rendering** — Trigger new video renders using dynamic templates and custom modifications via chat.
- **Template Exploration** — List and inspect available video templates and their dynamic fields.
- **Asset Management** — Manage your library of images, videos, and audio files used in your projects.
- **Status Tracking** — Monitor the progress of rendering tasks and retrieve final video URLs in real-time.

### How it works

1. Connect the Creatomate integration to your AI assistant.
2. Authorize using your Creatomate API Key (found in your project settings).
3. Scale your video production through intuitive conversation.

### Who is this for?

- **Content Creators** — Quickly generate variations of social media videos using simple text prompts.
- **Marketing Teams** — Automate the creation of personalized video ads and promotional content.
- **Developers** — Audit rendering pipelines and manage project assets via chat.


## Available Tools
- **get_project_settings**: Retrieve settings and metadata for the current project
- **get_render_status**: Check the status and get the URL of a rendered video
- **get_template_details**: Get structure and dynamic fields for a template
- **list_media_assets**: List uploaded media assets (images, videos, audio)
- **list_video_automations**: List automated video workflows
- **list_recent_renders**: List recent video rendering tasks and their status
- **list_video_templates**: List all video templates available in your project
- **render_video**: Trigger a new video render using a template and modifications
- **search_templates_by_name**: Search for video templates by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creatomate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Render a video using template 't8s9df7' with the text 'Flash Sale!' and background image 'sale.jpg'."

**🤖 AI Agent:**
> Rendering task started (ID: r123abc). I'll let you know as soon as the 'Flash Sale!' video is ready. Should I send the final link to your marketing channel?

---

**👤 You:**
> "What's the status of my video render 'r123abc'?"

**🤖 AI Agent:**
> Your video 'r123abc' is 100% complete. You can download or view it here: [Link]. The file format is MP4 and it lasts 15 seconds. Anything else?

---

**👤 You:**
> "List all video templates in my project."

**🤖 AI Agent:**
> I've found 4 templates in your project: 'Instagram Story Ad', 'YouTube Intro', 'Product Demo', and 'Customer Testimonial'. Which one would you like to use for a new render?


## ❓ FAQ

**Q: How do I get a Creatomate API Key?**
Log in to your Creatomate account, select your project, and navigate to **Project Settings > API Keys** to generate a secret key.

**Q: Can I provide dynamic text for videos?**
Yes, you can use the 'modifications' parameter in the render_video tool to swap text, images, or colors defined in your template.

**Q: What is the rendering time?**
Rendering time depends on video length and complexity, but Creatomate is optimized for speed. You can use the get_render_status tool to check when it's done.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/creatomate](https://vinkius.com/mcp/creatomate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creatomate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `creatomate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creatomate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creatomate": {
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
