# Anxiety Screening Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/anxiety-screening-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Scores anxiety screening questionnaires like GAD-7 to provide severity assessments and clinical recommendations.

## Description
This MCP server provides clinical scoring for validated anxiety screening instruments. It allows AI agents to process questionnaire responses to determine anxiety severity levels and functional impairment. Key capabilities include using `calculate_gad7_score` to determine clinical classifications, `assess_functional_impact` to evaluate daily life disruption, and `get_clinical_recommendations` to provide actionable guidance based on scores and impairment levels. It also includes `validate_instrument_integrity` to ensure response counts match the required instrument structure.


## Available Tools (4)
- **assess_functional_impact**: Determines the level of daily life disruption based on the patient's self-reported impairment
- **calculate_gad7_score**: Calculates the total score and severity classification for a GAD-7 questionnaire
- **get_clinical_recommendations**: Provides actionable guidance based on the calculated score and impairment
- **validate_instrument_integrity**: Ensures the responses provided correspond to the structure of a specific validated instrument


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Anxiety Screening Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the GAD-7 score for these responses: [1, 0, 3, 2, 1, 0, 2]."

**🤖 AI Agent:**
> The total GAD-7 score is 9, which falls into the Moderate severity category.

---

**👤 You:**
> "What is the clinical recommendation for a score of 15 with moderate impairment?"

**🤖 AI Agent:**
> For a score of 15 and moderate impairment, the recommendation is to seek a professional clinical evaluation immediately, with a High priority level.

---

**👤 You:**
> "Assess the functional impact for someone reporting 'severe' impairment."

**🤖 AI Agent:**
> Severe impairment indicates a high level of daily life disruption and requires prioritized clinical intervention.


## ❓ FAQ

**Q: What instruments can be scored?**
The server is primarily designed for the GAD-7 (Generalized Anxiety Disorder 7-item scale), but it includes validation tools to support various validated instruments.

**Q: How is the severity determined?**
Severity is determined by mapping the total score from `calculate_gad7_score` to standardized clinical thresholds (e.g., Minimal, Mild, Moderate, Severe).

**Q: Can I get clinical guidance?**
Yes, by using `get_clinical_recommendations`, the server provides actionable guidance and a priority level based on the score and reported impairment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/anxiety-screening-scorer](https://vinkius.com/en/ai-agent-connect/anxiety-screening-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Anxiety Screening Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `anxiety-screening-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Anxiety Screening Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "anxiety-screening-scorer": {
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
