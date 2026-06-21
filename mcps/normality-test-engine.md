# Normality Test Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/normality-test-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Test whether your data is normally distributed using Skewness and Kurtosis analysis local. Essential pre-check before running parametric statistical tests.

## Description
Before running t-tests, ANOVA, or linear regression, you need to verify that your data is normally distributed. LLMs cannot eyeball a distribution from raw numbers — they will guess and often guess wrong.

This MCP uses `simple-statistics` to compute exact Skewness and Kurtosis coefficients, then applies a Jarque-Bera test to determine normality. The AI gets a definitive pass/fail verdict with the exact test statistic and p-value.

### The Superpowers

- **Zero Hallucination:** Exact statistical coefficients computed locally.
- **Automated Verdict:** Returns a clear 'normal' or 'not normal' interpretation.
- **Descriptive Statistics:** Also provides exact Mean, Std Dev, Skewness, and Kurtosis.
- **Data Privacy:** Your research data stays entirely on your local machine.


## Available Tools
- **test_normality**: Perform an exact deterministic Jarque-Bera normality test on numeric data without LLM math hallucinations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Normality Test Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this residuals array is normally distributed before I run my regression."

**🤖 AI Agent:**
> The Jarque-Bera test returns p = 0.42. We fail to reject the normality hypothesis — your residuals appear normally distributed. Proceed with the regression.

---

**👤 You:**
> "Is this sensor data normally distributed or should I use a non-parametric test?"

**🤖 AI Agent:**
> The data shows significant positive skewness (1.8) and high kurtosis (5.2). The Jarque-Bera p-value is 0.001 — the data is not normally distributed. Use a non-parametric test.

---

**👤 You:**
> "Run a normality test on the 'Revenue' column before I calculate confidence intervals."

**🤖 AI Agent:**
> Normality test passed (p = 0.61). Skewness is 0.3 and kurtosis is 2.9 — both close to normal parameters. Your confidence intervals will be valid.


## ❓ FAQ

**Q: Is this the Shapiro-Wilk test?**
This engine implements the Jarque-Bera normality test, which uses Skewness and Kurtosis. It is highly effective for medium-to-large samples and avoids the Shapiro-Wilk implementation gaps in JavaScript.

**Q: How many data points do I need?**
The Jarque-Bera test works best with 30 or more samples. For very small samples (n < 20), consider using visual QQ-plot analysis as a complement.

**Q: What does a 'not normal' result mean for my analysis?**
If your data is not normally distributed, parametric tests like t-tests and ANOVA may be unreliable. Consider using non-parametric alternatives like Spearman correlation or Mann-Whitney U tests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/normality-test-engine](https://vinkius.com/mcp/normality-test-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Normality Test Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `normality-test-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Normality Test Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "normality-test-engine": {
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
