# Microlink MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/microlink)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Turn any website into data — extract metadata, take screenshots, generate PDFs, and run performance audits directly from your AI agent.

## Description
Connect **Microlink** to your AI agent to transform the web into a programmable interface. This server allows your agent to browse, capture, and analyze any URL with industrial-grade reliability.

### What you can do

- **Metadata Extraction** — Fetch normalized titles, descriptions, social images, and author data from any URL using `extract_metadata`.
- **Visual Captures** — Generate high-quality screenshots of websites, specific DOM elements, or mobile-emulated views with `take_screenshot`.
- **Document Generation** — Convert web pages into clean, formatted PDF documents for archiving or reporting via `generate_pdf`.
- **Technical Insights** — Identify underlying technologies (Wappalyzer) and run Lighthouse performance reports using `get_insights`.
- **Browser Automation** — Perform advanced queries with ad-blocking, custom scripts, and animation control through `advanced_query`.

### How it works

1. Subscribe to this server
2. Enter your Microlink API Key (optional for low-volume, but recommended)
3. Start processing URLs directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Automate link previews, generate dynamic PDFs, or debug site performance without leaving the terminal.
- **Content Creators** — Instantly gather metadata and visual assets from reference links for research or social sharing.
- **Data Analysts** — Extract structured information from websites and audit technical stacks at scale.


## Available Tools (5)
- **advanced_query**: Advanced Microlink API query with full parameter control
- **extract_metadata**: Extract structured metadata from any URL
- **generate_pdf**: Supports custom formats, margins, and scaling.

Generate a PDF from a website
- **get_insights**: Get performance and technology insights for a URL
- **take_screenshot**: Can capture full page, specific elements, or emulate devices.

Take a screenshot of a website


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Microlink** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the metadata and social image from https://microlink.io"

**🤖 AI Agent:**
> I've extracted the metadata for Microlink. The title is 'Microlink — Enter the browser as a service', and I've found the primary OpenGraph image and description for you.

---

**👤 You:**
> "Take a full-page screenshot of https://github.com emulating an iPhone 15."

**🤖 AI Agent:**
> I've generated a full-page screenshot of GitHub using an iPhone 15 viewport. You can view the mobile-optimized layout in the generated image.

---

**👤 You:**
> "Run a Lighthouse performance audit for https://vercel.com"

**🤖 AI Agent:**
> The Lighthouse report for Vercel is ready. It shows high scores in Performance and Best Practices, with specific metrics for First Contentful Paint and Speed Index.


## ❓ FAQ

**Q: Can I take a screenshot of a specific element on a page instead of the whole screen?**
Yes! Use the `take_screenshot` tool and provide a CSS selector in the `element` parameter. The agent will return a precise capture of just that component.

**Q: How do I see what software or frameworks a website is built with?**
Use the `get_insights` tool with `technologies: true`. It uses Wappalyzer to identify the CMS, analytics, web servers, and JavaScript frameworks used by the URL.

**Q: Can I generate a PDF in a specific paper format like A4?**
Absolutely. Use the `generate_pdf` tool and specify 'A4' in the `format` parameter. You can also adjust margins and orientation (landscape/portrait).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microlink](https://vinkius.com/mcp/microlink)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Microlink** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `microlink` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Microlink** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "microlink": {
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
