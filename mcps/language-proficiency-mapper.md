# Language Proficiency Mapper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/language-proficiency-mapper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Translate raw exam scores (IELTS, TOEFL, DELF, etc.) into CEFR levels and check visa/university requirements.

## Description
**Need to prove language skill for travel or study?** 🌍 Getting accepted to a university or securing a visa requires more than just passing an exam; it demands proof of a specific, standardized proficiency level. The complexity lies in translating diverse scoring systems--like IELTS' band scores versus TOEFL' raw points--into one common standard. This tool solves that gap by providing reliable CEFR mapping and cross-border requirement checks.


## Available Tools (3)
- **get_cross_exam_equivalency**: Useful for understanding how one score compares to other major exams.

Get equivalent proficiency levels across different language exams for a given CEFR level
- **map_exam_score_to_cefr**: Returns the mapped CEFR level from A1 to C2.

Map a language exam score to its equivalent CEFR proficiency level
- **check_minimum_requirements**: Returns pass/fail status and the required minimum level.

Check if a CEFR proficiency level meets minimum language requirements for a country and purpose


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Language Proficiency Mapper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I took the DELF exam. I scored B2 in French. What does this mean for admission to a German university?"

**🤖 AI Agent:**
> First, let's map your score using `map_exam_score_to_cefr`. Then, we can use `check_minimum_requirements` by setting the country to Germany and the purpose to 'University Enrollment'.

---

**👤 You:**
> "I need to know if my TOEFL score of 105 is enough for a UK Student Visa."

**🤖 AI Agent:**
> We will first use `map_exam_score_to_cefr` with my TOEFL details. Once we have the CEFR level, I will run `check_minimum_requirements` for 'UK' and 'Student Visa'.

---

**👤 You:**
> "My primary exam is Cambridge C1 Advanced. What are some equivalent levels in TOEFL or DELF?"

**🤖 AI Agent:**
> I can run `get_cross_exam_equivalency` for you, specifying 'Cambridge C1 Advanced' and the resulting CEFR level (likely B2). This will give you a helpful comparative map.


## ❓ FAQ

**Q: What is the core function of this service?**
The primary function is to use the `map_exam_score_to_cefr` tool. You provide a raw score (e.g., IELTS band 7), and it converts that into the standardized CEFR level (B2). This mapping is critical for all subsequent checks.

**Q: How can I check if my score meets a university's minimum requirement?**
Use the `check_minimum_requirements` tool. Simply input your target country (e.g., Germany), the purpose (University Enrollment), and your current CEFR level. The system will tell you if you pass or fail against hardcoded policy rules.

**Q: I have a B2 score on IELTS; what does that mean for other exams?**
For cross-comparison, use the `get_cross_exam_equivalency` tool. You provide your primary exam and CEFR level (e.g., IELTS, B2), and it retrieves documented advisory equivalencies for other major tests like TOEFL or DELF.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/language-proficiency-mapper](https://vinkius.com/mcp/language-proficiency-mapper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Language Proficiency Mapper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `language-proficiency-mapper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Language Proficiency Mapper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "language-proficiency-mapper": {
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
