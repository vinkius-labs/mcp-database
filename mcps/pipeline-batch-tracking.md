# Pipeline Batch Tracking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pipeline-batch-tracking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Monitor product batch positions, transmix volumes, and delivery timing in liquid pipelines.

## Description
This MCP server provides real-time monitoring for multi-product liquid pipelines. It allows AI agents to track the exact location of products using `get_batch_positions`, calculate the volume of mixed products (transmix) via `calculate_interface_volumes`, and predict arrival times with `estimate_delivery_timing`. It also accounts for physical variables like line pack and pressure-driven volume changes through `analyze_pipeline_compressibility` to ensure high-precision tracking.


## Available Tools (4)
- **analyze_pipeline_compressibility**: Evaluates how much the product volume is expanding or contracting due to pressure variations
- **calculate_interface_volumes**: Identifies the volume of mixed product (transmix) generated at the boundaries between different product batches
- **estimate_delivery_timing**: Predicts when a specific batch or interface will reach the delivery terminal
- **get_batch_positions**: Determines the current location of all active product batches within the pipeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipeline Batch Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where are the current batches located in the pipeline?"

**🤖 AI Agent:**
> Batch B1 is at 450km, Batch B2 is at 120km, and Batch B3 is at 15km.

---

**👤 You:**
> "When will Batch B2 reach the delivery terminal?"

**🤖 AI Agent:**
> Batch B2 is estimated to arrive at the terminal on 2024-10-25T14:30:00Z with a confidence interval of 0.95.

---

**👤 You:**
> "What is the volume of transmix between Batch 1 and Batch 2?"

**🤖 AI Agent:**
> The transmix volume between Batch 1 and Batch 2 is 1,250 cubic meters.


## ❓ FAQ

**Q: How accurate are the batch position calculations?**
Positions are calculated using the current flow rate and cumulative injected volumes, providing real-time distance tracking from the injection point.

**Q: Can I predict when a batch will arrive at the terminal?**
Yes, you can use the estimation tools to predict arrival times based on distance, flow rate, and line pack adjustments.

**Q: How is transmix volume handled?**
The system identifies the volume of mixed products at batch boundaries by applying a mixing factor to the interface between adjacent products.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pipeline-batch-tracking](https://vinkius.com/en/ai-agent-connect/pipeline-batch-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipeline Batch Tracking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipeline-batch-tracking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipeline Batch Tracking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipeline-batch-tracking": {
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
