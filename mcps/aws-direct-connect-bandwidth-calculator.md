# AWS Direct Connect Bandwidth Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-direct-connect-bandwidth-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate AWS Direct Connect connection counts, redundancy requirements, and architectural limits.

## Description
This MCP server provides deterministic calculations for AWS Direct Connect (DX) planning. It determines the exact number of connections required based on your traffic needs, redundancy models (1:1 or N:1), and connection speeds. Use `calculate_connection_requirements` to find the necessary connection count and `validate_architectural_limits` to ensure your plan adheres to AWS constraints like regional capacity, location limits, and VIF restrictions.


## Available Tools (3)
- **calculate_connection_requirements**: Determines the core physical connection count and capacity validation
- **get_mtu_configuration**: Provides the MTU settings based on the connection type
- **validate_architectural_limits**: Checks if the requested connection plan violates AWS physical and logical constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS Direct Connect Bandwidth Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need 10 Gbps of bandwidth across 2 regions with 1:1 redundancy using 10 Gbps connections. How many connections do I need?"

**🤖 AI Agent:**
> You will need 2 connections total (1 per region) for the base requirement, which doubles to 4 connections total to satisfy the 1:1 redundancy model.

---

**👤 You:**
> "What is the MTU setting if I enable jumbo frames?"

**🤖 AI Agent:**
> With jumbo frames enabled, the MTU is set to 8500 bytes.

---

**👤 You:**
> "Check if my plan of 20 connections for 1 Gbps links in 1 region violates AWS limits."

**🤖 AI Agent:**
> Yes, this plan violates the location limit, as a single location is capped at 4 connections for 1 Gbps links.


## ❓ FAQ

**Q: How do I calculate the number of connections needed for my traffic?**
You can use the `calculate_connection_requirements` tool. Provide your required traffic in Gbps, the number of regions, your redundancy model, and the connection speed to get a precise connection plan.

**Q: Can this tool check if I am exceeding AWS limits?**
Yes. The `validate_architectural_limits` tool checks your plan against AWS constraints, including regional limits, location capacity, and VIF limits.

**Q: What is the difference between 1:1 and N:1 redundancy in the calculator?**
1:1 redundancy doubles your connection count to ensure every active link has a standby. N:1 redundancy uses the base connection count required to meet your traffic threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-direct-connect-bandwidth-calculator](https://vinkius.com/ai-agent-connect/aws-direct-connect-bandwidth-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS Direct Connect Bandwidth Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-direct-connect-bandwidth-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS Direct Connect Bandwidth Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-direct-connect-bandwidth-calculator": {
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
