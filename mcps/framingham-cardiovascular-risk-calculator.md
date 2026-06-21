# Framingham Cardiovascular Risk Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/framingham-cardiovascular-risk-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/framingham-cardiovascular-risk-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/framingham-cardiovascular-risk-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-assessment](../categories/risk-assessment.md)

Calculates your estimated 10-year cardiovascular risk percentage and estimates your vascular age using medical guidelines.

## Description
**Do you know your true heart risk?** Many people assume that based on general health advice, but true cardiovascular risk requires detailed metrics. The Framingham model provides a standardized way to predict the probability of major events like heart attack or stroke over ten years.


## Available Tools
- **calculate_ten_year_risk**: Requires age, sex, total cholesterol, HDL-C, systolic blood pressure, smoking status, and diabetes status.

Calculate the 10-year cardiovascular risk percentage using the Framingham Risk Score model
- **estimate_vascular_age**: Requires total cholesterol, HDL-C, systolic blood pressure, and age.

Estimate the patient vascular age based on cardiovascular markers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Framingham Cardiovascular Risk Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a 55-year-old male. My total cholesterol is 240 mg/dL, HDL-C is 45 mg/dL, and SBP is 135 mmHg. I smoke sometimes and have no diabetes. What is my risk?"

**🤖 AI Agent:**
> Based on the parameters provided, running `calculate_ten_year_risk` suggests a moderate risk classification for your 10-year outlook. It's important to monitor these numbers.

---

**👤 You:**
> "Can you estimate my vascular age? I am 45, female, with total cholesterol of 210 and HDL-C of 60. My SBP is 120."

**🤖 AI Agent:**
> Using the `estimate_vascular_age` tool, your estimated vascular age is [X] years. This suggests your arterial system appears to be [Y] years older/younger than your chronological age.

---

**👤 You:**
> "I need a comprehensive risk assessment for an 68-year-old male. Inputs: Total Chol=270, HDL=35, SBP=160. Smoker and diabetic."

**🤖 AI Agent:**
> I recommend running both `calculate_ten_year_risk` and `estimate_vascular_age`. The risk calculation will provide the 10-year probability, while the vascular age tool provides insight into your current arterial stress levels.


## Installation & Usage

To install and use the **Framingham Cardiovascular Risk Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/framingham-cardiovascular-risk-calculator](https://vinkius.com/mcp/framingham-cardiovascular-risk-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
