# UTM Campaign Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/utm-campaign-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip Marketing Agents to generate flawless tracking links. Safely encode UTM parameters and prevent broken Google Analytics routing.

## Description
When a Martech AI Agent drafts social media posts or email campaigns, it needs to append tracking data to the links (UTMs). LLMs are notorious for hallucinating query strings—adding double `??`, forgetting to URL-encode spaces, or breaking existing parameters. This ruins data attribution in Google Analytics. This MCP solves that perfectly.

### The Superpowers

- **Strict URL Encoding:** Merges `utm_source`, `utm_medium`, and other parameters cleanly into any base URL using strict browser-grade encoding.
- **Analytics Protection:** Guarantees that every generated link works perfectly without causing 404s or dropping tracking data.


## Available Tools (1)
- **build_utm_url**: Provide the base landing page URL, utm_source, and utm_medium as required fields. Optionally add campaign, term, and content. The engine handles all URL encoding and query string merging safely.

Safely constructs and encodes marketing UTM tracking URLs. Prevents AI from hallucinating broken query strings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UTM Campaign Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Build a tracking URL for `https://vinkius.com/pricing` with source `linkedin` and medium `social`."

**🤖 AI Agent:**
> UTM Campaign URL: Generated successfully.

---

**👤 You:**
> "Add UTM tracking to this link for our Black Friday email blast."

**🤖 AI Agent:**
> UTM Campaign URL: Generated successfully.

---

**👤 You:**
> "I have this landing page that already has `?ref=affiliate`. Append the UTM source `facebook` safely."

**🤖 AI Agent:**
> UTM Campaign URL: Appended successfully.


## ❓ FAQ

**Q: What if the base URL already has parameters?**
The engine safely detects existing parameters and appends the UTMs using `&` instead of `?`, preserving all previous data.

**Q: Does it URL-encode spaces in the campaign name?**
Yes. A campaign name like `Summer Sale` will automatically be encoded to `Summer+Sale` or `Summer%20Sale`.

**Q: Which UTM parameters are mandatory?**
Only `source` and `medium` are mandatory. The engine will throw an error if the agent forgets to provide them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/utm-campaign-builder](https://vinkius.com/mcp/utm-campaign-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UTM Campaign Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `utm-campaign-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UTM Campaign Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "utm-campaign-builder": {
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
