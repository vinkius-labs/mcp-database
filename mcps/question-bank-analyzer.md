# Question Bank Analyzer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/question-bank-analyzer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/question-bank-analyzer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/question-bank-analyzer-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze study performance by identifying critical topics and exam board focus areas.

## Description
The Question Bank Analyzer is a specialized performance engine that evaluates your learning efficiency. By using tools like `analyze_topic_performance`, you can identify subjects where your accuracy falls below the 50% critical threshold. The server also allows you to track progress over time with `track_mock_evolution` and align your study plan with specific exam boards using `fetch_board_focus`. Finally, use `calculate_priority_gaps` to find high-priority topics that are both critical for you and highly relevant to your target examiner.


## Available Tools
- **analyze_topic_performance**: Analyze accuracy rates across different subjects
- **calculate_priority_gaps**: Find high-priority study areas by cross-referencing bad performance with board importance
- **fetch_board_focus**: g., CESPE, FGV) and returns its focus areas.

Retrieve predefined subject importance for a specific exam board
- **track_mock_evolution**: Visualize performance changes across mock exam sessions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Question Bank Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my performance: I got 10 correct and 15 incorrect in Math, and 20 correct and 5 incorrect in History."

**🤖 AI Agent:**
> In Math, your hit rate is 40%, which is a critical topic. In History, your hit rate is 80%, indicating stable knowledge.

---

**👤 You:**
> "What are the main focus areas for the FGV exam board?"

**🤖 AI Agent:**
> The primary focus areas for FGV include Portuguese, Law, and Administrative Logic.

---

**👤 You:**
> "Identify my priority study gaps for the College Board exam based on my critical topics: ['Algebra', 'Geometry']."

**🤖 AI Agent:**
> Your high-priority study areas for the College Board are Algebra and Geometry.


## Installation & Usage

To install and use the **Question Bank Analyzer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/question-bank-analyzer](https://vinkius.com/mcp/question-bank-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
