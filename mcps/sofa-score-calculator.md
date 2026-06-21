# SOFA Score Calculator MCP Server

Calculate SOFA scores, mortality risk, and sepsis status.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sofa-score-calculator)

## Overview
**Category:** healthcare
**Tools Count:** 4

## Description
The SOFA Score Calculator is a clinical decision support tool designed to quantify organ dysfunction in patients. Using the `compute_organ_scores` tool, you can convert raw physiological measurements like PaO2, FiO2, and creatinine levels into standardized 0-4 scores for respiratory, coagulation, hepatic, cardiovascular, neurological, and renal systems. Once individual scores are obtained, use `calculate_total_sofa` to aggregate them into a single total score and determine the clinical severity level. The tool also provides advanced insights: `estimate_mortality_risk` uses the total score to provide mortality risk tiers, while `evaluate_sepsis_status` identifies Sepsis-3 criteria by detecting an acute change of 2 or more points from a baseline SOFA score.


## Available Tools
- **calculate_total_sofa**: Aggregates individual organ scores into a single SOFA score and severity level
- **compute_organ_scores**: Converts clinical values into standardized 0-4 SOFA organ scores
- **estimate_mortality_risk**: Provides mortality risk classification based on the total SOFA score
- **evaluate_sepsis_status**: Determines if a patient meets Sepsis-3 criteria


## Installation & Usage

To install and use the **SOFA Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sofa-score-calculator](https://vinkius.com/mcp/sofa-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
