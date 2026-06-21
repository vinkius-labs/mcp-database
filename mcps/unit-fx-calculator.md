# Unit & FX Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unit-fx-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/unit-fx-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/unit-fx-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Stop LLMs from mixing metric and imperial units or hallucinating exchange rates. Deterministic physical unit conversion and live currency rates.

## Description
LLMs notoriously struggle with complex compound conversions (e.g. converting km/h to mph with specific decimal rounding). Worse, they hallucinate foreign exchange (FX) rates based on their historical training data rather than current markets. This MCP bridges that gap.

### The Superpowers

- **Physical Determinism:** Converts length, mass, volume, temperature, and speed using the exact mathematical engine of `mathjs`. Completely eliminates metric/imperial hallucination.
- **Live FX Rates:** Uses the Frankfurter API to fetch the latest European Central Bank reference rates for absolutely precise currency conversion.
- **In-Memory Edge Cache:** FX rates are cached in a native V8 `Map` for 1 hour, meaning massive batch conversions run instantly without getting rate-limited.


## Available Tools
- **batch_convert**: ). Pass the value, source unit, and target unit for exact mathematical conversion.

Converts multiple physical units in a single deterministic pass
- **convert_unit**: Deterministically converts physical units (e.g. km/h to mph, celsius to fahrenheit)using mathjs
- **get_rate**: Gets the exact foreign exchange rate between two currencies using Frankfurter API (1h cache)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unit & FX Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 120 km/h into miles per hour (mph) and round strictly to 2 decimals."

**🤖 AI Agent:**
> ✅ **Converted Unit:** `74.56 mph`

---

**👤 You:**
> "Fetch the live exchange rate to convert `USD` to `BRL`."

**🤖 AI Agent:**
> ✅ **Live FX Rate:** `5.21` (Fetched from European Central Bank, cached locally).

---

**👤 You:**
> "Batch convert this array of 5 temperatures from Celsius to Fahrenheit deterministically."

**🤖 AI Agent:**
> ✅ **Batch Completed:** Processed 5 units instantly with 0 loss in float precision.


## Installation & Usage

To install and use the **Unit & FX Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unit-fx-calculator](https://vinkius.com/mcp/unit-fx-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
