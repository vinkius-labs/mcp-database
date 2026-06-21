# T-Test Statistics Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/t-test-statistics-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Run exact Student's, Welch's, and Paired t-tests local. Get CPU-guaranteed p-values instead of LLM-hallucinated guesses.

## Description
LLMs are notoriously bad at math. If you ask an AI to calculate a p-value for a dataset, it will likely hallucinate a plausible-looking but completely wrong number. Data Scientists cannot tolerate this.

This MCP brings deterministic statistical computation to your AI. It delegates the complex math (Student's t-test, Welch's t-test, Paired t-tests) to the robust local `jstat` engine. The AI simply extracts the data, sends it to this engine, and gets back the mathematically guaranteed t-score, degrees of freedom, and exact p-value.

### The Superpowers

- **Zero Hallucination:** Exact p-values calculated by a CPU, not a language model.
- **Full T-Test Suite:** Supports Independent, Paired, and One-Sample tests.
- **Data Privacy:** Your company's experimental data stays local.
- **Automated Interpretation:** Automatically tells the AI whether to reject the null hypothesis at alpha=0.05.


## Available Tools
- **calculate_t_test**: Perform exact deterministic Student's t-tests (independent, paired, one-sample) to calculate statistical significance without LLM hallucinations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **T-Test Statistics Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run an independent t-test to see if the conversion rates for Variant A and Variant B are significantly different."

**🤖 AI Agent:**
> The t-score is 2.45 and the p-value is 0.018. Since p < 0.05, there is a statistically significant difference between the two variants.

---

**👤 You:**
> "Do a paired t-test on these pre-treatment and post-treatment blood pressure readings."

**🤖 AI Agent:**
> The paired t-test gives a p-value of 0.002. We reject the null hypothesis — the treatment had a statistically significant effect on blood pressure.

---

**👤 You:**
> "Perform a one-sample t-test to check if this batch's mean weight differs from the target of 500g."

**🤖 AI Agent:**
> The calculated p-value is 0.34. We fail to reject the null hypothesis — the batch weight is not significantly different from the 500g target.


## ❓ FAQ

**Q: Why shouldn't I just ask the AI to calculate the p-value directly?**
Because Large Language Models generate text based on probability, not logic. They frequently hallucinate complex floating-point math. This engine forces the AI to use a real local calculator, producing exact results every single time.

**Q: Does it assume equal variances?**
For independent tests, it currently uses the standard Student's t-test which assumes equal variance. Paired and one-sample tests calculate their specific formulas independently.

**Q: What alpha level is used for significance interpretation?**
The engine automatically interprets significance using the standard alpha = 0.05 (95% confidence level). The exact p-value is always returned so you can apply any custom threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/t-test-statistics-engine](https://vinkius.com/mcp/t-test-statistics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **T-Test Statistics Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `t-test-statistics-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **T-Test Statistics Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "t-test-statistics-engine": {
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
