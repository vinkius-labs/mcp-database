# One Rep Max Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/one-rep-max-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/one-rep-max-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/one-rep-max-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate your maximum lifting capacity using Epley, Brzycki, and Lander models.

## Description
This MCP server provides specialized tools for strength athletes to predict their One Repetition Maximum (1RM) without the physical strain of a true max test. Use `get_epley_estimate` for a widely recognized method, `get_brzycki_estimate` for an alternative approach based on intensity ratios, or `get_lander_estimate` for a more complex statistical model. You can also use `get_lift_intensity` to determine the training load percentage of your sets.


## Available Tools
- **get_brzycki_estimate**: Determine the estimated 1RM using the Brzycki method
- **get_epley_estimate**: Determine the estimated 1RM using the Epley method
- **get_lift_intensity**: Calculate the percentage of a user's maximum capability used
- **get_lander_estimate**: Determine the estimated 1RM using the Lander/Lombardi method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **One Rep Max Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my estimated 1RM if I lifted 100kg for 5 reps using the Epley method?"

**🤖 AI Agent:**
> Using `get_epley_estimate`, your estimated 1RM is 125kg.

---

**👤 You:**
> "Calculate the intensity of a 80lb set if my max is 100lb."

**🤖 AI Agent:**
> The `get_lift_intensity` tool shows your training intensity was 80%.

---

**👤 You:**
> "Estimate my max using Brzycki with 200lbs for 3 reps."

**🤖 AI Agent:**
> The `get_brzyck_estimate` tool predicts a 1RM of approximately 210.53lbs.


## Installation & Usage

To install and use the **One Rep Max Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/one-rep-max-calculator](https://vinkius.com/mcp/one-rep-max-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
