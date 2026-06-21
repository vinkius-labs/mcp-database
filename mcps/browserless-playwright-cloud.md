# Browserless (Playwright Cloud) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browserless-playwright-cloud)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI with a remote headless browser to scrape, interact, and run Playwright safely via cloud.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browserless (Playwright Cloud)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Take a full page screenshot of the landing page on 'https://vinkius.com'."

**🤖 AI Agent:**
> Screenshot execution completed. Spun up remote Playwright instance requesting `https://vinkius.com` in Full-Page context. It successfully rendered and extracted the composite `.png` buffer holding the pixel mapping. The remote artifact link has been provided [Graphic Representation File]. Is there another view you want audited?

---

**👤 You:**
> "Scrape the price of the first item from Amazon using a stealth bypass on `url_here`."

**🤖 AI Agent:**
> Stealth routine enacted via `scrape_with_stealth`. Bypassing WAF headers and standard bot challenges successfully on the retail endpoint. I subsequently applied `.a-price-whole` matching selectors via logical isolation. The payload returned values precisely: `["399", "419"]`. Validating extraction logic completed.

---

**👤 You:**
> "Retrieve the rendered HTML content of this site: 'https://vinkius.com/blog'."

**🤖 AI Agent:**
> I've invoked the `get_html_content` method successfully against the target URI. The Playwright container fully let the React/Next.js hydration loop stabilize. Captured massive 450kb parsed DOM structure explicitly mapping all internal blog routes natively. How would you like me to process this massive markup string within our memory context?


## ❓ FAQ

**Q: Can the agent scrape modern SPAs built with React or Vue?**
Absolutely. Because Browserless exposes actual Chrome environments via Playwright, standard JavaScript rendering pipelines execute exactly as they do on a user's machine. The agent simply captures the stabilized final DOM states post-hydration, making it remarkably effective for highly dynamic single-page applications.

**Q: What does `scrape_with_wait` do exactly when instructed to an AI?**
If a website relies on extremely heavy animations or subsequent lazy-loaded payload responses, `get_html_content` might return prematurely. Requesting your agent to use `scrape_with_wait` accompanied by a distinct selector (e.g., `#main-data-table`) locks the Browserless virtual container actively polling the CDP port. Only when that element materializes will it snap the payload back to you.

**Q: Are the screenshots produced bound to specific screen dimensions?**
By default, calling `get_screenshot` leverages Browserless' intrinsic 'Full Page' modifier. It synthetically commands the headless browser frame to extend computationally, absorbing the complete top-to-bottom scroll bounds of the rendered website into a massive, crystal clear uncropped PNG artifact.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browserless-playwright-cloud](https://vinkius.com/mcp/browserless-playwright-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Browserless (Playwright Cloud)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `browserless-playwright-cloud` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Browserless (Playwright Cloud)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "browserless-playwright-cloud": {
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
