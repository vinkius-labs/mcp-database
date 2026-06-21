# WHO-5 Wellbeing Index MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/who-5-wellbeing-index)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/who-5-wellbeing-index-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/who-5-wellbeing-index-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate the WHO-5 Well-Being Index score and identify potential wellbeing risks.

## Description
This MCP server provides specialized tools to quantify psychological well-being using the World Health Organization's WHO-5 scale. Use `calculate_wellbeing_assessment` to input five responses (0-5) and receive a normalized score from 0 to 100, along with a wellbeing classification and risk assessment. You can also use `fetch_scale_instructions` to understand the numeric mapping for each response or `validate_assessment_range` to verify if a specific score falls within the standard valid bounds.


## Available Tools
- **validate_assessment_range**: Verifies if a score is within the 0-100 range
- **calculate_wellbeing_assessment**: Calculates the WHO-5 Well-Being Index score
- **fetch_scale_instructions**: Provides context for the WHO-5 scale


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WHO-5 Wellbeing Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my wellbeing score with these responses: 5, 4, 5, 4, 5."

**🤖 AI Agent:**
> The `calculate_wellbeing_assessment` tool would return a score of 90, indicating Normal Wellbeing with no high-risk indicators detected.

---

**👤 You:**
> "What does the scale mapping look like?"

**🤖 AI Agent:**
> By using `fetch_scale_instructions`, you can see that 0 represents 'Never' and 5 represents 'All the time'.

---

**👤 You:**
> "Is a score of 45 valid?"

**🤖 AI Agent:**
> The `validate_assessment_range` tool would confirm that 45 is within the valid range (0-100), though it indicates a low wellbeing state.


## Installation & Usage

To install and use the **WHO-5 Wellbeing Index** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/who-5-wellbeing-index](https://vinkius.com/mcp/who-5-wellbeing-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
