# Canva MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/canva)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Empower your AI agents to manage Canva designs, upload branding assets, and trigger automatic exports directly from your chat.

## Description
Connect your **Canva** account to any AI agent and take full control of your creative workflow through natural conversation.

### What you can do

- **Design Management** — List all your active designs, fetch complete details, and create new preset formats (Posters, Presentations).
- **Media Assets** — Upload external images or videos organically through AI, list storage assets, or delete outdated creative files.
- **Automated Exports** — Trigger asynchronous export jobs to turn your Canva cloud designs into PDFs, MP4s, or JPEGs automatically.
- **Brand Templates** — Retrieve organizationally approved brand templates to ensure aesthetic consistency.
- **User Insights** — Read metadata associated with the authenticated user profile and team capabilities.

### How it works

1. Subscribe to this server
2. Provide your Canva Client credentials and Connect your account
3. Command your agent to upload logos, fetch presentation links, or export visuals dynamically.

### Who is this for?

- **Social Media Managers** — Upload daily graphic assets directly to your Canva media library while scheduling campaigns.
- **Content Creatives** — Instruct the agent to fetch the raw JPEG exports of newly finalized Canva posters without opening multiple tabs.
- **Marketing Teams** — Quickly search your approved Brand templates to scaffold new presentations programmatically.


## Available Tools
- **list_designs**: List all designs on Canva. Canva is the leading online design platform. Returns design IDs, titles, types, and thumbnails
- **get_design**: Get full details of a Canva design including title, type, page count, dimensions, and created/updated timestamps
- **create_design**: Create a new Canva design. Supports preset types like Presentation, Poster, InstagramPost
- **export_design**: Export a Canva design to a file format. Supports PDF, JPEG, PNG, GIF, PPTX, MP4. Returns an export job ID
- **get_export**: Get the status of a Canva export job tracking completion progress returning a native physical download URL
- **list_assets**: List uploaded standard image or video graphical assets stored in the user Canva asset pipeline
- **upload_asset**: Upload an asset directly into the Canva storage context for future embedding into complex native designs
- **delete_asset**: Irreversibly delete an existing custom asset from the Canva platform structure
- **list_templates**: Retrieve the organizationally explicit Canva branded layout templates isolating core structural configurations
- **get_user**: Get standard metadata describing the authenticated Canva user and organizational bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Canva** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch my latest presentation design and export it as a PDF."

**🤖 AI Agent:**
> I've listed your most recent designs and located 'Q3 Strategy'. I initiated a PDF export job (Job ID: eXP...). Checking its status... The export is complete. You can download your PDF file safely from this url.

---

**👤 You:**
> "Upload this generated logo URL directly to my Canva assets."

**🤖 AI Agent:**
> I successfully triggered the upload routine for your remote image URL. The asset (ID: ass88sA9...) 'Generated_Logo_2026' was accepted by Canva and is now permanently accessible in your graphical inventory.

---

**👤 You:**
> "List all the approved brand templates in my Canva organization."

**🤖 AI Agent:**
> Here are 4 Brand Templates mapped in your environment. You have access to: 'Annual Review Matrix', 'Sales Cold Outreach', 'Tech Update Blank', and 'Social Media Grid'. Tell me if you desire to list additional data.


## ❓ FAQ

**Q: Can my AI agent export my presentation as a PDF and give me the download link?**
Yes! You can ask the AI to export any of your specific designs. The agent triggers an asynchronous export job in Canva (supporting PDF, MP4, JPEG, and more), monitors the progress, and ultimately provides you the native physical download URL right in the chat.

**Q: Am I able to upload midjourney or generated assets directly to Canva folders?**
Absolutely. The agent can take image URLs from anywhere and upload them directly into your Canva asset pipeline securely. It creates the structural IDs automatically, so the new images are immediately available when you open Canva's design editor.

**Q: Can the agent create new design templates from scratch?**
The agent can provision standard new designs using preset types (like Presentation, Poster, or InstagramPost) and retrieve your existing brand templates to keep everything aligned. However, actually placing visual elements on a canvas is restricted to the Canva editor UI via web.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/canva](https://vinkius.com/mcp/canva)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Canva** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `canva` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Canva** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "canva": {
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
