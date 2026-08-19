# Agent A/B Test Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-ab-test-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

A deterministic statistical engine for evaluating performance differences between agent variants.

## Description
This MCP server provides a precise statistical engine to evaluate performance differences between different AI agent variants. It allows you to determine if a change in an agent's behavior resulted in a statistically significant improvement in conversion rates. Using tools like `analyze_variant_performance`, you can calculate p-values, confidence intervals, and relative lift while accounting for Bonferroni corrections in multi-variant tests. You can also use `estimate_test_requirements` to plan future experiments by calculating necessary sample sizes and test durations, or `calculate_bayesian_probability` to estimate the likelihood that one variant outperforms another using Beta distributions.


## Available Tools (3)
- **analyze_variant_performance**: 95 or 0.99), and the minimum detectable effect (MDE).

Analyzes the performance of multiple agent variants to determine statistical significance
- **calculate_bayesian_probability**: Calculates the Bayesian probability that variant B is better than variant A
- **estimate_test_requirements**: Estimates the required sample size and duration for an A/B test


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent A/B Test Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the performance of two variants: Variant A had 50 successes out of 1000 attempts, and Variant B had 70 successes out of 1000 attempts. Use a 95% confidence level."

**🤖 AI Agent:**
> Variant B shows a conversion rate of 7.0% compared to Variant A's 5.0%, resulting in a relative lift of 40.0%. This difference is statistically significant with a p-value of 0.012.

---

**👤 You:**
> "I expect a baseline conversion rate of 5% and want to detect a 2% MDE. My agent gets 100 attempts per day. How long will the test take with 95% confidence?"

**🤖 AI Agent:**
> To detect a 2% MDE with 95% confidence, you will need a total sample size of approximately 3,850 attempts. At 100 attempts per day, the test will take about 39 days.

---

**👤 You:**
> "What is the probability that Variant B (10 successes, 100 total) is better than Variant A (8 successes, 100 total)?"

**🤖 AI Agent:**
> The Bayesian probability that Variant B is better than Variant A is approximately 72.4%.


## ❓ FAQ

**Q: How do I know if my agent's performance improvement is real?**
You can use the `analyze_variant_performance` tool. It calculates the p-value to determine if the observed difference in conversion rates is statistically significant or likely due to chance.

**Q: Can I plan how long an experiment should run?**
Yes, the `estimate_test_requirements` tool calculates the required sample size and the estimated number of days needed to complete a test based on your daily traffic and desired sensitivity.

**Q: What is the difference between the frequentist and Bayesian approaches provided?**
The frequentist approach (via `analyze_variant_performance`) focuses on p-values and significance thresholds, while the Bayesian approach (via `calculate_bayesian_probability`) provides the direct probability that one variant is better than another.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-ab-test-calculator](https://vinkius.com/ai-agent-connect/agent-ab-test-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent A/B Test Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-ab-test-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent A/B Test Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-ab-test-calculator": {
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
