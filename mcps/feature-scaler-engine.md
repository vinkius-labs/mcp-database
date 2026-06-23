# Feature Scaler Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/feature-scaler-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Standardize (Z-Score) or MinMax scale numeric columns with mathematical perfection local. Essential normalization for neural networks and clustering algorithms.

## Description
Neural Networks and K-Means clustering algorithms fail spectacularly if features aren't normalized. If an LLM attempts to subtract the mean and divide by the standard deviation across 5,000 rows, it will hallucinate 90% of the math.

This MCP brings deterministic Feature Scaling to your AI using `simple-statistics`. The AI specifies whether it wants Standard scaling (Mean=0, Variance=1) or MinMax scaling (Range 0-1), and the engine flawlessly transforms the target columns in milliseconds — returning the exact computed metrics for auditability.

### The Superpowers

- **Flawless Normalization:** No LLM math hallucinations — exact scaling computed by your CPU.
- **Multi-Column Support:** Scale multiple features simultaneously in a single call.
- **Automated Metric Extraction:** Returns the exact Means, Std Devs, Mins, and Maxs used for scaling.
- **Data Privacy:** Your sensitive training data stays entirely on your machine.


## Available Tools (1)
- **scale_features**: Deterministically Standardize (Z-Score) or MinMax Scale numeric columns offline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Feature Scaler Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Standardize the 'Age' and 'Salary' columns to have a mean of 0 and variance of 1."

**🤖 AI Agent:**
> Scaling complete. The Age column had a mean of 34 (std dev 5.2) and the Salary column had a mean of $85k (std dev $22k). Both columns are now centered at 0.

---

**👤 You:**
> "Apply MinMax scaling to the 'PixelIntensity' feature so all values are between 0 and 1."

**🤖 AI Agent:**
> Done. The original values ranged from 0 to 255. All PixelIntensity values are now compressed precisely between 0.0 and 1.0, ready for your neural network.

---

**👤 You:**
> "Normalize all numeric features in this dataset before training my K-Means clustering model."

**🤖 AI Agent:**
> All 12 numeric columns have been standard-scaled. Each column now has mean ≈ 0 and std dev ≈ 1. The computed metrics have been returned for future inverse transformations.


## ❓ FAQ

**Q: What is the difference between Standard and MinMax scaling?**
Standard scaling (Z-Score) centers data at 0 with a variance of 1, ideal for algorithms that assume normally distributed features. MinMax compresses all values precisely between 0 and 1, ideal for neural networks and distance-based algorithms.

**Q: Are the computed scaling parameters returned for inverse transforms?**
Yes. The JSON response includes the exact Mean and Std Dev (for Standard) or Min and Max (for MinMax) used to scale each column, enabling precise inverse transformations when needed.

**Q: Can it scale 10+ columns at once?**
Absolutely. Pass a JSON array of all column names and they will all be scaled simultaneously in memory. The engine processes each column independently with its own computed metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/feature-scaler-engine](https://vinkius.com/mcp/feature-scaler-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Feature Scaler Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `feature-scaler-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Feature Scaler Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "feature-scaler-engine": {
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
