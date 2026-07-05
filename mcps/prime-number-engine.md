# Prime Number Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prime-number-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Advanced computational engine for primality testing, integer factorization, and prime distribution analysis.

## Description
The Prime Number Engine provides high-performance mathematical tools for number theory. Use `test_primality` to determine if a large integer is prime using Trial Division, Deterministic Miller-Rabin, or Probabilistic Miller-Rabin methods. The `factorize_integer` tool decomposes integers into their prime components using trial division and Pollard's rho algorithm. For proximity analysis, `find_adjacent_primes` locates the nearest primes above or below a target value, while `get_prime_density_info` provides statistical insights like estimated prime counts and prime gap sizes.


## Available Tools (4)
- **find_adjacent_primes**: Locate the nearest prime numbers above or below a specified value
- **get_prime_density_info**: Provide statistical insights into prime distribution
- **test_primality**: Determine whether a given integer is prime
- **factorize_integer**: Find all prime factors of an integer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prime Number Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is 104729 a prime number?"

**🤖 AI Agent:**
> Yes, 104729 is a prime number.

---

**👤 You:**
> "What are the prime factors of 123456789?"

**🤖 AI Agent:**
> The prime factors of 123456789 are 3, 3, 3607, and 3803.

---

**👤 You:**
> "Find the next prime after 1000."

**🤖 AI Agent:**
> The next prime number after 1000 is 1009.


## ❓ FAQ

**Q: How accurate is the primality test?**
The engine uses Deterministic Miller-Rabin for numbers up to $3.3 \times 10^{24}$, providing 100% certainty. For larger numbers, the Probabilistic Miller-Rabin method is used with a configurable number of rounds to minimize error probability.

**Q: What algorithm is used for factorization?**
The engine employs trial division up to the cube root of the target number, followed by Pollard's rho algorithm to efficiently find larger prime factors.

**Q: Can I find primes near a specific large number?**
Yes, the `find_adjacent_primes` tool allows you to search for the next, previous, or both adjacent primes relative to any provided integer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prime-number-engine](https://vinkius.com/mcp/prime-number-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prime Number Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prime-number-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prime Number Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prime-number-engine": {
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
