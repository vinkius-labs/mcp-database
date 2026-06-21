# Bullwhip Effect Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bullwhip-effect-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bullwhip-effect-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bullwhip-effect-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Quantify demand amplification and identify instability patterns in supply chains.

## Description
The Bullwhip Effect Calculator allows you to measure how demand fluctuations increase as they move upstream through the supply chain. Using tools like `get_segment_amplification`, you can calculate the amplification ratio between specific stages. You can also use `assess_chain_severity` to evaluate overall health (Low, Medium, or Severe) and `identify_instability_source` to pinpoint which tier--Retailer, Distributor, or Manufacturer--is driving variance increases.


## Available Tools
- **assess_chain_severity**: Evaluates the overall health of the supply chain by classifying the total cumulative amplification
- **get_segment_amplification**: If downstream <= upstream, ratio is 1.

Determines the specific amplification ratio for a single transition between two supply chain stages
- **identify_instability_source**: Identifies which specific tier in the supply chain is most responsible for amplification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bullwhip Effect Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the amplification ratio between a retailer with 10 units of demand variance and a distributor with 25 units of order variance."

**🤖 AI Agent:**
> The amplification ratio is 2.50x.

---

**👤 You:**
> "Assess the severity of a supply chain where the first segment ratio is 1.2 and the second is 3.5."

**🤖 AI Agent:**
> The supply chain severity is classified as Severe due to the high amplification in the second segment.

---

**👤 You:**
> "Identify the source of instability given consumer variance 5, retailer 10, distributor 40, and manufacturer 100."

**🤖 AI Agent:**
> The primary driver of instability is the Manufacturer tier.


## Installation & Usage

To install and use the **Bullwhip Effect Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bullwhip-effect-calculator](https://vinkius.com/mcp/bullwhip-effect-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
