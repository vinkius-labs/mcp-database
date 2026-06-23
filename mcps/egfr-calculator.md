# eGFR Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/egfr-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Estimate Glomerular Filtration Rate (eGFR) using CKD-EPI 2021 and MDRD formulas with clinical staging.

## Description
This MCP server provides precise tools for estimating kidney function. Use `calculate_ckdepi_2021` to obtain the modern gold standard estimation without race-based adjustments, or `calculate_mdrd_formula` for the traditional MDRD calculation. After obtaining an eGFR value, use `get_clinical_classification` to determine the KDIGO CKD stage (G1 to G5) and receive specific medication dosage adjustment recommendations based on renal function.


## Available Tools (3)
- **calculate_ckdepi_2021**: Returns estimated GFR without race adjustment.

Calculates eGFR using the CKD-EPI 2021 formula
- **calculate_mdrd_formula**: Returns estimated GFR.

Calculates eGFR using the MDRD formula
- **get_clinical_classification**: Determines CKD stage and dosing advice


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eGFR Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate eGFR using CKD-EPI 2021 for a 45-year-old male with a serum creatinine of 1.2 mg/dL."

**🤖 AI Agent:**
> The estimated GFR (eGFR) using the CKD-EFR 2021 formula is 75 mL/min/1.73m².

---

**👤 You:**
> "What is the clinical stage for an eGFR of 12 mL/min/1.73m²?"

**🤖 AI Agent:**
> An eGFR of 12 mL/min/1.73m² corresponds to Stage G5 (Kidney Failure). Medication dosage adjustment is recommended.

---

**👤 You:**
> "Calculate MDRD eGFR for a 60-year-old female with creatinine of 2.0 mg/dL."

**🤖 AI Agent:**
> The estimated GFR using the MDRD formula is 28 mL/min/1.73m².


## ❓ FAQ

**Q: What is the difference between CKD-EPI 2021 and MDRD?**
CKD-EPI 2021 is the current gold standard that provides accurate estimation without using race-based coefficients, while MDRD is an older formula often used for comparison.

**Q: How do I determine the CKD stage?**
After calculating your eGFR using `calculate_ckdepi_2021` or `calculate_mdrd_formula`, pass the resulting value into the `get_clinical_classification` tool to see the KDIGO stage.

**Q: Does this tool require race information?**
No. The `calculate_ckdepi_2021` tool specifically follows modern clinical standards by providing an accurate estimation without any race-based modifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/egfr-calculator](https://vinkius.com/mcp/egfr-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **eGFR Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `egfr-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **eGFR Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "egfr-calculator": {
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
