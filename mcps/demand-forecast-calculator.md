# Demand Forecast Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/demand-forecast-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/demand-forecast-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/demand-forecast-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Generate 3-month demand projections using SMA, WMA, and Exponential Smoothing methods.

## Description
This MCP server provides advanced forecasting capabilities to predict future demand based on historical data. It implements three distinct mathematical models: Simple Moving Average (`analyze_sma`), Weighted Moving Average (`analyze_wma`), and Exponential Smoothing (`analyze_exponential_smoothing`). For each method, the tools perform error backtesting to provide Mean Absolute Error (MAE) and Mean Absolute Percentage Error (MAPE), allowing you to identify the most accurate model for your specific dataset. Use these tools in Cursor, VS Code, Claude Desktop, or Windsurf to automate demand planning.


## Available Tools
- **analyze_exponential_smoothing**: Calculate demand forecast using Exponential Smoothing
- **analyze_sma**: Calculate demand forecast using Simple Moving Average (SMA)
- **analyze_wma**: Calculate demand forecast using Weighted Moving Average (WMA)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Demand Forecast Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a 3-month forecast using SMA with a window size of 3 for this demand: [10, 12, 15, 14, 18]"

**🤖 AI Agent:**
> The `analyze_sma` tool has processed your data. The forecast for the next three months is [15.67, 15.67, 15.67] with a calculated MAPE of approximately 8.2%.

---

**👤 You:**
> "Use Exponential Smoothing to predict demand for [100, 110, 120] with alpha=0.5 and beta=0.3."

**🤖 AI Agent:**
> Using `analyze_exponential_smoothing`, the predicted demand for the next three periods is [130, 140, 150].

---

**👤 You:**
> "Analyze demand using WMA with weights [0.5, 0.3, 0.2] for data: [50, 60, 70]"

**🤖 AI Agent:**
> The `analyze_wma` tool calculated the forecast as [76, 76, 76] based on your provided weights and historical sequence.


## Installation & Usage

To install and use the **Demand Forecast Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/demand-forecast-calculator](https://vinkius.com/mcp/demand-forecast-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
