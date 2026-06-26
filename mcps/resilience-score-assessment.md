# Resilience Score Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/resilience-score-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify your psychological resilience and identify areas of strength or vulnerability.

## Description
The Resilience Score MCP server provides a specialized assessment tool based on the Connor-Davidson Resilience Scale (CD-RISC). It allows AI agents to process survey responses and calculate an aggregate resilience score, classify the overall resilience level (Low, Moderate, or High), and identify specific psychological dimensions--Control, Adaptability, and Perseverance--that may be vulnerable. Using tools like `calculate_resilience_score`, `analyze_dimension_vulnerability`, and `get_dimension_breakdown`, agents can provide deep insights into an individual's capacity to bounce back from adversity.


## Available Tools (3)
- **analyze_dimension_vulnerability**: Identify which resilience dimensions are below average
- **calculate_resilience_score**: Calculate total resilience score and level
- **get_dimension_breakdown**: Get the raw score breakdown by dimension


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resilience Score Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the resilience score for these responses: {"q1": 5, "q2": 4, "q3": 2, "q4": 5, "q5": 3, "q6": 4}."

**🤖 AI Agent:**
> The total resilience score is 23, which corresponds to a High level of resilience.

---

**👤 You:**
> "Check if any dimensions are vulnerable in this assessment: {"q1": 1, "q2": 5, "q3": 5, "q4": 5, "q5": 5, "q6": 5}."

**🤖 AI Agent:**
> The vulnerable dimension identified is: Control.

---

**👤 You:**
> "Show me the breakdown of scores by dimension for these responses: {"q1": 4, "q2": 2, "q3": 5, "q4": 4, "q5": 1, "q6": 5}."

**🤖 AI Agent:**
> The scores by dimension are: Control: 6, Adaptability: 3, Perseverance: 10.


## ❓ FAQ

**Q: What dimensions are measured in the assessment?**
The assessment measures three key psychological dimensions: Control, Adaptability, and Perseverance.

**Q: How is the resilience level determined?**
The level is determined by calculating the total score from all responses and comparing it against predefined thresholds for Low, Moderate, or High resilience.

**Q: What does it mean if a dimension is 'vulnerable'?**
A dimension is flagged as vulnerable if its average score is lower than the overall assessment average, indicating a specific area for improvement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/resilience-score-assessment](https://vinkius.com/mcp/resilience-score-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resilience Score Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resilience-score-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resilience Score Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resilience-score-assessment": {
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
