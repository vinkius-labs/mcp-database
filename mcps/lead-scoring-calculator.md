# Lead Scoring Calculator MCP Server

Calculate a lead's conversion readiness score instantly using configurable firmographic and behavioral data points.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lead-scoring-calculator)

## Overview
**Category:** marketing-automation
**Tools Count:** 3

## Description
**How to Assess Lead Value in Minutes.**Finding high-potential leads is difficult. Traditional methods rely on guesswork or simple demographic matching, leading teams to waste time nurturing cold contacts. The core problem is accurately quantifying a lead's readiness for sales handoff.**The Solution: Weighted Predictive Scoring.** This calculator provides an objective score (0-100) based on measurable data. It operates in three steps:1. **Gather Profile Data:** We first use `query_lead_profile_data` to collect foundational attributes like company size, industry sector, and job title.2. **Retrieve Weights:** Next, we call `query_scoring_configuration` to fetch the latest scoring weights and qualification thresholds (e.g., what constitutes an MQL vs. SQL).3. **Calculate Score:** Finally, `calculate_converted_score` executes the weighted algorithm using all gathered data and configuration parameters, returning a composite score, classification status, and estimated conversion probability.**Key Advantage:** This system moves beyond simple lead counting. It provides actionable intelligence--a definitive status (Cold, Warm, Hot, MQL, SQL)--allowing sales teams to prioritize outreach based on calculated value, maximizing efficiency for the entire pipeline.


## Available Tools
- **calculate_converted_score**: Returns total score, qualification status (Cold/Warm/Hot/MQL/SQL), and estimated conversion probability.

Calculate composite lead score with qualification status and conversion probability
- **query_lead_profile_data**: Optionally specify a scoring version ID.

Retrieve raw lead profile data for scoring
- **query_scoring_configuration**: Retrieve current scoring configuration weights and thresholds


## Installation & Usage

To install and use the **Lead Scoring Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lead-scoring-calculator](https://vinkius.com/mcp/lead-scoring-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
