# Bayesian A/B Testing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bayesian-ab-testing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify conversion probability, expected loss, and uplift using Bayesian inference.

## Description
This MCP server provides a powerful statistical engine for evaluating A/B test results. Using the Beta-Bernoulli conjugate prior relationship, it allows you to move beyond simple p-values and understand the actual probability of one variant outperforming another. You can use tools like `calculate_superiority_probability` to determine how confident you are in a winner, `calculate_expected_loss` to quantify the risk of making a wrong decision, and `evaluate_decision_recommendation` to get actionable next steps based on your specific confidence threshold.


## Available Tools (4)
- **evaluate_decision_recommendation**: Evaluate the decision recommendation based on a threshold
- **calculate_superiority_probability**: Calculate the probability that Variant B is better than Variant A
- **calculate_expected_loss**: Calculate the expected loss for choosing either variant
- **calculate_expected_uplift**: Calculate the expected uplift of Variant B over Variant 1


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bayesian A/B Testing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the probability that Variant B is better than Variant A, where A has 100 conversions out of 1000 visitors and B has 130 conversions out of 1000 visitors."

**🤖 AI Agent:**
> The probability that Variant B is superior to Variant A is approximately 94.5%.

---

**👤 You:**
> "What is the expected loss if I choose Variant B, given A has 50/500 conversions and B has 60/500 conversions?"

**🤖 AI Agent:**
> The expected loss for choosing Variant B is approximately 0.004 (or 0.4%).

---

**👤 You:**
> "Evaluate the decision recommendation for A: 20/200, B: 30/200 with a 95% threshold."

**🤖 AI Agent:**
> The decision is INCONCLUSIVE because the probability of superiority does not meet the 95% threshold.


## ❓ FAQ

**Q: What does the superiority probability tell me?**
It tells you the likelihood that Variant B's conversion rate is higher than Variant A's, based on your observed data.

**Q: How do I use the decision recommendation tool?**
Provide your conversion and visitor counts for both variants. You can also set a `confidenceThreshold` (e.g., 0.95) to define how much certainty you require before the tool recommends choosing Variant B.

**Q: What is 'Expected Loss' in this context?**
Expected loss quantifies the potential downside risk. It represents the expected reduction in conversion rate if you choose a variant that is actually inferior to the other.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bayesian-ab-testing-calculator](https://vinkius.com/mcp/bayesian-ab-testing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bayesian A/B Testing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bayesian-ab-testing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bayesian A/B Testing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bayesian-ab-testing-calculator": {
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
