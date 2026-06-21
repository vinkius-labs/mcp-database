# VO2max Estimator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vo2max-estimator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/vo2max-estimator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/vo2max-estimator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate aerobic capacity using Cooper, Rockport, Step, and YMCA Bike protocols.

## Description
This MCP server provides specialized tools to estimate VO2max (maximal oxygen uptake) through four standardized physical fitness protocols: `calculate_cooper` for the 12-minute run, `calculate_rockport` for the one-mile walk test, `calculate_step_test` for cardiovascular recovery analysis, and `calculate_ymca_bike` for steady-state cycling assessments. Each tool calculates oxygen uptake in ml/kg/min and provides an ACSM fitness classification based on age and sex.


## Available Tools
- **calculate_rockport**: Estimate VO2max using the Rockport Walk Test
- **calculate_step_test**: Estimate VO2max using the Step Test
- **calculate_ymca_bike**: Estimate VO2max using the YMCA Bike Test
- **calculate_cooper**: Estimate VO2max using the Cooper 12-minute run test


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VO2max Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much VO2max did I achieve in my 12-minute run of 2500 meters, assuming I am a 25 year old male?"

**🤖 AI Agent:**
> Your estimated VO2max is 48.5 ml/kg/min, which falls into the Excellent category for a 25-year-old male.

---

**👤 You:**
> "Calculate my VO2max using the Rockport Walk Test: 15 minutes for one mile, heart rate of 140 bpm, weight 75kg, age 30, female."

**🤖 AI Agent:**
> Your estimated VO2max is 38.2 ml/kg/min, which falls into the Good category for a 30-year-old female.

---

**👤 You:**
> "What is my fitness level based on a Step Test with a recovery heart rate of 110 bpm and baseline of 70 bpm for a 40 year old male?"

**🤖 AI Agent:**
> Your estimated VO2max is 35.4 ml/kg/min, which falls into the Fair category for a 40-year-old male.


## Installation & Usage

To install and use the **VO2max Estimator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vo2max-estimator](https://vinkius.com/mcp/vo2max-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
