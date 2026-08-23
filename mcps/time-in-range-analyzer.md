# Time in Range Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/time-in-range-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates clinical glycemic control metrics like TIR, GMI, and CV from glucose readings.

## Description
This MCP server provides precise statistical analysis for Continuous Glucose Monitor (CGM) data. It calculates essential glycemic metrics including Time in Range (TIR), Time Above Range (TAR), Time Below Range (TBR), Glucose Management Indicator (GMI), and Coefficient of Variation (CV). Use `analyze_glycemic_metrics` to get a full clinical report with risk flags, or `get_glycemic_summary_stats` for basic descriptive statistics like mean and standard deviation.


## Available Tools (3)
- **analyze_glycemic_metrics**: Calculates comprehensive glycemic control metrics from a series of glucose readings
- **get_glycemic_summary_stats**: Provides basic descriptive statistics for a set of glucose readings
- **validate_target_parameters**: Validates that the provided target ranges are clinically logical


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Time in Range Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these glucose readings: [110, 125, 140, 95, 185, 210, 65, 75, 130, 150]"

**🤖 AI Agent:**
> The analysis shows a TIR of 70%, a TAR of 20%, and a TBR of 10%. The GMI is 135 mg/dL and the CV is 32%. A 'Dangerous Hypoglycemia Risk' flag is present due to the TBR being above 4%.

---

**👤 You:**
> "Give me the summary statistics for these readings: [100, 110, 120, 130]"

**🤖 AI Agent:**
> The mean glucose is 115 mg/dL, the standard deviation is 11.18 mg/dL, the minimum is 100 mg/dL, the maximum is 130 mg/dL, and there were 4 readings processed.

---

**👤 You:**
> "Is a target range of 70 to 180 valid?"

**🤖 AI Agent:**
> Yes, the target range of 70 to 180 is clinically valid.


## ❓ FAQ

**Q: What is Time in Range (TIR)?**
TIR is the percentage of time your glucose levels stay within your target range, which is a key indicator of glycemic stability.

**Q: How can I check for high glycemic variability?**
You can use the `analyze_glycemic_metrics` tool. It automatically flags high glycemic variability if the Coefficient of Variation (CV) exceeds 36%.

**Q: What are clinical flags?**
Clinical flags are automated warnings triggered when metrics reach dangerous levels, such as high hypoglycemia risk (TBR > 4%).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/time-in-range-analyzer](https://vinkius.com/ai-agent-connect/time-in-range-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Time in Range Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `time-in-range-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Time in Range Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "time-in-range-analyzer": {
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
