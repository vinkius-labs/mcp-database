# Password Strength Evaluator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/password-strength-evaluator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/password-strength-evaluator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/password-strength-evaluator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Equip SecOps agents with Dropbox's zxcvbn engine. Algorithmically evaluate password entropy and crack times local.

## Description
When a Security Operations (SecOps) AI Agent audits a database of plain-text passwords or handles user creation, it needs to evaluate password strength. LLMs use subjective, probabilistic guessing which often approves weak passwords that bypass simple regex checks (like `P@ssword1`). This MCP solves that entirely.

### The Superpowers

- **Algorithmic Evaluation:** Uses the industry-standard `zxcvbn` engine to calculate true mathematical entropy, pattern matching, and dictionary analysis.
- **Crack Time Estimation:** Returns the precise estimated time an attacker would need to crack the password via local fast hashing.


## Available Tools
- **evaluate_password**: Pass the raw password string and receive a score (0-4), estimated crack time, and specific weakness feedback. Use the score to enforce minimum security policies.

Algorithmsically evaluates password strength and estimates offline crack time. Essential for SecOps agents auditing user credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Password Strength Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate the strength of this generated password: `P@ssw0rd123!`"

**🤖 AI Agent:**
> Password Evaluation: Score is 2, crack time is 12 days. Feedback: Add another word or two. Uncommon words are better.

---

**👤 You:**
> "Check if this temporary password meets our security policy of score 3 or higher."

**🤖 AI Agent:**
> Password Evaluation: Score is 4, crack time is centuries.

---

**👤 You:**
> "Audit this credential and tell me how long it would take to crack via local fast hashing."

**🤖 AI Agent:**
> Password Evaluation: Crack time is less than a second.


## Installation & Usage

To install and use the **Password Strength Evaluator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/password-strength-evaluator](https://vinkius.com/mcp/password-strength-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
