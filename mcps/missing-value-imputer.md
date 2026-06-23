# Missing Value Imputer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/missing-value-imputer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automatically fill NaN and missing values in datasets using Mean, Median, Mode, or Zero strategies deterministically local. Essential ML data preparation.

## Description
Preparing a dataset for machine learning requires handling missing values. Asking an LLM to find and replace NaN entries row-by-row in a 10,000-row JSON consumes an absurd amount of context tokens and is guaranteed to corrupt your data.

This MCP delegates the imputation logic to a local engine powered by `simple-statistics`. The AI sends the raw data, and the engine mathematically computes the exact Mean, Median, or Mode across all valid entries, then seamlessly replaces every missing value — all in memory, all local.

### The Superpowers

- **Zero Hallucination:** The fill value is computed exactly from your data by the CPU, never estimated by a language model.
- **Multiple Strategies:** Choose Mean, Median, Mode, or Zero filling depending on your statistical needs.
- **Fast and Private:** Processes thousands of rows in milliseconds entirely on your machine.
- **Transparent Reporting:** Returns the exact fill value applied and the number of rows imputed for full auditability.


## Available Tools (1)
- **impute_missing_values**: Deterministically fill NaN/missing values in a dataset using Mean, Median, Mode, or Zero


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Missing Value Imputer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fill all missing values in the 'Age' column with the median age of the dataset."

**🤖 AI Agent:**
> Done. The computed median age was 34 years. 15 missing rows were successfully imputed. Here is a preview of the first 10 cleaned rows.

---

**👤 You:**
> "Use the mean strategy to fix the NaN values in the 'Salary' column before I train my model."

**🤖 AI Agent:**
> The missing salary fields have been replaced with the exact mean of $85,420. 42 rows were imputed. The dataset is now clean and ready for model training.

---

**👤 You:**
> "Replace all missing discount entries with zero since no discount should be assumed."

**🤖 AI Agent:**
> I've replaced 243 missing Discount entries with 0. This preserves the business logic that no discount was applied to these transactions.


## ❓ FAQ

**Q: Does it modify the original data file on disk?**
No. The engine processes the JSON payload entirely in memory and returns the cleaned array back to the AI. Your original files are never touched.

**Q: What happens if the entire target column is empty?**
If you try to compute mean or median on a completely empty column, the engine throws a deterministic error explaining the issue. You can fall back to the 'zero' strategy instead.

**Q: How does it decide which cells are 'missing'?**
The engine treats null, undefined, empty strings, and NaN as missing values. Any cell that cannot be parsed as a valid number is flagged for imputation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/missing-value-imputer](https://vinkius.com/mcp/missing-value-imputer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Missing Value Imputer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `missing-value-imputer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Missing Value Imputer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "missing-value-imputer": {
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
