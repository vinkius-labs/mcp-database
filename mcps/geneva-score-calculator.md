# Geneva Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geneva-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate pulmonary embolism risk using the Revised Geneva Score algorithm.

## Description
The Geneva Score Calculator provides a clinical decision support system for assessing the probability of Pulmonary Embolism (PE). By using tools like `compute_geneva_score`, clinicians can input patient parameters such as age, heart rate, and recent surgery to determine risk tiers. You can also use `get_diagnostic_protocol` to retrieve recommended next steps like D-dimer testing or CTPA imaging. Additionally, the `validate_clinical_parameters` tool ensures all entered data is within physiologically plausible ranges.


## Available Tools (3)
- **validate_clinical_parameters**: Validates clinical parameters are within physiological bounds
- **compute_geneva_score**: Calculates the Geneva Score for Pulmonary Embolism risk
- **get_diagnostic_protocol**: Provides recommended diagnostic steps based on risk tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Geneva Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Geneva score for a 70-year-old with a heart rate of 120, recent surgery, and hemoptys."

**🤖 AI Agent:**
> The total score is 10, placing the patient in the High risk category.

---

**👤 You:**
> "What is the protocol for a low-risk patient?"

**🤖 AI Agent:**
> For Low risk patients, the recommended test is a D-dimer assay to rule out embolism.

---

**👤 You:**
> "Check if age 150 and heart rate 40 are valid."

**🤖 AI Agent:**
> The validation check confirms these parameters are within physiologically plausible ranges.


## ❓ FAQ

**Q: How do I calculate the risk score?**
Use the `compute_geneva_score` tool by providing patient details like age, heart rate, and clinical indicators such as hemoptysis or recent surgery.

**Q: What diagnostic steps are recommended for high-risk patients?**
For high-risk patients, the `get_diagnostic_protocol` tool recommends immediate definitive imaging via CTPA.

**Q: Can I validate patient data before scoring?**
Yes, use the `validate_clinical_parameters` tool to ensure age and heart rate are within physiologically plausible bounds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geneva-score-calculator](https://vinkius.com/mcp/geneva-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Geneva Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `geneva-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Geneva Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geneva-score-calculator": {
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
