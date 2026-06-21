# Ideal Weight Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ideal-weight-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ideal-weight-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ideal-weight-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate your target weight range using scientific formulas like Lorentz, Devine, and Robinson.

## Description
This MCP server provides a precise engine for calculating healthy weight ranges. By utilizing established physiological models including the Lorentz, Devine, and Robinson formulas, alongside a BMI 22 benchmark, it helps you understand your target body mass. Use `calculate_ideal_weight_metrics` to find your range, `assess_bmi_status` to check your current BMI category, and `calculate_weight_gap` to determine exactly how much weight you need to gain or lose to reach your ideal window.


## Available Tools
- **assess_bmi_status**: Assess current BMI and category
- **calculate_ideal_weight_metrics**: Calculate target weight values using various scientific formulas
- **calculate_weight_gap**: Analyze the gap between current weight and target range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ideal Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my ideal weight range if I am a 180cm male?"

**🤖 AI Agent:**
> Based on the Lorentz, Devine, and Robinson models, your target weight range is approximately 67.5kg to 78.2kg.

---

**👤 You:**
> "I am 165cm and weigh 70kg. What is my BMI?"

**🤖 AI Agent:**
> Your current Body Mass Index (BMI) is 25.7, which falls into the Overweight category.

---

**👤 You:**
> "How much weight do I need to lose to reach a target range of 60kg to 65kg if I currently weigh 72kg?"

**🤖 AI Agent:**
> You are currently 7kg above your maximum target weight and 12kg above your minimum target weight.


## Installation & Usage

To install and use the **Ideal Weight Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ideal-weight-calculator](https://vinkius.com/mcp/ideal-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
