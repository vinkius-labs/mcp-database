# Blood Type Compatibility & Demographics MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blood-type-compatibility-demographics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/blood-type-compatibility-demographics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/blood-type-compatibility-demographics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Check blood and plasma transfusion compatibility, pregnancy risks, and regional blood type distributions.

## Description
This MCP server provides specialized tools for medical and demographic inquiries regarding blood types. Use `get_rbc_compatibility` to determine if red blood cells can be safely transfused between donors and recipients. Use `get_plasma_rag_compatibility` (wait, checking tool name... it's `get_plasma_compatibility`) to check plasma transfusion safety. The `analyze_pregnancy_risk` tool evaluates Rh incompatibility risks for expectant mothers, while `get_population_distribution` provides statistical data on blood type prevalence in specific regions.


## Available Tools
- **get_plasma_compatibility**: Determines if a donor blood type can safely provide plasma to a recipient
- **get_population_distribution**: Retrieves the blood type distribution for a specific region
- **analyze_pregnancy_risk**: Evaluates the risk of Rh incompatibility between two partners
- **get_rbc_compatibility**: Determines if a donor blood type can safely provide red blood cells to a recipient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blood Type Compatibility & Demographics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is O- compatible with AB+ for red blood cells?"

**🤖 AI Agent:**
> Yes, O- is a universal donor and is compatible with AB+ for red blood cell transfusion.

---

**👤 You:**
> "What is the risk if the mother is A- and the father is O+?"

**🤖 AI Agent:**
> There is a risk of Rh sensitization because the mother is Rh-negative and the father is Rh-positive.

---

**👤 You:**
> "Show me the blood type distribution in Brazil."

**🤖 AI Agent:**
> In Brazil, the distribution is: O+ (36%), A+ (34%), B+ (7%), O- (5%), A- (4%), AB+ (2%), B- (1%), and AB- (1%).


## Installation & Usage

To install and use the **Blood Type Compatibility & Demographics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blood-type-compatibility-demographics](https://vinkius.com/mcp/blood-type-compatibility-demographics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
