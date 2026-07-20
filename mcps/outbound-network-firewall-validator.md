# Outbound Network Firewall Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/outbound-network-firewall-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Validates outbound network requests against allowed domains and ports to prevent data exfiltration.

## Description
The Outbound Network Firewall Validator acts as a security layer for AI agents. It prevents unauthorized egress by checking URLs against an allowlist and blocking private IP ranges. Using tools like `validate_outbound_request`, it ensures that requests to sensitive internal infrastructure are blocked, mitigating SSRF risks.


## Available Tools (3)
- **validate_outbound_request**: Validate an outbound URL against security policies
- **check_domain_membership**: Check if a hostname belongs to an allowed domain list
- **evaluate_ip_risk**: Evaluate the risk level of an IPv4 address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outbound Network Firewall Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is `https://api.github.com/repos/mcpfusion/core` allowed?"

**🤖 AI Agent:**
> Yes, `api.github.com` is in the allowed domains list.

---

**👤 You:**
> "Check if `http://192.168.1.50:8080` is safe."

**🤖 AI Agent:**
> No, this request is blocked because 192.168.1.50 belongs to a private IP range.

---

**👤 You:**
> "Verify membership for `sub.mysite.org`."

**🤖 AI Agent:**
> The hostname `sub.mysite.org` is authorized as it matches the `mysite.org` suffix.


## ❓ FAQ

**Q: How does it prevent SSRF?**
It blocks private IP ranges like 127.0.0.1 using bitwise math to ensure agents cannot access internal infrastructure.

**Q: Can I use it for subdomains?**
Yes, if you allow `mysite.org`, then `api.mysite.org` is also authorized via suffix matching.

**Q: What happens if a URL is invalid?**
The `validate_outbound_request` tool will return an error state and the reason for failure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/outbound-network-firewall-validator](https://vinkius.com/mcp/outbound-network-firewall-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outbound Network Firewall Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outbound-network-firewall-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outbound Network Firewall Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outbound-network-firewall-validator": {
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
