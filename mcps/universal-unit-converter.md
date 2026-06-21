# Universal Unit Converter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/universal-unit-converter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/universal-unit-converter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/universal-unit-converter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A zero-latency deterministic engine for exact physical conversions. Instantly convert weights, lengths, temperatures, and digital storage local.

## Description
Large Language Models often approximate metric-to-imperial conversions, which can lead to critical errors in engineering, development, or logistics. The Universal Unit Converter MCP delegates these conversions to a robust, exact mathematical engine.

### The Superpowers
- **Zero Approximation:** Guarantees absolute mathematical precision by replacing LLM guesses with deterministic JavaScript algorithms.
- **Universal Coverage:** Flawlessly converts across Length (metric/imperial), Weight, Temperature (C/F/K), and Digital Storage (using binary 1024 multipliers).
- **Privacy First (Local):** Executes 100% locally. Zero API calls, meaning your sensitive engineering metrics or server logs never leave your machine.


## Available Tools
- **convert_digital_storage**: g., 1 KB = 1024 B).

Converts digital storage using binary prefixes (B, KB, MB, GB, TB)
- **convert_length**: Converts length between metric and imperial (km, m, cm, mm, mi, yd, ft, in)
- **convert_temperature**: Converts temperature between Celsius (C), Fahrenheit (F), and Kelvin (K)
- **convert_weight**: Converts weight between metric and imperial (kg, g, lb, oz)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Universal Unit Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 135 pounds (lb) to kilograms."

**🤖 AI Agent:**
> Using the convert_weight tool: 135 lb is exactly 61.2350 kg.

---

**👤 You:**
> "If a server requires 8192 MB of RAM, how many GB is that?"

**🤖 AI Agent:**
> Using the convert_digital_storage tool: 8192 MB is exactly 8 GB.

---

**👤 You:**
> "Convert 78 degrees Fahrenheit to Celsius for the weather report."

**🤖 AI Agent:**
> Using the convert_temperature tool: 78 F is 25.56 C.


## Installation & Usage

To install and use the **Universal Unit Converter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/universal-unit-converter](https://vinkius.com/mcp/universal-unit-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
