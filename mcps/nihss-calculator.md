# NIHSS Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nihss-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nihss-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nihss-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate NIH Stroke Scale scores and assess stroke severity instantly.

## Description
The NIHSS Calculator is a clinical decision support tool that allows healthcare professionals to quantify neurological impairment following an acute stroke. By using the `calculate_nihss` tool, users can input individual scores for eleven neurological components--including consciousness level, gaze, facial palsy, and motor function--to receive an immediate total score and severity classification. Additionally, the `get_scoring_guide` tool provides detailed scoring ranges for each component, while `evaluate_urgency` offers standardized clinical instructions based on the patient's neurological state. This MCP server acts as a bridge between clinical assessment data and AI agents in clients like Cursor, VS Code, Claude Desktop, and Windsurf.


## Available Tools
- **calculate_nihss**: Calculate the NIHSS score and severity
- **evaluate_urgency**: Evaluate clinical urgency based on NIHSS score
- **get_scoring_guide**: Retrieve the scoring guide for NIHSS components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NIHSS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the NIHSS score for a patient with these scores: consciousnessLevel: 1, consciousnessQuestions: 0, consciousnessCommands: 0, gaze: 0, visualFields: 0, facialPalsy: 2, motorFunction: 1, ataxia: 0, sensory: 0, language: 1, dysarthria: 0, extinction: 0."

**🤖 AI Agent:**
> The total NIHSS score is 5, which falls into the Moderate severity classification.

---

**👤 You:**
> "What is the scoring guide for facial palsy?"

**🤖 AI Agent:**
> For facial palsy, a score of 0 indicates no paralysis, while higher scores represent increasing degrees of facial muscle asymmetry or drooping.

---

**👤 You:**
> "Based on a total NIHSS score of 18, what is the clinical urgency?"

**🤖 AI Agent:**
> The urgency level is Severe, and the clinical note is: Immediate intervention and intensive monitoring are required due to high neurological impairment.


## Installation & Usage

To install and use the **NIHSS Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nihss-calculator](https://vinkius.com/mcp/nihss-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
