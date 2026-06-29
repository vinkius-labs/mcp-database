# AB Test Sample Size Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ab-test-sample-size-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate required sample size, test duration, and peeking risk for A/B experiments.

## Description
This MCP server provides essential statistical tools for running reliable A/B tests. Use `calculate_required_sample_size` to determine the number of users needed per variant based on your baseline conversion rate and desired Minimum Detectable Effect (MDE). With `estimate_test_duration`, you can project how many days your experiment must run given your daily traffic. Finally, use `assess_peeking_risk` to evaluate the danger of stopping a test prematurely, helping you avoid false positives caused by early analysis.


## Available Tools (3)
- **calculate_required_sample_size**: Determine the required sample size for an A/B test
- **estimate_test_duration**: Estimate the duration of an A/B test
- **assess_peeking_risk**: Assess the risk of stopping an A/B test early


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AB Test Sample Size Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a baseline conversion rate of 10% (0.10). I want to detect a 5% relative change (0.05) with 95% confidence and 80% power. How many users do I need?"

**🤖 AI Agent:**
> To detect a 5% relative change from a 10% baseline with 95% confidence and 80% power, you will need approximately 156,432 users per variant, for a total of 312,864 users.

---

**👤 You:**
> "If I need 50,000 total users and my site gets 2,500 visitors per day, how long will the test take?"

**🤖 AI Agent:**
> Based on a requirement of 50,000 users and daily traffic of 2,500, your test is estimated to run for 20 days.

---

**👤 You:**
> "My A/B test has been running for 5 days. The planned duration was 14 days. What is my risk level?"

**🤖 AI Agent:**
> With only 5 days elapsed out of a planned 14, your peeking risk is High. You should continue the test until the planned duration is reached to avoid false positives.


## ❓ FAQ

**Q: How do I know if my sample size is sufficient?**
You can use the `calculate_required_sample_size` tool. By providing your baseline conversion rate, MDE, confidence level, and statistical power, it will return exactly how many users you need per variant.

**Q: What is the risk of 'peeking' at my results?**
Peeking refers to checking results and stopping a test before its planned duration. This significantly increases your False Positive rate. Use `assess_peeking_risk` to see if your current progress is safe or if you are at high risk of making an incorrect decision.

**Q: How can I estimate when my test will finish?**
Once you have the total required users from the sample size tool, use `estimate_test_duration` along with your average daily traffic to calculate the estimated number of days needed for the experiment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ab-test-sample-size-calculator](https://vinkius.com/mcp/ab-test-sample-size-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AB Test Sample Size Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ab-test-sample-size-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AB Test Sample Size Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ab-test-sample-size-calculator": {
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
