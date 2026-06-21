# Reorder Point Calculator MCP Server

Calculate optimal reorder points and safety stock levels based on demand volatility and service level targets.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/reorder-point-calculator)

## Overview
**Category:** inventory-management
**Tools Count:** 3

## Description
This MCP server provides advanced inventory management capabilities to prevent stockouts and optimize holding costs. Using the `calculate_reorder_metrics` tool, you can determine your exact reorder point (ROP), safety stock quantity, coverage days, and annual holding costs by providing average daily demand, lead time, and demand standard deviation. Additionally, use `get_service_level_zscore` to find statistical multipliers for different service levels, or `analyze_volatility_impact` to simulate how changes in demand uncertainty will affect your required inventory buffers.


## Available Tools
- **analyze_volatility_impact**: Analyze how changes in demand uncertainty affect stock levels
- **calculate_reorder_metrics**: Calculate optimal reorder point and safety stock
- **get_service_level_zscore**: Retrieve Z-score for a specific service level


## Installation & Usage

To install and use the **Reorder Point Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/reorder-point-calculator](https://vinkius.com/mcp/reorder-point-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
