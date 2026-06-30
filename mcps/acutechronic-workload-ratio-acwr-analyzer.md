# Acute:Chronic Workload Ratio (ACWR) Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acutechronic-workload-ratio-acwr-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports-science](../categories/sports-science.md)

Predict injury risk by analyzing the relationship between recent and long-term training loads.

## Description
The ACWR Analyzer connects AI agents to sports science metrics, allowing for precise monitoring of athlete training stress. Using tools like `calculate_acwr_series`, `evaluate_risk_tier`, `detect_load_trend`, and `generate_training_prescription`, the server calculates the ratio between acute (recent) and chronic (baseline) workloads. It identifies potential injury zones, such as the 'Danger Zone' for high-intensity spikes, or 'Under-training' for insufficient load. Coaches can use this to receive actionable training prescriptions based on real-time workload fluctuations.


## Available Tools (4)
- **calculate_acwr_series**: Calculates a series of ACWR values
- **detect_load_trend**: Detects training load trend
- **evaluate_risk_tier**: Evaluates injury risk tier
- **generate_training_prescription**: Generates coaching advice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acute:Chronic Workload Ratio (ACWR) Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ACWR for these weekly loads: [100, 120, 110, 150] with a 4-week chronic window."

**🤖 AI Agent:**
> The calculated ACWR for the latest week is 1.25, which falls within the Safe Zone.

---

**👤 You:**
> "What is the injury risk if my current ACWR is 1.6?"

**🤖 AI Agent:**
> A ratio of 1.6 puts the athlete in the Danger Zone, indicating a high risk of injury due to an excessive workload spike.

---

**👤 You:**
> "Analyze the trend for these ACWR values: [1.0, 1.1, 1.3, 1.4]."

**🤖 AI Agent:**
> The training load trend is increasing, with a volatility of approximately 0.15.


## ❓ FAQ

**Q: What is the purpose of the `calculate_acwr_series` tool?**
It processes a sequence of weekly training loads to generate a series of ACWR values and summary statistics.

**Q: How does `evaluate_risk_tier` determine injury risk?**
It applies specific thresholds to the current ratio: below 0.8 is Under-training, 0.8-1.3 is Safe, 1.3-1.5 is Moderate Risk, and above 1.5 is the Danger Zone.

**Q: Can I get coaching advice using this server?**
Yes, the `generate_training_prescription` tool provides actionable instructions like 'Maintain', 'Increase', or 'Reduce' load based on your current ratio and trend.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acutechronic-workload-ratio-acwr-analyzer](https://vinkius.com/mcp/acutechronic-workload-ratio-acwr-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acute:Chronic Workload Ratio (ACWR) Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `acutechronic-workload-ratio-acwr-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acute:Chronic Workload Ratio (ACWR) Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acutechronic-workload-ratio-acwr-analyzer": {
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
