# GRACE Score Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grace-score-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/grace-score-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/grace-score-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cardiology](../categories/cardiology.md)

Calculates the Global Registry of Acute Coronary Events (GRACE) risk score to predict in-hospital and six-month mortality for ACS patients.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GRACE Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the GRACE score for a 65-year-old male with HR of 90, SBP of 120, creatinine of 1.1, Killip Class II, no cardiac arrest, ST deviation of 1, and troponin elevated."

**🤖 AI Agent:**
> First, I will call `calculate_grace_score` with the provided vitals. Then, using the resulting score, I will call `get_risk_category` to get the final risk assessment and mortality estimates.

---

**👤 You:**
> "I need an estimated 6-month mortality risk for a patient with a calculated GRACE score of 78, who is age 75 and Killip Class III."

**🤖 AI Agent:**
> To determine the long-term prognosis, I will use `get_risk_category` (or a related prediction endpoint if available) with the score of 78. This function is designed to provide mortality estimates based on age and Killip class.

---

**👤 You:**
> "What are the critical parameters for the calculator?"

**🤖 AI Agent:**
> The core calculation relies on inputting vitals like SBP, HR, and lab results (creatinine/troponin) via `calculate_grace_score` to generate the initial score.


## Installation & Usage

To install and use the **GRACE Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grace-score-calculator](https://vinkius.com/mcp/grace-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
