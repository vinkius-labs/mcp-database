# BannerBite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bannerbite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Dynamic image and video generation — generate media from templates and manage projects via AI.

## Description
Empower your AI agent to orchestrate your visual content production with **BannerBite**, the powerful media generation engine. By connecting BannerBite to your agent, you transform complex graphic design tasks into a natural conversation. Your agent can instantly generate custom images or videos from your pre-defined templates, audit recent renders, and list project scenes (bites) without you ever touching a design tool. Whether you're automating social media assets or personalizing marketing graphics, your agent acts as a real-time creative production manager for your brand.

### What you can do

- **Media Generation** — Generate high-quality images (PNG) or videos (MP4) from templates by providing dynamic layer modifications via natural language.
- **Project Oversight** — List and explore all BannerBite projects and their associated scenes (bites) to map your creative assets.
- **Render Auditing** — Retrieve and list recent media renders, checking statuses and accessing final delivery URLs instantly.
- **Dynamic Modifications** — Update text, images, and other layers within a template dynamically during the generation process.
- **Creative Automation** — Integrate visual media generation directly into your AI workflows for rapid content scaling.

### How it works

1. Subscribe to this server
2. Enter your BannerBite API Key
3. Start generating dynamic media through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — automate the creation of personalized campaign graphics and videos through natural language.
- **Content Creators** — generate social media assets and thumbnails without manual design software interaction.
- **Operations Leads** — monitor media rendering status and audit creative project backlogs directly from chat.
- **Developers** — integrate dynamic media generation capabilities into automated notification or marketing flows.


## Available Tools (9)
- **generate_image**: Convenience tool to generate a static image from a project
- **generate_media**: Generate an image or video from a template
- **generate_video**: Convenience tool to generate a video from a project
- **get_account_check**: Verify Bannerbite connection
- **get_project**: Get details for a specific project
- **get_render**: Get details and status for a specific render
- **list_bites**: List all bites (scenes) for a specific project
- **list_projects**: List all Bannerbite projects
- **list_renders**: List all recent media renders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BannerBite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my BannerBite projects."

**🤖 AI Agent:**
> I've retrieved your BannerBite projects. You have 3 active projects: 'Summer Sale', 'New Feature Announcement', and 'Event Invite'. Which one would you like to use for generation?

---

**👤 You:**
> "Generate an image for project 'Summer Sale' with text '50% OFF' on layer 'headline'."

**🤖 AI Agent:**
> I'm starting the render for your 'Summer Sale' image with the requested headline. Your static image will be ready in a few seconds. Render ID: `rend_12345`.

---

**👤 You:**
> "Show me the status of my recent renders."

**🤖 AI Agent:**
> I've found 5 recent renders. The last one (`rend_12345`) is 'Completed' and available at this URL: https://bannerbite.com/r/abc.png. The others are also finished.


## ❓ FAQ

**Q: How do I specify which text to change in a template?**
When using the `generate_media` tool, provide a JSON string in the `modifications_json` parameter. Use the layer names from your BannerBite project as keys (e.g., `{"text_1": "New Headline"}`). Your agent can help you identify these layers by listing project bites.

**Q: Can I generate static images instead of videos?**
Yes. Use the `generate_image` tool for static PNG files or `generate_video` for MP4 files. Both tools allow for the same dynamic layer modifications through natural language commands.

**Q: Where do I find the final generated media file?**
The generation tools return a Render object containing a public URL. You can also use the `get_render` tool with a Render ID to retrieve the status and download link for any recent production.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bannerbite](https://vinkius.com/mcp/bannerbite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BannerBite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bannerbite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BannerBite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bannerbite": {
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
