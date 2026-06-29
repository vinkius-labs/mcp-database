# Wells Score DVT Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wells-score-dvt-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Clinical decision support tool for estimating Deep Vein Thrombosis (DVT) probability using the Wells scoring system.

## Description
The Wells Score DVT Calculator provides a standardized method for healthcare professionals to assess the likelihood of Deep Vein Thrombosis. By evaluating nine clinical indicators--including recent surgery, active cancer, and leg swelling--the tool calculates a total score and assigns a risk tier (Low, Moderate, or High). This assessment guides critical diagnostic decisions: Low and Moderate risk patients are directed toward D-dimer testing, while High risk patients are recommended for immediate venous ultrasonography. The server includes tools like `calculate_risk_score` to compute clinical scores, `get_diagnostic_protocol` to determine the next medical steps, and `fetch_prevalence_data` to provide historical context on DVT prevalence within each risk group.


## Available Tools (3)
- **calculate_risk_score**: Compute the Wells Score and assign a risk tier
- **fetch_prevalance_data**: Retrieve historical DVT prevalence data
- **get_diagnostic_protocol**: Determine the recommended medical testing pathway


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wells Score DVT Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Wells score for a patient with recent surgery and leg swelling."

**🤖 AI Agent:**
> The calculated total score is 2, placing the patient in the Moderate risk tier. The recommended next step is a D-dimer assay to rule out DVT.

---

**👤 You:**
> "What is the recommended protocol for a High risk patient?"

**🤖 AI Agent:**
> For a High risk tier, the recommended test is Compression Ultrasonography to visualize potential clots.

---

**👤 You:**
> "Show me the prevalence data for all risk tiers."

**🤖 AI Agent:**
> The historical prevalence of DVT is: Low Risk (0.5%), Moderate Risk (5.0%), and High Risk (25.0%).


## ❓ FAQ

**Q: What is the purpose of this tool?**
It helps clinicians estimate the probability of Deep Vein Thrombosis (DVT) using the validated Wells scoring system to decide between D-dimer testing or ultrasound.

**Q: How does the calculation work?**
The `calculate_risk_score` tool evaluates nine clinical indicators. Each indicator present adds one point to the total score, which then determines the risk tier.

**Q: What are the diagnostic recommendations?**
Based on the `get_diagnostic_protocol` tool, Low and Moderate risk tiers recommend a D-dimer assay, while High risk patients should proceed directly to imaging via ultrasound.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wells-score-dvt-calculator](https://vinkius.com/mcp/wells-score-dvt-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wells Score DVT Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wells-score-dvt-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wells Score DVT Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wells-score-dvt-calculator": {
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
