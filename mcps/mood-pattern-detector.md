# Mood Pattern Detector MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mood-pattern-detector)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mood-pattern-detector-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mood-pattern-detector-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identify recurring emotional trends and correlations between mood fluctuations and lifestyle variables.

## Description
The Mood Pattern Detector analyzes historical mood logs to uncover cyclical patterns and the impact of external factors. Use `analyze_weekly_cycle` to find days associated with specific moods, `evaluate_activity_impact` to measure how variables like exercise or sleep influence your emotional state, and `identify_mood_anomalies` to flag significant deviations from your baseline mood.


## Available Tools
- **analyze_weekly_cycle**: Determine if specific days of the week are associated with better or worse moods
- **evaluate_activity_impact**: Measure how a specific recorded variable influences mood levels
- **identify_mood_anomalies**: Flag specific dates where the mood was significantly different from the norm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mood Pattern Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any specific days of the week where my mood tends to be lower?"

**🤖 AI Agent:**
> The `analyze_weekly_cycle` tool would examine your logs and return the day with the lowest average mood score, such as identifying a 'Monday Slump'.

---

**👤 You:**
> "Does my exercise routine affect my emotional well-being?"

**🤖 AI Agent:**
> By using `evaluate_activity_impact` with 'exercise' as the variable, the tool will compare your average mood on days you exercised versus days you did not.

---

**👤 You:**
> "Check if there were any unusual spikes or drops in my mood recently."

**🤖 AI Agent:**
> The `identify_mood_anomalies` tool will scan your historical data and list specific dates where your mood was significantly higher or lower than your norm.


## Installation & Usage

To install and use the **Mood Pattern Detector** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mood-pattern-detector](https://vinkius.com/mcp/mood-pattern-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
