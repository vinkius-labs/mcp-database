# ENEM Score Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enem-score-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/enem-score-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/enem-score-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate ENEM performance metrics and simulate university admission possibilities based on historical cutoff scores.

## Description
This MCP server provides specialized tools to quantify student performance in the ENEM exam. Use `calculate_area_averages` to determine the arithmetic mean of objective exam areas. You can also use `calculate_weighted_score` to compute a final score based on specific subject weights, and `simulate_admission_possity` to compare your results against historical cutoff scores for various courses and universities.


## Available Tools
- **simulate_admission_possibility**: Compare a student's score against historical data to predict admission success
- **calculate_area_averages**: Calculate the arithmetic mean of the four objective exam areas
- **calculate_weighted_score**: Calculate the final performance score based on custom importance weights


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ENEM Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my average for the four objective areas with these scores: Languages 600, Math 700, Science 550, Humanities 650."

**🤖 AI Agent:**
> The `calculate_area_averages` tool would return an average score of 625.0.

---

**👤 You:**
> "Will I pass Medicine at University X if my weighted score is 800 in 2023?"

**🤖 AI Agent:**
> You can use `simulate_admission_possibility` with the course and university IDs to check this against historical records.

---

**👤 You:**
> "Calculate a weighted score: Languages 600 (weight 1), Math 700 (weight 2), Science 550 (weight 1), Humanities 650 (weight 1), and Essay 800 (weight 3)."

**🤖 AI Agent:**
> The `calculate_weighted_score` tool will process these inputs to return your final weighted performance score.


## Installation & Usage

To install and use the **ENEM Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/enem-score-calculator](https://vinkius.com/mcp/enem-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
