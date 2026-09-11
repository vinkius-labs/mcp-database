# Resource Classification System MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/resource-classification-system)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Classifies mineral resources into JORC or NI 43-101 categories.

## Description
This MCP server provides professional-grade tools for mineral resource estimation. It allows AI agents to determine resource categories like Measured, Indicated, or Inferred by analyzing geological confidence, drilling density, and data quality. Use `classify_resource` to determine categories, `get_classification_thresholds` to retrieve regulatory benchmarks, `evaluate_data_readiness` to check if datasets are sufficient, and `compare_standards` to analyze differences between JORC and NI 43-101 frameworks.


## Available Tools (4)
- **classify_resource**: Determine the resource category based on geological and spatial data
- **compare_standards**: Highlights the differences in requirements between JORC and NI 43-101
- **evaluate_data_readiness**: Determines if the current data set is sufficient to attempt a classification
- **get_classification_thresholds**: Provides benchmark values used to distinguish between resource categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resource Classification System** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify a resource with high geological confidence, 50m drilling density, and excellent data quality."

**🤖 AI Agent:**
> The resource is classified as Measured.

---

**👤 You:**
> "What are the density limits for the JORC standard?"

**🤖 AI Agent:**
> The density limits for JORC are: Measured (0-25m), Indicated (25-50m), and Inferred (50-100m).

---

**👤 You:**
> "Is my data ready? I have 10 drill holes and excellent data quality."

**🤖 AI Agent:**
> The data is ready for classification with a Low risk level.


## ❓ FAQ

**Q: Which regulatory standards are supported?**
The system supports the JORC and NI 43-101 international reporting standards.

**Q: How does geological complexity affect classification?**
High geological complexity requires higher drilling density to achieve the same resource category classification.

**Q: Can I check if my data is ready for classification?**
Yes, you can use the `evaluate_data_readiness` tool to determine if your sample count and data quality meet the minimum requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/resource-classification-system](https://vinkius.com/en/ai-agent-connect/resource-classification-system)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resource Classification System** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resource-classification-system` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resource Classification System** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resource-classification-system": {
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
