# Chi-Square Test Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chi-square-test-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Run exact Chi-Square independence tests on contingency tables local. Get CPU-guaranteed chi² statistics and p-values for categorical analysis.

## Description
The Chi-Square test determines whether two categorical variables are independent. Asking an LLM to compute expected frequencies across a matrix and then sum the chi² residuals is a recipe for hallucinated results.

This MCP computes the full test deterministically using `jstat`. The AI sends the observed frequency matrix, and the engine calculates exact expected frequencies, the chi² statistic, degrees of freedom, and the p-value — all locally on your CPU.

### The Superpowers

- **Zero Hallucination:** Exact chi² statistics computed deterministically.
- **Automatic Expected Frequencies:** The engine builds the entire expected matrix internally.
- **Any Matrix Size:** Supports 2x2, 3x3, or larger contingency tables.
- **Data Privacy:** Your survey and business data stays local.


## Available Tools (1)
- **calculate_chi_square**: Perform exact deterministic Chi-Square tests of independence on categorical contingency tables without LLM math hallucinations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chi-Square Test Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is there a statistically significant relationship between user gender and subscription tier?"

**🤖 AI Agent:**
> The Chi-Square test returns chi² = 8.42, df = 2, p-value = 0.015. Since p < 0.05, there is a statistically significant relationship between gender and subscription tier.

---

**👤 You:**
> "Check if the distribution of customer complaints varies by product category."

**🤖 AI Agent:**
> The p-value is 0.32. We cannot reject the null hypothesis — the complaint distribution appears independent of product category.

---

**👤 You:**
> "Run a chi-square test on this survey data to see if education level affects voting preference."

**🤖 AI Agent:**
> Chi² = 15.8, df = 6, p-value = 0.015. The result is statistically significant — education level and voting preference are not independent.


## ❓ FAQ

**Q: What is a contingency table?**
It's a matrix showing the frequency distribution of two categorical variables (e.g., rows = Gender, columns = Subscription Tier). The AI will automatically convert your raw data into this format.

**Q: Does it handle expected frequencies below 5?**
The engine computes the result regardless, but the AI is instructed to warn you when expected frequencies are low, as the chi² approximation becomes less reliable in those cases.

**Q: Can it test more than two variables at once?**
This engine performs a single pairwise independence test per execution. For multi-variable analysis, the AI can chain multiple calls to test different variable pairs sequentially.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chi-square-test-engine](https://vinkius.com/mcp/chi-square-test-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chi-Square Test Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chi-square-test-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chi-Square Test Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chi-square-test-engine": {
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
