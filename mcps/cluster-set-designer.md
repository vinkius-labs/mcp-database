# Cluster Set Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cluster-set-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Design optimized cluster set training protocols for strength and hypertrophy.

## Description
This MCP server provides specialized tools to design cluster set training protocols. By breaking large sets into smaller mini-sets, you can maintain higher intensity and manage fatigue more effectively. Use `get_cluster_configuration` to structure your mini-sets, `calculate_set_metrics` to determine total workload, `design_rest_protocol` to find optimal recovery times, and `validate_protocol_viability` to ensure your training plan is physically realistic.


## Available Tools (4)
- **calculate_set_metrics**: Calculate the total workload and relative intensity profile of the planned cluster set
- **design_rest_protocol**: Determine the necessary inter-cluster rest duration to maintain technical proficiency
- **get_cluster_configuration**: Determine the optimal structure of mini-sets based on a total rep goal and fatigue management preferences
- **validate_protocol_viability**: Check if the proposed cluster set design is physically realistic for a standard training session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cluster Set Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to do 10 total reps using a low-reps-per-cluster approach. How should I structure this?"

**🤖 AI Agent:**
> For a total of 10 reps with low reps per cluster, you should perform 5 clusters of 2 repetitions each, with the recommended rest intervals provided by the tool.

---

**👤 You:**
> "Calculate the total volume for 4 clusters of 5 reps at 100kg."

**🤖 AI Agent:**
> The total volume for 4 clusters of 5 reps at 100kg is 2000kg.

---

**👤 You:**
> "Is a protocol of 12 reps in 2 clusters of 6 reps with 10 seconds rest viable?"

**🤖 AI Agent:**
> The protocol is considered unviable because the rest duration is too short for the number of repetitions per cluster, which may lead to excessive fatigue.


## ❓ FAQ

**Q: What are cluster sets?**
Cluster sets are a training technique where a large set is divided into smaller mini-sets separated by short rest intervals, allowing for higher intensity and volume.

**Q: How do I know if my training plan is safe?**
You can use the `validate_protocol_viability` tool to check if your proposed cluster set design is physically realistic and assess its risk level.

**Q: Can I use this for both strength and muscle growth?**
Yes, the tool supports different fatigue management profiles that cater to Power, Strength, and Hypertrophy training tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cluster-set-designer](https://vinkius.com/en/ai-agent-connect/cluster-set-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cluster Set Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cluster-set-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cluster Set Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cluster-set-designer": {
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
