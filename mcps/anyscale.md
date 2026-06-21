# Anyscale MCP Server

Orchestrate your Anyscale infrastructure — manage LLM queries, vectors, services, and cluster batch jobs directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/anyscale)

## Overview
**Category:** ai-frontier
**Tools Count:** 7

## Description
Connect your **Anyscale** environment to your AI agent and manage both AI inference and backend scalable infrastructure natively through natural conversation.

### What you can do

- **Model Discovery and Querying** — List all active foundational models inside your environment and send conversational or zero-shot instruct prompts
- **Embeddings Pipeline** — Generate semantic vector embeddings for arrays of text inputs directly in-flight
- **Services Fleet** — Monitor deployed Ray services, fetch cluster states, and map live service endpoint configurations 
- **Cluster Jobs** — Query Ray batch jobs to inspect recent execution statuses and training metrics right from your terminal

### How it works

1. Subscribe to this server
2. Provide your Anyscale API Key and Base URL
3. Interface with your models, services, and Ray cluster via Claude, Cursor, or your favorite MCP agent

Scale up your AI operations without opening terminal panes to check Ray cluster status.

### Who is this for?

- **AI & MLOps Engineers** — automate the inspection of deployed models, jobs, and embeddings safely during CI workflows
- **Data Scientists** — submit rapid completion tasks to specialized LLMs running inside your Anyscale VPC
- **Backend Developers** — debug service health metrics and endpoint statuses without navigating the heavy cloud dashboard


## Available Tools
- **list_models**: g., meta-llama/Llama-2-70b-chat-hf).

List available AI models on Anyscale Endpoints
- **chat_completion**: Pass an array of messages with roles (user, assistant, system).

Generate conversational responses via Anyscale LLMs
- **text_completion**: Use for foundational instruct generation.

Generate text completion using Anyscale generic completion API
- **generate_embeddings**: Generate semantic vector embeddings for text
- **list_services**: List Anyscale deployed services
- **get_service**: Retrieve details about a specific Anyscale service
- **list_jobs**: List Anyscale batch or training jobs


## Installation & Usage

To install and use the **Anyscale** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anyscale](https://vinkius.com/mcp/anyscale)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
