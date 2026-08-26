# Lentil Splitting Yield Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/lentil-splitting-yield-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predicts lentil splitting yield, breakage, and cooking performance.

## Description
This MCP server provides specialized tools for predicting the processing yield and quality of lentils intended for dhal production. Use `predict_splitting_yield` to calculate expected dhal yield and broken seed percentages based on seed size, coat thickness, and moisture. You can also use `estimate_cooking_performance` to determine cooking time and hydration capacity, or `classify_grade` to assign commercial grades based on predicted outcomes.


## Available Tools (4)
- **classify_grade**: Assigns a commercial grade to the batch based on predicted yield and quality
- **estimate_cooking_performance**: Predicts the time required for cooking and the water absorption properties
- **get_processing_margin**: Provides a financial or efficiency buffer based on the predicted loss during splitting
- **predict_splitting_yield**: Calculates the expected volume of usable dhal and the expected percentage of broken seeds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lentil Splitting Yield Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected yield for a lentil variety with a seed size of 5mm, coat thickness of 0.2mm, and 12% moisture?"

**🤖 AI Agent:**
> The expected dhal yield is 85% with a broken percentage of 4%.

---

**👤 You:**
> "Predict the cooking performance for a variety with 5mm size and 10% moisture content."

**🤖 AI Agent:**
> The estimated cooking time is 18 minutes with a high hydration capacity.

---

**👤 You:**
> "What grade will a batch get if it has 88% yield and 3% breakage with a quality rating of 8?"

**🤖 AI Agent:**
> The batch is classified as Grade A.


## ❓ FAQ

**Q: How does harvest timing affect the results?**
Harvest timing influences seed coat integrity. Using `predict_splitting_yield` with a 'late' harvest timing will account for increased fragility and higher breakage risk.

**Q: Can I determine the commercial grade of my batch?**
Yes, by using the `classify_grade` tool with the yield and breakage data obtained from the prediction tools.

**Q: What information is needed to predict cooking time?**
To use `estimate_cooking_performance`, you need to provide the seed size, moisture content, cooking quality rating, and the specific variety.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/lentil-splitting-yield-predictor](https://vinkius.com/ai-agent-connect/lentil-splitting-yield-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lentil Splitting Yield Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lentil-splitting-yield-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lentil Splitting Yield Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lentil-splitting-yield-predictor": {
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
