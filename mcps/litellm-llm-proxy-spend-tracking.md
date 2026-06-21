# LiteLLM (LLM Proxy & Spend Tracking) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/litellm-llm-proxy-spend-tracking)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/litellm-llm-proxy-spend-tracking-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/litellm-llm-proxy-spend-tracking-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage your LLM gateway via LiteLLM — generate API keys, track spending, and orchestrate model fallback paths.

## Description
Connect your **LiteLLM Proxy** instance to any AI agent and take full control of your LLM infrastructure, load balancing, and spend management through natural conversation.

### What you can do

- **Key Orchestration** — Generate and manage proxy API keys to isolate distinct microservices or teams, including precise budget and rate limit constraints directly from your agent
- **Model Routing Intelligence** — Get detailed info on fallback paths (e.g., OpenAI -> Anthropic -> Groq) and verify exact routing endpoints assigned to your models
- **Real-time Spend Audit** — Track total USD consumed by specific end-users or teams and monitor budget ceilings to ensure cost-effective AI deployments
- **Dynamic Model Control** — Inject fresh routing endpoints (e.g., new AWS Bedrock or Azure OpenAI deployments) into your proxy runtime with zero downtime
- **Team & Organizational Isolation** — Create and manage team profiles to track exact cost limits and operational boundaries per organizational division
- **Infrastructure Security** — Instantly vaporize malicious or leaked keys and remove broken LLM deployments to prevent downstream 500 errors dynamically

### How it works

1. Subscribe to this server
2. Enter your LiteLLM API URL and Master Key
3. Start managing your LLM gateway from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Platform Engineers** — manage global LLM gateway configurations and audit model fallback paths through natural conversation
- **AI Ops Teams** — monitor real-time AI spending and adjust team budgets across multiple LLM providers
- **Backend Developers** — generate sub-keys for new microservices and verify model routing availability without leaving your IDE


## Available Tools
- **create_model**: Inject completely fresh routing endpoints (ex: new Bedrock Llama 4 endpoints)
- **create_team**: Generate pristine organizational isolation tracking exact cost limits per division
- **create_user**: Insert specific End-User identities bridging Vinkius with Proxy logs
- **delete_key**: Delete an existing LLM proxy key entirely
- **delete_model**: Delete explicitly routed LLM deployments preventing 500s dynamically
- **generate_key**: Generate a new proxy API key isolating distinct microservices or teams
- **get_key_info**: Get configuration and budget bounds for a specific LiteLLM API Key
- **get_model_info**: Get array endpoints tracing exact Fallback paths like OpenAI -> Anthropic
- **get_team_info**: Get internal logic bounds matching multiple routing users via Team UUID
- **get_user_info**: Return precise End-User abstractions tracking total USD consumed natively


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LiteLLM (LLM Proxy & Spend Tracking)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active model fallback paths in LiteLLM"

**🤖 AI Agent:**
> I've retrieved your model configurations. Your current fallback paths include: 'gpt-4' -> 'claude-3-opus', 'text-embedding-3-small' -> 'voyage-2', and 'llama-3' -> 'mistral-large'. Would you like to check the latency for any of these providers?

---

**👤 You:**
> "Generate a new API key for the 'Customer-Service' team with a $50 monthly budget"

**🤖 AI Agent:**
> Generating key… Done. I've successfully provisioned a new sub-key for the 'Customer-Service' team (ID: team-987) with a hard budget limit of $50.00. The new key is: `sk-litellm-abc123...`. You can now use this for their microservice deployment.

---

**👤 You:**
> "How much has user 'alex_dev' spent on LLM tokens today?"

**🤖 AI Agent:**
> Retrieving data for user 'alex_dev'… So far today, this user has consumed 12,450 total tokens across 45 requests, resulting in a total cost of $0.85 USD. Their most used model is 'gpt-3.5-turbo'. Would you like to see their remaining daily budget?


## Installation & Usage

To install and use the **LiteLLM (LLM Proxy & Spend Tracking)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/litellm-llm-proxy-spend-tracking](https://vinkius.com/mcp/litellm-llm-proxy-spend-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
