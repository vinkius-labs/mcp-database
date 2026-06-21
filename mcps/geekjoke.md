# GeekJoke MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geekjoke)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/geekjoke-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/geekjoke-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Get random geeky and programming-related jokes to lighten up your development workflow.

## Description
Connect to the **GeekJoke** API to fetch humorous content specifically tailored for developers and tech enthusiasts. Whether you need a quick laugh during a debugging session or want to share a joke with your team, this server provides instant access to a curated collection of geeky humor.

### What you can do

- **Random Jokes** — Fetch a random programming or geek joke instantly using the standard query method.
- **API Metadata** — Access information about the underlying API source, including author details and project links.
- **Alternative Generation** — Use an alternative action-based method to retrieve humor content via POST requests.

### How it works

1. Subscribe to this server
2. No API key is required as the service is public
3. Start asking for jokes in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — to break the tension during long coding sessions or frustrating bugs.
- **Team Leads** — to start standups or meetings with a lighthearted, relatable moment.
- **AI Enthusiasts** — to add personality and humor to their custom AI agents.


## Available Tools
- **get_metadata**: Get GeekJoke API metadata
- **generate_random_joke**: Get a random geeky joke via POST
- **get_random_joke**: Get a random geeky joke


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GeekJoke** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me a random geeky joke."

**🤖 AI Agent:**
> Using `get_random_joke`... 'Why do programmers always mix up Halloween and Christmas? Because Oct 31 == Dec 25.'

---

**👤 You:**
> "Show me the metadata for the GeekJoke API."

**🤖 AI Agent:**
> Fetching metadata via `get_metadata`... The API is authored by Sameer Kumar and the project can be found at https://github.com/sameerkumar18/geek-joke-api.

---

**👤 You:**
> "Generate a joke using the POST method."

**🤖 AI Agent:**
> Executing `generate_random_joke`... 'A SQL query goes into a bar, walks up to two tables, and asks, "Can I join you?"'


## Installation & Usage

To install and use the **GeekJoke** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geekjoke](https://vinkius.com/mcp/geekjoke)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
