# Browserless (Playwright Cloud) MCP Server

Equip your AI with a remote headless browser to scrape, interact, and run Playwright safely via cloud.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/browserless-playwright-cloud)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Grant your AI agent the absolute power of an untethered, scalable **Browserless / Playwright Cloud** cluster. Unlike basic REST fetchers, this MCP connector spins up a legitimate remote Chromium/Webkit instance. Your agent can now execute full JavaScript lifecycles natively, scrape heavy SPAs (Single Page Applications), wait for CSS selectors, or simply ask for a high-fidelity PDF render of any site.

### What you can do

- **Remote Scraping** — Pull down the fully rendered HTML DOM of any complex site (`get_html_content`) bypassing typical bot-blocks. Intercept specific payload slices selectively using explicitly mapped CSS queries (`scrape_elements`).
- **Visual Operations** — Command the agent to spawn an ephemeral browser and snap an immediate `get_screenshot` of a live staging site or construct a print-perfect `get_pdf` document autonomously.
- **Evasion & Stealth** — Avoid standard Cloudflare/Data Dome constraints by wrapping requests in `scrape_with_stealth` to emulate human environments, or bounce TCP endpoints completely out utilizing a residential `scrape_with_proxy`.
- **Live Execution** — Embed dynamic lifecycle alterations into the target memory structure. Run `scrape_with_js` to click modals inside the remote page prior to extraction, or `run_custom_function` exposing the raw Chrome DevTools Protocol to your LLM.

### How it works

1. Append the Browserless integration to your AI settings
2. Provide your securely managed Browserless HTTP Token
3. Start fetching full visual DOM objects via prompts inside Claude or Cursor

### Who is this for?

- **QA Automation Teams** — instruct the AI to spin up ephemeral browser endpoints rendering and screenshotting daily builds silently.
- **Data Engineers** — execute data extractions dynamically reading through complex React/Vue frontend pages that actively combat standard scraping.
- **Security Researchers** — proxy malicious URL queries entirely through isolated cloud environments avoiding all local machine contamination.


## Available Tools
- **get_html_content**: Get raw HTML content using Playwright Cloud (Browserless)
- **send_custom_payload**: Send custom JSON payload to any Browserless REST endpoint
- **run_custom_function**: Execute custom JS function inside remote Playwright browser
- **scrape_with_js**: evaluate` lifecycle executing imperative DOM manipulations like button clicks prior to scraping the final mutated HTML state.

Inject and run a custom JS script before extracting content
- **get_pdf**: Print page to PDF using Playwright Cloud
- **scrape_with_proxy**: Scrape URL using a specified proxy server
- **scrape_elements**: Extract specific elements from page using CSS selectors
- **get_screenshot**: Take a full-page screenshot using Playwright Cloud
- **scrape_with_stealth**: Scrape using stealth mode plugins to avoid bot detection
- **scrape_with_wait**: Scrape content and wait for a CSS selector


## Installation & Usage

To install and use the **Browserless (Playwright Cloud)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserless-playwright-cloud](https://vinkius.com/mcp/browserless-playwright-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
