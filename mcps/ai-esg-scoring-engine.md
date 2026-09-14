# AI ESG Scoring Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ai-esg-scoring-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate holistic AI ESG scores, compliance gaps, and required investment needs.

## Description
This MCP server provides a specialized scoring engine to evaluate the Environmental, Social, and Governance (ESG) impact of AI systems. It allows AI agents to analyze ethics frameworks, bias mitigation, transparency, and governance structures. Using `calculate_ai_esg_score`, agents can determine a composite responsibility score (0-100) and identify specific compliance gaps. For deeper analysis, `evaluate_bias_risk` assesses social impact, while `assess_governance_readiness` evaluates organizational oversight. Additionally, `project_investment_needs` helps simulate the capital required to reach target ESG milestones.


## Available Tools (4)
- **assess_governance_readiness**: Evaluate if the organizational structure is sufficient to manage AI risks
- **calculate_ai_esg_score**: Compute the primary holistic ESG score and associated financial/compliance metrics
- **evaluate_bias_risk**: Provide a deep dive into the social risk component of the AI system
- **project_investment_needs**: Simulate how much investment is needed to reach specific ESG target milestones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI ESG Scoring Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the AI ESG score for a system with a bias mitigation level of 0.8, transparency rating of 0.7, governance strength of 0.9, and stakeholder impact of 0.8."

**🤖 AI Agent:**
> The calculated AI ESG score is 82. The system shows high governance stability but has minor compliance gaps in transparency documentation.

---

**👤 You:**
> "What is the social risk if my bias mitigation level is 0.5 and the demographic parity gap is 0.3?"

**🤖 AI Agent:**
> The social risk score is 45. Mitigation urgency is Scheduled. It is recommended to increase training data diversity to reduce the demographic parity gap.

---

**👤 You:**
> "How much investment is needed to move my current score of 65 to a target of 85?"

**🤖 AI Agent:**
> The estimated required investment is €45,000 to achieve a projected score increase of 20 points.


## ❓ FAQ

**Q: What is the AI ESG score?**
The AI ESG score is a composite metric from 0 to 100 that represents the holistic responsibility and ethical standing of an AI system based on its governance, social impact, and transparency.

**Q: How can I estimate the cost of improving my AI's ethical standing?**
You can use the `project_investment_needs` tool to simulate the required investment in Euros to reach a specific target ESG score.

**Q: Does this tool account for regulatory requirements like the EU AI Act?**
Yes, the scoring model incorporates compliance gaps that reflect the distance between current system states and requirements set by regulatory bodies and institutional investors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ai-esg-scoring-engine](https://vinkius.com/en/ai-agent-connect/ai-esg-scoring-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI ESG Scoring Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-esg-scoring-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI ESG Scoring Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-esg-scoring-engine": {
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
