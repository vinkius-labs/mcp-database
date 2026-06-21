# LiteLLM (LLM Proxy & Spend Tracking) MCP Server

Manage your LLM gateway via LiteLLM — generate API keys, track spending, and orchestrate model fallback paths.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/litellm-llm-proxy-spend-tracking)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

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


## Installation & Usage

To install and use the **LiteLLM (LLM Proxy & Spend Tracking)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/litellm-llm-proxy-spend-tracking](https://vinkius.com/mcp/litellm-llm-proxy-spend-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
