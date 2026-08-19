# AWS MSK Partition & Throughput Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-msk-partition-throughput-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Deterministic sizing for AWS MSK clusters, calculating partitions, storage, and network limits.

## Description
This MCP server provides precise sizing calculations for AWS Managed Streaming for Apache Kafka (MSK) clusters. It uses deterministic logic to determine the required partition count per broker based on a 100 MB/s throughput threshold, calculates total storage needs across the retention period, and validates hardware constraints for specific AWS instance types. Use `calculate_partition_and_storage_needs` to find foundational scaling requirements, `evaluate_broker_capacity` to check if your partition count fits within the limits of instances like kafka.m5.large or kafka.m5.4xlarge, and `calculate_network_and_limits` to verify network throughput and cluster-wide architectural ceilings.


## Available Tools (3)
- **calculate_network_and_limits**: Analyzes network throughput requirements and validates cluster-wide architectural limits
- **calculate_partition_and_storage_needs**: Determines foundational scaling requirements (partitions and storage) based on throughput and time
- **evaluate_broker_capacity**: Checks if the proposed partition count is physically supported by the chosen AWS MSK instance types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS MSK Partition & Throughput Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a message rate of 500 messages per second, each 10 KB, with a 7-day retention and 3 brokers. How many partitions and how much storage do I need?"

**🤖 AI Agent:**
> You will need 1 partition per broker (total 3 partitions) and approximately 2.86 GB of storage per broker.

---

**👤 You:**
> "Will a kafka.m5.large instance support 5000 partitions per broker?"

**🤖 AI Agent:**
> No, a kafka.m5.large instance is limited to a maximum of 4,000 partitions per broker.

---

**👤 You:**
> "Calculate the network requirements for 10,000 messages/sec at 50 KB each with 4 brokers."

**🤖 AI Agent:**
> The network throughput per broker is 1.0 Gbps.


## ❓ FAQ

**Q: How does this tool calculate partition counts?**
The tool calculates the partition count per broker by dividing the required message rate by the 100 MB/s throughput threshold per partition.

**Q: What AWS MSK instances are supported?**
The calculator supports common MSK instance types, including kafka.m5.large and kafka.m5.4xlarge, to validate partition limits.

**Q: Can I check if my cluster will exceed network limits?**
Yes, by using `calculate_network_and_limits`, you can determine if the per-broker network throughput exceeds the 10 Gbps ceiling.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-msk-partition-throughput-calculator](https://vinkius.com/ai-agent-connect/aws-msk-partition-throughput-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS MSK Partition & Throughput Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-msk-partition-throughput-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS MSK Partition & Throughput Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-msk-partition-throughput-calculator": {
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
