# Heart Rate Zones Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heart-rate-zones-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/heart-rate-zones-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/heart-rate-zones-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise physiological training zones using Simple % and Karvonen (HRR) methods.

## Description
This MCP server provides a precision fitness utility for calculating five distinct heart rate training zones. It supports two primary calculation methodologies: the Simple Percentage method, which uses your maximum heart rate as a baseline, and the Karvonen (Heart Rate Reserve) method, which incorporates your resting heart rate for a more personalized intensity range. The server also includes advanced estimation models like Tanaka and Gulati to predict your maximum heart rate based on age and gender. Use `estimate_max_hr` to find your predicted ceiling, then apply `calculate_simple_zones` or `calculate_karvonen_zones` to define your training boundaries.


## Available Tools
- **estimate_max_hr**: Estimate maximum heart rate based on age and gender
- **calculate_karvonen_zones**: Calculate training zones using the Karvonen (HRR) method
- **calculate_simple_zones**: Calculate training zones using simple percentage of MaxHR


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heart Rate Zones Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a 30-year-old male. What is my estimated max heart rate?"

**🤖 AI Agent:**
> Based on the Tanaka model for a 30-year-old male, your estimated maximum heart rate is 191 BPM.

---

**👤 You:**
> "My max HR is 180 and my resting HR is 60. What are my training zones using the Karvonen method?"

**🤖 AI Agent:**
> Using the Karvonen method, your training zones are: Zone 1 (90-108 BPM), Zone 2 (108-126 BPM), Zone 3 (126-144 BPM), Zone 4 (144-162 BPM), and Zone 5 (162-180 BPM).

---

**👤 You:**
> "Calculate my simple training zones if my max HR is 190."

**🤖 AI Agent:**
> Based on a maximum heart rate of 190 BPM, your simple intensity zones are: Zone 1 (95-114 BPM), Zone 2 (114-133 BPM), Zone 3 (133-152 BPM), Zone 4 (152-171 BPM), and Zone 5 (171-190 BPM).


## Installation & Usage

To install and use the **Heart Rate Zones Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heart-rate-zones-calculator](https://vinkius.com/mcp/heart-rate-zones-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
