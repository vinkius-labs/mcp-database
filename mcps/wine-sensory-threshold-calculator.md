# Wine Sensory Threshold Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-sensory-threshold-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predict sensory detection and impact of chemical compounds in wine using matrix-correction factors.

## Description
This MCP server provides analytical tools to predict how chemical compounds behave within a wine matrix. By applying matrix-correction factors--accounting for alcohol content and pH levels--it calculates whether a compound is sub-threshold or supra-threshold. Use `get_compound_thresholds` to find base detection limits, `calculate_matrix_correction` to adjust for the wine's environment, `evaluate_detection_status` to determine perception probability, and `calculate_sensory_impact` to quantify the prominence of compounds like TCA, 4-EP, or Diacetyl.


## Available Tools (4)
- **calculate_matrix_correction**: Determines how much the environment (pH and Alcohol) will shift the base sensory threshold
- **calculate_sensory_impact**: Quantifies the sensory prominence of a compound in the wine
- **evaluate_detection_status**: Determines if a compound is detectable and calculates the probability of perception
- **get_compound_thresholds**: Retrieves the base sensory threshold values for specific chemical compounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Sensory Threshold Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the sensory threshold for TCA?"

**🤖 AI Agent:**
> The base sensory threshold for TCA is typically measured in µg/L.

---

**👤 You:**
> "Is a 0.05 mg/L concentration of 4-EP detectable in a wine with 13% alcohol and pH 3.5?"

**🤖 AI Agent:**
> At a concentration of 0.05 mg/L with 13% alcohol and pH 3.5, the 4-EP is supra-threshold with a high detection probability.

---

**👤 You:**
> "Calculate the sensory impact of Diacetyl at 0.1 mg/L in a wine with 12% alcohol and pH 3.2."

**🤖 AI Agent:**
> The sensory impact score for Diacetyl in this matrix is 0.45, which falls into the 'Trace' perceptual category.


## ❓ FAQ

**Q: How does the tool account for wine composition?**
The tool uses `calculate_matrix_correction` to adjust standard sensory thresholds based on the specific alcohol content and pH level of the wine sample.

**Q: Can I check if a specific fault like TCA is detectable?**
Yes, you can use `evaluate_detection_status` with the compound name 'TCA' to determine if its concentration is supra-threshold in your specific wine matrix.

**Q: What is the difference between sub-threshold and supra-threshold?**
Sub-threshold means the concentration is too low to be perceived given the matrix effects, while supra-threshold means the compound is likely to be detected by a taster.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-sensory-threshold-calculator](https://vinkius.com/ai-agent-connect/wine-sensory-threshold-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Sensory Threshold Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-sensory-threshold-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Sensory Threshold Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-sensory-threshold-calculator": {
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
