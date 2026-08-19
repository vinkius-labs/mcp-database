# AWS IoT Core Device & Limits Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-iot-core-device-limits-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate AWS IoT Core messaging throughput, device scale, and resource limits.

## Description
This MCP server provides deterministic calculations for AWS IoT Core architectures. It helps engineers determine if their device fleet and messaging patterns align with AWS best practices and hard limits. Use `calculate_messaging_load` to validate throughput and payload sizes, `calculate_resource_limits` to plan security and management resources, and `calculate_connectivity_summary` to get a high-level adherence report for your account.


## Available Tools (3)
- **calculate_connectivity_summary**: Provides a high-level summary of the account's adherence to AWS IoT best practices
- **calculate_messaging_load**: Calculates the total messaging throughput and validates against message size constraints
- **calculate_resource_limits**: Calculates the capacity and distribution of security and management resources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS IoT Core Device & Limits Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the messaging load for 50,000 devices sending 2 messages per second with a 50 KB payload."

**🤖 AI Agent:**
> The total messaging throughput is 100,000 messages per second, with a total data throughput of 5,000,000 KBps. The message size is valid and the device count is within the recommended limit.

---

**👤 You:**
> "What are the recommended resource limits for an account with 2,000,000 devices and 50 rules?"

**🤖 AI Agent:**
> For 2,000,000 devices and 50 rules, the recommended limits are 10 certificates per thing, 10 policies per certificate, 100 rules per account, 10 actions per rule, 100,000 jobs per account, 1,000 queries per second, and 10 shadow updates per second per thing.

---

**👤 You:**
> "Check the connectivity summary for 150,000 msg/s, 2,000,000 devices, and a 150 KB message size."

**🤖 AI Agent:**
> The account exceeds the recommended messaging throughput (150,000 > 100,000), exceeds the recommended device count (2,000,000 > 1,000,000), and violates the hard message size limit (150 KB > 128 KB).


## ❓ FAQ

**Q: How do I check if my message size is valid?**
You can use the `calculate_messaging_load` tool. It will validate if your message size is within the 128 KB hard limit.

**Q: Can I calculate resource limits for my IoT account?**
Yes, the `calculate_resource_limits` tool calculates recommended certificates, policies, rules, and jobs based on your device count.

**Q: What is the maximum recommended messaging throughput?**
AWS recommends staying within 100,000 messages per second per account to ensure stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-iot-core-device-limits-calculator](https://vinkius.com/ai-agent-connect/aws-iot-core-device-limits-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS IoT Core Device & Limits Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-iot-core-device-limits-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS IoT Core Device & Limits Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-iot-core-device-limits-calculator": {
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
