# MACD & RSI Oscillator Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/macd-rsi-oscillator-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/macd-rsi-oscillator-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/macd-rsi-oscillator-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Calculate exact MACD and Relative Strength Index (RSI) technical indicators local for quantitative analysis.

## Description
The Relative Strength Index (RSI) and Moving Average Convergence Divergence (MACD) are complex oscillators that require multiple passes of exponential averages. Asking an LLM to compute RSI over 100 days is a guaranteed failure. This engine integrates institutional-grade TS indicator math into the Vinkius edge runtime, providing autonomous trading and analysis agents with perfect signals.


## Available Tools
- **calculate_macd_rsi**: Provide data array and configuration parameters.

Calculates MACD or RSI technical oscillators from a price array


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MACD & RSI Oscillator Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the 14-period RSI for this daily stock price array. Tell me if the final day is below 30 (Oversold)."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Run the MACD calculator. Check the last 3 days and tell me if the MACD line has crossed above the Signal line (bullish)."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "I see the price making a new high here. Calculate the RSI and tell me if the RSI is making a lower high (bearish divergence)."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## Installation & Usage

To install and use the **MACD & RSI Oscillator Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/macd-rsi-oscillator-engine](https://vinkius.com/mcp/macd-rsi-oscillator-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
