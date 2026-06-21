# Accept Language Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accept-language-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Parse HTTP Accept-Language headers into priority-ordered language preferences with quality weights.

## Description
When a global routing agent reads `Accept-Language: en-US,pt-BR;q=0.9,fr;q=0.8`, it needs to correctly parse quality weights and determine the user's preferred language. This MCP does it deterministically.

### The Superpowers

- **RFC 7231 Compliant:** Parses quality values (q-factors) exactly as specified by the HTTP standard.
- **Priority Ordered:** Returns languages sorted by quality weight, with the preferred language first.


## Available Tools
- **parse_accept_language**: Pass the raw header value (e.g. "en-US,pt-BR;q=0.9,fr;q=0.8") and receive a priority-ordered list of languages with their quality weights. Never try to parse quality weights manually.

Parses HTTP Accept-Language headers into an ordered list of user language preferences with quality weights. Essential for global routing and i18n agents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accept Language Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this Accept-Language header: en-US,pt-BR;q=0.9,fr;q=0.8"

**🤖 AI Agent:**
> Preferred: en-US (q=1) > pt-BR (q=0.9) > fr (q=0.8)

---

**👤 You:**
> "What is the user's preferred language from: de,en-GB;q=0.7,ja;q=0.3"

**🤖 AI Agent:**
> Preferred: de (q=1, German)

---

**👤 You:**
> "How many languages does the browser support based on this header: zh-CN,zh;q=0.9,en;q=0.8,ko;q=0.7,ar;q=0.6"

**🤖 AI Agent:**
> 5 languages detected: zh-CN, zh, en, ko, ar


## ❓ FAQ

**Q: What is a quality weight (q-factor)?**
A value from 0 to 1 indicating preference. `q=1` (default) is highest priority. `q=0` means the language is explicitly not accepted.

**Q: Does it handle regional subtags?**
Yes. `pt-BR` is parsed as code=pt, region=BR. `en-US` as code=en, region=US. The region is separated from the language code automatically.

**Q: What if no quality value is specified?**
Languages without an explicit q-value default to q=1 (highest priority), following the HTTP specification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accept-language-parser](https://vinkius.com/mcp/accept-language-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accept Language Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `accept-language-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accept Language Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accept-language-parser": {
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
