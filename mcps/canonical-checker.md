# Canonical Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/canonical-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [web-development](../categories/web-development.md)

Identify the authoritative URL version and detect SEO duplicate content risks.

## Description
The Canonical Checker MCP server helps SEO professionals identify the single, cleanest version of a URL from multiple variations. By analyzing protocol consistency (HTTP vs HTTPS), hostname standardization (www vs non-www), trailing slash presence, and query parameter noise, it prevents duplicate content issues. Use `identify_canonical_candidate` to find the best canonical tag candidate, `audit_url_equality` to detect structural discrepancies in URL groups, and `detect_parameter_drift` to separate static from variable tracking parameters.


## Available Tools (3)
- **identify_canonical_candidate**: ).

Determines the best candidate for the canonical tag
- **detect_parameter_drift**: Identifies which query parameters are causing URL divergence
- **audit_url_consistency**: Checks for structural discrepancies in a group of URLs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Canonical Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which of these is the best canonical URL: https://mysite.com/page, http://www.mysite.com/page/, and https://mysite.com/page?utm_source=email?"

**🤖 AI Agent:**
> The best canonical candidate is https://mysite.com/page because it uses the secure HTTPS protocol, has a standardized hostname without 'www', and contains no unnecessary query parameters.

---

**👤 You:**
> "Check these URLs for consistency: https://shop.com/item, https://shop.com/item/, and http://shop.com/item"

**🤖 AI Agent:**
> Discrepancies detected: Protocol mismatch (HTTP vs HTTPS) and trailing slash inconsistency.

---

**👤 You:**
> "Analyze these URLs for parameter drift: https://mysite.com/search?q=shoes, https://myssite.com/search?q=shirts&utm_medium=social, and https://myssite.com/search?q=hats&sessionid=123"

**🤖 AI Agent:**
> Variable parameters found: utm_medium, sessionid. Static parameters found: q.


## ❓ FAQ

**Q: How does the tool identify a canonical URL?**
The `identify_canonical_candidate` tool evaluates all provided URLs and selects the one with the fewest 'noise' elements, prioritizing HTTPS, standardized hostnames, and minimal query parameters.

**Q: Can I detect tracking parameters?**
Yes, using `detect_parameter_drift`, you can identify which query parameters are variable (like UTM or session IDs) and which are static across your URL list.

**Q: What kind of discrepancies does the audit tool find?**
The `audit_url_consistency` tool flags mismatches in protocol, subdomain usage (www vs non-www), trailing slashes, and parameter counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/canonical-checker](https://vinkius.com/mcp/canonical-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Canonical Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `canonical-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Canonical Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "canonical-checker": {
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
