# Password Strength Scorer MCP Server

Evaluate any password using the Dropbox zxcvbn engine — the same algorithm protecting 700M+ users. Returns a 0-4 score, real crack time estimates, and actionable improvement suggestions. No AI can do this.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/password-strength-scorer)

## Overview
**Category:** loved-by-devs
**Tools Count:** 1

## Description
Ask an AI if 'P@ssw0rd123' is a strong password. It will say 'yes — it has uppercase, lowercase, numbers, and symbols.' That's wrong. zxcvbn cracks it in under a second because it recognizes the pattern: 'Password' + common l33t substitutions + sequential numbers.

No AI can truly evaluate password strength. This MCP uses the Dropbox zxcvbn engine — the same algorithm trusted by 700M+ users — which performs real combinatorial analysis against dictionaries, keyboard patterns, dates, and l33t-speak.

### The Superpowers

- **Real Science, Not Rules:** Doesn't check 'has uppercase + number'. Analyzes actual crack difficulty using pattern matching and combinatorics.
- **4 Attack Scenarios:** Crack time estimates for online throttled, online unthrottled, local slow hash, and local fast hash.
- **Actionable Feedback:** Returns specific warnings ('Common l33t substitution') and improvement suggestions.
- **100% Local:** The password never leaves the engine. Zero network calls. Zero data leakage.


## Available Tools
- **score_password_strength**: The zxcvbn engine (created by Dropbox) detects common patterns, dictionary words, keyboard sequences (qwerty, zxcvbn), dates, and l33t-speak substitutions. It returns a score from 0 (very weak) to 4 (very strong), estimated crack times for different attack scenarios, and actionable feedback. No AI can truly evaluate password strength — this engine uses real combinatorial analysis.

Evaluates password strength using the Dropbox zxcvbn engine. Returns a 0-4 score, crack time estimates, and improvement suggestions


## Installation & Usage

To install and use the **Password Strength Scorer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/password-strength-scorer](https://vinkius.com/mcp/password-strength-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
