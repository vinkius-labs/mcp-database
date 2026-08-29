# Bacterial Growth Kinetics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bacterial-growth-kinetics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Models bacterial growth curves and extracts physiological parameters from OD measurements.

## Description
This MCP server provides tools to analyze bacterial population dynamics using Optical Density (OD) data. It allows researchers to calculate critical physiological constants such as lag phase duration, exponential growth rate, and generation time using `get_growth_parameters`. Users can also verify the quality of experimental datasets with `validate_growth_data`, estimate future culture states via `predict_future_growth`, and model the impact of nutrient depletion using `simulate_substrate_limitation`.


## Available Tools (4)
- **get_growth_parameters**: Extracts key physiological constants from a set of OD measurements
- **predict_future_growth**: Estimates the future state of a culture based on current growth trends
- **simulate_substrate_limitation**: Models how changing nutrient availability affects the growth curve
- **validate_growth_data**: Checks the quality and integrity of raw experimental data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bacterial Growth Kinetics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze these OD measurements: [{'timestamp': 0, 'opticalDensity': 0.05}, {'timestamp': 30, 'opticalDensity': 0.1}, {'timestamp': 60, 'opticalDensity': 0.4}, {'timestamp': 90, 'opticalDensity': 0.8}] at 37 degrees Celsius."

**🤖 AI Agent:**
> The analysis shows a lag phase of approximately 30 minutes, an exponential growth rate of 0.023 per minute, and a generation time of 30.1 minutes.

---

**👤 You:**
> "Check if this growth data is reliable: [{'timestamp': 0, 'opticalDensity': 0.1}, {'timestamp': 10, 'opticalDensity': 0.12}, {'timestamp': 20, 'opticalDensity': 0.11}]"

**🤖 AI Agent:**
> The data quality is classified as Low Reliability due to insufficient growth progression and sparse data points.

---

**👤 You:**
> "Predict the OD at timestamp 120 based on a growth state with max OD 1.2 and current rate 0.05."

**🤖 AI Agent:**
> The predicted optical density at timestamp 120 is 1.15, and the culture is expected to be in the stationary phase.


## ❓ FAQ

**Q: What kind of data is required for analysis?**
You need an array of measurements containing timestamps and optical density (OD) values. You can use `validate_growth_data` to check if your dataset is suitable for kinetic modeling.

**Q: How can I predict when a culture will reach stationary phase?**
First, use `get_growth_parameters` to establish the current growth state. Then, use `predict_future_growth` with a target timestamp to estimate the future OD and phase.

**Q: Can I simulate the effect of nutrient depletion?**
Yes, the `simulate_substrate_limitation` tool allows you to model how reducing the substrate concentration factor affects the maximum OD and growth rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bacterial-growth-kinetics](https://vinkius.com/ai-agent-connect/bacterial-growth-kinetics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bacterial Growth Kinetics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bacterial-growth-kinetics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bacterial Growth Kinetics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bacterial-growth-kinetics": {
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
