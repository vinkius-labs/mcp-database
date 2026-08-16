# URL SSRF Prevention Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/url-ssrf-prevention-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Prevents SSRF attacks by validating URL schemes and blocking internal IP ranges.

## Description
This MCP server provides a security layer to prevent Server-Side Request Forgery (SSRF) vulnerabilities. It ensures that AI agents only access safe, public web resources by validating the URL scheme and performing deterministic 32-bit integer math to block access to internal, private, and loopback IP ranges. Using the `validate_url` tool, agents can verify if a target is safe before attempting to browse, effectively shielding the host network from unauthorized probing. It is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client.


## Available Tools (3)
- **check_ip_safety**: Checks if an IP is in a private range
- **parse_url_components**: Parses URL into components
- **validate_url**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **URL SSRF Prevention Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the URL https://192.168.1.1 safe to visit?"

**🤖 AI Agent:**
> No, the URL is not safe because it targets a private IP range.

---

**👤 You:**
> "Check if https://vinkius.com is a safe URL."

**🤖 AI Agent:**
> Yes, https://vinkius.com is a safe, public URL.

---

**👤 You:**
> "Validate the safety of file:///etc/passwd"

**🤖 AI Agent:**
> No, the URL is not safe because the file scheme is prohibited.


## ❓ FAQ

**Q: How does this tool prevent SSRF attacks?**
The `validate_url` tool checks the URL scheme to ensure it is web-safe and uses bitwise integer math to block any requests targeting private or loopback IP ranges.

**Q: Which IP ranges are blocked?**
It blocks loopback addresses, Class A, B, and C private networks (10.x.x.x, 172.16.x.x, 192.168.x.x), and 0.0.0.0.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server is compatible with Claude Desktop and other MCP-compliant clients via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/url-ssrf-prevention-validator](https://vinkius.com/ai-agent-connect/url-ssrf-prevention-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **URL SSRF Prevention Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `url-ssrf-prevention-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **URL SSRF Prevention Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "url-ssrf-prevention-validator": {
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
