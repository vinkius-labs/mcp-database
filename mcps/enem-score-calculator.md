# ENEM Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enem-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate ENEM scores using simplified IRT, compute averages, and simulate university admission feasibility.

## Description
The ENEM Score Calculator is a specialized engine designed to transform raw exam performance into scaled scores using a simplified Item Response Theory (IRT) model. By providing the number of correct answers in Languages, Mathematics, Natural Sciences, and Human Sciences, along with your essay score, you can use `calculate_area_scores` to obtain subject-specific results. The toolset also allows for computing an overall aggregate average via `calculate_overall_average` and performing admission simulations using `simulate_admission_cutof_match` against historical university cutoff data.


## Available Tools (3)
- **simulate_admission_cutoff_match**: Determines if a student's average meets the historical requirement for a specific course/university
- **calculate_area_scores**: Transforms raw correct answers into scaled subject scores using simplified IRT logic
- **calculate_overall_average**: Computes the final aggregate score from individual component scores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ENEM Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my ENEM scores: 35 correct in Languages, 30 in Math, 25 in Natural Sciences, 30 in Human Sciences, and an essay score of 900."

**🤖 AI Agent:**
> Your scaled scores are: Languages: 620.5, Mathematics: 710.2, Natural Sciences: 580.8, Human Sciences: 640.3, and Essay: 900.0.

---

**👤 You:**
> "What is my final average if my component scores are: languagesScore: 600, mathScore: 700, naturalSciencesScore: 550, humanSciencesScore: 650, and essayScore: 800?"

**🤖 AI Agent:**
> Your final aggregate average score is 650.0.

---

**👤 You:**
> "With an average of 750, can I get into Medicine at USP?"

**🤖 AI Agent:**
> No, your score is 45.0 points below the historical cutoff for Medicine at USP.


## ❓ FAQ

**Q: How does the scoring calculation work?**
The system uses a simplified Item Response Theory (IRT) model. It takes your raw correct answers and applies a difficulty constant unique to each subject area to produce a scaled score between 0 and 1000.

**Q: Can I simulate admission for specific universities?**
Yes. By using the `simulate_admission_cutoff_match` tool, you can compare your calculated average against historical cutoff scores for various universities and courses.

**Q: What inputs are required for the area scores tool?**
You need to provide the number of correct answers for Languages, Mathematics, Natural Sciences, and Human Sciences, plus your essay score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/enem-score-calculator](https://vinkius.com/mcp/enem-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ENEM Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enem-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ENEM Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enem-score-calculator": {
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
