# NIHSS Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nihss-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate NIH Stroke Scale scores and assess stroke severity instantly.

## Description
The NIHSS Calculator is a clinical decision support tool that allows healthcare professionals to quantify neurological impairment following an acute stroke. By using the `calculate_nihss` tool, users can input individual scores for eleven neurological components--including consciousness level, gaze, facial palsy, and motor function--to receive an immediate total score and severity classification. Additionally, the `get_scoring_guide` tool provides detailed scoring ranges for each component, while `evaluate_urgency` offers standardized clinical instructions based on the patient's neurological state. This MCP server acts as a bridge between clinical assessment data and AI agents in clients like Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools
- **calculate_nihss**: Calculate the NIHSS score and severity
- **evaluate_urgency**: Evaluate clinical urgency based on NIHSS score
- **get_scoring_guide**: Retrieve the scoring guide for NIHSS components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NIHSS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the NIHSS score for a patient with these scores: consciousnessLevel: 1, consciousnessQuestions: 0, consciousnessCommands: 0, gaze: 0, visualFields: 0, facialPalsy: 2, motorFunction: 1, ataxia: 0, sensory: 0, language: 1, dysarthria: 0, extinction: 0."

**🤖 AI Agent:**
> The total NIHSS score is 5, which falls into the Moderate severity classification.

---

**👤 You:**
> "What is the scoring guide for facial palsy?"

**🤖 AI Agent:**
> For facial palsy, a score of 0 indicates no paralysis, while higher scores represent increasing degrees of facial muscle asymmetry or drooping.

---

**👤 You:**
> "Based on a total NIHSS score of 18, what is the clinical urgency?"

**🤖 AI Agent:**
> The urgency level is Severe, and the clinical note is: Immediate intervention and intensive monitoring are required due to high neurological impairment.


## ❓ FAQ

**Q: How do I calculate the total NIHSS score?**
You can use the `calculate_nihss` tool by providing a JSON object containing the scores for each of the eleven neurological components.

**Q: Where can I find the scoring ranges for each item?**
The `get_scoring_guide` tool provides a detailed mapping of score ranges and descriptions for every component in the scale.

**Q: How does the tool determine clinical urgency?**
The `evaluate_urgency` tool analyzes the total NIHSS score and returns a standardized instruction, such as 'Immediate Intervention Required', based on the severity level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nihss-calculator](https://vinkius.com/mcp/nihss-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NIHSS Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nihss-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NIHSS Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nihss-calculator": {
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
