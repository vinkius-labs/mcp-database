# DAS Payment Scheduler MCP Server

Automated annual calendar generator for Brazilian Simples Nacional tax payments, handling holiday-based date shifts and overdue period alerts.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/das-payment-scheduler)

## Overview
**Category:** productivity
**Tools Count:** 3

## Description
The DAS Payment Scheduler is a specialized tool for Brazilian entrepreneurs to manage their Simples Nacional tax obligations. It automatically calculates the exact payment deadlines by checking if the standard 20th of the month falls on a weekend or a national holiday, shifting the date forward to the next business day when necessary. Using `generate_annual_schedule`, you can view your entire year's payment plan at once. If you are unsure why a specific date changed, use `inspect_holiday_impact` to see the reason for the shift. Additionally, the `identify_overdue_periods` tool helps you stay on top of your taxes by alerting you to any months where the deadline has already passed.


## Available Tools
- **generate_annual_schedule**: Generates a yearly schedule of DAS payments
- **inspect_holiday_impact**: Inspects if a specific payment date was moved due to holidays or weekends
- **identify_overdue_periods**: Identifies which months have passed their DAS payment deadline


## Installation & Usage

To install and use the **DAS Payment Scheduler** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/das-payment-scheduler](https://vinkius.com/mcp/das-payment-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
