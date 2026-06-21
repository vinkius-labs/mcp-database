# Deterministic URL Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-url-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI with flawless URL deconstruction. Deterministically parse URIs, extract deep query strings, and inject tracking parameters without concatenation errors.

## Description
When LLMs try to manipulate URLs manually, they often produce broken links. Injecting a tracking parameter like `utm_source` usually results in catastrophic double-question marks (`??utm=`) or broken ampersands (`&&`). The URL Parser MCP solves this by delegating all URI mechanics to a pristine V8 deterministic engine.

### The Superpowers
- **Flawless Injection:** Safely inject JSON key-value pairs directly into complex URIs. The engine guarantees mathematically correct `?` and `&` concatenation every single time.
- **Deep Deconstruction:** Split any URL into its core atomic components (protocol, port, hash, pathname) preventing parsing errors in scraping or API-calling workflows.
- **Query Extraction:** Instantly pull tracking codes or auth tokens from long, convoluted query strings without risky Regex gymnastics.
- **Zero-Dependency Architecture:** Pure Javascript runtime execution means absolute processing speed with no bloated packages.


## Available Tools
- **extract_query**: Safely extracts a specific query string parameter value from a URL without regex errors
- **inject_query**: Provide the new params as a JSON string.

Injects or updates query string parameters in a URL safely, guaranteeing correct ? and & concatenation
- **parse_url**: Deconstructs a URL into its core components: protocol, host, pathname, query parameters, and hash


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic URL Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this tracking URL and show me its base hostname: https://google.com/search?q=test&lang=en"

**🤖 AI Agent:**
> Using the parse_url tool: The base hostname is 'google.com'.

---

**👤 You:**
> "Inject a UTM campaign parameter into this link: https://vinkius.com/pricing"

**🤖 AI Agent:**
> Using the inject_query tool (params: {"utm_campaign": "summer"}): The new URL is https://vinkius.com/pricing?utm_campaign=summer.

---

**👤 You:**
> "Extract just the 'token' value from this callback URL."

**🤖 AI Agent:**
> Using the extract_query tool (paramKey='token'): The extracted token value is 'ABC123XYZ'.


## ❓ FAQ

**Q: Why use an MCP instead of letting the AI format the URL?**
AIs are probabilistic text generators, not web browsers. If a URL already has a `?`, adding another parameter requires `&`. LLMs frequently guess the wrong delimiter, breaking critical affiliate tracking or API requests. The MCP guarantees correct serialization.

**Q: Can it extract multiple parameters?**
Yes! If you use the `parse_url` tool, it returns a `queryParams` JSON object containing every single key and value found in the URL. If you only want one, use `extract_query`.

**Q: Does this tool execute network requests?**
No. The entire engine executes pure algorithmic parsing on strings. It does not validate if the URL is active online, it merely processes its mathematical construction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-url-engine](https://vinkius.com/mcp/deterministic-url-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic URL Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deterministic-url-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic URL Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-url-engine": {
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
