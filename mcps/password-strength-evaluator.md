# Password Strength Evaluator MCP Server

Equip SecOps agents with Dropbox's zxcvbn engine. Algorithmically evaluate password entropy and crack times local.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/password-strength-evaluator)

## Overview
**Category:** loved-by-devs
**Tools Count:** 1

## Description
When a Security Operations (SecOps) AI Agent audits a database of plain-text passwords or handles user creation, it needs to evaluate password strength. LLMs use subjective, probabilistic guessing which often approves weak passwords that bypass simple regex checks (like `P@ssword1`). This MCP solves that entirely.

### The Superpowers

- **Algorithmic Evaluation:** Uses the industry-standard `zxcvbn` engine to calculate true mathematical entropy, pattern matching, and dictionary analysis.
- **Crack Time Estimation:** Returns the precise estimated time an attacker would need to crack the password via local fast hashing.


## Available Tools
- **evaluate_password**: Pass the raw password string and receive a score (0-4), estimated crack time, and specific weakness feedback. Use the score to enforce minimum security policies.

Algorithmsically evaluates password strength and estimates offline crack time. Essential for SecOps agents auditing user credentials


## Installation & Usage

To install and use the **Password Strength Evaluator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/password-strength-evaluator](https://vinkius.com/mcp/password-strength-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
