# Unit & FX Calculator MCP Server

Stop LLMs from mixing metric and imperial units or hallucinating exchange rates. Deterministic physical unit conversion and live currency rates.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/unit-fx-calculator)

## Overview
**Category:** productivity
**Tools Count:** 3

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


## Installation & Usage

To install and use the **Unit & FX Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unit-fx-calculator](https://vinkius.com/mcp/unit-fx-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
