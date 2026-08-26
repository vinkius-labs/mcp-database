# Soil Texture Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/soil-texture-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Classifies soil texture using the USDA soil texture triangle based on particle size distribution.

## Description
This MCP server provides specialized tools for soil scientists and agricultural engineers to determine soil texture classifications. By inputting the percentages of sand, silt, and clay, users can utilize `classify_soil_texture` to identify the specific USDA texture class. The server also includes `validate_composition` to ensure laboratory measurements sum to exactly 100%, `get_texture_boundaries` to retrieve threshold ranges for the 12 USDA classes, and `batch_classify_samples` for processing multiple samples at once. It is designed to handle edge cases by providing warnings when soil compositions fall near classification boundaries.


## Available Tools (4)
- **get_texture_boundaries**: Retrieve the definitions or threshold ranges for the 12 USDA texture classes
- **batch_classify_samples**: Process multiple laboratory samples in a single operation
- **classify_soil_texture**: The sum must be exactly 100.

Identify the specific USDA texture class for a given soil sample
- **validate_composition**: Verify if a set of laboratory measurements is mathematically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soil Texture Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify a soil sample with 40% sand, 40% silt, and 20% clay."

**🤖 AI Agent:**
> The soil texture is classified as Loam.

---

**👤 You:**
> "Check if a sample with 50% sand, 45% silt, and 5% clay is valid."

**🤖 AI Agent:**
> The composition is valid as the total percentage is 100%.

---

**👤 You:**
> "What are the boundaries for the Clay texture class?"

**🤖 AI Agent:**
> The Clay texture class is defined by specific minimum clay content thresholds within the USDA triangle.


## ❓ FAQ

**Q: How do I ensure my soil sample is valid for classification?**
You can use the `validate_composition` tool to verify that your sand, silt, and clay percentages sum to exactly 100% before attempting to classify the texture.

**Q: What happens if my soil sample is near a texture boundary?**
The `classify_soil_texture` tool identifies edge cases. If a sample is near a boundary, it will return a warning message to alert you that a slight variation in measurement could change the classification.

**Q: Can I process multiple soil samples at the same time?**
Yes, the `batch_classify_samples` tool allows you to process an array of multiple laboratory samples in a single operation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/soil-texture-classifier](https://vinkius.com/ai-agent-connect/soil-texture-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soil Texture Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soil-texture-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soil Texture Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soil-texture-classifier": {
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
