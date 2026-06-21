# SOFA Score Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sofa-score-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sofa-score-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sofa-score-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate SOFA scores, mortality risk, and sepsis status.

## Description
The SOFA Score Calculator is a clinical decision support tool designed to quantify organ dysfunction in patients. Using the `compute_organ_scores` tool, you can convert raw physiological measurements like PaO2, FiO2, and creatinine levels into standardized 0-4 scores for respiratory, coagulation, hepatic, cardiovascular, neurological, and renal systems. Once individual scores are obtained, use `calculate_total_sofa` to aggregate them into a single total score and determine the clinical severity level. The tool also provides advanced insights: `estimate_mortality_risk` uses the total score to provide mortality risk tiers, while `evaluate_sepsis_status` identifies Sepsis-3 criteria by detecting an acute change of 2 or more points from a baseline SOFA score.


## Available Tools
- **calculate_total_sofa**: Aggregates individual organ scores into a single SOFA score and severity level
- **compute_organ_scores**: Converts clinical values into standardized 0-4 SOFA organ scores
- **estimate_mortality_risk**: Provides mortality risk classification based on the total SOFA score
- **evaluate_sepsis_status**: Determines if a patient meets Sepsis-3 criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SOFA Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the SOFA organ scores for a patient with PaO2 80, FiO2 0.4, platelets 150, bilirubin 1.2, MAP 70, no vasopressors, GCS 15, creatinine 1.0, and urine output 1.5."

**🤖 AI Agent:**
> The calculated organ scores are: Respiratory: 1, Coagulation: 0, Hepatic: 0, Cardiovascular: 0, Neurological: 0, Renal: 0.

---

**👤 You:**
> "What is the mortality risk for a total SOFA score of 15?"

**🤖 AI Agent:**
> A total SOFA score of 15 falls into the High Risk tier, with an estimated mortality probability in the severe range.

---

**👤 You:**
> "A patient's baseline SOFA score was 4, and their current score is 7. Do they meet sepsis criteria?"

**🤖 AI Agent:**
> Yes, the patient meets Sepsis-3 criteria because there is an increase of 3 points from their baseline score.


## Installation & Usage

To install and use the **SOFA Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sofa-score-calculator](https://vinkius.com/mcp/sofa-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
