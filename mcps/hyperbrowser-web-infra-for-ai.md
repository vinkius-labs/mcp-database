# Hyperbrowser (Web Infra for AI) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hyperbrowser-web-infra-for-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [superpower](../categories/superpower.md)

Cloud browsers for AI agents via Hyperbrowser — manage sessions, scrape pages, and extract structured data.

## Description
Connect your **Hyperbrowser** account to any AI agent and take full control of your web automation and cloud browser infrastructure through natural conversation.

### What you can do

- **Managed Sessions** — Create and manage remote headless browser sessions with built-in support for proxies, stealth mode, and specific browser versions
- **AI Scraping** — Trigger asynchronous scraping jobs that handle dynamic loading, retries, and CAPTCHAs automatically to retrieve clean HTML payloads
- **Data Extraction** — Use LLM-powered capabilities to extract structured data from any URL by simply providing a natural language prompt and optional JSON schema
- **Visual Capture** — Capture full-page screenshots of any rendered URL to audit visual changes or document web states accurately
- **Remote Scripts** — Execute custom JavaScript within active browser sessions to perform complex interactions or evaluate page states in real-time
- **DOM Access** — Retrieve raw, rendered HTML synchronously to process page content without managing complex scraping infrastructures

### How it works

1. Subscribe to this server
2. Enter your Hyperbrowser API Key
3. Start automating the web from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **AI Agent Builders** — provide your agents with a robust web interface to navigate and interact with the internet securely
- **Data Scientists** — automate the extraction of clean, structured data from complex websites through natural language instructions
- **QA & Automation Engineers** — monitor web application states and perform visual audits across different browser configurations in the cloud


## Available Tools (10)
- **page_content**: Get raw HTML content synchronously via Hyperbrowser
- **create_session**: Returns a connection URL and session details. Pass optional JSON config for proxy, stealth, browser version, etc.

Create a new Hyperbrowser remote session
- **extract_data**: g., "Extract product name and price"). Optionally pass JSON schema. The platform will render, extract, and return clean JSON.

Use Hyperbrowser LLM capabilities to extract structured data
- **get_scrape_job**: When status is completed, the response will contain the HTML payload and metadata.

Get status/results of a Hyperbrowser scraping job
- **get_session**: Returns duration, connection endpoints, and current health/status.

Get status of a specific Hyperbrowser session
- **list_sessions**: Pass optional status (active, completed, failed) to filter.

List active or past Hyperbrowser sessions
- **run_script**: The browser will execute and return the evaluation result.

Execute JS script inside a running Hyperbrowser session
- **start_scrape**: Returns a job ID. Use get_scrape_job to poll for completion. Pass target URL and optional JSON config.

Start a Hyperbrowser async scraping job
- **page_screenshot**: Returns image metadata or URL.

Take a managed screenshot via Hyperbrowser
- **stop_session**: Terminate an active Hyperbrowser session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hyperbrowser (Web Infra for AI)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the latest pricing and features from 'https://example.com/pricing'"

**🤖 AI Agent:**
> Processing extraction… I've successfully extracted the following tiers: 1) Free ($0/mo) - Basic features, 2) Pro ($29/mo) - Advanced analytics, 3) Enterprise (Contact sales) - Custom limits. Would you like the full JSON data?

---

**👤 You:**
> "Take a full-page screenshot of 'https://news.ycombinator.com'"

**🤖 AI Agent:**
> Rendering page and capturing screenshot… Done. You can access the full-page capture of Hacker News at the following temporary cloud URL: [screenshot-url]. The image metadata shows a resolution of 1920x4500.

---

**👤 You:**
> "List all my active Hyperbrowser sessions"

**🤖 AI Agent:**
> I've found 2 active browser sessions: 1) Session ID 'sb-123' (Running for 12 mins, US-East Proxy), 2) Session ID 'sb-456' (Running for 2 mins, Stealth Mode). Would you like to terminate either of these?


## ❓ FAQ

**Q: Can my agent extract specific product data from an e-commerce site?**
Yes. Use the `extract_data` tool and provide the target URL along with a prompt like 'Extract product name, price, and customer rating'. Hyperbrowser's LLM will render the page and return clean JSON data according to your request.

**Q: How do I handle websites that require dynamic JavaScript loading?**
Hyperbrowser is built for dynamic content. Tools like `page_content` and `start_scrape` wait for JavaScript to settle before returning results, ensuring your agent sees the fully rendered version of any web application.

**Q: Can I run custom automation scripts in the cloud?**
Absolutely. The `run_script` tool allows you to execute JavaScript strings inside an active browser session. This is perfect for simulating complex user interactions or extracting data that requires custom logic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hyperbrowser-web-infra-for-ai](https://vinkius.com/mcp/hyperbrowser-web-infra-for-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hyperbrowser (Web Infra for AI)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hyperbrowser-web-infra-for-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hyperbrowser (Web Infra for AI)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hyperbrowser-web-infra-for-ai": {
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
