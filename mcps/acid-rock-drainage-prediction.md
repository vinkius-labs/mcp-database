# Acid Rock Drainage Prediction MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/acid-rock-drainage-prediction)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Predict environmental risk from acid rock drainage using geochemical and kinetic data.

## Description
This MCP server provides specialized tools for evaluating the environmental risk of Acid Rock Drainage (ARD). It allows AI agents to analyze geochemical and mineralogical data through standard predictive methodologies. Users can perform static Acid Base Accounting (ABA) using `analyze_static_aba`, conduct Net Acid Generation (NAG) assessments with `run_nag_test`, and refine predictions using time-dependent weathering data via `evaluate_kinetic_risk`. The server also provides a unified risk assessment through `classify_drainage_risk`, which combines static, NAG, and kinetic results to determine the final environmental impact classification.


## Available Tools (4)
- **classify_drainage_risk**: 
- **evaluate_kinetic_risk**: 
- **run_nag_test**: 
- **analyze_static_aba**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acid Rock Drainage Prediction** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the acid potential for a sample with 5% sulfur and 20 units of neutralization potential."

**🤖 AI Agent:**
> The acid potential is 5.0 and the neutralization potential is 20.0, resulting in a high neutralization potential ratio.

---

**👤 You:**
> "Run a NAG test with 15 units of acidity and a sample mass of 100."

**🤖 AI Agent:**
> The sample is classified as acid-generating with a moderate risk level.

---

**👤 You:**
> "What is the kinetic risk if the static AP is 10, static NP is 15, and the weathering rate is 2?"

**🤖 AI Agent:**
> The kinetic risk is categorized as a delayed risk due to the current buffering capacity.


## ❓ FAQ

**Q: What is the difference between static and kinetic testing?**
Static testing, like `analyze_static_aba`, provides a snapshot of acid-generating and neutralizing potential. Kinetic testing, handled by `evaluate_kinetic_risk`, simulates time-dependent weathering to predict how these potentials change over time.

**Q: How do I get a final risk assessment?**
You can use the `classify_drainage_risk` tool. It takes the outputs from your static, NAG, and kinetic tests to provide a unified classification and confidence level.

**Q: Can I use NAG test results?**
Yes, you can use `run_nag_test` to predict acid generation based on the acidity produced during the Net Acid Generation test.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/acid-rock-drainage-prediction](https://vinkius.com/ai-agent-connect/acid-rock-drainage-prediction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acid Rock Drainage Prediction** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `acid-rock-drainage-prediction` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acid Rock Drainage Prediction** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acid-rock-drainage-prediction": {
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
