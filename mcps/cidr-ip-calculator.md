# CIDR IP Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cidr-ip-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Perform IPv4 and IPv6 subnet mathematics, including network boundaries and host range calculations.

## Description
The CIDR IP Calculator is a specialized networking utility for performing precise IPv4 and IPv6 subnet mathematics. By connecting this MCP server to your AI workflow via Vinkius Edge, you can automate complex network calculations. Use the `cidr_calculate` tool to instantly retrieve the network address, broadcast address, and total/usable host counts from any CIDR notation input. The `ip_check` tool allows for rapid verification of whether a specific IP address falls within a designated subnet range. This server acts as a bridge between your AI agent and essential networking logic, ensuring accuracy in network planning and auditing.


## Available Tools (2)
- **cidr_calculate**: psi IPv4 or IPv6).

Calculate network details for a CIDR range
- **ip_check**: Check if an IP address is within a CIDR range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CIDR IP Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the details for 192.168.1.0/24."

**🤖 AI Agent:**
> For 192.168.1.0/24:
- Network Address: 192.168.1.0
- Broadcast Address: 192.168.1.255
- First Usable Host: 192.168.1.1
- Last Usable Host: 192.168.1.254
- Total Hosts: 256
- Usable Hosts: 254

---

**👤 You:**
> "Is 10.0.0.5 inside 10.0.0.0/8?"

**🤖 AI Agent:**
> Yes, 10.0.0.5 is within the range of 10.0.0.0/8.

---

**👤 You:**
> "Check if 2001:db8::1 is in 2001:db8::/32."

**🤖 AI Agent:**
> Yes, 2001:db8::1 is within the range of 2001:db8::/32.


## ❓ FAQ

**Q: What can I calculate with the `cidr_calculate` tool?**
The `cidr_calculate` tool provides a complete breakdown of a CIDR range, including the network address, broadcast address, first and last usable host addresses, and the total number of available hosts.

**Q: How do I check if an IP is part of a specific subnet?**
You can use the `ip_check` tool by providing both the target IP address and the CIDR notation you want to check against.

**Q: Does this support IPv6?**
Yes, the server fully supports both IPv4 and IPv6 subnet calculations and range checks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cidr-ip-calculator](https://vinkius.com/mcp/cidr-ip-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CIDR IP Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cidr-ip-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CIDR IP Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cidr-ip-calculator": {
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
