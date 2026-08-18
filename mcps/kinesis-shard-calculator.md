# Kinesis Shard Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/kinesis-shard-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Calculate optimal AWS Kinesis Data Streams shard counts and storage needs.

## Description
This MCP server provides deterministic calculations for AWS Kinesis Data Streams. It helps you determine the exact number of shards required for ingestion and consumption, estimate total storage footprint based on retention periods, and identify available Enhanced Fan-Out (EFO) slots. Use `calculate_shard_requirements` to find the minimum shard count, `calculate_storage_and_efo` for storage and EFO capacity, and `calculate_scaling_operations` to plan shard splits or merges.


## Available Tools (3)
- **calculate_scaling_operations**: Determines the necessary shard management actions to reach a target state
- **calculate_shard_requirements**: Determines the minimum number of shards required to satisfy both ingestion and consumption demands
- **calculate_storage_and_efo**: Calculates the physical storage footprint and identifies Enhanced Fan-Out consumer capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kinesis Shard Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many shards do I need for an ingestion rate of 5000 KB/s and 2000 records per second with 3 consumers using shared throughput?"

**🤖 AI Agent:**
> You need 5 shards to handle the ingestion rate and 2 shards for consumption, resulting in a total of 5 shards.

---

**👤 You:**
> "Calculate the storage needed for 1000 KB/s ingestion with a 24-hour retention period."

**🤖 AI Agent:**
> The total storage required for a 24-hour retention period at 1000 KB/s is approximately 86.4 GB.

---

**👤 You:**
> "I have 10 shards and I want to scale to 25 shards. How many operations are needed?"

**🤖 AI Agent:**
> You will need to perform 15 split operations to reach your target of 25 shards.


## ❓ FAQ

**Q: How do I calculate the number of shards needed for my data?**
You can use the `calculate_shard_requirements` tool. Provide your ingestion rate in KB/s, records per second, and your consumer profile to get the total shard count.

**Q: Can I estimate my AWS storage costs with this tool?**
While it doesn't provide direct dollar amounts, the `calculate_storage_and_efo` tool provides the total storage in GB, which you can use to estimate your AWS costs.

**Q: How do I scale my Kinesis stream up or down?**
Use the `calculate_scaling_operations` tool. Input your current shard count and your target shard count to see how many splits or merges are required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/kinesis-shard-calculator](https://vinkius.com/ai-agent-connect/kinesis-shard-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kinesis Shard Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kinesis-shard-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kinesis Shard Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kinesis-shard-calculator": {
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
