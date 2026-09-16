# Grape Receiving & Weighing Logistics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grape-receiving-weighing-logistics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Calculate truck queuing, sampling protocols, and receiving schedules for grape harvests.

## Description
This MCP server provides essential logistics calculations for winery receiving operations. It connects AI agents to core winery metrics, allowing for precise management of truck arrivals and quality control. Use `get_queue_metrics` to predict truck wait times and total receiving duration. Determine quality control needs with `calculate_sampling_protocol` based on incoming volume. Optimize arrival sequences using `optimize_receiving_schedule` to respect lot segregation requirements, and monitor facility bottlenecks with `get_facility_utilization` to ensure the weighbridge or crush capacity is not overwhelmed.


## Available Tools (4)
- **calculate_sampling_protocol**: Determines how often quality samples should be taken based on incoming volume
- **get_facility_utilization**: Evaluates if the planned receiving batch will overwhelm the facility
- **get_queue_metrics**: Answers how long trucks will wait and how long the receiving process will take
- **optimize_receiving_schedule**: Generates an optimized sequence of arrivals to minimize congestion and honor segregation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grape Receiving & Weighing Logistics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will 20 trucks wait if the weighbridge processes 5 per hour and crush capacity is 10 per hour?"

**🤖 AI Agent:**
> The average wait time for the 20 trucks will be 1.5 hours, with a total receiving duration of 4 hours.

---

**👤 You:**
> "What is the sampling protocol for 500 tons of premium grapes with a sampling rate of 0.05 samples per ton?"

**🤖 AI Agent:**
> For 500 tons of premium grapes, you need to take 25 total samples, with a sampling interval of 12 minutes.

---

**👤 You:**
> "Generate a schedule for 10 trucks that must be grouped by lot segregation requirements starting at 8 AM."

**🤖 AI Agent:**
> The optimized arrival sequence starts at 08:00, grouping the required lots consecutively to ensure smooth flow through the weighbridge.


## ❓ FAQ

**Q: How can I predict truck wait times?**
You can use the `get_queue_metrics` tool by providing the truck count, average capacity, weighbridge throughput, and crush capacity.

**Q: How do I ensure quality control for a specific grape lot?**
Use `calculate_sampling_protocol` with the total expected volume, the required sampling rate, and the lot type (e.g., premium, standard, or bulk).

**Q: Can I prevent facility bottlenecks?**
Yes, the `get_facility_utilization` tool identifies whether the weighbridge or the crush capacity will act as the primary bottleneck for your planned batch.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grape-receiving-weighing-logistics](https://vinkius.com/en/ai-agent-connect/grape-receiving-weighing-logistics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grape Receiving & Weighing Logistics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grape-receiving-weighing-logistics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grape Receiving & Weighing Logistics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grape-receiving-weighing-logistics": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
