# Kubernetes HPA Scaling Simulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kubernetes-hpa-scaling-simulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [devops](../categories/devops.md)

Simulate Kubernetes Horizontal Pod Autoscaler behavior and stability.

## Description
This MCP server provides a high-fidelity simulation engine for Kubernetes Horizontal Pod Autoscaler (HPA) behavior. It allows you to project how replica counts will evolve over time based on varying load patterns, applying standard HPA scaling logic and stabilization windows. Use `calculate_target_replicas` to find the ideal pod count for a specific metric, `simulate_scaling_timeline` to model long-term scaling trends, and `identify_thrashing_patterns` to detect potential oscillation risks in your configuration. It also includes `validate_hpa_config` to ensure your parameters like min/max replicas and cooldown windows are logically sound.


## Available Tools (4)
- **identify_thrashing_patterns**: Analyzes a scaling timeline to detect frequent oscillations (thrashing)
- **validate_hpa_config**: Validates the HPA configuration parameters
- **calculate_target_replicas**: Calculates the target number of replicas based on current metric and utilization
- **simulate_scaling_timeline**: Simulates how the replica count evolves over a series of metric observations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kubernetes HPA Scaling Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the target replicas if I have 5 pods running, current CPU is 80%, and my target is 50%."

**🤖 AI Agent:**
> Based on a current usage of 80% against a 50% target, the required number of replicas is 8.

---

**👤 You:**
> "Will my HPA config with min 2, max 10, and a 300s window be valid?"

**🤖 AI Agent:**
> Yes, the configuration is valid. The minimum replicas do not exceed the maximum, and the stabilization window is non-negative.

---

**👤 You:**
> "Analyze this timeline for thrashing: [{'timestamp': '2024-01-01T00:00:00Z', 'observedMetric': 50, 'activeReplicaCount': 2}, {'timestamp': '2024-01-01T00:05:00Z', 'observedMetric': 90, 'activeReplicaCount': 3}, {'timestamp': '2024-01-01T00:10:00Z', 'observedMetric': 40, 'activeReplicaCount': 2}]"

**🤖 AI Agent:**
> The scaling timeline shows 1 oscillation event. The risk level is low as it does not exceed the threshold.


## ❓ FAQ

**Q: How does the simulator calculate target replicas?**
It uses the standard HPA formula: (current metric / target utilization) * current replicas, then rounds up and clamps within your min/max bounds.

**Q: Can I detect if my scaling configuration will cause thrashing?**
Yes, by using the `identify_thrashing_patterns` tool on a generated timeline, you can see if your stabilization windows are too short for your load volatility.

**Q: What kind of input does `simulate_scaling_timeline` require?**
It requires a JSON array of objects containing timestamps and metric values, representing your observed load pattern.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kubernetes-hpa-scaling-simulator](https://vinkius.com/mcp/kubernetes-hpa-scaling-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kubernetes HPA Scaling Simulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kubernetes-hpa-scaling-simulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kubernetes HPA Scaling Simulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kubernetes-hpa-scaling-simulator": {
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
