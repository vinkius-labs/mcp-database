# Drug Renal Dose Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/drug-renal-dose-adjuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate medication dose modifications and interval extensions based on renal function levels (CrCl or eGFR) and identify contraindications.

## Description
The Drug Renal Dose Adjuster is a clinical decision support tool designed to assist healthcare professionals in managing medication regimens for patients with varying stages of Chronic Kidney Disease (CKD). By providing the patient's Creatinine Clearance (CrCl) or estimated Glomerular Filtration Rate (eGFR), users can use tools like `calculate_renal_adjustment` to determine precise dose reductions or interval extensions. The tool also identifies critical contraindications where a drug should not be used due to high toxicity risk at specific renal thresholds. Use `list_all_drugs` to browse the supported medication catalog and `get_drug_baseline` to retrieve standard dosing information.


## Available Tools (3)
- **calculate_renal_adjustment**: Calculates adjusted dose based on renal function
- **get_drug_baseline**: Gets the baseline dose and interval for a drug
- **list_all_drugs**: Lists all supported drugs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drug Renal Dose Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the standard dose for Vancomycin?"

**🤖 AI Agent:**
> The baseline dose for Vancomycin is 1000 mg every 12 hours.

---

**👤 You:**
> "Adjust the dose of Metformin for a patient with an eGFR of 30."

**🤖 AI Agent:**
> For Metformin with an eGFR of 30, the adjusted dose is 500 mg every 24 hours. Note that this patient is in Stage 4 CKD.

---

**👤 You:**
> "Is Gentamicin safe for a patient with CrCl of 20?"

**🤖 AI Agent:**
> No, Gentamicin is contraindicated for this patient because their CrCl has fallen below the safety threshold.


## ❓ FAQ

**Q: How do I find which drugs are supported?**
You can use the `list_all_drugs` tool to retrieve a complete, searchable list of all medications currently available in our hardcoded catalog.

**Q: What renal metrics can I use for calculations?**
The tool supports both Creatinine Clearance (CrCl) and estimated Glomerular Filtration Rate (eGFR). When using `calculate_renal_adjustment`, simply specify the measurement type.

**Q: How does the tool handle drug contraindications?**
The `calculate_renal_adjustment` tool automatically checks if the patient's renal value has fallen below a safety threshold. If it has, the tool will flag the drug as contraindicated and provide a clinical warning.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drug-renal-dose-adjuster](https://vinkius.com/mcp/drug-renal-dose-adjuster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drug Renal Dose Adjuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drug-renal-dose-adjuster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drug Renal Dose Adjuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drug-renal-dose-adjuster": {
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
