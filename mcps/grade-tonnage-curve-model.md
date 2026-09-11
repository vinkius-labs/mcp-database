# Grade-Tonnage Curve Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grade-tonnage-curve-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mining](../categories/mining.md)

Analyze resource models to generate grade-tonnage curves and calculate ore quantities.

## Description
This MCP server provides tools to analyze mineral resource models by calculating the relationship between cut-off grades and resulting ore quantities. It allows for the generation of full grade-tonnage curves, calculation of tonnage, average grade, and contained metal, and the application of physical mining constraints like minimum mining width and maximum dilution. Use `validate_resource_model` to ensure model integrity before running `get_curve_data` or `get_tonnage_stats`.


## Available Tools (4)
- **get_constrained_tonnage**: Determines the maximum ore tonnage extractable given specific physical mining constraints
- **get_curve_data**: Generates a set of data points to plot a full Grade-Tonnage curve
- **get_tonnage_stats**: Calculates the fundamental relationship between a specific cut-off grade and the resulting resource quantities
- **validate_resource_model**: Verifies the integrity and completeness of a resource model before attempting curve generation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grade-Tonnage Curve Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the tonnage and average grade for resource model RM-101 at a 0.5 cut-off grade?"

**🤖 AI Agent:**
> For resource model RM-101 at a 0.5 cut-off grade, the total tonnage is 1,250,000 tonnes with an average grade of 0.65%.

---

**👤 You:**
> "Generate a grade-tonnage curve for model M-500 using these cut-off grades: 0.1, 0.2, 0.3, 0.4, 0.5."

**🤖 AI Agent:**
> The curve data for model M-500 is: 0.1 cut-off: 5,000,000t @ 0.15%; 0.2 cut-off: 4,200,000t @ 0.22%; 0.3 cut-off: 3,100,000t @ 0.31%; 0.4 cut-off: 2,050,000t @ 0.42%; 0.5 cut-off: 1,100,000t @ 0.55%.

---

**👤 You:**
> "Calculate the constrained tonnage for RM-202 with a 0.4 cut-off and a minimum mining width of 5 meters."

**🤖 AI Agent:**
> Applying a minimum mining width of 5 meters to RM-202 at a 0.4 cut-off results in 850,000 tonnes of ore with an average grade of 0.48%.


## ❓ FAQ

**Q: How do I check if my resource model is ready for analysis?**
You can use the `validate_resource_model` tool to verify the integrity and completeness of your resource model before performing calculations.

**Q: Can I account for mining dilution in my calculations?**
Yes, the `get_constrained_tonnage` tool allows you to specify a `maxDilution` parameter to account for waste mixed with ore.

**Q: How do I generate a full curve of data points?**
Use the `get_curve_data` tool by providing a list of cut-off grades in the `gradeSteps` parameter.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grade-tonnage-curve-model](https://vinkius.com/en/ai-agent-connect/grade-tonnage-curve-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grade-Tonnage Curve Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grade-tonnage-curve-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grade-Tonnage Curve Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grade-tonnage-curve-model": {
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
