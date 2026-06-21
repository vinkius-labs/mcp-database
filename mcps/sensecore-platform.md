# SenseCore Platform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sensecore-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sensecore-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sensecore-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate SenseCore AI services — manage models, trigger chat completions, and handle compute resources directly from any AI agent.

## Description
Connect your AI agents to the **SenseCore Platform**, the industrial-grade AI infrastructure by SenseTime. This MCP provides 10 tools to manage advanced foundation models, orchestrate large-scale chat completions, and monitor high-performance compute resources programmatically.

### What you can do

- **SenseChat Interaction** — Trigger chat completions with SenseTime's foundation models using persistent context and history
- **Model Intelligence** — List all available foundation models and retrieve granular technical specifications for each version
- **Resource Management** — Monitor compute node availability and track quota consumption across your organizational projects
- **Service Monitoring** — Check real-time health and latency metrics for deployed model services
- **Async Operations** — List and track the status of long-running training or inference tasks on the SenseCore infrastructure

### How it works

1. Subscribe to this server
2. Log in to the [**SenseCore Console**](https://platform.sensecore.cn/)
3. Navigate to **API Management** to obtain your **API Key** and **Secret Key**
4. Identify your **Organization ID** and the target **Project ID**
5. Insert your credentials into the fields below to start managing your SenseTime AI infrastructure.

### Who is this for?

- **Enterprise AI Developers** — automate the integration of SenseTime's industrial models into custom applications
- **Infrastructure Engineers** — monitor GPU cluster utilization and model service health programmatically
- **Machine Learning Ops** — orchestrate and track large-scale inference tasks on the SenseCore platform


## Available Tools
- **create_assistant**: Define a new AI assistant
- **get_assistant_details**: Get complete configuration for an assistant
- **create_message**: Add a message to a thread
- **chat_completions**: Send a message to a SenseCore large language model
- **create_run**: Execute an assistant on a thread
- **create_thread**: Initialize a new conversation thread
- **get_run_status**: Check the status of an active assistant run
- **list_assistants**: List all configured assistants
- **list_files**: List uploaded files
- **list_messages**: Retrieve the message history of a thread
- **list_models**: List all available SenseNova models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SenseCore Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Chat with SenseChat-5 and ask 'Compare the features of traditional neural networks and transformers'."

**🤖 AI Agent:**
> Connecting to SenseCore engine... SenseChat-5 responded: 'While both are neural architectures, transformers use self-attention mechanisms to process sequential data in parallel, unlike RNNs...' Would you like me to go deeper into self-attention?

---

**👤 You:**
> "List all active models in project 'Research_AI_2024'."

**🤖 AI Agent:**
> Fetching model list for project 'Research_AI_2024'... I found 3 active models: 1. SenseChat-5 (Foundation), 2. SenseVision (Multimodal), 3. SenseAudio (Specialized). Which one would you like to interact with?

---

**👤 You:**
> "What is the health status of service ID 'svc_gpu_999'?"

**🤖 AI Agent:**
> Querying service health metrics... Service 'svc_gpu_999' is currently 'Healthy'. Uptime: 99.98%, P99 Latency: 45ms, and Request Success Rate: 100% over the last 60 minutes.


## Installation & Usage

To install and use the **SenseCore Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sensecore-platform](https://vinkius.com/mcp/sensecore-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
