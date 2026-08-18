# AWS API Gateway Throttling Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aws-api-gateway-throttling-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate AWS API Gateway RPS, burst capacity, quotas, and operational limits.

## Description
This MCP server provides deterministic calculations for AWS API Gateway constraints. It helps engineers predict throttling behavior and manage service limits for both REST and HTTP APIs. Use `calculate_throttling_limits` to determine allowed RPS and burst capacity based on the token bucket algorithm. Use `calculate_quota_usage` to check if sustained traffic will exceed daily, weekly, or monthly limits. You can also use `get_operational_constraints` to retrieve payload size limits and integration timeouts, or `simulate_canary_traffic` to plan traffic splitting for new deployments.


## Available Tools (4)
- **get_operational_constraints**: Returns the fixed technical limits for the selected API type
- **calculate_quota_usage**: Evaluates if a user's planned request volume will exceed defined time-based quotas
- **calculate_throttling_limits**: Determines the RPS and burst capacity for a specific API stage
- **simulate_canary_traffic**: Calculates the distribution of traffic between a production environment and a canary environment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AWS API Gateway Throttling Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the throttling limits and burst capacity for a REST API with 5000 RPS?"

**🤖 AI Agent:**
> For a REST API with 5000 RPS, the allowed RPS is 10,000 and the burst capacity is 20,000.

---

**👤 You:**
> "Will 500 RPS exceed a daily quota of 1,000,000 requests?"

**🤖 AI Agent:**
> No, 500 RPS results in 43,200,000 requests per day, which exceeds the 1,000,000 daily quota.

---

**👤 You:**
> "Calculate the traffic split for a 1000 RPS total volume with a 10% canary deployment."

**🤖 AI Agent:**
> The traffic split will be 900 RPS for production and 100 RPS for the canary stage.


## ❓ FAQ

**Q: How is burst capacity calculated?**
Burst capacity is calculated as exactly twice the allowed RPS, following the token bucket algorithm used by AWS.

**Q: What are the differences between REST and HTTP API limits?**
REST APIs have a soft limit of 10,000 RPS, while HTTP APIs support up to 100,000 RPS. Integration timeouts also differ: 29 seconds for REST and 30 seconds for HTTP.

**Q: Can I check if my planned traffic will exceed my daily quota?**
Yes, you can use the `calculate_quota_usage` tool to evaluate if your planned RPS will exceed defined daily, weekly, or monthly quotas.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aws-api-gateway-throttling-calculator](https://vinkius.com/ai-agent-connect/aws-api-gateway-throttling-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AWS API Gateway Throttling Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aws-api-gateway-throttling-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AWS API Gateway Throttling Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aws-api-gateway-throttling-calculator": {
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
