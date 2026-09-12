# BTX Extraction Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/btx-extraction-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [process-design](../categories/process-design.md)

Design BTX extraction units using liquid-liquid extraction and extractive distillation logic.

## Description
This MCP server provides specialized tools for designing Benzene, Toluene, and Xylene (BTX) extraction processes. It allows engineers to evaluate feedstock suitability using `analyze_feedstock_suitability`, identify the best chemical candidates with `select_optimal_solvent`, calculate physical equipment sizes via `design_extractor_dimensions`, and predict final product yields through `calculate_recovery_performance`.


## Available Tools (4)
- **analyze_feedstock_suitability**: Determines if a given feedstock composition is compatible with standard extraction methods and estimates the primary separation challenge
- **calculate_recovery_performance**: Predicts the final purity and recovery percentage for the target product
- **design_extractor_dimensions**: Calculates the physical size and capacity of the extraction unit (column or mixer-settler)
- **select_optimal_solvent**: Identifies the best solvent candidate based on the desired separation performance and feedstock type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BTX Extraction Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my feedstock suitable for extraction?"

**🤖 AI Agent:**
> The feedstock has an aromatic fraction of 0.4 and a non-aromatic concentration of 0.6, making it suitable for Liquid-Liquid Extraction (LLE) with medium process intensity.

---

**👤 You:**
> "What is the best solvent for benzene extraction with a selectivity of 15?"

**🤖 AI Agent:**
> The recommended solvent is Sulfolane, which provides an estimated selectivity of 18.5 and high capacity for benzene.

---

**👤 You:**
> "Calculate the column diameter for a 100 m3/h feed using Sulfolane."

**🤖 AI Agent:**
> The calculated column diameter is 2.4 meters with a height of 12.5 meters for the specified flow rate and solvent ratio.


## ❓ FAQ

**Q: What is the difference between LLE and ED?**
Liquid-Liquid Extraction (LLE) uses solubility differences to separate aromatics, while Extractive Distillation (ED) uses a solvent to alter relative volatility in a distillation column.

**Q: How do I determine the equipment size?**
You can use the `design_extractor_dimensions` tool by providing the selected solvent name, feed flow rate, and solvent-to-feed ratio.

**Q: Can I predict product purity?**
Yes, the `calculate_recovery_performance` tool predicts aromatic recovery, product purity, and raffinate purity based on your design parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/btx-extraction-designer](https://vinkius.com/en/ai-agent-connect/btx-extraction-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BTX Extraction Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `btx-extraction-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BTX Extraction Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "btx-extraction-designer": {
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
