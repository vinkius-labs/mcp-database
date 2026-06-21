# ProUni Eligibility Calculator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prouni-eligibility-calculator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/prouni-eligibility-calculator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/prouni-eligibility-calculator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Instantly calculate scholarship eligibility (Full or Partial) for ProUni by inputting family income, household size, and ENEM scores.

## Description
**Are you considering higher education but unsure about scholarship eligibility?** Many students face the challenge of matching their financial background and academic performance against complex, shifting institutional criteria. Trying to calculate eligibility manually using minimum wage multipliers and specific score cutoffs is time-consuming and prone to error.


## Available Tools
- **determine_eligibility_tier**: Determine scholarship eligibility tier based on per capita income
- **identify_eligible_courses**: Public school students receive a score bonus. Lower scholarship tiers restrict available courses.

Identify eligible courses based on ENEM scores, public school status, and scholarship tier
- **calculate_per_capita_income**: Calculate per capita income from gross family income and number of members
- **query_university_locations**: Query universities participating in ProUni by city


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProUni Eligibility Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My family's gross income is 60,000 and there are 4 members. I scored well in Science."

**🤖 AI Agent:**
> First, we calculate your per capita income using `calculate_per_capita_income`. Based on that result and your ENEM scores, I can then run the `identify_eligible_courses` tool to suggest majors you qualify for.

---

**👤 You:**
> "I want to know which universities are in São Paulo that offer ProUni programs."

**🤖 AI Agent:**
> I will use the `query_university_locations` tool with 'São Paulo' as the city. This provides a list of available universities and campuses for your planning.

---

**👤 You:**
> "My per capita income is 1800, and I attended a public school. What tier am I in?"

**🤖 AI Agent:**
> The `determine_eligibility_tier` tool will analyze your income against the 1.5x and 3x minimum wage thresholds to provide a definitive scholarship tier, which is crucial for all subsequent checks.


## Installation & Usage

To install and use the **ProUni Eligibility Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prouni-eligibility-calculator](https://vinkius.com/mcp/prouni-eligibility-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
