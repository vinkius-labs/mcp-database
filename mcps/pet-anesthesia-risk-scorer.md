# Pet Anesthesia Risk Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-anesthesia-risk-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [medical](../categories/medical.md)

Estimate ASA physical status classification for veterinary patients based on physiological and medical markers.

## Description
The Pet Anesthesia Risk Scorer provides clinical decision support by estimating the ASA (American Society of Anesthesiologists) physical status classification. Using tools like `calculate_asa_class`, `evaluate_body_condition_risk`, and `summarize_medical_severity`, veterinarians can assess patient risk levels from Class I to Class V based on age, weight, body condition score, and pre-existing medical conditions.


## Available Tools (3)
- **calculate_asa_class**: Estimates the ASA physical status classification for a pet
- **evaluate_body_condition_risk**: Analyzes airway and cardiovascular risks based on weight and BCS
- **summarize_medical_severity**: Aggregates medical conditions into a simplified impact tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Anesthesia Risk Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the ASA class for a 5-year-old dog weighing 30kg with a BCS of 5 and minimal pre-existing severity?"

**🤖 AI Agent:**
> The estimated ASA class is Class I, indicating a healthy patient with no systemic disease.

---

**👤 You:**
> "Evaluate the anesthetic risk for an 11kg cat with a BCS of 8."

**🤖 AI Agent:**
> The assessment indicates increased respiratory risk and potential for difficult intubation due to obesity.

---

**👤 You:**
> "Summarize the severity of these conditions: [renal failure, hypertension] with moderate impact on vital organs."

**🤖 AI Agent:**
> The resulting severity tier is Moderate, indicating significant impact on surgery and anesthesia planning.


## ❓ FAQ

**Q: What is the ASA physical status classification?**
It is a standardized ranking of a patient's systemic health, ranging from Class I (healthy) to Class V (moribund), used to assess anesthetic risk.

**Q: How does the `calculate_asa_class` tool work?**
The tool takes parameters such as age, weight, body condition score (1-9), and pre-existing severity to determine the most appropriate ASA class.

**Q: Can I use this for different species?**
The tool is specifically designed for veterinary patients, focusing on parameters like Body Condition Score (BCS) common in pet medicine.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-anesthesia-risk-scorer](https://vinkius.com/mcp/pet-anesthesia-risk-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Anesthesia Risk Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-anesthesia-risk-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Anesthesia Risk Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-anesthesia-risk-scorer": {
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
