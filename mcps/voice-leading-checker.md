# Voice Leading Checker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/voice-leading-checker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/voice-leading-checker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/voice-leading-checker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analysis](../categories/analysis.md)

Analyze musical voice-leading integrity between chord voicings using classical harmonic principles.

## Description
The Voice Leading Checker is an analytical engine designed to evaluate the movement of musical notes across four distinct melodic ranges: Bass, Tenor, Alto, and Soprano (SATB). By using tools like `analyze_voice_conduction`, `check_voice_hierarchy`, and `evaluate_smoothness`, AI agents can detect harmonic errors such as parallel fifths, parallel octaves, voice crossing, and excessive melodic leaps. This MCP server provides direct access to precise musical analysis, returning violation details, quality scores, and suggested alternative voicings to ensure smooth and correct harmonic transitions.


## Available Tools
- **analyze_voice_conduction**: Analytes the conduction between two chord voicings
- **check_voice_hierarchy**: Validates that voices are in correct ascending order
- **evaluate_smoothness**: Evaluates the smoothness of a musical transition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Voice Leading Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this transition is harmonically correct: Initial {bass: 36, tenor: 48, alto: 55, soprano: 67} to Target {bass: 39, tenor: 51, alto: 58, soprano: 70}."

**🤖 AI Agent:**
> The `analyze_voice_conduction` tool has analyzed the transition. No parallel fifths or octaves were detected, and the movement is smooth.

---

**👤 You:**
> "Evaluate the smoothness of a transition with 2 violations and a leap magnitude sum of 12."

**🤖 AI Agent:**
> Using `evaluate_smoothness`, the quality grade is determined based on the error count and leap magnitude provided.

---

**👤 You:**
> "Is this voicing valid: Bass 40, Tenor 38, Alto 50, Soprano 60?"

**🤖 AI Agent:**
> The `check_voice_hierarchy` tool indicates this is invalid because the Tenor pitch (38) is lower than the Bass pitch (40), violating the required ascending order.


## Installation & Usage

To install and use the **Voice Leading Checker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/voice-leading-checker](https://vinkius.com/mcp/voice-leading-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
