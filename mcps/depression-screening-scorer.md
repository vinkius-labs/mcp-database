# Depression Screening Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/depression-screening-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Clinical tool for scoring PHQ-9 depression assessments and analyzing symptom clusters.

## Description
This MCP server provides clinical utility for processing responses from validated depression screening instruments like the PHQ-9. It allows AI agents to calculate total scores, determine severity categories, and perform granular symptom domain analysis. Using `score_phq9`, agents can obtain a full assessment including clinical recommendations. The `analyze_symptom_clusters` tool identifies specific physiological or emotional impacts, while `evaluate_risk_flags` identifies critical items requiring immediate attention. It is designed to assist practitioners in determining levels of care based on standardized clinical protocols.


## Available Tools (4)
- **analyze_symptom_clusters**: Provides a granular view of which physiological or emotional domains are most affected
- **evaluate_risk_flags**: Specifically checks for critical items that require immediate attention, regardless of the total score
- **get_severity_thresholds**: Retrieves the scoring ranges used to define clinical severity
- **score_phq9**: Calculates the comprehensive depression score and severity for a single PHQ-9 assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Depression Screening Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Score this PHQ-9 assessment: [1, 0, 2, 1, 0, 0, 1, 0, 0]"

**🤖 AI Agent:**
> The total score is 5, which falls into the Minimal depression category.

---

**👤 You:**
> "Analyze the symptom clusters for these responses: [0, 0, 0, 0, 0, 0, 0, 0, 3]"

**🤖 AI Agent:**
> The analysis shows a high impact in the critical risk domain due to the reported symptom.

---

**👤 You:**
> "What are the severity thresholds for the USA?"

**🤖 AI Agent:**
> In the USA, the categories are: Minimal (0-4), Mild (5-6), Moderate (7-9), Moderately Severe (10-14), and Severe (15-27).


## ❓ FAQ

**Q: How do I use the scoring tool?**
Provide an array of 9 integers (ranging from 0 to 3) representing the PHQ-9 responses to the `score_phq9` tool.

**Q: Can this tool detect high-risk symptoms?**
Yes, the `evaluate_risk_flags` tool specifically checks for critical items that require immediate clinical attention.

**Q: Does this provide a medical diagnosis?**
No, this is a clinical utility tool designed to assist practitioners with quantitative scoring and guidance; it is not a substitute for professional diagnosis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/depression-screening-scorer](https://vinkius.com/en/ai-agent-connect/depression-screening-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Depression Screening Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `depression-screening-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Depression Screening Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "depression-screening-scorer": {
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
