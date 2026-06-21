# Forgetting Curve Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/forgetting-curve-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/forgetting-curve-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/forgetting-curve-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Predict memory decay and schedule learning reinforcements using the Ebbinghaus Forgetting Curve.

## Description
The Forgetting Curve Calculator is a mathematical engine designed to help learners master long-term retention. Based on the principles of the Ebbinghaus Forgetting Curve, this MCP server provides tools to track how information decays over time and when you should intervene with review sessions. Use `get_current_retention` to see your current memory strength, `predict_decay_thresholds` to identify upcoming critical drop-off points (70%, 50%, and 20%), and `estimate_maintenance_effort` to plan the number of future reviews needed for long-term stability. It acts as a bridge between your learning data and AI agents like Cursor, Claude Desktop, and Windsurf, allowing you to automate your study scheduling.


## Available Tools
- **estimate_maintenance_effort**: Estimate required future reviews for long-term stability
- **get_current_retention**: Calculate current memory retention percentage
- **predict_decay_thresholds**: Predict when memory will drop below critical thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Forgetting Curve Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I studied biology on 2024-05-01. I have done 2 reviews with a 7-day interval. What is my current retention?"

**🤖 AI Agent:**
> Your current memory retention for biology is 85%.

---

**👤 You:**
> "Based on my study date of 2024-06-10, 3 revisions, and a 5-day interval, when will my retention drop below 70%?"

**🤖 AI Agent:**
> Your retention is predicted to drop below the 70% threshold in approximately 4 days.

---

**👤 You:**
> "I want to maintain a 90% retention for my history topic. I currently have 75% retention with a 10-day interval. How many more reviews do I need?"

**🤖 AI Agent:**
> You will need approximately 3 more review sessions to reach and maintain your target of 90% retention.


## Installation & Usage

To install and use the **Forgetting Curve Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/forgetting-curve-calculator](https://vinkius.com/mcp/forgetting-curve-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
