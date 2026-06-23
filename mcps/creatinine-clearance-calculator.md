# Creatinine Clearance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/creatinine-clearance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate creatinine clearance using the Cockcroft-Gault equation and identify drug dose adjustments.

## Description
This MCP server provides clinical decision support by calculating creatinine clearance (CrCl) via the Cockcroft-Gault method. It allows users to input patient age, weight, serum creatinine, and sex to determine kidney filtration efficiency. Beyond simple calculation, it uses `evaluate_renal_function_stage` to classify renal health into stages like Normal or Severe Impairment, and `retrieve_drug_adjustments` to identify critical medication dosage changes for antibiotics and anticoagulants based on the calculated clearance.


## Available Tools (3)
- **calculate_creatinine_clearance**: Calculate creatinine clearance using Cockcroft-Gault
- **evaluate_renal_function_stage**: Evaluate renal function stage
- **retrieve_drug_adjustments**: Retrieve medication dose adjustments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Creatinine Clearance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the creatinine clearance for a 65-year-old male, weighing 70kg, with a serum creatinine of 1.2 mg/dL."

**🤖 AI Agent:**
> The calculated creatinine clearance is 65.33 ml/min.

---

**👤 You:**
> "What is the renal function stage for a CrCl of 20 ml/min?"

**🤖 AI Agent:**
> A clearance of 20 ml/min corresponds to the Severe Impairment stage.

---

**👤 You:**
> "Are there any drug adjustments needed for a patient with 25 ml/min clearance?"

**🤖 AI Agent:**
> Yes, the following adjustments are required: Vancomycin - Reduce dose or increase interval.


## ❓ FAQ

**Q: How is the creatinine clearance calculated?**
The tool uses the Cockcroft-Gault equation, which factors in patient age, body weight, serum creatinine levels, and biological sex (applying a 15% reduction for females).

**Q: Can I see which medications need dose adjustments?**
Yes. By using the `retrieve_drug_adjustments` tool with your calculated CrCl value, you can identify specific instructions for drugs like Vancomycin or Enoxaparin.

**Q: What does the renal function stage classification mean?**
The `evaluate_renal_function_stage` tool categorizes kidney health from 'Normal' (above 90 ml/min) to 'End-Stage/Failure' (below 15 ml/min).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/creatinine-clearance-calculator](https://vinkius.com/mcp/creatinine-clearance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Creatinine Clearance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `creatinine-clearance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Creatinine Clearance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "creatinine-clearance-calculator": {
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
