# Agent SLA Compliance Monitor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-sla-compliance-monitor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Deterministic SLA compliance calculator for agent orchestration systems.

## Description
This MCP server provides deterministic tools to evaluate the operational health of AI agents. It compares real-world performance metrics against strict Service Level Agreements (SLAs). Use `calculate_tenant_compliance` to evaluate specific tenant metrics like response time, availability, accuracy, and throughput. Use `get_tenant_targets` to retrieve unique SLA configurations for a tenant, or `summarize_fleet_health` to get an aggregated view of compliance across all tenants to identify systemic issues.


## Available Tools (3)
- **calculate_tenant_compliance**: Evaluates the specific SLA compliance for a single tenant based on their provided targets and a window of recorded measurements
- **get_tenant_targets**: Retrieves the specific SLA target configurations for a given tenant
- **summarize_fleet_health**: Provides an aggregated view of compliance across all tenants to identify systemic issues


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent SLA Compliance Monitor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the SLA compliance for tenant 'tenant-123' using these measurements: [{'latencyMs': 150, 'isSuccess': true, 'isCorrect': true, 'timestamp': '2024-01-01T00:00:00Z'}]."

**🤖 AI Agent:**
> The compliance score for tenant-123 is 100% across all metrics, and the error budget remains fully intact.

---

**👤 You:**
> "What is the current health status of the entire agent fleet?"

**🤖 AI Agent:**
> The fleet status is Healthy, with a global alert count of 0.

---

**👤 You:**
> "Get the SLA targets for tenant 'customer-alpha'."

**🤖 AI Agent:**
> The targets for customer-alpha are: 200ms P99 latency, 99.9% availability, 95% accuracy, and 10 RPS throughput.


## ❓ FAQ

**Q: How is the composite SLA score calculated?**
The composite score is derived from the geometric mean of all individual metric compliance percentages, including response time, availability, accuracy, and throughput.

**Q: Can I monitor different SLAs for different tenants?**
Yes, the `calculate_tenant_compliance` tool supports multi-tenancy by evaluating metrics against specific targets provided for each unique tenant ID.

**Q: What defines a critical SLA violation?**
A violation is classified as critical if any metric breaches its target by more than 5%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-sla-compliance-monitor](https://vinkius.com/ai-agent-connect/agent-sla-compliance-monitor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent SLA Compliance Monitor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-sla-compliance-monitor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent SLA Compliance Monitor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-sla-compliance-monitor": {
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
