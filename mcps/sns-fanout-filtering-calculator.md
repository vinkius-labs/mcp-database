# SNS Fanout & Filtering Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sns-fanout-filtering-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate AWS SNS fanout, throughput, and filter policy complexity.

## Description
This MCP server provides deterministic calculations for AWS SNS architectures. Use `calculate_fanout_and_limits` to verify if message payloads and attribute counts stay within the 256 KB limit. Use `evaluate_policy_and_throughput` to determine maximum messages per second for FIFO or Standard topics and validate filter policy nesting depth. Use `analyze_delivery_resilience` to calculate SQS visibility timeouts and exponential backoff retry delays.


## Available Tools (3)
- **analyze_delivery_resilience**: Calculate the impact of SQS settings on message availability and retry behavior
- **calculate_fanout_and_limits**: Calculate total fanout and verify if the message payload adheres to AWS physical constraints
- **evaluate_policy_and_throughput**: Assess if the message filtering logic and topic type are compatible with the required scale


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SNS Fanout & Filtering Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fanout for a message with 10 SQS subscribers and 5 Lambda subscribers, with a 150 KB message size and 5 attributes."

**🤖 AI Agent:**
> The total fanout is 15 delivery attempts, and the payload is valid.

---

**👤 You:**
> "What is the max throughput for a FIFO topic with batching enabled?"

**🤖 AI Agent:**
> The maximum throughput for a FIFO topic with batching enabled is 3000 messages per second.

---

**👤 You:**
> "If my SQS visibility timeout is 30 seconds, what is the effective retention for the first retry attempt?"

**🤖 AI Agent:**
> The effective retention is 30 seconds.


## ❓ FAQ

**Q: How do I check if my SNS message is too large?**
You can use the `calculate_fanout_and_limits` tool. It checks if the `messageSizeKb` and `attributeCount` combined stay within the AWS 256 KB limit.

**Q: What is the throughput difference between FIFO and Standard topics?**
Use `evaluate_policy_and_throughput` to find out. FIFO topics support 300 msg/s or 3000 msg/s with batching, while Standard topics are designed for much higher, throttled throughput.

**Q: How does SNS handle retries?**
SNS uses an immediate retry followed by exponential backoff. You can calculate the specific delay using the `analyze_delivery_resilience` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sns-fanout-filtering-calculator](https://vinkius.com/ai-agent-connect/sns-fanout-filtering-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SNS Fanout & Filtering Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sns-fanout-filtering-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SNS Fanout & Filtering Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sns-fanout-filtering-calculator": {
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
