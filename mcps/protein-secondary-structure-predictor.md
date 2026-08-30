# Protein Secondary Structure Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/protein-secondary-structure-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predict protein secondary structures like alpha-helices and beta-sheets from amino acid sequences.

## Description
This MCP server provides specialized tools for analyzing protein primary sequences to predict their secondary structural elements. Using established scientific methods, it calculates the distribution of alpha-helices, beta-sheets, and coils. Researchers can use `predict_structure_chou_fasman` for statistical propensity-based analysis or `predict_structure_gor` for information theory-based predictions. The tool also allows for direct comparison of these methods using `compare_prediction_methods` to identify specific structural biases.


## Available Tools (4)
- **get_amino_acid_propensities**: Retrieves the specific propensity values for amino acids used in secondary structure prediction
- **compare_prediction_methods**: Compares the results of Chou-Fasman and GOR methods for a single sequence
- **predict_structure_chou_fasman**: Predicts the secondary structure of a protein sequence using the Chou-Fasman statistical propensity method
- **predict_structure_gor**: Note that GOR requires a minimum sequence length for window calculation.

Predicts the secondary structure of a protein sequence using the GOR (information theory) approach


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Protein Secondary Structure Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the secondary structure for the sequence MVLSAALALAL."

**🤖 AI Agent:**
> The predicted structure for the sequence MVLSAALALAL is 45% alpha-helix, 15% beta-sheet, and 40% coil.

---

**👤 You:**
> "Compare the Chou-Fasman and GOR predictions for the sequence MAVS."

**🤖 AI Agent:**
> Chou-Fasman predicts 25% alpha-helix and 25% beta-sheet, while GOR predicts 30% alpha-helix and 20% beta-sheet. The difference in helix is 5% and the difference in sheet is 5%.

---

**👤 You:**
> "What are the propensity values for the chou_fasman method?"

**🤖 AI Agent:**
> The Chou-Fasman propensity values include: Alanine (A) has a high helix propensity, while Proline (P) acts as a helix breaker.


## ❓ FAQ

**Q: What methods are used for prediction?**
The server implements the Chou-Fasman statistical propensity method and the GOR (Garnier-Osguthorpe-Robson) information theory approach.

**Q: How can I compare different prediction results?**
You can use the `compare_prediction_methods` tool to run both Chou-Fasman and GOR algorithms on the same sequence and see the differences in helix and sheet percentages.

**Q: What input format is required?**
The tools require a string representing the primary amino acid sequence using standard single-letter codes (e.g., 'MVLSA').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/protein-secondary-structure-predictor](https://vinkius.com/ai-agent-connect/protein-secondary-structure-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Protein Secondary Structure Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `protein-secondary-structure-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Protein Secondary Structure Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "protein-secondary-structure-predictor": {
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
