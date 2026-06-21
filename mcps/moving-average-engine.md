# Moving Average Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moving-average-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moving-average-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moving-average-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Calculate Simple (SMA) and Exponential (EMA) moving averages exactly. Stop LLMs from estimating financial technical indicators.

## Description
Large Language Models are notoriously bad at sequential math. If you give an LLM 100 days of stock closing prices and ask for a 14-day SMA, it will hallucinate the averages. This engine processes arrays natively in JS, computing mathematically precise Simple and Exponential Moving Averages local, giving your financial agents the reliable technical indicators they need for quantitative analysis.


## Available Tools
- **calculate_moving_average**: Calculates exact Simple (SMA) or Exponential (EMA) moving averages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Average Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Here are 200 daily closing prices for Apple. Calculate the 50-day Simple Moving Average."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "I need to spot short-term trends. Run a 9-period EMA on these hourly crypto prices."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Calculate both a 50-day SMA and a 200-day SMA for this dataset. Tell me the exact index where the 50 crosses above the 200."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## Installation & Usage

To install and use the **Moving Average Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moving-average-engine](https://vinkius.com/mcp/moving-average-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
