# Pediatric Growth Percentile Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pediatric-growth-percentile-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate pediatric growth percentiles and Z-scores using WHO (0-60m) and CDC (61-216m) standards.

## Description
This MCP server provides a clinical calculation engine to determine pediatric growth percentiles and Z-scores. It uses the WHO Multicentre Growth Reference Study for children aged 0 to 60 months and CDC Growth Charts for children aged 61 to 216 months. You can use tools like `calculate_percentile`, `calculate_zscore`, and `identify_growth_classification` to analyze weight, height, and head circumference measurements based on age and biological sex.


## Available Tools (3)
- **calculate_percentile**: Determines the specific growth percentile for a given physical measurement
- **calculate_zscore**: Calculates the Z-score for a physical measurement
- **identify_growth_classification**: Provides a qualitative clinical description of growth status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pediatric Growth Percentile Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the percentile for a 24-month-old male weighing 12kg?"

**🤖 AI Agent:**
> A weight of 12kg for a 24-month-old male falls at approximately the 50th percentile.

---

**👤 You:**
> "Calculate the Z-score for a 72-month-old female with a height of 115cm."

**🤖 AI Agent:**
> The calculated Z-score for a height of 115cm at 72 months for a female is approximately 0.5.

---

**👤 You:**
> "Is a head circumference of 33cm normal for a 3-month-old male?"

**🤖 AI Agent:**
> A head circumference of 33cm for a 3-month-old male is within the 'Normal' growth classification.


## ❓ FAQ

**Q: Which growth standards are used for the calculations?**
The engine uses the WHO Multicentre Growth Reference Study for children up to 60 months and CDC Growth Charts for children aged 61 to 216 months.

**Q: What physical measurements can I calculate?**
You can calculate percentiles and Z-scores for weight, height (or length), and head circumference.

**Q: How is growth status classified?**
Growth classification is based on Z-score thresholds: 'Below Average' for Z < -2, 'Normal' for Z between -2 and 2, and 'Above Average' for Z > 2.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pediatric-growth-percentile-calculator](https://vinkius.com/mcp/pediatric-growth-percentile-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pediatric Growth Percentile Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pediatric-growth-percentile-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pediatric Growth Percentile Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pediatric-growth-percentile-calculator": {
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
