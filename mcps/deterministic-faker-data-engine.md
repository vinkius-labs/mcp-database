# Deterministic Faker Data Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-faker-data-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate thousands of mock names, addresses, and paragraphs instantly. Perfectly deterministic, 100% local, and ready for E2E testing.

## Description
Using real user data in staging environments or passing production PII to an LLM context is a massive security violation. On the flip side, asking an LLM to invent 500 fake users is slow, wastes tokens, and breaks test determinism because the AI invents different names every time. This MCP solves both issues by acting as a high-speed local data generator.

### The Superpowers
- **Mathematical Determinism:** Pass an optional `seed` integer, and the generator will spit out the exact same names and addresses every single time. Perfect for Cypress or Playwright CI/CD test setups.
- **Instant Scale:** Need 1,000 JSON addresses? Generated in less than 5 milliseconds locally.
- **Zero-API Security:** Never leak your testing intentions to external "fake data" SaaS APIs. The PRNG (Pseudo-Random Number Generator) runs completely locked inside your infrastructure.


## Available Tools
- **generate_fake_addresses**: Provide a count and optionally a numeric seed to guarantee deterministic reproducible outputs.

Deterministically generates random addresses based on a seed
- **generate_fake_names**: Provide a count and optionally a numeric seed to guarantee deterministic reproducible outputs.

Deterministically generates random names and identities based on a seed
- **generate_fake_text**: Provide the number of paragraphs and optionally a numeric seed to guarantee deterministic reproducible outputs.

Deterministically generates random lorem-ipsum paragraphs based on a seed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic Faker Data Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate 5 fake names using seed 42 so I can use them in my Cypress tests."

**🤖 AI Agent:**
> Using the generate_mock_names tool (count=5, seed=42): ['Amelia Anderson', 'Joseph Davis', 'Harper Moore', 'John Smith', 'Olivia Taylor'].

---

**👤 You:**
> "Give me a mock JSON array containing 3 realistic addresses."

**🤖 AI Agent:**
> Using the generate_mock_addresses tool (count=3): I have generated the addresses successfully. Example: '5842 Pine Ln, Springfield, CA 45812'.


## ❓ FAQ

**Q: Why do I need a 'seed' parameter?**
In software testing, you often need the data to be 'fake' but 'repeatable'. If a test fails for user 'John Smith', you want it to generate 'John Smith' again when you re-run the test tomorrow. A seed guarantees mathematical consistency.

**Q: Does it use Faker.js under the hood?**
No. To maintain the 'zero-dependency' utility promise and keep latency at absolute zero, it relies on a custom, lightweight Linear Congruential Generator (LCG) algorithm built directly into the MCP core.

**Q: Is my mock data sent to the cloud?**
No. All generation happens locally in your environment. This ensures 100% compliance with strict enterprise development policies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-faker-data-engine](https://vinkius.com/mcp/deterministic-faker-data-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic Faker Data Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deterministic-faker-data-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic Faker Data Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-faker-data-engine": {
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
