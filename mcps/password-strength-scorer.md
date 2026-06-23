# Password Strength Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/password-strength-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Evaluate any password using the Dropbox zxcvbn engine — the same algorithm protecting 700M+ users. Returns a 0-4 score, real crack time estimates, and actionable improvement suggestions. No AI can do this.

## Description
Ask an AI if 'P@ssw0rd123' is a strong password. It will say 'yes — it has uppercase, lowercase, numbers, and symbols.' That's wrong. zxcvbn cracks it in under a second because it recognizes the pattern: 'Password' + common l33t substitutions + sequential numbers.

No AI can truly evaluate password strength. This MCP uses the Dropbox zxcvbn engine — the same algorithm trusted by 700M+ users — which performs real combinatorial analysis against dictionaries, keyboard patterns, dates, and l33t-speak.

### The Superpowers

- **Real Science, Not Rules:** Doesn't check 'has uppercase + number'. Analyzes actual crack difficulty using pattern matching and combinatorics.
- **4 Attack Scenarios:** Crack time estimates for online throttled, online unthrottled, local slow hash, and local fast hash.
- **Actionable Feedback:** Returns specific warnings ('Common l33t substitution') and improvement suggestions.
- **100% Local:** The password never leaves the engine. Zero network calls. Zero data leakage.


## Available Tools (1)
- **score_password_strength**: The zxcvbn engine (created by Dropbox) detects common patterns, dictionary words, keyboard sequences (qwerty, zxcvbn), dates, and l33t-speak substitutions. It returns a score from 0 (very weak) to 4 (very strong), estimated crack times for different attack scenarios, and actionable feedback. No AI can truly evaluate password strength — this engine uses real combinatorial analysis.

Evaluates password strength using the Dropbox zxcvbn engine. Returns a 0-4 score, crack time estimates, and improvement suggestions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Password Strength Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our new hire set their password to 'Summer2024!'. Is that actually secure?"

**🤖 AI Agent:**
> Score: 1 (Weak). Warning: Common word + predictable year + single symbol. Crack time: 3 minutes local. Suggest: use unrelated words.

---

**👤 You:**
> "Is 'correct horse battery staple' really stronger than 'Tr0ub4dor&3'?"

**🤖 AI Agent:**
> Yes. 'correct horse battery staple': Score 4 (Very Strong), centuries to crack. 'Tr0ub4dor&3': Score 1, common l33t pattern.

---

**👤 You:**
> "Audit our auto-generated API keys for security compliance before deployment."

**🤖 AI Agent:**
> Score: 4 (Very Strong). Crack time: centuries at 10B guesses/sec. Entropy exceeds compliance minimum.


## ❓ FAQ

**Q: Why can't my AI evaluate password strength?**
AI checks superficial rules like 'has uppercase + number + symbol'. zxcvbn does combinatorial analysis — it knows 'P@ssw0rd' is just 'Password' with l33t substitutions, and rates it as weak despite passing every 'rule-based' check.

**Q: Is the password sent to any external server?**
No. 100% local. The embedded dictionary and pattern matching engine run entirely in-process. Zero network calls, zero data leakage, zero risk.

**Q: What do the crack time numbers actually mean?**
Four real attack scenarios: Online throttled (100/hour — most login pages), Online unthrottled (10/sec), Local slow hash (10K/sec — bcrypt), Local fast hash (10B/sec — MD5/SHA). Choose the scenario matching your system.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/password-strength-scorer](https://vinkius.com/mcp/password-strength-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Password Strength Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `password-strength-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Password Strength Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "password-strength-scorer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
