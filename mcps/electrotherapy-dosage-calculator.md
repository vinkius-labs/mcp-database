# Electrotherapy Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/electrotherapy-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Clinical decision support for determining electrotherapy parameters.

## Description
This MCP server provides clinical decision support for determining precise electrotherapy parameters. It allows practitioners to calculate specific dosages using `calculate_dosage`, verify patient safety with `check_safety`, receive anatomical guidance via `suggest_placement`, and ensure physiological compliance with `validate_parameters`. It covers major modalities including TENS, IFC, and NMES to ensure accurate treatment planning based on tissue depth and patient sensitivity.


## Available Tools (4)
- **calculate_dosage**: Calculate dosage
- **check_safety**: Check safety
- **suggest_placement**: Suggest placement
- **validate_parameters**: Validate parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Electrotherapy Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dosage for TENS for pain relief in superficial tissue for a patient with low sensitivity."

**🤖 AI Agent:**
> The recommended parameters are a frequency of 100 Hz and an intensity of 15 mA, with bipolar electrode placement.

---

**👤 You:**
> "Suggest electrode placement for NMES on the quadriceps muscle."

**🤖 AI Agent:**
> Place electrodes over the motor points of the quadriceps muscle for effective stimulation.

---

**👤 You:**
> "Is it safe to use IFC on a patient with a pacemaker?"

**🤖 AI Agent:**
> No, the treatment is unsafe due to the patient's pacemaker condition.


## ❓ FAQ

**Q: How do I calculate the correct dosage for a patient?**
You can use the `calculate_dosage` tool by providing the modality type, treatment goal, tissue depth, and patient sensitivity.

**Q: Can this tool help with electrode positioning?**
Yes, the `suggest_placement` tool provides anatomical guidance for electrode positioning based on the modality and target area.

**Q: How does the tool ensure patient safety?**
The tool uses `check_safety` to identify risks based on patient conditions and `validate_parameters` to ensure the dosage stays within safe physiological limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/electrotherapy-dosage-calculator](https://vinkius.com/en/ai-agent-connect/electrotherapy-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Electrotherapy Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `electrotherapy-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Electrotherapy Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "electrotherapy-dosage-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
