# Bioassay Potency Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bioassay-potency-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate relative potency and analyze dose-response parallelism.

## Description
This MCP server provides specialized computational tools for bioassay analysis. It allows AI agents to determine the relative potency of a test substance compared to a reference standard using 4PL modeling. Key capabilities include using `analyze_parallelism` to verify curve shapes, `calculate_relative_potency` for potency and confidence intervals, `calculate_slope_ratio` to compare curve steepness, and `compare_efficacy` to evaluate maximum biological effects.


## Available Tools (4)
- **calculate_slope_ratio**: Isolate and compare the steepness of the two dose-response curves
- **calculate_relative_potency**: Calculate the relative potency and its associated confidence intervals using a 4PL model
- **analyze_parallelism**: Determine if the Test and Reference dose-response curves are parallel enough to permit potency comparison
- **compare_efficacy**: Determine if the maximum biological effect (efficacy) of the Test substance is significantly different from the Reference


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bioassay Potency Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if these two dose-response datasets are parallel: testData=[{'dose': 0.1, 'response': 10}, {'dose': 1, 'response': 50}, {'dose': 10, 'response': 90}] and referenceData=[{'dose': 0.1, 'response': 12}, {'dose': 1, 'response': 48}, {'dose': 10, 'response': 92}]."

**🤖 AI Agent:**
> The curves are parallel with a slope ratio of 0.98 and a p-value of 0.85, confirming they can be compared.

---

**👤 You:**
> "Calculate the relative potency for these datasets: testData=[{'dose': 0.5, 'response': 20}, {'dose': 5, 'response': 80}] and referenceData=[{'dose': 1, 'response': 20}, {'dose': 10, 'response': 80}]."

**🤖 AI Agent:**
> The relative potency is 2.0, with a confidence interval between 1.85 and 2.15.

---

**👤 You:**
> "Compare the efficacy of the test substance against the reference using these data points: testData=[{'dose': 1, 'response': 100}] and referenceData=[{'dose': 1, 'response': 80}]."

**🤖 AI Agent:**
> The efficacy ratio is 1.25, indicating the test substance has a higher maximum biological effect than the reference.


## ❓ FAQ

**Q: How do I ensure my data is suitable for potency calculation?**
You should first use `analyze_parallelism` to confirm that the test and reference dose-response curves have similar slopes, which is a requirement for valid potency comparison.

**Q: What model is used for the calculations?**
The server utilizes a Four-Parameter Logistic (4PL) regression model to fit dose-response curves and derive potency values.

**Q: Can I compare the maximum effect of two substances?**
Yes, you can use the `compare_efficacy` tool to determine if the maximum biological effect of the test substance differs significantly from the reference.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bioassay-potency-calculator](https://vinkius.com/ai-agent-connect/bioassay-potency-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bioassay Potency Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bioassay-potency-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bioassay Potency Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bioassay-potency-calculator": {
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
