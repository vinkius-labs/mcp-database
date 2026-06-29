# A/B Test Significance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ab-test-significance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate statistical significance, p-values, and uplift for A/B tests.

## Description
This MCP server provides a specialized engine for evaluating A/B test results. By connecting your AI agent to this tool, you can instantly compute critical experimental metrics including p-values, confidence intervals (90%, 95%, and 99%), relative and absolute uplift, and statistical power. Use `calculate_significance_metrics` to determine the probability of observed differences occurring by chance, `calculate_uplift_analysis` to measure the magnitude of change between groups, and `generate_experiment_verdict` to receive actionable business recommendations on whether to end a test or continue collecting data.


## Available Tools (3)
- **generate_experiment_verdict**: Provides a business recommendation on whether to end the test or continue collecting data
- **calculate_significance_metrics**: Calculates core probability metrics and confidence ranges for the experiment
- **calculate_uplift_analysis**: Computes the magnitude of change between the control and variant groups


## 💬 Prompt Examples

Here are some examples of how you can interact with the **A/B Test Significance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have an A/B test where the control group had 1000 visitors and 50 conversions, while the variant group had 1100 visitors and 70 conversions. What is the significance?"

**🤖 AI Agent:**
> The p-value for this test is approximately 0.145, which suggests that the observed difference is not statistically significant at the 95% confidence level.

---

**👤 You:**
> "Calculate the uplift for a control group with 5000 visitors and 200 conversions, and a variant group with 5200 visitors and 250 conversions."

**🤖 AI Agent:**
> The relative uplift is approximately 12.5%, and the absolute uplift is an increase of 0.96 percentage points.

---

**👤 You:**
> "Based on a p-value of 0.03 and a statistical power of 0.85, should I end my experiment with a significance threshold of 0.05?"

**🤖 AI Agent:**
> Yes, you should end the test. The result is conclusive because the p-value is below the threshold and the power meets the required level.


## ❓ FAQ

**Q: How can I determine if my A/B test result is significant?**
You can use the `calculate_significance_metrics` tool. It will return a p-value; if this value is below your significance threshold (typically 0.05), the result is considered statistically significant.

**Q: What does 'relative uplift' mean in this context?**
Relative uplift represents the percentage change in the conversion rate of your variant group compared to your control group, calculated using `calculate_uplift_analysis`.

**Q: Can this tool help me decide when to stop an experiment?**
Yes. By using `generate_experiment_verdict`, you can provide the p-value and statistical power to receive a recommendation on whether to end the test or continue collecting data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ab-test-significance-calculator](https://vinkius.com/mcp/ab-test-significance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **A/B Test Significance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ab-test-significance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **A/B Test Significance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ab-test-significance-calculator": {
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
