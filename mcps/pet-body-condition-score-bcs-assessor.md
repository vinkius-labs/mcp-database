# Pet Body Condition Score (BCS) Assessor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-body-condition-score-bcs-assessor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess pet weight and nutritional status using a 9-point Body Condition Score (BCS) system.

## Description
This MCP server provides veterinary-grade tools to determine a pet's Body Condition Score (BCS) on a standardized 9-point scale. By analyzing physical indicators such as rib palpability, waist definition, and abdominal fat presence, the `compute_body_condition_score` tool calculates a precise numerical score. Additionally, you can use `get_body_classification` to translate that score into weight categories like Underweight, Ideal, or Obese, and `evaluate_health_risk` to understand the clinical implications and potential health risks associated with specific scores. This is an essential tool for pet owners and veterinary professionals to monitor nutritional health and prevent obesity-related diseases.


## Available Tools (3)
- **compute_body_condition_score**: Calculates the specific numerical Body Condition Score (1-to-9) based on physical examination findings
- **evaluate_health_risk**: Provides a clinical risk assessment and potential health implications for a given BCS
- **get_body_classification**: Converts a numerical BCS into a human-readable weight category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Body Condition Score (BCS) Assessor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My dog's ribs are very easy to feel, the waist is extremely visible, and there is minimal abdominal fat. What is his BCS?"

**🤖 AI Agent:**
> Based on those findings, your dog has a Body Condition Score of 2, which falls into the Underweight category.

---

**👤 You:**
> "The pet's ribs are impossible to feel, there is no visible waist, and significant abdominal fat is present. What is the score and what are the risks?"

**🤖 AI Agent:**
> The calculated Body Condition Score is 9. This indicates extreme obesity, which carries a High Risk level due to potential metabolic and joint-related health concerns.

---

**👤 You:**
> "What is the classification for a BCS of 5?"

**🤖 AI Agent:**
> A Body Condition Score of 5 is classified as Ideal.


## ❓ FAQ

**Q: How is the Body Condition Score calculated?**
The score is calculated using the `compute_body_condition_score` tool, which evaluates three key physical indicators: how easily ribs can be felt (rib palpability), the visibility of the waist from above (waist visibility), and the amount of fat felt around the abdomen (abdominal fat presence).

**Q: What does a BCS score of 5 mean?**
A score of 5 is considered the ideal nutritional state. At this level, ribs should be easily palpable without excessive pressure, and a visible waist should be present when viewed from above.

**Q: Can I assess health risks with this tool?**
Yes, by using the `evaluate_health_risk` tool, you can receive a clinical risk assessment and specific notes regarding potential health implications, such as risks related to malnutrition or metabolic diseases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-body-condition-score-bcs-assessor](https://vinkius.com/mcp/pet-body-condition-score-bcs-assessor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Body Condition Score (BCS) Assessor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-body-condition-score-bcs-assessor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Body Condition Score (BCS) Assessor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-body-condition-score-bcs-assessor": {
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
