# Heart Score Calculator MCP Server

Determine acute myocardial infarction (AMI) risk using five key clinical metrics.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/heart-score-calculator)

## Overview
**Category:** cardiology
**Tools Count:** 3

## Description
# Heart Score Calculator: Acute Myocardial Infarction Risk Assessment

The initial assessment of chest pain patients is complex. Determining if symptoms are benign or indicative of a serious cardiac event requires aggregating information from multiple sources--a process prone to human variability and omission.

**The Problem:** Standard clinical pathways require synthesizing data from History, ECGs, Age, Comorbidities (Risk Factors), and Troponin levels into a single, actionable risk score. This synthesis must adhere strictly to AHA/ESC guidelines for immediate patient triage.

**The Mechanism:** This MCP connects AI agents directly to the necessary medical logic using three specialized tools:
1.  `calculate_heart_score`: Aggregates all five components (H, E, A, R, T) into a total score of 0-10.
2.  `classify_risk_and_triage`: Takes the resulting score and maps it to 'Low', 'Moderate', or 'High' risk categories with a defined triage level.
3.  `recommend_clinical_conduct`: Uses the final risk classification to generate mandatory diagnostic pathways, management directives, and follow-up schedules based on current medical standards.

**The Advantage:** The system provides deterministic, guideline-backed clinical decision support. Instead of generic advice, it outputs specific next steps--which tests to order, and where the patient should be managed--allowing clinicians to focus immediately on high-priority care.


## Available Tools
- **calculate_heart_score**: History and ECG scores are optional and default to 0 if not provided.

Calculate the total HEART score for acute myocardial infarction risk assessment
- **classify_risk_and_triage**: Patient age group is optional for validation.

Classify a HEART score into risk category and determine triage priority
- **recommend_clinical_conduct**: Adjusts for emergency room setting and patient gender when provided.

Provide evidence-based clinical recommendations based on risk classification


## Installation & Usage

To install and use the **Heart Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heart-score-calculator](https://vinkius.com/mcp/heart-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
