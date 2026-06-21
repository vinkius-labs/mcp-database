# Public Suffix Extractor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/public-suffix-extractor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/public-suffix-extractor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/public-suffix-extractor-mcp)
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


## Installation & Usage

To install and use the **Public Suffix Extractor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/public-suffix-extractor](https://vinkius.com/mcp/public-suffix-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
