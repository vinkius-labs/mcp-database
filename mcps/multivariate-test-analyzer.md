# Multivariate Test Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/multivariate-test-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Perform 2k factorial analysis to identify optimal element combinations and interaction effects in multivariate experiments.

## Description
The Multivariate Test Analyzer is a statistical engine designed for simplified 2k Factorial Design of Experiments (DOE). It allows AI agents to analyze complex multivariate tests by evaluating how different elements (factors) and their variants impact conversion rates. By using tools like `calculate_main_effects`, `analyze_interaction_effects`, and `identify_winning_combination`, you can isolate the direct impact of individual elements, detect dependencies between pairs of factors, and pinpoint the statistically optimal configuration for your experiments.


## Available Tools (3)
- **analyze_interaction_effects**: Analyates interaction effects between pairs of factors
- **calculate_main_effects**: Each combination must have levels, conversions, and visits.

Calculates main effects for each factor in an experiment
- **identify_winning_combination**: Identifies the winning combination in an experiment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Multivariate Test Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which headline variant performed best in my experiment?"

**🤖 AI Agent:**
> The 'Sale' headline variant resulted in a 5% increase in conversion rate compared to the baseline.

---

**👤 You:**
> "Are there any interactions between button color and text size?"

**🤖 AI Agent:**
> Yes, a significant interaction was detected: the 'Large' text size performs significantly better when paired with the 'Green' button color.

---

**👤 You:**
> "What is the winning combination for my latest multivariate test?"

**🤖 AI Agent:**
> The optimal configuration is: Headline 'Summer Sale', Button 'Green', and Text Size 'Large', with an expected conversion rate of 12.5%.


## ❓ FAQ

**Q: What is the purpose of `calculate_main_effects`?**
This tool answers which individual elements or variants are driving the most significant change in conversions by calculating the average performance impact of switching a factor from its baseline to its variant level.

**Q: How can I detect if two elements work better together?**
Use the `analyze_interaction_effects` tool. It compares the observed performance of two-factor combinations against the expected performance if they acted independently, identifying significant dependencies.

**Q: How do I find the best configuration for my test?**
The `identify_winning_combination` tool identifies the specific setup with the highest conversion rate and verifies if it is statistically significantly better than the baseline using error variance analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/multivariate-test-analyzer](https://vinkius.com/mcp/multivariate-test-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Multivariate Test Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `multivariate-test-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Multivariate Test Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "multivariate-test-analyzer": {
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
