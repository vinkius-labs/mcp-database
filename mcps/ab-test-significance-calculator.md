# A/B Test Significance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ab-test-significance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Calculate statistical significance, required sample sizes, and power for A/B tests.

## Description
This MCP server provides a complete statistical engine for analyzing A/B test results. It allows you to determine if observed differences in conversion rates are statistically significant using the `analyze_conversion_difference` tool. You can plan future experiments by estimating necessary visitor counts with `calculate_required_sample_size`. Additionally, monitor your ongoing tests' strength via `calculate_statistical_power` and protect against false positives by using `check_peeking_risk` to detect the dangers of early data analysis.


## Available Tools (4)
- **analyze_conversion_rab_difference**: Analyze the difference in conversion rates between two groups
- **calculate_statistical_power**: Calculate the current power of an ongoing test
- **calculate_required_sample_size**: Calculate the required sample size per group for a new A/B test
- **check_peeking_risk**: Check the risk of peeking at A/B test results


## 💬 Prompt Examples

Here are some examples of how you can interact with the **A/B Test Significance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the difference between 500 conversions in 10,000 visitors (Group A) and 550 conversions in 10,000 visitors (Group B) statistically significant at a 95% confidence level?"

**🤖 AI Agent:**
> Yes, the p-value is approximately 0.032, which is below the 0.05 threshold, indicating statistical significance.

---

**👤 You:**
> "How many visitors do I need per group for a new test with a baseline conversion rate of 0.10, an MDE of 0.02, power of 0.80, and alpha of 0.05?"

**🤖 AI Agent:**
> You will need approximately 3,975 visitors per group to achieve the desired statistical power.

---

**👤 You:**
> "I have checked my A/B test results 5 times so far. The current sample size is 1,200 and the planned sample size was 5,000. What is my risk level?"

**🤖 AI Agent:**
> The risk level is high because you have performed multiple checks while only a small fraction of the planned sample size has been reached.


## ❓ FAQ

**Q: How can I check if my current A/B test results are significant?**
You can use the `analyze_conversion_difference` tool by providing the number of visitors and conversions for both your control and variant groups.

**Q: How do I know if I am checking my results too frequently?**
Use the `check_peeking_risk` tool to assess the risk level associated with multiple data inspections before reaching the target sample size.

**Q: Can I estimate how many users are needed for a new experiment?**
Yes, use the `calculate_required_sample_size` tool by specifying your baseline conversion rate and desired minimum detectable effect.


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
