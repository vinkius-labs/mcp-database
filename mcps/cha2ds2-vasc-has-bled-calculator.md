# CHA₂DS₂-VASc & HAS-BLED Calculator MCP Server

Calculate stroke risk (CHA₂DS₂-VASc) and bleeding risk (HAS-BLED) for atrial fibrillation patients using established clinical guidelines.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cha2ds2-vasc-has-bled-calculator)

## Overview
**Category:** risk-assessment
**Tools Count:** 3

## Description
# Atrial Fibrillation Risk Assessment

The diagnosis of Atrial Fibrillation (AFib) requires careful risk stratification to determine the appropriate balance between preventing stroke and avoiding excessive bleeding. Simply calculating a score is not enough; clinicians need integrated guidance.

**The Problem:** Traditional assessment methods often evaluate thromboembolic risk and hemorrhagic risk separately, leading to disjointed treatment plans. A patient with high AFib risk but also high bleeding risk needs nuanced advice that weighs both factors simultaneously.

**Our Mechanism (Tools):** This MCP connector provides a three-step workflow using specialized tools:
1. **`query_cha2ds2_vasc_score`**: Calculates the total CHA₂DS₂-VASc score based on patient demographics and comorbidities (sex, age, HTN, DM, etc.).
2. **`calculate_hasbled_score`**: Assesses the bleeding risk using the HAS-BLED scale, considering factors like blood pressure control and diuretic use.
3. **`get_risk_recommendations`**: Takes both scores to generate a final recommendation, providing the annual stroke risk percentage (based on ESC 2020 criteria) and definitive anticoagulant guidance ('O' or 'A').

**Advantage:** By running these tools together, agents can provide comprehensive patient care pathways. Instead of just listing a score, they deliver actionable advice that synthesizes both high thromboembolic risk *and* high bleeding risk concerns, guiding the clinician toward optimal therapy.


## Available Tools
- **query_cha2ds2_vasc_score**: Calculate the CHA2DS2-VASc score for atrial fibrillation stroke risk assessment
- **calculate_hasbled_score**: Calculate the HAS-BLED score for bleeding risk assessment during anticoagulation
- **get_risk_recommendations**: Get clinical recommendations based on CHA2DS2-VASc and HAS-BLED scores


## Installation & Usage

To install and use the **CHA₂DS₂-VASc & HAS-BLED Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cha2ds2-vasc-has-bled-calculator](https://vinkius.com/mcp/cha2ds2-vasc-has-bled-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
