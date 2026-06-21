# Public Suffix Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/public-suffix-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extract the true root domain, TLD, and subdomain from any URL using the official Mozilla Public Suffix List.

## Description
When an analytics agent processes URLs, it cannot guess that in `app.vinkius.co.uk` the TLD is `.co.uk` (not `.uk`). This MCP uses the official Mozilla Public Suffix List to fragment hostnames with 100% accuracy.

### The Superpowers

- **Official List:** Uses the same Public Suffix List maintained by Mozilla and used by every major browser.
- **Complex TLDs:** Correctly handles .co.uk, .com.br, .org.au, .amazonaws.com, and 9,000+ other suffixes.


## Available Tools
- **extract_domain**: The AI cannot reliably determine that the TLD of "app.vinkius.co.uk" is ".co.uk" (not ".uk"). This engine uses the official Mozilla Public Suffix List to fragment hostnames with 100% accuracy.

Extracts the true root domain, TLD, subdomain, and SLD from any hostname using the official Mozilla Public Suffix List. Handles complex TLDs like .co.uk, .com.br correctly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Public Suffix Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the root domain of app.vinkius.co.uk?"

**🤖 AI Agent:**
> Domain: vinkius.co.uk | TLD: co.uk | Subdomain: app

---

**👤 You:**
> "Extract the registrable domain from https://shop.example.com.br/products?id=1"

**🤖 AI Agent:**
> Domain: example.com.br | TLD: com.br | Subdomain: shop

---

**👤 You:**
> "Is mybucket.s3.amazonaws.com a registrable domain or a cloud subdomain?"

**🤖 AI Agent:**
> Domain: mybucket.s3.amazonaws.com | TLD: s3.amazonaws.com (PSL-listed cloud suffix)


## ❓ FAQ

**Q: Why can't I just split the domain by dots?**
Because TLDs like .co.uk, .com.br, and .org.au have multiple parts. Splitting by dots would incorrectly identify the root domain. The PSL has 9,000+ entries.

**Q: Does it handle cloud provider domains?**
Yes. Domains like *.amazonaws.com, *.azurewebsites.net, and *.cloudfront.net are in the PSL and handled correctly.

**Q: Can I pass a full URL with protocol and path?**
Yes. The engine automatically strips the protocol (http/https), path, and query parameters before parsing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/public-suffix-extractor](https://vinkius.com/mcp/public-suffix-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Public Suffix Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `public-suffix-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Public Suffix Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "public-suffix-extractor": {
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
