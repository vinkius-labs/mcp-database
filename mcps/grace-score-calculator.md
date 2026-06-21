# GRACE Score Calculator MCP Server

Calculates the Global Registry of Acute Coronary Events (GRACE) risk score to predict in-hospital and six-month mortality for ACS patients.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/grace-score-calculator)

## Overview
**Category:** cardiology
**Tools Count:** 2

## Description
The clinical assessment of a patient with Acute Coronary Syndrome (ACS) requires more than just looking at vital signs. A comprehensive risk score is needed to predict short-term mortality and guide immediate treatment decisions. The GRACE Score Calculator addresses this gap by providing a standardized, clinically validated toolset for accurate risk stratification.

### How it works:
The system takes nine core clinical parameters--including age, heart rate, systolic blood pressure, creatinine level, Killip class, cardiac arrest status, ST deviation, and troponin concentration. It uses these inputs to compute the composite GRACE score (0-100).

**Mechanism:**
1.  The primary calculation is handled by `calculate_grace_score`. This tool computes a weighted risk score based on established medical guidelines.
2.  Once the raw score is generated, `get_risk_category` maps that numerical output to an actionable risk category (Low, Intermediate, or High). 
3.  Furthermore, the system estimates both in-hospital and six-month mortality probabilities using hardcoded lookup tables for precise clinical prediction.

The result provides a clear, data-driven view of the patient's immediate and long-term prognosis, allowing care teams to prioritize resources and intervene before adverse events occur.


## Available Tools
- **calculate_grace_score**: Calculate GRACE risk score for acute coronary syndrome patients
- **get_risk_category**: Get risk category and recommendation for a GRACE score


## Installation & Usage

To install and use the **GRACE Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grace-score-calculator](https://vinkius.com/mcp/grace-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
