# US Statute of Limitations Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-statute-of-limitations-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/us-statute-of-limitations-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/us-statute-of-limitations-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Calculate US legal filing deadlines based on claim type, state, and accrual date.

## Description
This MCP server provides precise tools for determining the statute of limitations for various legal actions across US states. Use `calculate_statute_deadline` to find standard deadlines for contract, tort, or fraud claims. The server also supports evaluating the discovery rule via `evaluate_discovery_rule` and assessing how tolling events like minority or incapacity might extend your deadline using `check_tolling_impact`.


## Available Tools
- **check_tolling_impact**: Identifies if any known tolling events have extended the existing deadline
- **calculate_statute_deadline**: Determines the standard filing deadline based on claim type, state, and the date of the incident
- **evaluate_discovery_rule**: Re-calculates a deadline based on the moment the harm was discovered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Statute of Limitations Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the statute of limitations for a breach of contract in California that occurred on 2023-01-01."

**🤖 AI Agent:**
> The calculated deadline for your contract claim in CA is 2026-01-01.

---

**👤 You:**
> "What happens if I discovered a fraud on 2024-05-20 that originally occurred on 2020-01-01 in New York?"

**🤖 AI Agent:**
> The revised deadline based on the discovery rule is 2030-05-20.

---

**👤 You:**
> "Check if a tolling event on 2022-06-15 extends my current deadline of 2024-01-01."

**🤖 AI Agent:**
> The extended deadline after accounting for the tolling event is 2025-06-15.


## Installation & Usage

To install and use the **US Statute of Limitations Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-statute-of-limitations-calculator](https://vinkius.com/mcp/us-statute-of-limitations-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
