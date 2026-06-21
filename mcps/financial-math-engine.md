# Financial Math Engine MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/financial-math-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/financial-math-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/financial-math-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI with zero-hallucination financial calculation powers. Calculate flawless Amortization Schedules (SAC/PRICE), Compound Interest, and Loan projections.

## Description
LLMs are notoriously bad at math, often hallucinating numbers when calculating large tables. This MCP solves that by offloading complex financial calculations to a deterministic TypeScript engine.

### Superpowers

- **Flawless Amortization:** Ask the AI to generate a 360-month loan schedule (SAC or PRICE). The MCP calculates the exact principal, interest, and remaining balance for every single month without missing a cent.
- **Compound Interest:** Project investments over years with monthly contributions. 
- **Zero External APIs:** This engine is self-contained and runs securely within the Vinkius platform, requiring no third-party internet connections or API keys.


## Available Tools
- **calculate_amortization**: Type can be SAC (Constant Amortization) or PRICE (French Amortization System).

Calculates a perfect amortization schedule (SAC or PRICE) without hallucination
- **calculate_compound_interest**: Calculates exact compound interest over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Financial Math Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a PRICE amortization table for a $100,000 loan over 12 months at 1.5% monthly interest."

**🤖 AI Agent:**
> I calculated the PRICE table for $100,000 at 1.5% for 12 months.

Your fixed monthly installment is **$9,168.00**.
Total Interest Paid: **$10,015.99**.
Total Amount Paid: **$110,015.99**.

Here is the month-by-month breakdown...

---

**👤 You:**
> "Calculate compound interest for a $10,000 initial investment over 240 months, with a $500 monthly contribution at 0.8% monthly return."

**🤖 AI Agent:**
> Here is the 20-year (240 months) compound interest projection:

- **Initial Principal:** $10,000.00
- **Total Out of Pocket:** $130,000.00
- **Total Interest Earned:** $286,413.91
- **Final Balance:** $416,413.91

The power of compound interest means you more than tripled your total contributed amount over 20 years.

---

**👤 You:**
> "Generate a SAC amortization table for a $500,000 mortgage over 360 months at a 0.75% monthly rate."

**🤖 AI Agent:**
> I generated the SAC (Constant Amortization System) table for the $500,000 mortgage.

Your first installment will be **$5,138.89**, decreasing every month until your final installment of **$1,399.31**.
- **Total Interest:** $676,875.00
- **Total Paid:** $1,176,875.00

Here is the detailed table showing exactly how your interest decreases each month.


## Installation & Usage

To install and use the **Financial Math Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/financial-math-engine](https://vinkius.com/mcp/financial-math-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
