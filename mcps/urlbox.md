# Urlbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/urlbox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Render website screenshots — audit high-fidelity visual content via AI.

## Description
Empower your AI agent to orchestrate your entire visual rendering and website capturing workflow with **Urlbox**, the professional API for pixel-perfect screenshots. By connecting Urlbox to your agent, you transform complex rendering tasks into a natural conversation. Your agent can instantly take high-fidelity screenshots, generate mobile-optimized views, and produce professional PDFs without you ever touching a dashboard. Whether you are conducting visual QA or archiving dynamic web content, your agent acts as a real-time rendering engine, ensuring your visual records are always accurate and high-resolution.

### What you can do

- **Visual Auditing** — Take pixel-perfect screenshots of any URL and retrieve the direct image links instantly.
- **Full-page Oversight** — Capture entire website pages from top to bottom to maintain a complete view of dynamic content.
- **Mobile Intelligence** — Generate screenshots using mobile user agents to verify responsive designs and layouts.
- **Retina Discovery** — Retrieve high-resolution retina screenshots for professional design audits.
- **Document Intelligence** — Convert any website into a professional PDF document for easy sharing and offline access.

### How it works

1. Subscribe to this server
2. Enter your Urlbox API Key
3. Start managing your visual renders through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Designers & Art Directors** — monitor website aesthetics and retrieve high-resolution renders straight from your workflow.
- **QA Specialists** — verify responsive designs and audit mobile layouts without manual browsing.
- **Content Marketers** — perform rapid audits of landing pages and generate high-quality visual archives through natural language.
- **Operations Leads** — automate website rendering to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **get_metadata**: Get metadata for a URL (Placeholder)
- **generate_pdf**: Generate a PDF from a URL
- **take_full_page_screenshot**: Take a full-page screenshot of a URL
- **take_mobile_screenshot**: Take a screenshot with a mobile user agent
- **take_retina_screenshot**: Take a high-resolution retina screenshot
- **take_screenshot**: Take a PNG screenshot of a URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Urlbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Render a high-fidelity screenshot of https://vinkius.com."

**🤖 AI Agent:**
> I've rendered the screenshot! You can access the pixel-perfect image via the provided URL. Would you like a retina version or a mobile layout capture as well?

---

**👤 You:**
> "Take a mobile screenshot of https://github.com."

**🤖 AI Agent:**
> Mobile capture initiated! I've retrieved the image showing how GitHub renders on a smartphone. Would you like to compare it with a desktop retina capture?

---

**👤 You:**
> "Convert https://www.bbc.com into a PDF."

**🤖 AI Agent:**
> Conversion complete! I've generated a professional PDF of the BBC homepage. You can download the document using the provided URL. Would you like me to capture any other site?


## ❓ FAQ

**Q: How do I find my Urlbox API Key?**
Log in to your [**Urlbox dashboard**](https://urlbox.io/dashboard), and you will find your API Key on the main page. Copy and paste it below.

**Q: Can the agent take screenshots for mobile devices?**
Yes. Use the `take_mobile_screenshot` tool. Your agent will render the website using a mobile user agent to verify how it looks on smartphones.

**Q: Does it support high-resolution (Retina) images?**
Yes. The `take_retina_screenshot` tool enables 2x scaling to provide high-density images suitable for high-resolution displays.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/urlbox](https://vinkius.com/mcp/urlbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Urlbox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `urlbox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Urlbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "urlbox": {
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
