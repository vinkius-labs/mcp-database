# Accelerator Cohort Diversity Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-cohort-diversity-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Analyze cohort diversity, inclusion indices, and performance correlations.

## Description
This MCP server provides deep analytical insights into startup accelerator cohorts. It allows users to calculate a holistic diversity score, measure the inclusion index against target benchmarks, and identify selection or outreach bias. By using tools like `calculate_diversity_metrics`, `analyze_selection_bias`, and `evaluate_performance_correlation`, accelerators can quantify the relationship between demographic variety and cohort success metrics.


## Available Tools (3)
- **analyze_selection_bias**: Analyzes selection and outreach bias
- **calculate_diversity_metrics**: Calculates diversity, inclusion, and cohort composition metrics
- **evaluate_performance_correlation**: Evaluates correlation between diversity and performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Cohort Diversity Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the diversity metrics for a cohort with these demographics: { "gender": {"m": 10, "f": 10}, "raceEthnicity": {"groupA": 10, "groupB": 10}, "geography": {"us": 15, "intl": 5} }, industries: ["SaaS", "FinTech"], and education: ["University"]"

**🤖 AI Agent:**
> The cohort has a diversity score of 0.85 and an inclusion index of 0.92, reflecting a highly balanced composition across gender and ethnicity.

---

**👤 You:**
> "Analyze the bias between an applicant pool of { "groupA": 50, "groupB": 50 } and a selected cohort of { "groupA": 40, "groupB": 10 }."

**🤖 AI Agent:**
> The analysis indicates a high selection bias score, suggesting the selection process is favoring groupA over groupB.

---

**👤 You:**
> "Is there a correlation between these diversity scores [0.5, 0.7, 0.9] and these performance metrics [1M, 2M, 5M]?"

**🤖 AI Agent:**
> There is a strong positive correlation (0.98) between diversity scores and performance outcomes, which is statistically significant.


## ❓ FAQ

**Q: How is the diversity score calculated?**
The `calculate_diversity_metrics` tool aggregates variety across gender, race/ethnicity, and geography to produce a holistic score.

**Q: Can I detect if my selection process is biased?**
Yes, the `analyze_selection_bias` tool compares the applicant pool to the selected cohort to identify selection-driven or outreach-driven skew.

**Q: Does diversity impact cohort performance?**
You can evaluate this using `evaluate_performance_correlation`, which measures the mathematical relationship between diversity scores and performance outcomes like capital raised.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-cohort-diversity-analytics](https://vinkius.com/ai-agent-connect/accelerator-cohort-diversity-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Cohort Diversity Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-cohort-diversity-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Cohort Diversity Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-cohort-diversity-analytics": {
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
