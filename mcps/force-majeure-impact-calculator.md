# Force Majeure Impact Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/force-majeure-impact-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/force-majeure-impact-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/force-majeure-impact-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Calculate the legal and operational impact of Force Majeure events on contract obligations.

## Description
This MCP server provides tools to assess how Force Majeure events affect contractual duties. Using `calculate_suspension_period`, you can determine when obligations are expected to resume based on event start dates and estimated durations. The `determine_notice_deadline` tool identifies the critical window for formal notification, accounting for differences between US Common Law and EU Civil Law jurisdictions. Finally, `evaluate_termination_trigger` helps identify if an event's duration has reached the threshold required to exercise termination rights for Service, Supply, or Construction contracts.


## Available Tools
- **calculate_suspension_period**: Determines the exact date when the suspension of contractual obligations is expected to end
- **determine_notice_deadline**: Identifies the final date by which the affected party must formally notify the counterparty
- **evaluate_termination_trigger**: Determines if the prolonged nature of the event has reached the threshold for termination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Force Majeure Impact Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "An event started on 2024-01-01 and is expected to last 20 days. When will obligations resume?"

**🤖 AI Agent:**
> You can use `calculate_suspension_period` with eventStartDate: '2024-01-01' and estimatedDurationDays: 20 to find the end date.

---

**👤 You:**
> "A construction contract event started on 2024-05-10 and has lasted 45 days. Can I terminate?"

**🤖 AI Agent:**
> Using `evaluate_termination_trigger` with eventDurationDays: 45, contractType: 'CONSTRUCTION', and jurisdiction: 'US_COMMON_LAW' will show that the threshold (90 days) has not yet been reached.

---

**👤 You:**
> "What is the notice deadline for a US contract that started yesterday?"

**🤖 AI Agent:**
> The `determine_notice_deadline` tool will calculate the 7-day window required for US Common Law jurisdictions.


## Installation & Usage

To install and use the **Force Majeure Impact Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/force-majeure-impact-calculator](https://vinkius.com/mcp/force-majeure-impact-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
