# URL and Email Token Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/url-and-email-token-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Detect URLs and emails to calculate potential LLM token savings.

## Description
This MCP server provides deterministic analysis of text to identify URLs and email addresses. It calculates the potential reduction in LLM token usage by replacing high-entropy strings with fixed-length placeholders. Use `analyze_text_tokens` to find the exact number of URLs and emails and the total tokens saved through optimization.


## Available Tools (2)
- **analyze_text_tokens**: 
- **get_token_summary_template**: Provides a template for reporting results


## 💬 Prompt Examples

Here are some examples of how you can interact with the **URL and Email Token Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text for token optimization: Check my site https://example.com and email me at test@domain.com"

**🤖 AI Agent:**
> url_count: 1, email_count: 1, total_url_tokens: 11, total_email_tokens: 5, tokens_saved: 14, optimization_possible: true

---

**👤 You:**
> "How many tokens can I save in this text: contact@service.org"

**🤖 AI Agent:**
> url_count: 0, email_count: 1, total_url_tokens: 0, total_email_tokens: 4, tokens_saved: 2, optimization_possible: true

---

**👤 You:**
> "Is there any optimization possible in: No URLs or emails here."

**🤖 AI Agent:**
> url_count: 0, email_count: 0, total_url_tokens: 0, total_email_tokens: 0, tokens_saved: 0, optimization_possible: false


## ❓ FAQ

**Q: How does this tool calculate token savings?**
It estimates the original token count by dividing the character length of detected URLs and emails by 4, then compares this to a fixed cost of 2 tokens per placeholder.

**Q: What tools are available in this server?**
The server provides `analyze_text_tokens` for calculating savings and `get_token_summary_template` for generating formatted reports.

**Q: Can I use this with Claude Desktop?**
Yes, this server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/url-and-email-token-detector](https://vinkius.com/ai-agent-connect/url-and-email-token-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **URL and Email Token Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `url-and-email-token-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **URL and Email Token Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "url-and-email-token-detector": {
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
