# SAT Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sat-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate Digital SAT 2024 scores, percentile rankings, and US university competitiveness.

## Description
The SAT Score Calculator is a specialized tool for students to estimate their Digital SAT performance. By providing the number of correct answers in Evidence-Based Reading & Writing and Mathematics, you can use `get_section_scaled_score` to find your scaled scores (200-800). The server also allows you to `calculate_aggregate_score` for a total composite score (400-1600), `evaluate_percentile_rank` to see where you stand globally, and `assess_university_competitiveness` to compare your results against benchmarks from top 50 US universities.


## Available Tools (4)
- **calculate_aggregate_score**: Computes the total composite SAT score
- **evaluate_percentile_rank**: Determines the global percentile tier
- **get_section_scaled_score**: Converts a raw count of correct answers into the standardized scaled score for a specific section
- **assess_university_competitiveness**: Compares score against Top 50 US university benchmarks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAT Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I got 45 correct in Reading & Writing and 48 correct in Math. What is my total score?"

**🤖 AI Agent:**
> Your scaled scores are 720 for Reading & Writing and 760 for Math, resulting in a total composite SAT score of 1480.

---

**👤 You:**
> "Is a score of 1500 competitive for top US universities?"

**🤖 AI Agent:**
> A score of 1500 is considered highly competitive for many top-tier institutions.

---

**👤 You:**
> "What percentile rank corresponds to a total score of 1200?"

**🤖 AI Agent:**
> A total score of 1200 falls into the Average performance tier.


## ❓ FAQ

**Q: How do I calculate my total SAT score?**
First, use `get_section_scaled_score` for both Reading & Writing and Math. Then, pass those two scaled scores into the `calculate_aggregate_score` tool to get your total composite score.

**Q: Can I see how competitive my score is for Ivy League schools?**
Yes. Use the `assess_university_competitiveness` tool with your total score to see if you fall within the competitive ranges of top 50 US universities.

**Q: What does the percentile rank tool tell me?**
The `evaluate_percentile_rank` tool compares your total score against historical performance brackets to determine if you are in the Elite, High Achievement, Average, or Low Performance tier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sat-score-calculator](https://vinkius.com/mcp/sat-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SAT Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sat-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SAT Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sat-score-calculator": {
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
