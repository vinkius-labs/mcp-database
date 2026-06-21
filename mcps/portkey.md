# Portkey MCP Server

AI gateway observability: monitor logs, costs, and manage LLM configurations via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/portkey)

## Overview
**Category:** ai-frontier
**Tools Count:** 10

## Description
### What you can do

Connect AI agents to the Portkey AI Gateway for enterprise-grade observability and management:

- **Monitor logs and traces** of all LLM calls passing through your gateway
- **Analyze token usage, latency, and costs** across models and teams
- **Submit feedback** (Likes/Dislikes) to improve model quality and agent performance
- **Export logs** for audit trails, compliance, and offline cost analysis
- **Review gateway configurations** including retry policies, fallbacks, and cache settings
- **Manage virtual keys** to track provider API key usage and limits
- **Discover supported models** from 1,600+ LLMs available via Portkey
- **Enforce budget policies** to prevent runaway AI costs per team or project

### How it works

1. **Get your Portkey API key** from the dashboard Settings
2. **Ask your AI agent** to check usage, review costs, or manage policies
3. **Natural language commands** replace manual Portkey dashboard navigation
4. **Unified observability** across all your LLM providers (OpenAI, Anthropic, Google, etc.)

### Who is this for?

Essential for **AI platform engineers**, **LLM ops teams**, **FinOps analysts**, **AI governance officers**, and **engineering managers** using multiple LLM providers. Let AI agents monitor gateway health, identify cost spikes, enforce budget policies, and optimize routing. Perfect for organizations spending $10k+/month on LLMs who need granular visibility into usage, latency, and model performance across the enterprise.


## Available Tools
- **create_policy**: Requires policy name, budget limit (USD or token count), and optionally the target users or virtual keys to restrict. Returns the created policy details. Use this to enforce cost controls on specific teams or projects using the gateway.

Create a new budget or usage policy for AI gateway access
- **delete_policy**: Requires the policy ID. Use this when a project ends or budget constraints are no longer needed.

Remove a budget or usage policy from Portkey
- **export_logs**: Optionally filters by date range, model, or user. Returns an export ID or download URL. Use this for audit trails, cost reporting, or offline analysis of AI usage patterns.

Export AI gateway logs for external analysis or compliance reporting
- **get_log_details**: Requires the log ID from list_logs results. Use this for deep debugging of specific AI interactions.

Get detailed information about a specific AI gateway log entry
- **get_virtual_keys**: Virtual keys map to underlying provider keys (OpenAI, Anthropic, etc.) with metadata, usage limits, and policy associations. Returns key IDs, names, provider targets, current usage, and status. Use this to audit API key usage or identify keys approaching limits.

List all virtual API keys managed by Portkey
- **list_configs**: Returns config IDs, names, creation dates, and associated virtual keys. Use this to review how LLM requests are routed or to audit gateway behavior.

List all gateway configurations stored in Portkey
- **list_logs**: Returns log IDs, timestamps, model names, token usage, latency, costs, and status codes. Use this to monitor AI usage, identify expensive calls, or debug latency issues. Supports pagination via limit/offset.

List recent AI gateway logs and traces from Portkey
- **list_models**: ). Returns model names, provider names, supported endpoints (chat, embeddings, etc.), and capabilities. Use this to discover which models are routable via your gateway.

List all LLM models supported by the Portkey gateway
- **list_policies**: Returns policy names, limits, current consumption, and affected users/keys. Use this to review guardrails preventing runaway AI costs.

List all budget and usage policies defined in Portkey
- **submit_feedback**: Requires the log ID, rating (LIKE, DISLIKE, or UNLIKE to remove), and optional text feedback. Use this to build RLHF datasets or monitor user satisfaction with AI outputs.

Submit user feedback (Like/Dislike) for a specific AI response log


## Installation & Usage

To install and use the **Portkey** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/portkey](https://vinkius.com/mcp/portkey)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
