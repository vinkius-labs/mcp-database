# ScreenshotOne MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/screenshotone)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Capture website screenshots — audit visual content and generate PDFs via AI.

## Description
Empower your AI agent to orchestrate your entire visual auditing and website capturing workflow with **ScreenshotOne**, the reliable API for high-quality screenshots. By connecting ScreenshotOne to your agent, you transform complex capturing tasks into a natural conversation. Your agent can instantly take full-page screenshots, generate PDFs from URLs, and audit page metadata without you ever touching a browser. Whether you are monitoring site changes or archiving visual content, your agent acts as a real-time visual archiver, ensuring your records are always clear and comprehensive.

### What you can do

- **Visual Auditing** — Take high-resolution screenshots of any URL and retrieve the direct image links instantly.
- **Full-page Oversight** — Capture entire website pages from top to bottom to maintain a complete view of site design and content.
- **Document Intelligence** — Generate professional PDFs from any website for easy sharing and offline auditing.
- **Metadata Discovery** — Retrieve website titles, descriptions, and page sizes without performing a full capture.
- **Targeted Capturing** — Take screenshots of specific CSS elements or custom viewports to focus on what matters most.

### How it works

1. Subscribe to this server
2. Enter your ScreenshotOne Access Key
3. Start managing your visual captures through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — monitor website layouts and retrieve visual regression screenshots straight from your workflow.
- **Designers** — verify how sites look across different viewports and audit element alignment.
- **Archivists** — perform rapid audits of visual content and generate PDF archives through natural language.
- **Operations Leads** — automate website capturing to orchestrate cross-functional creative teams smoothly.


## Available Tools (6)
- **get_page_metadata**: ) without capturing.

Get metadata for a website (title, size, etc.) without capturing
- **generate_pdf**: Generate a PDF from a URL
- **take_element_screenshot**: Take a screenshot of a specific CSS element
- **take_full_page_screenshot**: Take a full-page screenshot of a URL
- **take_screenshot**: Take a screenshot of a URL
- **take_viewport_screenshot**: Take a screenshot with a specific viewport size


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ScreenshotOne** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Take a screenshot of https://vinkius.com."

**🤖 AI Agent:**
> I've captured the screenshot for you! You can access the high-quality image via the provided URL. Would you like a full-page capture or a PDF version as well?

---

**👤 You:**
> "Capture the full page of https://github.com/vinkius."

**🤖 AI Agent:**
> Full-page capture initiated! I've retrieved the image showing the entire GitHub profile. It includes all repositories and contributions. Would you like the direct link?

---

**👤 You:**
> "Show metadata for https://www.google.com."

**🤖 AI Agent:**
> I've retrieved the metadata for Google. The site title is 'Google' and the page size is approximately 50KB. Would you like me to take a screenshot now?


## ❓ FAQ

**Q: How do I find my ScreenshotOne Access Key?**
Log in to your [**ScreenshotOne dashboard**](https://screenshotone.com/app/settings), and you will find your Access Key under the 'API Keys' section. Copy and paste it below.

**Q: Can the agent capture elements by ID or Class?**
Yes. Use the `take_element_screenshot` tool providing a valid CSS selector (e.g., `#header` or `.product-card`). Your agent will return a screenshot of just that element.

**Q: Is PDF generation supported for all sites?**
Yes. The `generate_pdf` tool works for any publicly accessible URL, converting the website content into a high-quality PDF document instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/screenshotone](https://vinkius.com/mcp/screenshotone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ScreenshotOne** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `screenshotone` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ScreenshotOne** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "screenshotone": {
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
