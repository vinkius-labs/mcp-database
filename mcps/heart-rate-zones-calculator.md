# Heart Rate Zones Calculator MCP Server

Calculate precise physiological training zones using Simple % and Karvonen (HRR) methods.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/heart-rate-zones-calculator)

## Overview
**Category:** health
**Tools Count:** 3

## Description
This MCP server provides a precision fitness utility for calculating five distinct heart rate training zones. It supports two primary calculation methodologies: the Simple Percentage method, which uses your maximum heart rate as a baseline, and the Karvonen (Heart Rate Reserve) method, which incorporates your resting heart rate for a more personalized intensity range. The server also includes advanced estimation models like Tanaka and Gulati to predict your maximum heart rate based on age and gender. Use `estimate_max_hr` to find your predicted ceiling, then apply `calculate_simple_zones` or `calculate_karvonen_zones` to define your training boundaries.


## Available Tools
- **estimate_max_hr**: Estimate maximum heart rate based on age and gender
- **calculate_karvonen_zones**: Calculate training zones using the Karvonen (HRR) method
- **calculate_simple_zones**: Calculate training zones using simple percentage of MaxHR


## Installation & Usage

To install and use the **Heart Rate Zones Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heart-rate-zones-calculator](https://vinkius.com/mcp/heart-rate-zones-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
