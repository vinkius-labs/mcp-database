# Bollinger Bands Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bollinger-bands-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bollinger-bands-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bollinger-bands-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate moving standard deviation and Bollinger Bands for financial time-series deterministically.

## Description
Bollinger Bands are crucial for measuring market volatility. They require computing a moving average, then a moving standard deviation, and then adding/subtracting it to form Upper and Lower bands. LLMs fail completely at calculating rolling standard deviations. This engine handles the complex math locally, returning exact arrays for the Upper, Middle, and Lower bands.


## Available Tools
- **calculate_bollinger_bands**: Provide an array of numbers and optional period/stdDev.

Calculates precise Bollinger Bands (Upper, Middle, Lower)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bollinger Bands Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the standard 20-period, 2-std-dev Bollinger Bands for this BTC price history."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Compute the Bollinger Bands, then list all the dates where the closing price was strictly greater than the Upper Band."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Calculate the width between the Upper and Lower bands. If the width shrinks by 50%, flag it as a 'Bollinger Squeeze'."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## Installation & Usage

To install and use the **Bollinger Bands Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bollinger-bands-engine](https://vinkius.com/mcp/bollinger-bands-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
