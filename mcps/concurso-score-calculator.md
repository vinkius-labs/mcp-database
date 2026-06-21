# Concurso Score Calculator MCP Server

Calculate final examination scores, manage stage thresholds, and estimate competition rankings for civil service exams.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/concurso-score-calculator)

## Overview
**Category:** productivity
**Tools Count:** 4

## Description
This MCP server provides specialized tools to automate the complex scoring logic of competitive examinations. Use `calculate_weighted_score` to determine a candidate's total score based on stage weights, and `verify_stage_thresholds` to ensure minimum requirements are met for each exam phase. You can also use `resolve_tiebreaker` to handle identical scores using a priority hierarchy, or `predict_ranking_position` to estimate a candidate's rank relative to available vacancies.


## Available Tools
- **predict_ranking_position**: Estimates where a candidate stands in the overall competition relative to available job openings
- **calculate_weighted_score**: All stages in scores must have corresponding weights, and total weight must be 1.0.

Determines the total accumulated score for a candidate based on stage performance and importance weights
- **resolve_tiebreaker**: Decides a winner between two or more candidates who have identical final weighted scores
- **verify_stage_thresholds**: All stages in thresholds must be present in scores.

Checks if a candidate's performance meets the minimum requirements to remain in the competition


## Installation & Usage

To install and use the **Concurso Score Calculator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/concurso-score-calculator](https://vinkius.com/mcp/concurso-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
