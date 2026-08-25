# IP Address & Subnet Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ip-address-subnet-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Perform precise bitwise IPv4 and IPv6 subnet calculations and membership checks.

## Description
This MCP server provides exact bitwise mathematical operations for IPv4 and IPv6 networking. It allows AI agents to calculate network boundaries, identify broadcast addresses, and determine usable host ranges. Use `calculate_subnet_details` to find the network address and host range, `check_ip_membership` to verify if an IP belongs to a specific subnet, and `get_host_capacity_stats` to determine the total addressable capacity of a network.


## Available Tools (3)
- **calculate_subnet_details**: Calculates network boundaries and capacity for a given IP and CIDR mask
- **get_host_capacity_stats**: Calculates the total and usable host capacity of a subnet
- **check_ip_membership**: Checks if a specific IP address is contained within a defined subnet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IP Address & Subnet Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the subnet details for 192.168.1.0/24?"

**🤖 AI Agent:**
> For 192.168.1.0/24, the network address is 192.168.1.0, the broadcast address is 192.168.1.255, and the usable host range is 192.168.1.1 to 192.168.1.254.

---

**👤 You:**
> "Is 10.0.0.5 in the 10.0.0.0/8 subnet?"

**🤖 AI Agent:**
> Yes, 10.0.0.5 is a member of the 10.0.0.0/8 subnet.

---

**👤 You:**
> "How many hosts are in a /24 IPv4 network?"

**🤖 AI Agent:**
> An IPv4 /24 network has 256 total addresses and 254 usable hosts.


## ❓ FAQ

**Q: How do I calculate the usable host range for a subnet?**
You can use the `calculate_subnet_details` tool by providing a valid IP address and the CIDR prefix length.

**Q: Can I check if an IP is part of a specific network?**
Yes, use the `check_ip_membership` tool to verify if a target IP address resides within a defined subnet range.

**Q: Does this support IPv6 calculations?**
Yes, all tools support both IPv4 and IPv6 bitwise math.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ip-address-subnet-calculator](https://vinkius.com/ai-agent-connect/ip-address-subnet-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IP Address & Subnet Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ip-address-subnet-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IP Address & Subnet Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ip-address-subnet-calculator": {
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
