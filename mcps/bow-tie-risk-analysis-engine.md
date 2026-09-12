# Bow-Tie Risk Analysis Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bow-tie-risk-analysis-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-management](../categories/risk-management.md)

A quantitative risk assessment engine for modeling threats, top events, and consequences using bow-tie analysis.

## Description
This MCP server provides a mathematical and visual framework for risk assessment. It allows AI agents to model the relationship between hazards, threats, and consequences. Using tools like `analyze_threat_path` and `analyze_consequence_path`, agents can evaluate how preventive and mitigative barriers affect risk likelihood and severity. The engine also includes `evaluate_barrier_health` to account for degradation factors and `calculate_risk_reduction_profile` to provide a high-level summary of total risk reduction.


## Available Tools (4)
- **analyze_threat_path**: Evaluates the relationship between a specific threat and the top event, accounting for preventive barriers
- **calculate_risk_reduction_profile**: Provides a high-level summary of how much risk is reduced by the current set of barriers
- **analyze_consequence_path**: Evaluates the relationship between the top event and a consequence, accounting for mitigative barriers
- **evaluate_barrier_health**: Assesses the current capability of a specific barrier by considering its degradation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bow-Tie Risk Analysis Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the threat path for threat 'T-101' leading to top event 'TE-202' using preventive barriers 'B-01' and 'B-02'."

**🤖 AI Agent:**
> The threat likelihood for T-101 is 0.8. After applying barriers B-01 and B-02, the residual threat likelihood is reduced to 0.15, and the path is successfully blocked.

---

**👤 You:**
> "What is the current health status of barrier 'B-500'?"

**🤖 AI Agent:**
> Barrier B-500 has a nominal effectiveness of 0.95, but due to degradation, its current effectiveness is 0.72. The status is currently 'Degraded'.

---

**👤 You:**
> "Calculate the risk reduction profile for top event 'TE-99'."

**🤖 AI Agent:**
> For top event TE-99, the unmitigated risk score is 100.0 and the mitigated risk score is 12.5, resulting in a total reduction percentage of 87.5%. No critical gaps were identified.


## ❓ FAQ

**Q: How does the engine handle barrier degradation?**
The engine uses `evaluate_barrier_health` to assess how degradation factors reduce a barrier's nominal effectiveness, providing a real-time view of current capability.

**Q: Can I see the total risk reduction for a specific event?**
Yes, you can use `calculate_risk_reduction_profile` to get a summary of unmitigated vs mitigated risk scores and identify critical gaps.

**Q: What is the difference between preventive and mitigative barriers?**
Preventive barriers act before a top event to stop threats, while mitigative barriers act after a top event to reduce the impact of consequences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bow-tie-risk-analysis-engine](https://vinkius.com/en/ai-agent-connect/bow-tie-risk-analysis-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bow-Tie Risk Analysis Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bow-tie-risk-analysis-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bow-Tie Risk Analysis Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bow-tie-risk-analysis-engine": {
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
