# MEWS Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mews-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mews-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mews-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Quantify patient physiological deterioration using the Modified Early Warning Score (MEWS) system.

## Description
The MEWS Calculator is a clinical assessment tool designed to identify patients at risk of clinical deterioration. By analyzing vital signs such as respiratory rate, SpO2, heart rate, systolic blood pressure, body temperature, and consciousness level (AVPU), it calculates a cumulative score. Use the `calculate_mews_score` tool to compute the numerical score, `get_clinical_classification` to determine risk levels, and `check_activation_threshold` to see if a Rapid Response Team activation is necessary.


## Available Tools
- **check_activation_threshold**: Checks if a MEWS score requires activation of the Rapid Response Team
- **calculate_mews_score**: Calculates the cumulative MEWS score based on vital signs
- **get_clinical_classification**: Determines the clinical risk category based on a MEWS score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MEWS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the MEWS score for a patient with RR 24, SpO2 92%, HR 110, SBP 95, Temp 38.5, and level V."

**🤖 AI Agent:**
> The calculated MEWS score is 5.

---

**👤 You:**
> "What is the clinical risk for a patient with a MEWS score of 2?"

**🤖 AI Agent:**
> A MEWS score of 2 indicates a Low Risk status.

---

**👤 You:**
> "Does a MEWS score of 6 require RRT activation?"

**🤖 AI Agent:**
> Yes, a score of 6 meets the threshold. Action Required: Activate Rapid Response.


## Installation & Usage

To install and use the **MEWS Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mews-calculator](https://vinkius.com/mcp/mews-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
